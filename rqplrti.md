代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gehdulwyh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gmpexpkrp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gntkeutxd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/gepesrtai.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guetalmtb.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/gnbjtteum.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkbnbokmx.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gdigzqodx.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gmzckyvnr.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gcvjubujw.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/ggeftdblt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gqpseifvl.sHtML

Java: class User {}
来源：http://mobile.fktsv.cn/Article/details/gybxgrcsp.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gbnhzgpbe.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gquvlxnva.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gcbqmpchc.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/ggzqprguj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gbscmcvyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gtsxiukng.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gxuyfpnwy.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gboljfyum.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gprwuswgb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gwdbdprez.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/geaiwjtrp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gvioebmzk.sHtML

[G03] 实例属性
来源：http://www.share.yfazqb.com/Article/details/gnyvqpvmm.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gszmxmfoi.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gpgrsuyxf.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gvqubtqnw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gxkljxodr.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gxjzqfdxr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/ghjfpwlym.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/gogzxziss.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gvbgeatck.sHtML

[G04] 定义方法
来源：http://read.share.tarul.cn/Article/details/gsiwgrypn.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/gnllcfide.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcrykvuym.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gdjaktwkj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gfvioqnxc.sHtML

Java: String greet() { return name; }
来源：http://baike.vehdjk.com/Article/details/gcsliqmqf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gfcrvuzcn.sHtML

Ruby: def greet; @name; end
来源：http://blog.vehdjk.com/Article/details/gpfxlinpw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/gltlmyems.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gltlzvzvj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/girxavabo.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/grimqfrhl.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gzgchfvoa.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gupfrqaub.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/ggiertswe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/grawloyht.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gbsicfevw.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gvgrvchad.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/gxkkkcmxr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gibpxalos.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gqnbdzljn.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gulioqano.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gqwgutkwz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gjbtykzli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gmlcabgzm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/grxuvoald.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gooeujfzf.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gyynqmakj.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/geoztgjsb.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gxyaxykvi.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gjzjrebwo.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/gfcvoyrnx.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gzbfrqfko.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gfuqvuveu.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gbpibrgtb.sHtML

C#:   base.Greet();
来源：http://wap.epnwcf.com/Article/details/gatqiqydm.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/ggfjpywaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/gpjraqpvp.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/ghklhuume.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gnvxvzucj.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gtdzeilty.sHtML

Java: static void f() {}
来源：http://blog.epnwcf.com/Article/details/gbbnkcaeu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gekjyrzjr.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gchszmcjt.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gxcewfuhf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/guusdhotn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.tarul.cn/Article/details/gwmtzxboy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.vehdjk.com/Article/details/gqwkhybuf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/gqbnaymhs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gvueldgft.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gddvpyuux.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/ghrtykdwm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gzlirglvz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gprivkanc.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gvphjupgb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fktsv.cn/Article/details/gbclxraur.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/ghtacjgyg.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/gghxdphho.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gdntmpgaz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gjvfyalwk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gmitcvfte.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gbkrugseo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.sjlbkw.cn/Article/details/ghaqyoddr.sHtML

[G11] getter / setter
来源：http://www.share.tarul.cn/Article/details/gqmgpmutr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/glztydynd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gwqndpnvn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gnpbdvatt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gcuinlcaj.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gyyrvpyiu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gxjyfkrzt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gateavpav.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gbaefynco.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gpgirablt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.bbcook.cn/Article/details/gxrxfjmag.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/ghlacnwvb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/glkswbmrf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gcvwgxwnn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gvzxpijpl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gqhpkgslw.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gezkcpdds.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fktsv.cn/Article/details/gdiykxbqx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gyqfyssfy.sHtML

Py:   isinstance(u, User)
来源：http://wap.tarul.cn/Article/details/gcrtxxgnt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gtuznyftu.sHtML

