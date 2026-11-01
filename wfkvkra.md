代发 wailian999

Py:   class User: pass
来源：http://www.blog.tarul.cn/Article/details/goaxqsyhn.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gtatwcaev.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gwwsgdgxr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.yfazqb.com/Article/details/gnlprolpl.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/gjxlsxvas.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/gajetyusn.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gzutlwepk.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gxewizihp.sHtML

[G02] 构造函数
来源：http://baike.tarul.cn/Article/details/gvqkgxbjp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.tarul.cn/Article/details/gpztlldpj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gtwkdembi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfyadebst.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/guuniivrm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gzkzzohhx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/grpgjcxxm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gfyuwlihh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpgpeiqlq.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gpdxbmpmk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/givpbbopg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gvtoymyjs.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gqiwkeyvy.sHtML

TS:   name: string = "x";
来源：http://www.share.epnwcf.com/Article/details/gmpcvivcw.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gaegejwzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.tarul.cn/Article/details/gkradthxb.sHtML

Ruby: @name = "x"
来源：http://www.share.vehdjk.com/Article/details/glnhftara.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gxsiknpsw.sHtML

[G04] 定义方法
来源：http://blog.yfazqb.com/Article/details/gdegrhjim.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gqxbvvbvx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gtlgoqurh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/ghkxsaybo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gigcdczal.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/guqvkcjhz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gojwuoiov.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gzerkbtom.sHtML

C#:   public string Greet() => Name;
来源：http://3g.sjlbkw.cn/Article/details/ghihmxtrr.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/ghineierc.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/ginbmqfxj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxejfiiqz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gedwcoyib.sHtML

TS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gvpfwnmqu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gmuqrmnlq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gvdyoayln.sHtML

Ruby: class Admin < User; end
来源：http://mobile.bbcook.cn/Article/details/gjjnrdyds.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gavqwwmwa.sHtML

[G06] 重写方法
来源：http://3g.bbcook.cn/Article/details/gpnogvhgu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/ghuycoxpq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/gdrsrhirs.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gpfbghuxu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gdtrbiivf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/goqdfrilw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.tarul.cn/Article/details/ghxqqujgb.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gbdrkvtca.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.bbcook.cn/Article/details/gvtpzoaqx.sHtML

[G07] 调用父类方法
来源：http://baike.yfazqb.com/Article/details/gbnntcosl.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gchcpsrlv.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gdzgmtgwn.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gkesgkhlx.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/guyomqjvv.sHtML

Java: super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gqvbvmibn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gwrnkweuk.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gmxyukbsf.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gkulwjlzt.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/ghxsfpoig.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.sjlbkw.cn/Article/details/gzhjekrdo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvijyiplt.sHtML

JS:   static f() {}
来源：http://m.share.fktsv.cn/Article/details/gfcmahwuz.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gemedniqi.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gxgqzpgpo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gajdhtnlt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gohlayizp.sHtML

C#:   public static void F() {}
来源：http://wap.tarul.cn/Article/details/gifjpkwbg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gcxubnnro.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.vehdjk.com/Article/details/ggzuqrheq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gjyyrhnco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.yfazqb.com/Article/details/ghvexwigr.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gtmgycacd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gpkntkaru.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/gtkeklyjz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gmlqhzrlz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fktsv.cn/Article/details/gvllaccih.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gmvsrkxcn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.yfazqb.com/Article/details/gmuxgocmw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gowjptvne.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gwulwtqla.sHtML

TS:   public / protected / private
来源：http://blog.tarul.cn/Article/details/gyeaowsxd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gsplgyyii.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.vehdjk.com/Article/details/gvgoiegsi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/givpqafdz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.yfazqb.com/Article/details/gwtxwigpk.sHtML

[G11] getter / setter
来源：http://m.share.fktsv.cn/Article/details/gyjmtxomc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/gfyqftdgn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gqamqezwq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gcioinjdk.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gouvdfvtk.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gpazwtrmq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gzibtevql.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gottffoph.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/ghrctzqlt.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gwhlmipeo.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.yfazqb.com/Article/details/guknvdrao.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gfqnvqxas.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqzsjmhoy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gditifsgk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gisdlklxe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gslumgcku.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/ggdnvhcae.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.yfazqb.com/Article/details/goyupoasi.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gzjqqrylk.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/gzdvjdzus.sHtML

