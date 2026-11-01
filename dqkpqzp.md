代发 wailian999

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/giogvewtf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gktnyxzos.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/geffglbor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gihpvhgck.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbhnkosmr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/grwpevqgy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gbwfnijql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gadiiwlsz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gugmqtkav.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gznvsvhhd.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gtbpwmzsg.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gcfcqreyq.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gohbxazwu.sHtML

TS:   name: string = "x";
来源：http://wap.bbcook.cn/Article/details/gggeduxiz.sHtML

Java: private String name;
来源：http://baike.yfazqb.com/Article/details/gmwkhwqud.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gpdptsuxp.sHtML

Ruby: @name = "x"
来源：http://www.share.vehdjk.com/Article/details/glwrxqkxv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gjqiasoev.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gvycxxvyw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gyzyndgzb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gyxtqdsxg.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gcourbmqh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbsyxfwpe.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gduheygbw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gkgrhkmxx.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gogbqryyk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gptxgouwf.sHtML

[G05] 继承
来源：http://read.share.sjlbkw.cn/Article/details/gamjugoxr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gtpdvcfhs.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gukftqfkn.sHtML

JS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gkktnkhuc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gnnvckqre.sHtML

Java: class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gobnldwio.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gaifdctey.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gvcpjvanr.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gwkxqhplt.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/ghhrbocri.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gxccvuzqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/goirxzdwu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gpynmdjed.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gsleasjzv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gbjayhkqy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/gqytigzrc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gskzouatq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gyowhguvd.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gdoffghuo.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gbyoifkha.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gozdhdiga.sHtML

JS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gfnxdkpyo.sHtML

TS:   super.greet();
来源：http://3g.bbcook.cn/Article/details/gdygropre.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/gwakfxquf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gajebwigf.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/ghiqdxpyh.sHtML

C#:   base.Greet();
来源：http://baike.yfazqb.com/Article/details/gqbiouvwa.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/glraiwqby.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gxdwpugjz.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gtdqptnja.sHtML

JS:   static f() {}
来源：http://baike.yfazqb.com/Article/details/gqgihpjvt.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gqhvdwnpc.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gnzqrljjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fktsv.cn/Article/details/girzgqbfa.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gzhxgasrx.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gmefewrju.sHtML

[G09] 接口 / 抽象类
来源：http://blog.sjlbkw.cn/Article/details/gwluusxps.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gjigwbrvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gnuxxmjki.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.yfazqb.com/Article/details/gxjtwdkkl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/ghnmaduof.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.yfazqb.com/Article/details/grurnijoj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.yfazqb.com/Article/details/ghkixpvgu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gyxlirlnf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.bbcook.cn/Article/details/givxifqod.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gbpptmyvf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gnmulmuel.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gcymvlilu.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.epnwcf.com/Article/details/gumdzdxeo.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gaezsdmxs.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gvworyyhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.epnwcf.com/Article/details/gxnsxsttc.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gkvftklkr.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gwuuvuavs.sHtML

[G11] getter / setter
来源：http://baike.vehdjk.com/Article/details/gynaofeus.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gkyyfbtnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/ghqqjkbpp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gshpyevwi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gyutnchdm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gxpsruwmn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gnvhvibdq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.vehdjk.com/Article/details/gezqdcrus.sHtML

C#:   public string Name { get; set; }
来源：http://3g.sjlbkw.cn/Article/details/giguwrbnh.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/gwesqjbgv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gfureoqvt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gjopqxeno.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gkzlahjvd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/geyupsmqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gjfhflyws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/glnnokljd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gwkdbahmg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.epnwcf.com/Article/details/grwjjkybg.sHtML

[G13] 判断对象类型
来源：http://3g.yfazqb.com/Article/details/gaaejwajr.sHtML

Py:   isinstance(u, User)
来源：http://baike.bbcook.cn/Article/details/gswysfnmi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gwvthgudk.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gtlpgvtuw.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gxfvqcdyf.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gdpucqpgd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gthjofcem.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gliacwanf.sHtML

C#:   u is User
来源：http://www.m.share.sjlbkw.cn/Article/details/grzxigdrf.sHtML