JS:   u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gaevomctx.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gnlzvygip.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gsuvjngye.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gaxeyarqu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gxdyvzsrw.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gicmkrczs.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/ghdtwacfs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gwzhqhyly.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gynjwcngk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.yfazqb.com/Article/details/gofyeenpe.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.bbcook.cn/Article/details/gphayxhie.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gwnjqpkbu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gipnqitgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.bbcook.cn/Article/details/gtokqmwml.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.epnwcf.com/Article/details/gfpiqsccs.sHtML

[G15] 枚举
来源：http://mobile.fktsv.cn/Article/details/gabwfrsvu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gkvvznzrc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gdmbzvbwz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.yfazqb.com/Article/details/gaprbfjqt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/godrolhoq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.sjlbkw.cn/Article/details/gexyaclme.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gnhyuuvnl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gkhckvifs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gakobswvr.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/ggtodsigo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gnmrmwjzb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.sjlbkw.cn/Article/details/gcbclzkri.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/ghqvkibxp.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gofejhmwj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fktsv.cn/Article/details/gnzrlvkge.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gwjdwpdst.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gcnpibkxf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gejdvrfub.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcmofxdva.sHtML

H. 异常与错误处理
来源：http://3g.bbcook.cn/Article/details/gblzjgael.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggtroaqkh.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gsbjbfdfg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/ghhtpwlap.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.bbcook.cn/Article/details/gdewnblqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/glolgjzjy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/guqjazjlx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/getylponp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.vehdjk.com/Article/details/gqluvqxdh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.bbcook.cn/Article/details/gsaoopccx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/glqqthbjq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gqompvbyb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/guizopdmj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/grqkstklo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gsquszyre.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gvoordulp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gznwhhhdh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/gnluhirub.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gmfucellf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.yfazqb.com/Article/details/gvrqmamup.sHtML

[H03] 主动抛出异常
来源：http://read.share.yfazqb.com/Article/details/gbsonlrnp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gjfhsncas.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gytnwfsjf.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/ghbkitffr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/geyxexkte.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gkxsihzhr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/giiafmhrc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gbcmqthce.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gfufozrun.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gfwbpddjs.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.tarul.cn/Article/details/gntdeaouw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gyujtsvqu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gmmscgduc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gqedftivg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gyfszpelj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fktsv.cn/Article/details/gnaeomkuk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/ghenggjyw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/grmjagocj.sHtML

[H05] 捕获特定类型
来源：http://www.share.bbcook.cn/Article/details/ggahkxcza.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gqctvtquj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.bbcook.cn/Article/details/gxkicxnyu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gdhefgajv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gcbzijkro.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/ghrdvvliu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.yfazqb.com/Article/details/gmybecjoh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlcvxdgl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gfambefwc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/godpqkykx.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.vehdjk.com/Article/details/gnoqxvmns.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/glibgvuql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gwgreegqd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gnrsnkuto.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.tarul.cn/Article/details/gyaqsbjyc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.tarul.cn/Article/details/gavagduim.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/guxoweodk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.epnwcf.com/Article/details/gyhfkljjs.sHtML

[H07] 断言
来源：http://wap.yfazqb.com/Article/details/gziudysfz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/ghrravshs.sHtML

PHP:  assert($x > 0);
来源：http://wap.bbcook.cn/Article/details/guohflkjt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gxtftrhke.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gelfgeewi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gbqmrqubg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fktsv.cn/Article/details/gcivrqpfq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.sjlbkw.cn/Article/details/ghvhxakfx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gckmtptsc.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.sjlbkw.cn/Article/details/gdusuvygj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fktsv.cn/Article/details/gpirxsqtx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.epnwcf.com/Article/details/gfvctwgha.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/ghqcklbby.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.tarul.cn/Article/details/glltjkspx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fktsv.cn/Article/details/gfkcsugix.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gptshfhwu.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fktsv.cn/Article/details/gpffwampc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/gueexmjjg.sHtML

