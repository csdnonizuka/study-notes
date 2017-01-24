1. 不要直接使用AppCompatActivity,重写一个BaseAcitivity去继承AppCompatActivity。
2. 同上，Application也一样。有些类里无法获取Context的时候，可以通过重写Application来实现获取context。
3. 自定义一个LogUtil。里面定义一个打印日志的label,用来控制输出的日志。
4. 尽量学会使用Parcelable,尽量不用Serializable.

5. SystemClock.elapsedRealtime() 获取系统开机至今所经历时间的毫秒数。
   System.currentTimeMillis() 获取从1970年1月1日0点至今所经历时间的毫秒数。
