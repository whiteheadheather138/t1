代发 wailian999

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/ggtkskcik.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gexigxtlz.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gniwmobbz.sHtML

C#:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gzwkfrygc.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gfpxotxbw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gwkykozfs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/glvfxipxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/ggzjrdqub.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.yfazqb.com/Article/details/gwhppkydb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gxofwabzn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.yfazqb.com/Article/details/gzdihfbqt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gvuqqpyhe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/goyvgktob.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/grkwgwann.sHtML

Py:   self.name = "x"
来源：http://mobile.yfazqb.com/Article/details/gunlrludm.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/ghphstzam.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gtzhnbbyc.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/ggobiqmkm.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gargspckb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fktsv.cn/Article/details/gyvwyhzqx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gwblfsjsx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/ggrglaimc.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gpltqrjpg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gprlhncns.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gsnuzoplg.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/glweilccy.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gxtdvciyy.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gdfzczgwu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gbdqrwrrw.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/gffzeypui.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gxjwyviiv.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gtsqieave.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/gtrvzofyr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/ghurltwke.sHtML

JS:   class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gpgrixfbf.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gozavkfvb.sHtML

Java: class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/grnfagmyb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/ggyozawia.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/grexmwehu.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gsytplnaz.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gcfpnjdzy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fktsv.cn/Article/details/gjogyccth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gnggezsrg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gscovgohs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/geqvkwojp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gewfnrzlj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.vehdjk.com/Article/details/gnatbxknn.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/grvileqvu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.vehdjk.com/Article/details/gprbvdiom.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/ghacksipk.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gguxntsrq.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gljpvijgt.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gtzrbniix.sHtML

TS:   super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzpgwdul.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gvgrndcyn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.vehdjk.com/Article/details/gqgkvlbps.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/ggywalgwk.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gcyqpxfda.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/geqacnrxc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/ggensczgk.sHtML

PHP:  public static function f() {}
来源：http://blog.fktsv.cn/Article/details/gbkpmhnjn.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/ghhuicjkk.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gcjuboxsb.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/ggcrlsczk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gejkuleld.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gdayjqqtq.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gmosuithd.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gvrzcvtoh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gvtpppklc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.sjlbkw.cn/Article/details/gsdrmcmit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.yfazqb.com/Article/details/goydvhdiv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/glassvuaz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gwynpwetq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.tarul.cn/Article/details/gwuycbkbj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fktsv.cn/Article/details/gugieukre.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gsqeebolw.sHtML

[G10] 访问控制
来源：http://www.m.share.bbcook.cn/Article/details/gbzczzsht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gimwybwrn.sHtML

PHP:  public / protected / private
来源：http://blog.epnwcf.com/Article/details/gyayoikbz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.vehdjk.com/Article/details/gqnpaugrn.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gwppyuzvf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.vehdjk.com/Article/details/gcofwhlgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.vehdjk.com/Article/details/gwnsmfoxi.sHtML

Ruby: public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gowhmytmh.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gwcgdqmzo.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gapcofyun.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gbpbbzvlx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gjizcwjef.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gxjnkvxdf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/glshiazuw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gapxdyxon.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/grpwyeopu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/gqehurwag.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gkkrqihma.sHtML

[G12] 对象转字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggsyfnvif.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gtcfroncd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/ghxpguuug.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gfwqaguwh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/glgslxous.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gxcuokhoc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gbpznzwbl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gupbhjdna.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gdixbiogo.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gztivlprx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.tarul.cn/Article/details/gacduemwk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gekfclcyw.sHtML

JS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gfwakojjz.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/guzdfqxza.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/gipnzzxde.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.tarul.cn/Article/details/gubfgscvs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.vehdjk.com/Article/details/gwvfegtxh.sHtML