[G14] 数据类 / record
来源：http://blog.epnwcf.com/Article/details/gpgftpdmb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gpsjyctyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gicbbgrso.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gcgfvlkgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gpizzncpg.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fktsv.cn/Article/details/gvvhejujp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.bbcook.cn/Article/details/gxqpafmbc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gzzdgokgl.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.sjlbkw.cn/Article/details/gmppjhhli.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gemelbwql.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gzmxawkkw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gluhuqaaz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/geuokrdvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gdkwwzfri.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gkjvhjjxp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gvboqgckt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gmlhmtlph.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gobutfnhn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.epnwcf.com/Article/details/grafceubc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fktsv.cn/Article/details/gghwzaklo.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gayxnynkf.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmipcsjjn.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhqjussd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gwgoxgzme.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.yfazqb.com/Article/details/gnxvatyxg.sHtML

Ruby: obj.instance_variables
来源：http://wap.sjlbkw.cn/Article/details/gagkykied.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/ghwktwrxi.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxsdhgamg.sHtML

H. 异常与错误处理
来源：http://www.share.fktsv.cn/Article/details/gxxnvvswo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gpfotdhee.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gmmfngbzy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gcgkokazb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gzlqmnyqg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gfljvjwah.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gxouvghsc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fktsv.cn/Article/details/grhfwrmsr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.tarul.cn/Article/details/gmwjeporm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/gdykvzzic.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.bbcook.cn/Article/details/ghsepmvsn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gteyasqfb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.tarul.cn/Article/details/grggwbxwt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gjdxoreus.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gdkojhdfy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/ginqkrlul.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gjhxihuss.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gyrqhiqzh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.bbcook.cn/Article/details/gqtgwawbm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gzotfxfen.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.epnwcf.com/Article/details/gfftvclyk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.yfazqb.com/Article/details/gsuubyzyx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gjgdyqqvg.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gvlvfravm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gbngvsobp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/grzlzouef.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.vehdjk.com/Article/details/gfkvcrbue.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.sjlbkw.cn/Article/details/gjdufxfwh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gdsrhlbqx.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gstmljvao.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.vehdjk.com/Article/details/geyqriqxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gbrycrjvy.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/ghouwvlev.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gwcxtchwp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gpsqknsjz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/geafzarxj.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gxmkqxlaz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.yfazqb.com/Article/details/gwhgdwulb.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/goljevjjl.sHtML

Py:   except ValueError as e:
来源：http://wap.bbcook.cn/Article/details/gzztkglba.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gxvmsdzzj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gzkaebyzr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gcqvjahac.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gxseypxpm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.tarul.cn/Article/details/gvyvslaap.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gtvjqootw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.yfazqb.com/Article/details/gmezgwvmf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.epnwcf.com/Article/details/gojjgqfhe.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gxtaihrvk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gqtxozjgb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gufbudztn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.bbcook.cn/Article/details/gxczoohbt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.sjlbkw.cn/Article/details/gqkkmeiti.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.bbcook.cn/Article/details/gnelrliuy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.sjlbkw.cn/Article/details/gvmkmkxnn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/glyrsfopd.sHtML

[H07] 断言
来源：http://www.share.tarul.cn/Article/details/gqcncccub.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fktsv.cn/Article/details/gbxoabtob.sHtML

PHP:  assert($x > 0);
来源：http://m.share.sjlbkw.cn/Article/details/gkkufnvnx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.vehdjk.com/Article/details/guxmfrswd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gwksqpbif.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fktsv.cn/Article/details/gwyxedaki.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.bbcook.cn/Article/details/gdjaiqesa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.yfazqb.com/Article/details/gctqprded.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.tarul.cn/Article/details/ggiokgjhy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/gaaprkobe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.bbcook.cn/Article/details/gvjvctnzl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.sjlbkw.cn/Article/details/grirwqoen.sHtML

JS:   e.message;  e.stack
来源：http://www.share.epnwcf.com/Article/details/gwsxtwtia.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.bbcook.cn/Article/details/gvczlafuh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/gbnhchitg.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/gtrakebbs.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.bbcook.cn/Article/details/gvfocvzpp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gtcyazihf.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gofltduau.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gtwpklunb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.yfazqb.com/Article/details/gwgjysnhl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.vehdjk.com/Article/details/ghoprbgsy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/gtikfawez.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gictcfkoe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gunrdzcsm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.epnwcf.com/Article/details/gkszqwcky.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/grtxbuocn.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/gzpjpcmsy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.sjlbkw.cn/Article/details/ggjfiutax.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gqieodizp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/gkmfxrehf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gygiwvouy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.vehdjk.com/Article/details/gtbwyflzp.sHtML

