
Task 'stacktrace' not found in root project 'My Application' and its subprojects.

* Try:
> Run gradle tasks to get a list of available tasks.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Exception is:
org.gradle.execution.TaskSelectionException: Task 'stacktrace' not found in root project 'My Application' and its subprojects.
	at org.gradle.execution.DefaultTaskSelector.getSelection(DefaultTaskSelector.java:86)
	at org.gradle.execution.selection.DefaultBuildTaskSelector.resolveTaskName(DefaultBuildTaskSelector.java:98)
	at org.gradle.execution.commandline.CommandLineTaskParser.parseTasks(CommandLineTaskParser.java:49)
	at org.gradle.execution.TaskNameResolvingBuildTaskScheduler.scheduleRequestedTasks(TaskNameResolvingBuildTaskScheduler.java:50)
	at org.gradle.execution.DefaultTasksBuildTaskScheduler.scheduleRequestedTasks(DefaultTasksBuildTaskScheduler.java:72)
	at org.gradle.initialization.DefaultTaskExecutionPreparer.lambda$scheduleRequestedTasks$0(DefaultTaskExecutionPreparer.java:46)
	at org.gradle.internal.Factories$1.create(Factories.java:31)
	at org.gradle.internal.work.DefaultWorkerLeaseService.withReplacedLocks(DefaultWorkerLeaseService.java:345)
	at org.gradle.api.internal.project.DefaultProjectStateRegistry$DefaultBuildProjectRegistry.withMutableStateOfAllProjects(DefaultProjectStateRegistry.java:227)
	at org.gradle.api.internal.project.DefaultProjectStateRegistry$DefaultBuildProjectRegistry.withMutableStateOfAllProjects(DefaultProjectStateRegistry.java:220)
	at org.gradle.initialization.DefaultTaskExecutionPreparer.scheduleRequestedTasks(DefaultTaskExecutionPreparer.java:45)
	at org.gradle.initialization.VintageBuildModelController.lambda$scheduleRequestedTasks$0(VintageBuildModelController.java:76)
	at org.gradle.internal.model.StateTransitionController.lambda$inState$2(StateTransitionController.java:121)
	at org.gradle.internal.model.StateTransitionController.lambda$inState$3(StateTransitionController.java:136)
	at org.gradle.internal.work.DefaultSynchronizer.withLock(DefaultSynchronizer.java:44)
	at org.gradle.internal.model.StateTransitionController.inState(StateTransitionController.java:132)
	at org.gradle.internal.model.StateTransitionController.inState(StateTransitionController.java:120)
	at org.gradle.initialization.VintageBuildModelController.scheduleRequestedTasks(VintageBuildModelController.java:76)
	at org.gradle.internal.build.DefaultBuildLifecycleController$DefaultWorkGraphBuilder.addRequestedTasks(DefaultBuildLifecycleController.java:260)
	at org.gradle.internal.buildtree.DefaultBuildTreeWorkPreparer.lambda$scheduleRequestedTasks$0(DefaultBuildTreeWorkPreparer.java:38)
	at org.gradle.internal.build.DefaultBuildLifecycleController.lambda$populateWorkGraph$4(DefaultBuildLifecycleController.java:148)
	at org.gradle.internal.build.DefaultBuildWorkPreparer.populateWorkGraph(DefaultBuildWorkPreparer.java:42)
	at org.gradle.internal.build.BuildOperationFiringBuildWorkPreparer$PopulateWorkGraph.populateTaskGraph(BuildOperationFiringBuildWorkPreparer.java:120)
	at org.gradle.internal.build.BuildOperationFiringBuildWorkPreparer$PopulateWorkGraph.run(BuildOperationFiringBuildWorkPreparer.java:91)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$1.execute(DefaultBuildOperationRunner.java:29)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$1.execute(DefaultBuildOperationRunner.java:26)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:66)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:157)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.run(DefaultBuildOperationRunner.java:47)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.run(DefaultBuildOperationExecutor.java:68)
	at org.gradle.internal.build.BuildOperationFiringBuildWorkPreparer.populateWorkGraph(BuildOperationFiringBuildWorkPreparer.java:68)
	at org.gradle.internal.build.DefaultBuildLifecycleController.lambda$populateWorkGraph$5(DefaultBuildLifecycleController.java:148)
	at org.gradle.internal.model.StateTransitionController.lambda$inState$2(StateTransitionController.java:121)
	at org.gradle.internal.model.StateTransitionController.lambda$inState$3(StateTransitionController.java:136)
	at org.gradle.internal.work.DefaultSynchronizer.withLock(DefaultSynchronizer.java:44)
	at org.gradle.internal.model.StateTransitionController.inState(StateTransitionController.java:132)
	at org.gradle.internal.model.StateTransitionController.inState(StateTransitionController.java:120)
	at org.gradle.internal.build.DefaultBuildLifecycleController.populateWorkGraph(DefaultBuildLifecycleController.java:148)
	at org.gradle.internal.build.DefaultBuildWorkGraphController$DefaultBuildWorkGraph.populateWorkGraph(DefaultBuildWorkGraphController.java:167)
	at org.gradle.composite.internal.DefaultBuildController.populateWorkGraph(DefaultBuildController.java:73)
	at org.gradle.composite.internal.DefaultIncludedBuildTaskGraph$DefaultBuildTreeWorkGraphBuilder.withWorkGraph(DefaultIncludedBuildTaskGraph.java:150)
	at org.gradle.internal.buildtree.DefaultBuildTreeWorkPreparer.lambda$scheduleRequestedTasks$1(DefaultBuildTreeWorkPreparer.java:38)
	at org.gradle.composite.internal.DefaultIncludedBuildTaskGraph$DefaultBuildTreeWorkGraph$1.run(DefaultIncludedBuildTaskGraph.java:197)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$1.execute(DefaultBuildOperationRunner.java:29)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$1.execute(DefaultBuildOperationRunner.java:26)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:66)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:157)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.run(DefaultBuildOperationRunner.java:47)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.run(DefaultBuildOperationExecutor.java:68)
	at org.gradle.composite.internal.DefaultIncludedBuildTaskGraph$DefaultBuildTreeWorkGraph.scheduleWork(DefaultIncludedBuildTaskGraph.java:192)
	at org.gradle.internal.buildtree.DefaultBuildTreeWorkPreparer.scheduleRequestedTasks(DefaultBuildTreeWorkPreparer.java:37)
	at org.gradle.configurationcache.VintageBuildTreeWorkController$scheduleAndRunRequestedTasks$1.apply(VintageBuildTreeWorkController.kt:36)
	at org.gradle.configurationcache.VintageBuildTreeWorkController$scheduleAndRunRequestedTasks$1.apply(VintageBuildTreeWorkController.kt:35)
	at org.gradle.composite.internal.DefaultIncludedBuildTaskGraph.withNewWorkGraph(DefaultIncludedBuildTaskGraph.java:109)
	at org.gradle.configurationcache.VintageBuildTreeWorkController.scheduleAndRunRequestedTasks(VintageBuildTreeWorkController.kt:35)
	at org.gradle.internal.buildtree.DefaultBuildTreeLifecycleController.lambda$fromBuildModel$2(DefaultBuildTreeLifecycleController.java:76)
	at org.gradle.internal.buildtree.DefaultBuildTreeLifecycleController.lambda$runBuild$4(DefaultBuildTreeLifecycleController.java:98)
	at org.gradle.internal.model.StateTransitionController.lambda$transition$6(StateTransitionController.java:177)
	at org.gradle.internal.model.StateTransitionController.doTransition(StateTransitionController.java:258)
	at org.gradle.internal.model.StateTransitionController.lambda$transition$7(StateTransitionController.java:177)
	at org.gradle.internal.work.DefaultSynchronizer.withLock(DefaultSynchronizer.java:44)
	at org.gradle.internal.model.StateTransitionController.transition(StateTransitionController.java:177)
	at org.gradle.internal.buildtree.DefaultBuildTreeLifecycleController.runBuild(DefaultBuildTreeLifecycleController.java:95)
	at org.gradle.internal.buildtree.DefaultBuildTreeLifecycleController.fromBuildModel(DefaultBuildTreeLifecycleController.java:73)
	at org.gradle.tooling.internal.provider.runner.AbstractClientProvidedBuildActionRunner.runClientAction(AbstractClientProvidedBuildActionRunner.java:43)
	at org.gradle.tooling.internal.provider.runner.ClientProvidedPhasedActionRunner.run(ClientProvidedPhasedActionRunner.java:53)
	at org.gradle.launcher.exec.ChainingBuildActionRunner.run(ChainingBuildActionRunner.java:35)
	at org.gradle.internal.buildtree.ProblemReportingBuildActionRunner.run(ProblemReportingBuildActionRunner.java:49)
	at org.gradle.launcher.exec.BuildOutcomeReportingBuildActionRunner.run(BuildOutcomeReportingBuildActionRunner.java:65)
	at org.gradle.tooling.internal.provider.FileSystemWatchingBuildActionRunner.run(FileSystemWatchingBuildActionRunner.java:140)
	at org.gradle.launcher.exec.BuildCompletionNotifyingBuildActionRunner.run(BuildCompletionNotifyingBuildActionRunner.java:41)
	at org.gradle.launcher.exec.RootBuildLifecycleBuildActionExecutor.lambda$execute$0(RootBuildLifecycleBuildActionExecutor.java:40)
	at org.gradle.composite.internal.DefaultRootBuildState.run(DefaultRootBuildState.java:122)
	at org.gradle.launcher.exec.RootBuildLifecycleBuildActionExecutor.execute(RootBuildLifecycleBuildActionExecutor.java:40)
	at org.gradle.internal.buildtree.DefaultBuildTreeContext.execute(DefaultBuildTreeContext.java:40)
	at org.gradle.launcher.exec.BuildTreeLifecycleBuildActionExecutor.lambda$execute$0(BuildTreeLifecycleBuildActionExecutor.java:65)
	at org.gradle.internal.buildtree.BuildTreeState.run(BuildTreeState.java:53)
	at org.gradle.launcher.exec.BuildTreeLifecycleBuildActionExecutor.execute(BuildTreeLifecycleBuildActionExecutor.java:65)
	at org.gradle.launcher.exec.RunAsBuildOperationBuildActionExecutor$3.call(RunAsBuildOperationBuildActionExecutor.java:61)
	at org.gradle.launcher.exec.RunAsBuildOperationBuildActionExecutor$3.call(RunAsBuildOperationBuildActionExecutor.java:57)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$CallableBuildOperationWorker.execute(DefaultBuildOperationRunner.java:204)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$CallableBuildOperationWorker.execute(DefaultBuildOperationRunner.java:199)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:66)
	at org.gradle.internal.operations.DefaultBuildOperationRunner$2.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:157)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.execute(DefaultBuildOperationRunner.java:59)
	at org.gradle.internal.operations.DefaultBuildOperationRunner.call(DefaultBuildOperationRunner.java:53)
	at org.gradle.internal.operations.DefaultBuildOperationExecutor.call(DefaultBuildOperationExecutor.java:73)
	at org.gradle.launcher.exec.RunAsBuildOperationBuildActionExecutor.execute(RunAsBuildOperationBuildActionExecutor.java:57)
	at org.gradle.launcher.exec.RunAsWorkerThreadBuildActionExecutor.lambda$execute$0(RunAsWorkerThreadBuildActionExecutor.java:36)
	at org.gradle.internal.work.DefaultWorkerLeaseService.withLocks(DefaultWorkerLeaseService.java:249)
	at org.gradle.internal.work.DefaultWorkerLeaseService.runAsWorkerThread(DefaultWorkerLeaseService.java:109)
	at org.gradle.launcher.exec.RunAsWorkerThreadBuildActionExecutor.execute(RunAsWorkerThreadBuildActionExecutor.java:36)
	at org.gradle.tooling.internal.provider.continuous.ContinuousBuildActionExecutor.execute(ContinuousBuildActionExecutor.java:110)
	at org.gradle.tooling.internal.provider.SubscribableBuildActionExecutor.execute(SubscribableBuildActionExecutor.java:64)
	at org.gradle.internal.session.DefaultBuildSessionContext.execute(DefaultBuildSessionContext.java:46)
	at org.gradle.tooling.internal.provider.BuildSessionLifecycleBuildActionExecuter$ActionImpl.apply(BuildSessionLifecycleBuildActionExecuter.java:100)
	at org.gradle.tooling.internal.provider.BuildSessionLifecycleBuildActionExecuter$ActionImpl.apply(BuildSessionLifecycleBuildActionExecuter.java:88)
	at org.gradle.internal.session.BuildSessionState.run(BuildSessionState.java:69)
	at org.gradle.tooling.internal.provider.BuildSessionLifecycleBuildActionExecuter.execute(BuildSessionLifecycleBuildActionExecuter.java:62)
	at org.gradle.tooling.internal.provider.BuildSessionLifecycleBuildActionExecuter.execute(BuildSessionLifecycleBuildActionExecuter.java:41)
	at org.gradle.tooling.internal.provider.StartParamsValidatingActionExecuter.execute(StartParamsValidatingActionExecuter.java:63)
	at org.gradle.tooling.internal.provider.StartParamsValidatingActionExecuter.execute(StartParamsValidatingActionExecuter.java:31)
	at org.gradle.tooling.internal.provider.SessionFailureReportingActionExecuter.execute(SessionFailureReportingActionExecuter.java:50)
	at org.gradle.tooling.internal.provider.SessionFailureReportingActionExecuter.execute(SessionFailureReportingActionExecuter.java:38)
	at org.gradle.tooling.internal.provider.SetupLoggingActionExecuter.execute(SetupLoggingActionExecuter.java:47)
	at org.gradle.tooling.internal.provider.SetupLoggingActionExecuter.execute(SetupLoggingActionExecuter.java:31)
	at org.gradle.launcher.daemon.server.exec.ExecuteBuild.doBuild(ExecuteBuild.java:65)
	at org.gradle.launcher.daemon.server.exec.BuildCommandOnly.execute(BuildCommandOnly.java:37)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.WatchForDisconnection.execute(WatchForDisconnection.java:39)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.ResetDeprecationLogger.execute(ResetDeprecationLogger.java:29)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.RequestStopIfSingleUsedDaemon.execute(RequestStopIfSingleUsedDaemon.java:35)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.ForwardClientInput$2.create(ForwardClientInput.java:78)
	at org.gradle.launcher.daemon.server.exec.ForwardClientInput$2.create(ForwardClientInput.java:75)
	at org.gradle.util.internal.Swapper.swap(Swapper.java:38)
	at org.gradle.launcher.daemon.server.exec.ForwardClientInput.execute(ForwardClientInput.java:75)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.LogAndCheckHealth.execute(LogAndCheckHealth.java:64)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.LogToClient.doBuild(LogToClient.java:63)
	at org.gradle.launcher.daemon.server.exec.BuildCommandOnly.execute(BuildCommandOnly.java:37)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.EstablishBuildEnvironment.doBuild(EstablishBuildEnvironment.java:84)
	at org.gradle.launcher.daemon.server.exec.BuildCommandOnly.execute(BuildCommandOnly.java:37)
	at org.gradle.launcher.daemon.server.api.DaemonCommandExecution.proceed(DaemonCommandExecution.java:104)
	at org.gradle.launcher.daemon.server.exec.StartBuildOrRespondWithBusy$1.run(StartBuildOrRespondWithBusy.java:52)
	at org.gradle.launcher.daemon.server.DaemonStateCoordinator$1.run(DaemonStateCoordinator.java:297)
	at org.gradle.internal.concurrent.ExecutorPolicy$CatchAndRecordFailures.onExecute(ExecutorPolicy.java:64)
	at org.gradle.internal.concurrent.ManagedExecutorImpl$1.run(ManagedExecutorImpl.java:49)

