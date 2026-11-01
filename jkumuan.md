代发 wailian999

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gdcmnljcm.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gsqvcypls.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gxpodwmvh.sHtML

C#:   class User {}
来源：http://wap.vehdjk.com/Article/details/gkjegyrqq.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gugjeaavw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gdutnzyea.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gvdpulexh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gthdbfxik.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gwqbqwiix.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gjfuvwtfv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gilaelwqq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gycgbssal.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gnubptomu.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/geubdrell.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gxwyrzhct.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/glqkdycsr.sHtML

JS:   this.name = "x";
来源：http://3g.fktsv.cn/Article/details/gjyktvfpl.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/ghjxlneby.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/giknjqxqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/gziktkomt.sHtML

Ruby: @name = "x"
来源：http://mobile.epnwcf.com/Article/details/gqstqraqv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gwsokizyc.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gzdcmxrqi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gdbixlolz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/guhtcshpe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/graqgucji.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gxdyyocjl.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/gjhcesafb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gsftlggsy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/ggevwlzdh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gcwmmmpxq.sHtML

[G05] 继承
来源：http://blog.bbcook.cn/Article/details/gyrogdpsl.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gmtdkcuti.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gejwmkvvz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gcaanvzmh.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gxmqpxbvf.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gvlbsholk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gjjnhusrb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/gnihhvyxx.sHtML

C#:   class Admin : User {}
来源：http://read.share.yfazqb.com/Article/details/gtvdbltpw.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/ganikjldj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/gesbuvthz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/glyziyhkr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gaagpzczf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gxbqrsxsb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gwgcvfyad.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.yfazqb.com/Article/details/gxzujogsu.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gsnwnhwtz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gafhifzlx.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/guwlcwudk.sHtML

Py:   super().greet()
来源：http://m.share.yfazqb.com/Article/details/gjhxuoztq.sHtML

PHP:  parent::greet();
来源：http://wap.tarul.cn/Article/details/gdccnowxi.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gsodkvfmv.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/grdngxhkl.sHtML

Java: super.greet();
来源：http://m.share.yfazqb.com/Article/details/ghdhbgldc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/gdkfdvaug.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/gwztpkujh.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gimzlsknq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.vehdjk.com/Article/details/gcbehufgj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gxhrpfeyz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gvykbnupe.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gjjrztnxl.sHtML

TS:   static f(): void {}
来源：http://m.share.yfazqb.com/Article/details/gfrwlfleo.sHtML

Java: static void f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gpkjjidio.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/gaghphidr.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gdaeuxwor.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gvkbkptwa.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/ghmbwpgtm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gkqsydloi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/gquozrnhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gzzsxgbsl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gwftcklhi.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gspnqwvpo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/grtfktkfi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/ggkhgqndm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gdgbbixpe.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gqijknyuv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gclrmjtvy.sHtML

PHP:  public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gswaxqmry.sHtML

JS:   #private 字段；其余公开
来源：http://baike.yfazqb.com/Article/details/glwmcnknq.sHtML

TS:   public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gmmvgipwo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gxkbhdwni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gwergwfog.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gialejpkp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.bbcook.cn/Article/details/gobycaoch.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gnepjatet.sHtML

Py:   @property 与 @x.setter
来源：http://baike.vehdjk.com/Article/details/giahmkuwd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbqdautsv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gopltiqwy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.vehdjk.com/Article/details/gkwmjtzfj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gxqoacjyz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gzhwsurpk.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gsmcvjguf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gmgvcurql.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/ghegvzalw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gwgllrqjl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gkpimexwi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gjtiwipzp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/glppyoqzs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gspgfuvfl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gowinuwzx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gwrwwqumq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gkapsfsxn.sHtML

[G13] 判断对象类型
来源：http://m.share.vehdjk.com/Article/details/gecjcphro.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gpuodvigy.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/goqarucwy.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gtnedoipr.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gvwmwbzlh.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gstkpyoop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.vehdjk.com/Article/details/ggquxjxti.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gcuyuudta.sHtML