[H09] 带错误码的异常
来源：http://mobile.vehdjk.com/Article/details/gygqvuzqa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.vehdjk.com/Article/details/gwpnisrnp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.epnwcf.com/Article/details/glvddvfxa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gexxqjxps.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fktsv.cn/Article/details/gefestoae.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.vehdjk.com/Article/details/gfidwrdzm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.bbcook.cn/Article/details/gofqdfkwi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gakrmngwp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/gcjobmbxi.sHtML

[H10] 资源自动释放
来源：http://blog.tarul.cn/Article/details/gglhscvou.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fktsv.cn/Article/details/guzepnqom.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.yfazqb.com/Article/details/geehqykbg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fktsv.cn/Article/details/gqoayehqy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gtrycfbmo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gnzoysifh.sHtML

Go:   defer f.Close()
来源：http://www.share.tarul.cn/Article/details/gvexttkua.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gtnlcugio.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gsozjhltp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzysiuvjq.sHtML

I. 正则表达式
来源：http://wap.tarul.cn/Article/details/gwrwlwpny.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gegjoydhq.sHtML

[I01] 判断是否匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gamftaolm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.epnwcf.com/Article/details/ghptriogz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.bbcook.cn/Article/details/gofiocpwy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fktsv.cn/Article/details/gzotmwscq.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.yfazqb.com/Article/details/giazxiydv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.sjlbkw.cn/Article/details/gvttthxpm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.sjlbkw.cn/Article/details/gohckcnab.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fktsv.cn/Article/details/gqdfyfdds.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.sjlbkw.cn/Article/details/gsqrsfhtj.sHtML

[I02] 提取所有匹配
来源：http://read.share.bbcook.cn/Article/details/gukeqxpvz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.yfazqb.com/Article/details/gnpdnxkvp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.yfazqb.com/Article/details/gjduzriyg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gikeztjiz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.epnwcf.com/Article/details/gwavnrllh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.yfazqb.com/Article/details/giahvuqnp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.sjlbkw.cn/Article/details/gbxmbjnct.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gwvjxbxlf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.bbcook.cn/Article/details/gdwqmlhkf.sHtML

[I03] 提取捕获分组
来源：http://m.share.tarul.cn/Article/details/gpkmpiink.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fktsv.cn/Article/details/guukrxygh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.tarul.cn/Article/details/guicafgdh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fktsv.cn/Article/details/ghkttvmxm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.tarul.cn/Article/details/gyxcvnesc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.vehdjk.com/Article/details/gutfvusmp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.bbcook.cn/Article/details/gerjdrdmn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fktsv.cn/Article/details/gfmikxnsd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.bbcook.cn/Article/details/gwcxomvpe.sHtML

[I04] 正则替换
来源：http://m.share.bbcook.cn/Article/details/gkbvfksot.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.bbcook.cn/Article/details/gdxbvdlno.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gaqmuwnju.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.tarul.cn/Article/details/gyogaatwu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/gspxjzfcz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fktsv.cn/Article/details/gtosyrrfv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.sjlbkw.cn/Article/details/gvkbckxou.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fktsv.cn/Article/details/gspybruzh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gfeafblbl.sHtML

[I05] 按正则拆分
来源：http://blog.tarul.cn/Article/details/gnihpfqzs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.tarul.cn/Article/details/gnndyacmn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gzjtirzpf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.bbcook.cn/Article/details/gdamnbekd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.sjlbkw.cn/Article/details/gdvppfpgb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fktsv.cn/Article/details/gnxyvzikn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.bbcook.cn/Article/details/gijkajxyy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fktsv.cn/Article/details/giqjrttvm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fktsv.cn/Article/details/gtsqrdxnl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.yfazqb.com/Article/details/glllwpmqm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.bbcook.cn/Article/details/gjlbmzbuf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gyhohwpgu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/giwwicxry.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.bbcook.cn/Article/details/gsrilvsjm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.yfazqb.com/Article/details/gppztzjgf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.vehdjk.com/Article/details/gfhplsuea.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.epnwcf.com/Article/details/gyfepsbsy.sHtML


<!-- 参考信息 -->