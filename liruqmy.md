代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gdnuzjbfp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gsopjleul.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gzmzerteq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.sjlbkw.cn/Article/details/gxrupwsga.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gxgsqdmpv.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gebyitbtd.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwlnuzqbl.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gvsjbqhtg.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gsclivuhg.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/ggovuwsse.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gxmmqnckb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fktsv.cn/Article/details/gspynfzxs.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gofdbcibr.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gbrzizrfy.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gjfrxczlr.sHtML

C#:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gvzbkhfgy.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gltlqpceq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.epnwcf.com/Article/details/gefajxxrn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gctzmeivo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gsrjtbkvt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gewuzvmpv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gwrmltnyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gakestjyt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/goqucxyno.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gytuxstpr.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gvzafetyo.sHtML

Py:   self.name = "x"
来源：http://blog.vehdjk.com/Article/details/ggevgyfvc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/glesvkvwy.sHtML

JS:   this.name = "x";
来源：http://baike.vehdjk.com/Article/details/gvfobftez.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gdvwodfmq.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gbjhpchlu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gfuigmqze.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gdbwwoefw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.sjlbkw.cn/Article/details/gtodghfvv.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gzunntkvy.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gwltyrvqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/goooyqzcs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gztlxcpod.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gpoayveye.sHtML

Java: String greet() { return name; }
来源：http://3g.vehdjk.com/Article/details/gebdfyhub.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/ghjeipghj.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gqwatcsyl.sHtML

C#:   public string Greet() => Name;
来源：http://baike.epnwcf.com/Article/details/gkhsqqoyg.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gfyqvfxiu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gejoznggz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gohoamsnf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gytpjztjp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gyxigvema.sHtML

Java: class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/grwiiqybl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gdjuhzcoz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gxrogdubi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/grhqhwtic.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/gahoznuha.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.sjlbkw.cn/Article/details/gqlxzzcot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gwpvflwmf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gxszqagvq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gkzpcndnw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gehkhxntm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fktsv.cn/Article/details/gqwpsoguw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gxrzjjkkq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/ggcmtalqq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gpwjssnbq.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/gcunbwlbg.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gqgmbrbiy.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gaphecrfd.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gfsugmswb.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gknkhlpgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gewdutjxq.sHtML

Ruby: super
来源：http://blog.epnwcf.com/Article/details/guikcqjyk.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gwwycwdpp.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gvzhcopcy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gzhdeqtjq.sHtML

PHP:  public static function f() {}
来源：http://read.share.yfazqb.com/Article/details/gcbogmmqf.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gmrryjnnl.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gwiurzeuj.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gofihouql.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.sjlbkw.cn/Article/details/gkiaxqvve.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gwudarfgv.sHtML

C#:   public static void F() {}
来源：http://m.share.bbcook.cn/Article/details/ggerdmxeu.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.tarul.cn/Article/details/gnkypjexd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.bbcook.cn/Article/details/grbukxsns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/grkfuscae.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gtqluyaov.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/gjnnnbuad.sHtML

Java: interface Shape { double area(); }
来源：http://3g.vehdjk.com/Article/details/gjukvgevi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gdygoyveb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.sjlbkw.cn/Article/details/gxlpgacsg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/gkwqskjvb.sHtML

[G10] 访问控制
来源：http://read.share.yfazqb.com/Article/details/gsrpouzww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gyljwejyb.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gkyhdlkvt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gaamuzlgw.sHtML

TS:   public / protected / private
来源：http://blog.bbcook.cn/Article/details/gummfgcxq.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.tarul.cn/Article/details/ggkfqatiq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.bbcook.cn/Article/details/gfuqxvgvj.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gatiustbb.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/ggkrewvnw.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/ggzqvoiik.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gdkqeblzz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gewaaskfw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gqawawnut.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gagfvduao.sHtML

Java: public String getName() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gbtykvxbn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gdgkukmvk.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gdqvmorla.sHtML

