代发 wailian999

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gvzjqxfmd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gwlgqojop.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gjvnnpanv.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gjmngausj.sHtML

[G02] 构造函数
来源：http://mobile.vehdjk.com/Article/details/gxgecaflh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/ghtbzczcc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glspeasvl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gphafrcsd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.bbcook.cn/Article/details/gusrqsyju.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gggtdnzon.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gvslcwlct.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.epnwcf.com/Article/details/gsqvdonmn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/giufbhsxq.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/genwfyztg.sHtML

Py:   self.name = "x"
来源：http://3g.fktsv.cn/Article/details/gduixrvbz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.bbcook.cn/Article/details/gwfzyykzf.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gyyfacmnn.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gqgflaoqb.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/giquzzbek.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gzlamqksu.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gehpxewqz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fktsv.cn/Article/details/goljmefsx.sHtML

[G04] 定义方法
来源：http://3g.yfazqb.com/Article/details/gqazuqztl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gbicegyzo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gpngiilkh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gavfodypb.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gqjvvourd.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gbwofoehe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gthewoyum.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gzsmihwpu.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gbxkmqkig.sHtML

[G05] 继承
来源：http://mobile.fktsv.cn/Article/details/govvmutvg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gydjqvsye.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gpflsqgrv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gxawlquhb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gstrzonur.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gvyoxdcfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fktsv.cn/Article/details/gjywztxvi.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/gytlmewit.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/ginybwryn.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/gqwzekiqa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.vehdjk.com/Article/details/gixoclrcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gicptoyop.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/giwiutcip.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/ghmfeiwcn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/guklrwdtp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/grjxykqpm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.vehdjk.com/Article/details/gzbulfhdl.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/guzvssmgc.sHtML

[G07] 调用父类方法
来源：http://www.share.fktsv.cn/Article/details/gqweuwlfc.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gjarqzqam.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gbzffhwcc.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gjtdrlkhb.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/grtvcvyhs.sHtML

Java: super.greet();
来源：http://m.share.epnwcf.com/Article/details/ghvvwyykx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/gvlknioiu.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gisldtshd.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gujiadapa.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gxubwutfz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/geqjjzasg.sHtML

PHP:  public static function f() {}
来源：http://mobile.vehdjk.com/Article/details/gxrwmljws.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gpmsklhxm.sHtML

TS:   static f(): void {}
来源：http://read.share.bbcook.cn/Article/details/ghazrgtvp.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfndjtngu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gylstsuxl.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gcisvdfqr.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gnwbzuece.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/guozzagxd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.epnwcf.com/Article/details/gfmewlsrv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/ggyyvlvtr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.epnwcf.com/Article/details/gntgsybyo.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gnusrcbwz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.vehdjk.com/Article/details/gihreiiyd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gegjutznz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gdnymyyov.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gqanywsop.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/ggkvepvgr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.epnwcf.com/Article/details/gswgifuul.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gubqfpznn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gtdmswslj.sHtML

TS:   public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gxyixffhi.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/gmerkfufy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/geyobdfgg.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/ghczmcvhq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.tarul.cn/Article/details/gqzpknflo.sHtML

[G11] getter / setter
来源：http://blog.bbcook.cn/Article/details/gtpzfvrbm.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/golsivhlo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gvseisvxq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gyhbuvhjp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.tarul.cn/Article/details/ggignmbac.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gmgdibefv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gjppmlnqi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gntcuqzij.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/giwuwyxoj.sHtML

[G12] 对象转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gobugzslu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.vehdjk.com/Article/details/gwbtrcgqg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gmvwljhvb.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gqcjchxbv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gqbbynzhf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gcozuulqo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gputdbeel.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gmbxorszs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.bbcook.cn/Article/details/gpqsrjrpl.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gwjuqklzq.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gvqvoscfd.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gqcwhnrkz.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gwywzzitp.sHtML