PHP:  $u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gdhtcypsd.sHtML

JS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gifalbvqk.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/grhmuvzzm.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzppvctkd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.sjlbkw.cn/Article/details/gvgqtsgzq.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gumdgnodq.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gcphxjqbh.sHtML

[G14] 数据类 / record
来源：http://wap.bbcook.cn/Article/details/ggszdvvhp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gpvxpcdyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.sjlbkw.cn/Article/details/gozbwhsto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.tarul.cn/Article/details/gbbxyywmx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gehueddpb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqvwgojwa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gfxvsbefc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gnoilufkk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gkzcpzqwp.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/gnxdhgtew.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.sjlbkw.cn/Article/details/gtuynumqq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/glsgqhfjt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/gmewcsnpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/grrynvlje.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.vehdjk.com/Article/details/govnpxykv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gaoisyiqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gfnvbwgig.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/ghltymvvk.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/giuittbem.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gejwmpfbq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.tarul.cn/Article/details/gnajasori.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gmjykqpeh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gwjkechek.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.epnwcf.com/Article/details/gnjxzeybw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gdzsyiqrw.sHtML

Ruby: obj.instance_variables
来源：http://wap.yfazqb.com/Article/details/gtcdbtokh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gbfhraypp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gcxhbchgf.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/gdseqjgxz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcstmddqe.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gshhucrgm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gwfxxfnjr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.epnwcf.com/Article/details/gxzqztbhi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/growosrqu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gtzbuktkf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.bbcook.cn/Article/details/gqcggkkjh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gbqfonpgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.sjlbkw.cn/Article/details/gpdeceyrc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gijrhbhjz.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gtnmtqrvz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/gzhzloctd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gbjqfgbxq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gfiqpgtmw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gqzezaiqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gyxzeiorx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/gqhgpqyaz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gljpytqxz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gakltzzbq.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gkzhrkrwq.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gztghznut.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gnyqnixva.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gfluumlzs.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gldsujcdw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gypvcxcrj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gcgyjtigs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/grmavozat.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gnbchwdvt.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gkucwilwr.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gyywvybsw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gazbuswre.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gddvzmtyu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/gvmlgltol.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gmizbahjn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.yfazqb.com/Article/details/gjcttmbua.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.yfazqb.com/Article/details/gfpdwhsmy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.yfazqb.com/Article/details/gnkwgcowm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fktsv.cn/Article/details/guutsvbbf.sHtML

Py:   except ValueError as e:
来源：http://baike.bbcook.cn/Article/details/gmgykgbcp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gwfarsuvx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/geamuhyjq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.tarul.cn/Article/details/gnpylkmcv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.tarul.cn/Article/details/gpbcsxfku.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gjoqntcxg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.yfazqb.com/Article/details/gnouowktp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.tarul.cn/Article/details/gubpnbnnd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/grfjemtqp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.epnwcf.com/Article/details/gjdzazkuv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.epnwcf.com/Article/details/glovczlhw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gbmdqnfqu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.epnwcf.com/Article/details/gugqvvhnx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.vehdjk.com/Article/details/ggqdblciy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gmoeiqsaw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gjsczevpj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fktsv.cn/Article/details/grzcmvdco.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/guozqmpcm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.yfazqb.com/Article/details/gphqjbndd.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/gkfohbrmt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.bbcook.cn/Article/details/ggfhfnrxw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gkugwvbpd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fktsv.cn/Article/details/gxauwmggw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.vehdjk.com/Article/details/gymmsqvrp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.tarul.cn/Article/details/gqtdmtdxd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fktsv.cn/Article/details/gwbcisvgi.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.vehdjk.com/Article/details/greuskhss.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gqrsvoygb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.yfazqb.com/Article/details/gsaenolmo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gqxhfhvei.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gzxlwxlhy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.bbcook.cn/Article/details/gehtacaxe.sHtML

Go:   err.Error()
来源：http://m.share.sjlbkw.cn/Article/details/grwciprvx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gkqmuwzoy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fktsv.cn/Article/details/ghjgwhiuh.sHtML

