# https-github.com-4lf4-tools-by-4lf4
## Report Info


**User Action**: `crash report`  
**Sender**: `TermuxActivity`  
**Report Timestamp**: `2025-07-05 13:51:10.530 UTC`  
##

## Crash Details

**Crash Thread**: `Thread[main,5,main]`  
**Crash Timestamp**: `2025-07-05 13:51:02.746 UTC`  

**Crash Message**:
```
Unable to start activity ComponentInfo{com.termux/com.termux.shared.activities.ReportActivity}: android.os.BadParcelableException: Parcelable encountered ClassNotFoundException reading a Serializable object (name = I0.a)
```


### Stacktrace

```
java.lang.RuntimeException: Unable to start activity ComponentInfo{com.termux/com.termux.shared.activities.ReportActivity}: android.os.BadParcelableException: Parcelable encountered ClassNotFoundException reading a Serializable object (name = I0.a)
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3903)
	at android.app.ActivityThread.handleLaunchActivity(ActivityThread.java:4049)
	at android.app.servertransaction.LaunchActivityItem.execute(LaunchActivityItem.java:101)
	at android.app.servertransaction.TransactionExecutor.executeCallbacks(TransactionExecutor.java:135)
	at android.app.servertransaction.TransactionExecutor.execute(TransactionExecutor.java:95)
	at android.app.ActivityThread$H.handleMessage(ActivityThread.java:2443)
	at android.os.Handler.dispatchMessage(Handler.java:106)
	at android.os.Looper.loopOnce(Looper.java:211)
	at android.os.Looper.loop(Looper.java:300)
	at android.app.ActivityThread.main(ActivityThread.java:8348)
	at java.lang.reflect.Method.invoke(Native Method)
	at com.android.internal.os.RuntimeInit$MethodAndArgsCaller.run(RuntimeInit.java:582)
	at com.android.internal.os.ZygoteInit.main(ZygoteInit.java:1028)
Caused by: android.os.BadParcelableException: Parcelable encountered ClassNotFoundException reading a Serializable object (name = I0.a)
	at android.os.Parcel.readSerializableInternal(Parcel.java:5062)
	at android.os.Parcel.readValue(Parcel.java:4604)
	at android.os.Parcel.readValue(Parcel.java:4312)
	at android.os.Parcel.-$$Nest$mreadValue(Unknown Source:0)
	at android.os.Parcel$LazyValue.apply(Parcel.java:4410)
	at android.os.Parcel$LazyValue.apply(Parcel.java:4369)
	at android.os.BaseBundle.getValueAt(BaseBundle.java:394)
	at android.os.BaseBundle.getValue(BaseBundle.java:374)
	at android.os.BaseBundle.getValue(BaseBundle.java:357)
	at android.os.BaseBundle.getValue(BaseBundle.java:350)
	at android.os.BaseBundle.getSerializable(BaseBundle.java:1451)
	at android.os.Bundle.getSerializable(Bundle.java:1144)
	at com.termux.shared.activities.ReportActivity.updateUI(ReportActivity.java:140)
	at com.termux.shared.activities.ReportActivity.onCreate(ReportActivity.java:93)
	at android.app.Activity.performCreate(Activity.java:8577)
	at android.app.Activity.performCreate(Activity.java:8541)
	at android.app.Instrumentation.callActivityOnCreate(Instrumentation.java:1437)
	at android.app.ActivityThread.performLaunchActivity(ActivityThread.java:3884)
	... 12 more
Caused by: java.lang.ClassNotFoundException: I0.a
	at java.lang.Class.classForName(Native Method)
	at java.lang.Class.forName(Class.java:607)
	at android.os.Parcel$2.resolveClass(Parcel.java:5039)
	at java.io.ObjectInputStream.readNonProxyDesc(ObjectInputStream.java:1733)
	at java.io.ObjectInputStream.readClassDesc(ObjectInputStream.java:1624)
	at java.io.ObjectInputStream.readOrdinaryObject(ObjectInputStream.java:1902)
	at java.io.ObjectInputStream.readObject0(ObjectInputStream.java:1442)
	at java.io.ObjectInputStream.readObject(ObjectInputStream.java:430)
	at android.os.Parcel.readSerializableInternal(Parcel.java:5045)
	... 29 more
Caused by: java.lang.ClassNotFoundException: I0.a
	... 38 more

```
##


## Termux App Info

**APP_NAME**: `Termux`  
**PACKAGE_NAME**: `com.termux`  
**VERSION_NAME**: `0.119.0-beta.3`  
**VERSION_CODE**: `1022`  
**UID**: `10361`  
**TARGET_SDK**: `28`  
**IS_DEBUGGABLE_BUILD**: `false`  
**SE_PROCESS_CONTEXT**: `u:r:untrusted_app_27:s0:c105,c257,c512,c768`  
**SE_FILE_CONTEXT**: `u:object_r:app_data_file:s0:c105,c257,c512,c768`  
**SE_INFO**: `default:targetSdkVersion=28:complete`  
**TERMUX_APP_PACKAGE_MANAGER**: `APT`  
**TERMUX_APP_PACKAGE_VARIANT**: `APT_ANDROID_7`  
**APK_RELEASE**: `F-Droid`  
**SIGNING_CERTIFICATE_SHA256_DIGEST**: `228FB2CFE90831C1499EC3CCAF61E96E8E1CE70766B9474672CE427334D41C42`  
##


## Device Info

### Software

**OS_VERSION**: `4.19.191-g6e5440f6a542`  
**SDK_INT**: `33`  
**RELEASE**: `13`  
**ID**: `TP1A.220624.014`  
**DISPLAY**: `TP1A.220624.014`  
**INCREMENTAL**: `V816.0.8.0.TKEIDXM`  
**SECURITY_PATCH**: `2024-12-01`  
**IS_DEBUGGABLE**: `0`  
**IS_TREBLE_ENABLED**: `true`  
**TYPE**: `user`  
**TAGS**: `release-keys`  
**MAX_PHANTOM_PROCESSES**: - (*Requires `DUMP` and `PACKAGE_USAGE_STATS` permission*)  
**MONITOR_PHANTOM_PROCS**: `true`  
**DEVICE_CONFIG_SYNC_DISABLED**: -  

### Hardware

**MANUFACTURER**: `Xiaomi`  
**BRAND**: `POCO`  
**MODEL**: `2201117PG`  
**PRODUCT**: `fleur_p_id`  
**BOARD**: `fleur`  
**HARDWARE**: `mt6781`  
**DEVICE**: `fleur`  
**SUPPORTED_ABIS**: `arm64-v8a, armeabi-v7a, armeabi`  
**SUPPORTED_32_BIT_ABIS**: `armeabi-v7a, armeabi`  
**SUPPORTED_64_BIT_ABIS**: `arm64-v8a`  
##