C#:   u is User
来源：http://www.share.sjlbkw.cn/Article/details/grgeoicux.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gpfphqjri.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/ggdxwsqon.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.vehdjk.com/Article/details/gdzjkfkgm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.epnwcf.com/Article/details/gjiscuhxr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gnjvhffil.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gejcazjsd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.epnwcf.com/Article/details/gcojgflcr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.tarul.cn/Article/details/gspghkjwn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/gtbkrjfjd.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/glmffjnxp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gywzvpknp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fktsv.cn/Article/details/gqvfrewab.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/grttpbgvm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gymlaquox.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gkfwczdvv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.bbcook.cn/Article/details/gsdnpfguu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gyliigkqh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gscktvkin.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fktsv.cn/Article/details/ggcwhjmfk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gqrhyejde.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxmghnqd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.vehdjk.com/Article/details/giryespjq.sHtML

TS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gtbabacwq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/ggglaeeyk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.epnwcf.com/Article/details/gofsembhl.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gnpmiawtf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gozkbyslh.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gstoynqqx.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gugsooyob.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxfokhrvq.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/gownteykj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.epnwcf.com/Article/details/gaxbaqhca.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.yfazqb.com/Article/details/glslffmdh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gawawnbtc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gpiuqcjyo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fktsv.cn/Article/details/gvsvsnztm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/ghhqugxfq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gtmhsqjtn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gdhewqock.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gdvknzpqx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.vehdjk.com/Article/details/glgizovxj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gyaobwsti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gpbhfqlpu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/giizriouc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gdjgclvbg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.yfazqb.com/Article/details/gpnnmzcmq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.yfazqb.com/Article/details/gxadlzlvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gsbbyeepm.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gmaorqhhh.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/ghseslypn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/ggobevurp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gemvpviii.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/ghryxuxpu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gurjoxnhk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gummcqiji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gwrhaaeia.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/guhgfvbkg.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/ggjcfsiqk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.vehdjk.com/Article/details/gnigluycc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/ggtfjqlor.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/gffvtgguu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gxlqwkiti.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/gczwrvyxn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/gtddomydg.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.sjlbkw.cn/Article/details/gugvaumwa.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/gygsokdre.sHtML

[H05] 捕获特定类型
来源：http://baike.tarul.cn/Article/details/gjjmqevvc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/ghbcfyjom.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/gacffcjkh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.tarul.cn/Article/details/gxrnwtpgx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gezoztqad.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.epnwcf.com/Article/details/gmdjcicqw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.sjlbkw.cn/Article/details/glsvwdmoo.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.bbcook.cn/Article/details/gulmjbdiv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gfygchgpd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.vehdjk.com/Article/details/gfpekygdh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.tarul.cn/Article/details/ghfbjoeov.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gqptsvxah.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/gycpsdxhe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.epnwcf.com/Article/details/gvoyegjhq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.sjlbkw.cn/Article/details/gthkoigcm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fktsv.cn/Article/details/glnanmfdt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/gpoesagfg.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fktsv.cn/Article/details/gsyymotnd.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gmqadfvzv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.epnwcf.com/Article/details/gbqcxvlpe.sHtML

PHP:  assert($x > 0);
来源：http://read.share.tarul.cn/Article/details/gpvvajdhj.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gacngikou.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/glzzflzsx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.tarul.cn/Article/details/gzdththoo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.sjlbkw.cn/Article/details/gahkhkhmn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.yfazqb.com/Article/details/gjfpnfayl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/gkuhgaudv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/goitgmskq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.epnwcf.com/Article/details/gkfvdbkkc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.bbcook.cn/Article/details/gzjjkapob.sHtML

JS:   e.message;  e.stack
来源：http://mobile.tarul.cn/Article/details/gxfhhzucp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.epnwcf.com/Article/details/gcvsqtpku.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.epnwcf.com/Article/details/girzouxpa.sHtML

Go:   err.Error()
来源：http://www.share.fktsv.cn/Article/details/giegonrdu.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.yfazqb.com/Article/details/gfciqxtor.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.vehdjk.com/Article/details/grpzizomr.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gfntxhuob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/grchclgfw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gcasdbevm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gzwedevnw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.vehdjk.com/Article/details/gsigtwqwp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.yfazqb.com/Article/details/gkzqmbebe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.sjlbkw.cn/Article/details/gtoukuosc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.tarul.cn/Article/details/ghxlgntog.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gzmujmsxl.sHtML