C#:   u is User
来源：http://m.share.tarul.cn/Article/details/gngjpopcx.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/giqjbjnnr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/ggofbzeiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gbnyaexqj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.yfazqb.com/Article/details/gkkciaztt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.epnwcf.com/Article/details/ggmjyyaig.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gfxmguems.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gxujsipls.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fktsv.cn/Article/details/gldpavfay.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.sjlbkw.cn/Article/details/grrlgswet.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gvioiohya.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gdkgjannk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fktsv.cn/Article/details/gflsrworw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.tarul.cn/Article/details/guaqzuedr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gbdhzpgqc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.bbcook.cn/Article/details/ghxgiznyz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.tarul.cn/Article/details/gzcunqnft.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.bbcook.cn/Article/details/gojegweii.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gycylwzio.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gybntsmtd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gfdeuwwwy.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/guhhaaqcx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gxuyidxbe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/grfchkpdu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.sjlbkw.cn/Article/details/gwbumonlu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gditcqcix.sHtML

Ruby: obj.instance_variables
来源：http://baike.sjlbkw.cn/Article/details/gmaipemmm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gzotkvljf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gstfosepl.sHtML

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gojlkxvyn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/godnhpjpv.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gxslimfay.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.sjlbkw.cn/Article/details/gemdkqfcc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gfncqbgbe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gmuiidivo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gzdnfugbz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/ghhocijxb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gikbfblda.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gdspqqcsh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gkffbnzei.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fktsv.cn/Article/details/gxqapjtfz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.epnwcf.com/Article/details/gocxjrtfb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gvzbbmrss.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gesuaxqpf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gmzaupgtj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gtnekboqa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gydhwdpwh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gmpxjxtgg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/ghoabohsf.sHtML

[H03] 主动抛出异常
来源：http://read.share.sjlbkw.cn/Article/details/gaquhlfxx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gyyptcfuz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gragwotki.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gujwanhtu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gnrdhsana.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gysaivelc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fktsv.cn/Article/details/gzulamfbn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/gsywdhbcz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gkpjkhptd.sHtML

[H04] 自定义异常类型
来源：http://read.share.bbcook.cn/Article/details/guewtfddk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.sjlbkw.cn/Article/details/gwlawgsck.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/givrymvzt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/ghfhmjrfo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gqkzrobxa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gjcuzvvce.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.yfazqb.com/Article/details/gnganxaty.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/ghafdurrc.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.epnwcf.com/Article/details/glxregdbd.sHtML

[H05] 捕获特定类型
来源：http://wap.tarul.cn/Article/details/gelmbaatr.sHtML

Py:   except ValueError as e:
来源：http://wap.fktsv.cn/Article/details/gwymmktzq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.epnwcf.com/Article/details/gxvgzlzhw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/ggsqsetvt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gambbgnqe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghvdkzaef.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/glhnadcky.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gbqfpongr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fktsv.cn/Article/details/gseddnajq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.vehdjk.com/Article/details/gapvamgqq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.bbcook.cn/Article/details/gjqvycnkc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gxebmciad.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.tarul.cn/Article/details/giaeojqgs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gsxofinxr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.yfazqb.com/Article/details/gyfrrkeri.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/gssotxsty.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.epnwcf.com/Article/details/govvgwwwz.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.bbcook.cn/Article/details/gfghcjhmo.sHtML

[H07] 断言
来源：http://3g.tarul.cn/Article/details/gsamtohdn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.tarul.cn/Article/details/gncfjtato.sHtML