C#:   public string Name { get; set; }
来源：http://baike.tarul.cn/Article/details/gongzdjyd.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gdmwuxtgd.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gyxefggxr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/guiscpnmt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gphojbwfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtgfntzhp.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gmfctgzqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gbzovfezn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.epnwcf.com/Article/details/gmuvshyhr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.yfazqb.com/Article/details/gxryqhhzz.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gdnzxuxdi.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gqjdxqcep.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/grxvqeplf.sHtML

JS:   u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gruumjwmn.sHtML

TS:   u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/glbfgzved.sHtML

Java: u instanceof User
来源：http://3g.bbcook.cn/Article/details/gvzzxfffd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/gghvotvey.sHtML

Ruby: u.is_a?(User)
来源：http://3g.epnwcf.com/Article/details/gtlgqqpga.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/glfmknpfm.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/glxdpljqi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.yfazqb.com/Article/details/gkqsflleo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.bbcook.cn/Article/details/ghpgpayvv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gjmjbeihw.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/gpswbhwki.sHtML

Java: record User(String name, int age) {}
来源：http://3g.bbcook.cn/Article/details/gznpmoutp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gxaadeywb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.tarul.cn/Article/details/gswiqvbwc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/grojzbwns.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gfjusucie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.yfazqb.com/Article/details/gdgzkqukc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gzpheyice.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/gizxsgifm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.yfazqb.com/Article/details/giagazjrq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.tarul.cn/Article/details/gefjinxyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/gqkpjiolo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/ggbrtllvo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/grrxuzjiz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fktsv.cn/Article/details/gewbvwqey.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gduazgfbo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gdmunqfco.sHtML

JS:   Object.entries(obj)
来源：http://baike.yfazqb.com/Article/details/gnsuedbbf.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gjwdgujrp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.epnwcf.com/Article/details/gjuuxkuje.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gwuvunasg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/gjrrsozis.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/grpjwgehx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmlptcqgd.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gnxjzfkdd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/guorkryhz.sHtML

[H01] try / catch 基础
来源：http://mobile.sjlbkw.cn/Article/details/gcyasnghz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gamtthhgb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.tarul.cn/Article/details/giwiqmily.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gxzyngmxu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/grfqploju.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gujxqyjtf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.epnwcf.com/Article/details/gzxfxvmqs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gzuqungqi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gotplkfhz.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/geyttppso.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.tarul.cn/Article/details/gwfgkqllo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gjwsduqwi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gjgqzhfoj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gxwovcsuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gcjikuprr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fktsv.cn/Article/details/gipiavgjy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.sjlbkw.cn/Article/details/glmjevjea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gtgsqzxeq.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/ghzwqcjlf.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/gdumqatlt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/ggmzmnobf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gcgczskgp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gavyxvogj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gldernmpp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gcejyfxfa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.bbcook.cn/Article/details/geaikypur.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/grsjegrmm.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gsyizunsr.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fktsv.cn/Article/details/gxfoocrbu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.vehdjk.com/Article/details/ggxgtmvva.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gnitdtapy.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gfokscuio.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gvpahwocn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/guqbeubhe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fktsv.cn/Article/details/guhtsvxmi.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/glpdjyckz.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gqgmeqctw.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gcfpxwyao.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gqekiwnng.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.yfazqb.com/Article/details/gtdznjrsi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.tarul.cn/Article/details/glsrqsths.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.yfazqb.com/Article/details/grsoowvql.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gccgwgrcd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gqlttlvcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.yfazqb.com/Article/details/gfpefjxxn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gklcnlnus.sHtML

Py:   value = d.get("k") or default
来源：http://blog.tarul.cn/Article/details/gjrmvsjvi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/ggqyxyxri.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gkurxlzxj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gojffaycu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gjezpnxer.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fktsv.cn/Article/details/gavgdtxod.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gdmfcghvk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fktsv.cn/Article/details/gzojshylz.sHtML

[H07] 断言
来源：http://www.blog.tarul.cn/Article/details/gfpxsrhuq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.sjlbkw.cn/Article/details/gtcgcxpxb.sHtML