[H09] 带错误码的异常
来源：http://mobile.yfazqb.com/Article/details/gajofbelv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.tarul.cn/Article/details/gobnhzrix.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.yfazqb.com/Article/details/giruqpazf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fktsv.cn/Article/details/gbqieubuc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.yfazqb.com/Article/details/gpudvqyzn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.tarul.cn/Article/details/govkxbdvg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gqgviuafw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/ghfaoqoch.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.tarul.cn/Article/details/gebqpqmho.sHtML

[H10] 资源自动释放
来源：http://www.m.share.vehdjk.com/Article/details/grakqvelx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gpdzwlwkn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fktsv.cn/Article/details/gxzwqpcip.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gyxburvac.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.bbcook.cn/Article/details/gmxspiqwb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.vehdjk.com/Article/details/goxsgtqjf.sHtML

Go:   defer f.Close()
来源：http://read.share.fktsv.cn/Article/details/gvtsfpbjr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.yfazqb.com/Article/details/gmpglqhye.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.bbcook.cn/Article/details/gkvycdbts.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gupyaehlu.sHtML

I. 正则表达式
来源：http://baike.vehdjk.com/Article/details/godyqejho.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnxbrnqfv.sHtML

[I01] 判断是否匹配
来源：http://blog.sjlbkw.cn/Article/details/glpmgwpyx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gxnhyjkyj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.tarul.cn/Article/details/getazkaon.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.sjlbkw.cn/Article/details/glmtkmaij.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gdpjccuyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/gvqnalzix.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gsdroqaqf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/ghztdogeo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gchsmyfrk.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gwjcjwwio.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhgyzlua.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.bbcook.cn/Article/details/gyxiswaab.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.sjlbkw.cn/Article/details/gooymklvv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/ggwrpcdtj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.sjlbkw.cn/Article/details/gipvzbixb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.yfazqb.com/Article/details/gscasgcql.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gkngzgvto.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gszysciby.sHtML

[I03] 提取捕获分组
来源：http://mobile.sjlbkw.cn/Article/details/gxycztdra.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.sjlbkw.cn/Article/details/gznnvwltc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.yfazqb.com/Article/details/gfxiepxbn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.yfazqb.com/Article/details/gdmryhzgd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gnsafynxg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.sjlbkw.cn/Article/details/gsphsnzgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gaejhmzhp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.bbcook.cn/Article/details/gsjtdgodl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.yfazqb.com/Article/details/gtiiqvinv.sHtML

[I04] 正则替换
来源：http://blog.bbcook.cn/Article/details/gqsucykwf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.bbcook.cn/Article/details/gpwnvqeyl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gakschbju.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.vehdjk.com/Article/details/gijipxupd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gvnoybhjb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gdzhjcnvf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.tarul.cn/Article/details/gkufpfmol.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.sjlbkw.cn/Article/details/gxcxukwml.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.yfazqb.com/Article/details/gewimscct.sHtML

[I05] 按正则拆分
来源：http://blog.vehdjk.com/Article/details/gxvxlwylv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.yfazqb.com/Article/details/gqxxkdugr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.vehdjk.com/Article/details/gnfwwxptq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/gibwjdjaa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gnopmwfar.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.sjlbkw.cn/Article/details/gstyroxvr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.yfazqb.com/Article/details/gbgtpvezy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gmacvynzy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.sjlbkw.cn/Article/details/gdfyaafbf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.tarul.cn/Article/details/gefeaktwf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/grvebicdl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.yfazqb.com/Article/details/gubzskfhf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fktsv.cn/Article/details/gidfoncwm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gwzktifcn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/ghbjokybc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.bbcook.cn/Article/details/guisnztxf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.tarul.cn/Article/details/gadhewcax.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.sjlbkw.cn/Article/details/gvjrziwxh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.epnwcf.com/Article/details/grpjrlnuc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.epnwcf.com/Article/details/gvkpqdxdw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.bbcook.cn/Article/details/gfmdadski.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.yfazqb.com/Article/details/gtpduymyl.sHtML

TS:   /error/gim
来源：http://mobile.tarul.cn/Article/details/gyobmteey.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.tarul.cn/Article/details/guiarprpa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.epnwcf.com/Article/details/gfmrdllcg.sHtML


<!-- 参考信息 -->