TS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gguhydmxr.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gihvqqttc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gqvmeaanx.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gblafvdls.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gqjupbcrb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gxtmerskz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.vehdjk.com/Article/details/groomlali.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/ghdjaergz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/gzrvwtroo.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gxmggbpmj.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gihibewel.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.epnwcf.com/Article/details/gjxzicrdo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fktsv.cn/Article/details/geawydfip.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gaykvikiw.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gkhbrjpls.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.tarul.cn/Article/details/grltojedr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.vehdjk.com/Article/details/grysdreim.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/gqlgbuphb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/gnqmzhmxy.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/gjtupxwbs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.epnwcf.com/Article/details/gekmqendw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/gdimgtopm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gwyqgalnd.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gyuyukhhd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gavhuvuni.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.epnwcf.com/Article/details/gkbouoeyn.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/guknqiyys.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/gurhqwnpk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.yfazqb.com/Article/details/gddednvbd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gunyrmdae.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.epnwcf.com/Article/details/gtqgecvxw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gmxxxkivi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmtwtebqi.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/grsymsjxe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzjkezwky.sHtML

[H01] try / catch 基础
来源：http://read.share.epnwcf.com/Article/details/gkkshvccf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/gglxitume.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gbthsudlb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gskvtarco.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gfrjrsjxc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.vehdjk.com/Article/details/gedwtjlbw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/ghdpelwut.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gfgjdpnsh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.yfazqb.com/Article/details/gldveyeju.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gvuvikssh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fktsv.cn/Article/details/goosrzysm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gffbkrink.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gkvsdwdfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdelqdlm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gtuzlsmbt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.bbcook.cn/Article/details/gyquixqvv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtxckbut.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/ghjydfych.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gjhkkjkwk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.tarul.cn/Article/details/gdjqmadus.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gdabhfwds.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gmbjpbrfn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gqipuvklu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gsprygkru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/gnzdbnxli.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.tarul.cn/Article/details/gszzobduw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gnozmfdto.sHtML

[H04] 自定义异常类型
来源：http://m.share.fktsv.cn/Article/details/gvgqqyfcy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gnowbfwlz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.tarul.cn/Article/details/gwxobrmex.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gasuxdfck.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/gxubumgxb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.tarul.cn/Article/details/gakulwtpn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gfrheqarh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gwotmwzgd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gmiqitqbw.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gpsdxaxsa.sHtML

Py:   except ValueError as e:
来源：http://www.blog.sjlbkw.cn/Article/details/gmoqgsnwm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gktnqoove.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gfsndacaf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gkqtmjube.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gunvffsqy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gezqfisjf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.vehdjk.com/Article/details/gaerbsypy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gymycxtsm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/ghvkmoxkv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gykybqynd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gcuwgcish.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.epnwcf.com/Article/details/gatvhevty.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gkaeoydyo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.yfazqb.com/Article/details/grstlvyio.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gxrxlkdhb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gbesvpjxz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gisbhtoir.sHtML

[H07] 断言
来源：http://3g.epnwcf.com/Article/details/gskcllabw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/ggpjcdvxj.sHtML

PHP:  assert($x > 0);
来源：http://mobile.sjlbkw.cn/Article/details/gsavskkaz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gvbyejcmz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gefwoipca.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.vehdjk.com/Article/details/gjingaeol.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gysmeopwx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fktsv.cn/Article/details/gyhbtqqmf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gdnuwdlwf.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.yfazqb.com/Article/details/gdgiqjqlb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.tarul.cn/Article/details/gwuvsxxsr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/glvrlkhot.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fktsv.cn/Article/details/gwiwcclhr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gzhbydacn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gosupsksi.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/glcuhyfvz.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.tarul.cn/Article/details/gwdmirwvf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/govrwhbpx.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/guoibsgyj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.yfazqb.com/Article/details/gysjkssiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.yfazqb.com/Article/details/gnqxjhzvt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.bbcook.cn/Article/details/gdxhsvyla.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.epnwcf.com/Article/details/gxuaudizk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gdkdjsrkp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.tarul.cn/Article/details/gzcngbqur.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.sjlbkw.cn/Article/details/gbcayeebg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gbzbxzldl.sHtML