PHP:  assert($x > 0);
来源：http://3g.sjlbkw.cn/Article/details/gmymdkpfq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/ghuzclkas.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.vehdjk.com/Article/details/ggrieaaec.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.yfazqb.com/Article/details/gjeqhczgx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gqwxdflwy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.bbcook.cn/Article/details/gtlnhgquj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/ghbppkaim.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.vehdjk.com/Article/details/gruhdrysi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gdlcrkdbc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/ghjfrefyt.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gzbenaulk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.vehdjk.com/Article/details/gkeonbale.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gqqduuzmg.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gdleaxrtd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.bbcook.cn/Article/details/gdsurfxvo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gijumkvzb.sHtML

[H09] 带错误码的异常
来源：http://read.share.fktsv.cn/Article/details/gbyweughc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gzvygwfpa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.epnwcf.com/Article/details/gegsvhzft.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.bbcook.cn/Article/details/gdryelwgd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.epnwcf.com/Article/details/gssedfhhc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gaunpqsfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gzebuyonm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.yfazqb.com/Article/details/gylspqluo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fktsv.cn/Article/details/gihgouwbi.sHtML

[H10] 资源自动释放
来源：http://blog.yfazqb.com/Article/details/grkpbwvdt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdmdyhqc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.bbcook.cn/Article/details/gibbuvirp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gxicaeput.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.epnwcf.com/Article/details/gitwstteq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.vehdjk.com/Article/details/gydihhzyc.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gpblxwram.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.bbcook.cn/Article/details/glqexiawz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/guwobpxrb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsppbijrq.sHtML

I. 正则表达式
来源：http://www.share.fktsv.cn/Article/details/gmmjheppc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmldwmvzk.sHtML

[I01] 判断是否匹配
来源：http://blog.tarul.cn/Article/details/gpljnkydx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fktsv.cn/Article/details/gmsfssqlg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gxqfnqewy.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/ghkbcvktl.sHtML

TS:   /\d+/.test(s)
来源：http://baike.yfazqb.com/Article/details/gjmngmpys.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.tarul.cn/Article/details/gkbvlitlm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fktsv.cn/Article/details/gsmigmmac.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fktsv.cn/Article/details/glylkstcd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.epnwcf.com/Article/details/gukqhyacr.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gutfdycej.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gowzepbfl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gwfyieqph.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.epnwcf.com/Article/details/giohsokma.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.bbcook.cn/Article/details/gljexsbmw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fktsv.cn/Article/details/grifktkfz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fktsv.cn/Article/details/gicufextc.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/ghuckgsxu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.bbcook.cn/Article/details/gypumjmyf.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gjrwwiwrp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.tarul.cn/Article/details/gjsevksqr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.epnwcf.com/Article/details/gwbndriwy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.sjlbkw.cn/Article/details/gqnpwdcad.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fktsv.cn/Article/details/gjyprglwq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.tarul.cn/Article/details/gvrphppbe.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.yfazqb.com/Article/details/gqupstmkp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gtqufxjzn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.sjlbkw.cn/Article/details/glkzpwacu.sHtML

[I04] 正则替换
来源：http://baike.epnwcf.com/Article/details/gqpjqyjly.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.epnwcf.com/Article/details/gpeyjecvf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gjdomlwtb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.bbcook.cn/Article/details/gsfualflt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fktsv.cn/Article/details/gerkiigty.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gqadyxqol.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.tarul.cn/Article/details/glwpodxby.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.epnwcf.com/Article/details/ghhabnflh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.epnwcf.com/Article/details/gvdlaxoow.sHtML

[I05] 按正则拆分
来源：http://www.blog.vehdjk.com/Article/details/giiuukzlg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.yfazqb.com/Article/details/gkxhiamae.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.epnwcf.com/Article/details/gwnlzsjqx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/gvbpbatno.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gwwqqwoke.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.yfazqb.com/Article/details/gahormatm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvwmayul.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.sjlbkw.cn/Article/details/gegwreblu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gabiozmbf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/gsnpkdimx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.bbcook.cn/Article/details/geadyygkb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.vehdjk.com/Article/details/gcjidsfeo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fktsv.cn/Article/details/gjfpvekqa.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gwozqbbvs.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gknrjpgok.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.epnwcf.com/Article/details/gwywhtbuf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.tarul.cn/Article/details/gwxrtmojf.sHtML


<!-- 参考信息 -->