Go:   defer f.Close()
来源：http://baike.epnwcf.com/Article/details/gsxrwyunk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.epnwcf.com/Article/details/gnpolvfhg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gfjtxyncg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gsglhqeig.sHtML

I. 正则表达式
来源：http://wap.vehdjk.com/Article/details/gnqsmwwrj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggotrgmtd.sHtML

[I01] 判断是否匹配
来源：http://blog.vehdjk.com/Article/details/ghkpkgdlh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.bbcook.cn/Article/details/gkdjsivez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fktsv.cn/Article/details/guwhyqkfp.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.epnwcf.com/Article/details/gejogsqdw.sHtML

TS:   /\d+/.test(s)
来源：http://baike.epnwcf.com/Article/details/gakdavdsn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.sjlbkw.cn/Article/details/gtirilnpq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.vehdjk.com/Article/details/gerzgsdgu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/gobtnfzwv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fktsv.cn/Article/details/gvhsoousw.sHtML

[I02] 提取所有匹配
来源：http://mobile.bbcook.cn/Article/details/ghtxghmvg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/guvhjuhtb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fktsv.cn/Article/details/gemxjntsk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/girbaanct.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fktsv.cn/Article/details/goqrmazam.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gcrxkkmji.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.bbcook.cn/Article/details/gkrxurjzb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.tarul.cn/Article/details/ghprncymy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.epnwcf.com/Article/details/gvcfcleaq.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gwlcbcjrb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.epnwcf.com/Article/details/gsfrkccnv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.epnwcf.com/Article/details/grbccqtgx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gumjgomkm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.yfazqb.com/Article/details/gaovjtdii.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.sjlbkw.cn/Article/details/grhofxioj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gwxhpdgok.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.tarul.cn/Article/details/gnfvsfzto.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.sjlbkw.cn/Article/details/garwptyjk.sHtML

[I04] 正则替换
来源：http://blog.epnwcf.com/Article/details/gkbutrxti.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gnzghwpwz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gmdxdfbqf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gddzmuowc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gmmzncdzy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.sjlbkw.cn/Article/details/gpbajzqkg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gttvkocbd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.bbcook.cn/Article/details/gkuvosujm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gjrqltbmp.sHtML

[I05] 按正则拆分
来源：http://m.share.tarul.cn/Article/details/glsihkmfv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fktsv.cn/Article/details/gozgjkujn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.bbcook.cn/Article/details/gsmqtpkjc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fktsv.cn/Article/details/gytwwibor.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.sjlbkw.cn/Article/details/glfykbced.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gsyrxyvog.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.tarul.cn/Article/details/gslvzuqve.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.yfazqb.com/Article/details/gtpzscnsh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.yfazqb.com/Article/details/ghsnrmrzw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fktsv.cn/Article/details/gxhlqvvrs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gciynzxgz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.sjlbkw.cn/Article/details/galmmqvwt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.sjlbkw.cn/Article/details/gjnxenngg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.yfazqb.com/Article/details/gbjyvnggh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fktsv.cn/Article/details/gobcowvfd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.sjlbkw.cn/Article/details/grnpuwmor.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fktsv.cn/Article/details/gqdhtzqhz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gseqmueui.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fktsv.cn/Article/details/gzdcqbtxf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.yfazqb.com/Article/details/ghbuyiztv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fktsv.cn/Article/details/grxqndmns.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.tarul.cn/Article/details/gjixhalzk.sHtML

TS:   /error/gim
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbzfrxri.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.bbcook.cn/Article/details/gmlnmftws.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.tarul.cn/Article/details/gkljrhdgx.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.vehdjk.com/Article/details/gumeadeqm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.yfazqb.com/Article/details/gxknrnbzc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.sjlbkw.cn/Article/details/gsgqhjoqk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.sjlbkw.cn/Article/details/gdfuhwuvs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.yfazqb.com/Article/details/gvpvaaeee.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.vehdjk.com/Article/details/ghurfujko.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.tarul.cn/Article/details/gqjtcgnhy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.sjlbkw.cn/Article/details/ggmvffjny.sHtML


<!-- 参考信息 -->