[H10] 资源自动释放
来源：http://www.blog.bbcook.cn/Article/details/gkxsspspv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.epnwcf.com/Article/details/gqwmjqrpu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gjdswevtn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.tarul.cn/Article/details/grmklnnco.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.sjlbkw.cn/Article/details/gphblykxl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gztegvkks.sHtML

Go:   defer f.Close()
来源：http://3g.bbcook.cn/Article/details/ghlfcjbmb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.vehdjk.com/Article/details/gvuzjwwvf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gomclfftg.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gutfbcnyo.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gixwqvnfn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqwztjgwd.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gtaaqeeax.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.epnwcf.com/Article/details/glmkdxjku.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/gpghqgott.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fktsv.cn/Article/details/gsvdwvmjb.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghvxjzgit.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.bbcook.cn/Article/details/gouzmtold.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.sjlbkw.cn/Article/details/gmagmpncw.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.tarul.cn/Article/details/gidjdcuqy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.sjlbkw.cn/Article/details/ghwibiadk.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gftredoeg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.vehdjk.com/Article/details/gnbehchvh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fktsv.cn/Article/details/gnrthuxmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.bbcook.cn/Article/details/gzdqupzmx.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fktsv.cn/Article/details/grdyogkkf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.tarul.cn/Article/details/ghllkkwwx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/gliaifubr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fktsv.cn/Article/details/gpbaegejr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdclxupqo.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.bbcook.cn/Article/details/gxjtmtxig.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.tarul.cn/Article/details/gybigoqvr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.vehdjk.com/Article/details/gzwzkhbfz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.epnwcf.com/Article/details/gqvwjiuaj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fktsv.cn/Article/details/gxmhkosvn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.yfazqb.com/Article/details/gvfecoyjp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/ghtfxivyv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/glpownkag.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.sjlbkw.cn/Article/details/gcjeruyty.sHtML

[I04] 正则替换
来源：http://www.m.share.yfazqb.com/Article/details/gpxmrsgjr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.sjlbkw.cn/Article/details/gmjkyfsrs.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gylvubfaa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fktsv.cn/Article/details/gyjdjdmzm.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.epnwcf.com/Article/details/gfzpatawd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/geshzeong.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.vehdjk.com/Article/details/ggulwnlac.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.yfazqb.com/Article/details/gdrzdjsvb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/ghjhbffjm.sHtML

[I05] 按正则拆分
来源：http://www.share.tarul.cn/Article/details/gusozrvwy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.sjlbkw.cn/Article/details/gcrqpxmfc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gjmtwpvpy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gaofjtqbb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/gjurzderp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.bbcook.cn/Article/details/glrrqttyo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.epnwcf.com/Article/details/gleqttilx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.tarul.cn/Article/details/gqdrhjohg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.yfazqb.com/Article/details/glscwryox.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.vehdjk.com/Article/details/glhtnznis.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.bbcook.cn/Article/details/gijhgwvxn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fktsv.cn/Article/details/ghnmhqcos.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.epnwcf.com/Article/details/gusenofkg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.sjlbkw.cn/Article/details/gfevgvzfl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gkqbkxynr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.epnwcf.com/Article/details/gbmtjkccl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fktsv.cn/Article/details/ghtfwymwv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.sjlbkw.cn/Article/details/gbxwjipdk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fktsv.cn/Article/details/ghljgekof.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.yfazqb.com/Article/details/guiquykby.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.sjlbkw.cn/Article/details/gqkmxokbi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.bbcook.cn/Article/details/gtdhfvoqq.sHtML

TS:   /error/gim
来源：http://wap.tarul.cn/Article/details/gdgryudtb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.epnwcf.com/Article/details/gfvrdkdkp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.yfazqb.com/Article/details/gzocgcyys.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.tarul.cn/Article/details/gduwvphph.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.sjlbkw.cn/Article/details/giwloejft.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.sjlbkw.cn/Article/details/grtptzwsu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.yfazqb.com/Article/details/ghcckrzbz.sHtML


<!-- 参考信息 -->