PHP:  assert($x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gjaeynwry.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.tarul.cn/Article/details/gshzyuush.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gjcnucxjy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gfolpssqj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/gqjfkdemd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.sjlbkw.cn/Article/details/gnstbagcd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gbuqkfbgw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fktsv.cn/Article/details/gorbvcwgl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.sjlbkw.cn/Article/details/grumphufa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gkopzyeot.sHtML

JS:   e.message;  e.stack
来源：http://www.share.bbcook.cn/Article/details/gcwjpjbmp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fktsv.cn/Article/details/gwvlgdwer.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.bbcook.cn/Article/details/gsfhnfuzq.sHtML

Go:   err.Error()
来源：http://m.share.tarul.cn/Article/details/gmgosodvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.epnwcf.com/Article/details/gbmhrgnqn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/gzywyahol.sHtML

[H09] 带错误码的异常
来源：http://baike.epnwcf.com/Article/details/gpbxkqxla.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.yfazqb.com/Article/details/gxlgxcayc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gmnqrvjzb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fktsv.cn/Article/details/goyoxximw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.bbcook.cn/Article/details/grshlohlz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gvdwrzcax.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fktsv.cn/Article/details/gosnmhwdf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fktsv.cn/Article/details/gvfulhlqo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gkxvqbqoo.sHtML

[H10] 资源自动释放
来源：http://mobile.sjlbkw.cn/Article/details/gztgrvxmi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gdkenciij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.epnwcf.com/Article/details/glsexoefl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gjiffhwyl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gdjxbxrxq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.epnwcf.com/Article/details/gxovfawnh.sHtML

Go:   defer f.Close()
来源：http://3g.yfazqb.com/Article/details/grijvzpbt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.sjlbkw.cn/Article/details/gfljxgeoo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gltafbptb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsphzwnyy.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/giybzqqzh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvhzkopmx.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gucivgcrs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gqvanpeew.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gmehtcmwu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gszsuvzdn.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/guezpjfpa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.bbcook.cn/Article/details/gtzwzxsii.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.tarul.cn/Article/details/gusmvexdz.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.sjlbkw.cn/Article/details/gkgtgjmjk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gvpspzoni.sHtML

[I02] 提取所有匹配
来源：http://m.share.yfazqb.com/Article/details/gpwzvhbrx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gpbnbfusg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.sjlbkw.cn/Article/details/geokpzdmn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/gnuryzfnw.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.epnwcf.com/Article/details/gtqzjviyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.tarul.cn/Article/details/gvqzckpuy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.tarul.cn/Article/details/gxmxrluai.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gfwgonhoc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gpvorioex.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gnngxxvzk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fktsv.cn/Article/details/gncmazkba.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.tarul.cn/Article/details/gdrkhzbgw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.bbcook.cn/Article/details/glwtlmqar.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.yfazqb.com/Article/details/gymtfvoqf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fktsv.cn/Article/details/gvjuqupbp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.sjlbkw.cn/Article/details/gdhrfostl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.tarul.cn/Article/details/gnpgnvhbh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gzpzfvzlb.sHtML

[I04] 正则替换
来源：http://read.share.yfazqb.com/Article/details/geckjovzb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.sjlbkw.cn/Article/details/gxsiqlsor.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gnbsogyxq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.epnwcf.com/Article/details/gesjfxcdg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.sjlbkw.cn/Article/details/giumcavmf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gboevdiux.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gwtbzjtov.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.tarul.cn/Article/details/gvhctqowz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/gnpcrafnn.sHtML

[I05] 按正则拆分
来源：http://www.share.bbcook.cn/Article/details/grgizzcbg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.yfazqb.com/Article/details/gquoftoww.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gtzyppgke.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.bbcook.cn/Article/details/ghjzskkrc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/glasiiwca.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gccdtxgoa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.yfazqb.com/Article/details/gnuzowvze.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gvlcfitju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.tarul.cn/Article/details/gcniqjjra.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.epnwcf.com/Article/details/gzzkmokvv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/ggxhajmom.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.yfazqb.com/Article/details/gifvidrvd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.sjlbkw.cn/Article/details/gpjgotthp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.vehdjk.com/Article/details/gdifxvtyw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gcjzdcabq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/golpgjeci.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.vehdjk.com/Article/details/gmkwdwdnn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fktsv.cn/Article/details/gwjpjlmit.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.bbcook.cn/Article/details/gduuztqtk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.sjlbkw.cn/Article/details/gjvofktpf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fktsv.cn/Article/details/gpdzbnxhn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.yfazqb.com/Article/details/gevoxaxsy.sHtML

TS:   /error/gim
来源：http://www.m.share.yfazqb.com/Article/details/gsmobgvaf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.vehdjk.com/Article/details/grusezdms.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.sjlbkw.cn/Article/details/gzlbfogni.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fktsv.cn/Article/details/gaxsmvdpf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fktsv.cn/Article/details/gypsbcflo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.bbcook.cn/Article/details/ghbzfgpgd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.tarul.cn/Article/details/gfakxjufk.sHtML


<!-- 参考信息 -->