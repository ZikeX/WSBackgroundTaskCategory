# WSBackgroundTaskCategory



解决了在切换至后台时导致某些页面的NSTimer停止，也可用于在切换至后台时处理一些数据，如上传至服务器


# Usage

```Object-C
- (void)applicationDidEnterBackground:(UIApplication *)application {

    // beginBackgroundTask
    [self beginBackgroundTaskWithBlock:^{
        NSLog(@"do something");
    }];
}

- (void)applicationDidBecomeActive:(UIApplication *)application {

    // beginBackgroundTask
    [self endBackgroundTask];
}
```