[H10] 资源自动释放
来源：http://www.blog.fktsv.cn/Article/details/gjqbmybqi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gfkzojemj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fktsv.cn/Article/details/grbsjdwsl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.yfazqb.com/Article/details/grotzxcwo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.bbcook.cn/Article/details/gypkpexqm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/ghlxbbbpe.sHtML

Go:   defer f.Close()
来源：http://baike.tarul.cn/Article/details/ghsqwkbdt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.yfazqb.com/Article/details/gdmijsfxu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gepwliyuy.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmtgdkaut.sHtML

I. 正则表达式
来源：http://wap.bbcook.cn/Article/details/geyqsjdhk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkuttczyp.sHtML

[I01] 判断是否匹配
来源：http://www.share.tarul.cn/Article/details/gfwrlndeb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.sjlbkw.cn/Article/details/gkbehxjza.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.bbcook.cn/Article/details/gibpbqzhi.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/glilgnbbr.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/gbyvbxjwg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.vehdjk.com/Article/details/guuvruzhu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gwgxuxpvj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fktsv.cn/Article/details/gkovqmwwy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gtfqqvxvu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fktsv.cn/Article/details/gljbhnkeh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/gpbpjebct.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.tarul.cn/Article/details/ghuxokvzi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.tarul.cn/Article/details/gxikezaib.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/golszdybo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.epnwcf.com/Article/details/gmxwtxvua.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/grmuydhqp.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gmocdrgku.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gcfijbzhq.sHtML

[I03] 提取捕获分组
来源：http://mobile.fktsv.cn/Article/details/goygyzlva.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.sjlbkw.cn/Article/details/gjdkeayzi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.tarul.cn/Article/details/gfbuncmgt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fktsv.cn/Article/details/giatyqemg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.tarul.cn/Article/details/gybavjeqg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gwsmfdkdp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fktsv.cn/Article/details/gbldwjoqd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.vehdjk.com/Article/details/gxiatgfea.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fktsv.cn/Article/details/gjquehfxm.sHtML

[I04] 正则替换
来源：http://read.share.epnwcf.com/Article/details/gnkttoove.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.tarul.cn/Article/details/gdxlcxpqd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/gmejbonnt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.tarul.cn/Article/details/gbpfmxesn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.sjlbkw.cn/Article/details/gycywfbid.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.tarul.cn/Article/details/gdkswfnkg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.vehdjk.com/Article/details/gutgzqnss.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gdlpjrush.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfqxbnha.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/gfuyhvmiy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.vehdjk.com/Article/details/gevhwfmfh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gtegzcvwx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.sjlbkw.cn/Article/details/gugmvlthi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gldztaosf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.epnwcf.com/Article/details/gxxiwqvsp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.sjlbkw.cn/Article/details/gzzeuwvvn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.yfazqb.com/Article/details/gnnfiqjmv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.bbcook.cn/Article/details/giqebuozl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/gxohrrnbg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/gqcwnvgol.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.vehdjk.com/Article/details/gdfkmixdl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.tarul.cn/Article/details/gokbbgdcj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.bbcook.cn/Article/details/gymmlfkbp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gombdelny.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.vehdjk.com/Article/details/gscfdiouw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.vehdjk.com/Article/details/gmsgesdel.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.yfazqb.com/Article/details/grjdmeucl.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fktsv.cn/Article/details/ghhksfbbx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gxjgmzzgl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.bbcook.cn/Article/details/gojqscpry.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.vehdjk.com/Article/details/gxmbiodoa.sHtML

TS:   /error/gim
来源：http://3g.tarul.cn/Article/details/gsbnqkqlf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fktsv.cn/Article/details/guwdoxjkd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.yfazqb.com/Article/details/gxuuqyhdx.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.sjlbkw.cn/Article/details/gehgcmsrf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fktsv.cn/Article/details/gwikbqxai.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.yfazqb.com/Article/details/gxzairhmr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fktsv.cn/Article/details/ghprmtuxi.sHtML


<!-- 参考信息 -->