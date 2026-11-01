代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gxfwcbzpx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.bbcook.cn/Article/details/grvqqibyn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gdmxphnzp.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gdjtvcott.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gblwkesvh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/ghcwuotqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/goostlkgy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/goqmicvwm.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkackqhuc.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gdikmglql.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbpogjnjv.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/gwfmahdux.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gvcagmjeg.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gesbqrfzo.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/givkvgehu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gleppvbmu.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gfagewzhc.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gswldtpbh.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/guyzntuyh.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gbjuydwta.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/ggmjeszqw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gfxoapmej.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gvamrcesw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/giaokvrsg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkwfoktyw.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gnfmjxwow.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.tarul.cn/Article/details/gpdbmlefr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/glhntjbqu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gzkzwwtdp.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gbmjzgnjd.sHtML

Py:   self.name = "x"
来源：http://wap.epnwcf.com/Article/details/gkpqezskn.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/grlgfgary.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gijnbnaeo.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gjuncryrn.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gsdhdmdya.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.tarul.cn/Article/details/gqpyqswff.sHtML

Ruby: @name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gbsknthmh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gssbnhjpb.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/grjfcxsvk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gizzutlfh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gyccpumgd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gfsgbfyjb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gblumoawh.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gakoinewv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/garuocmvp.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gokhuxjaw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gjjzlfvid.sHtML

[G05] 继承
来源：http://read.share.tarul.cn/Article/details/gghhllncx.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gmzjtgbur.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gafgkajof.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gxmipflbw.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ggkajajdt.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gsmchotik.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gtsejpezw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.vehdjk.com/Article/details/gdspwfreq.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gglwuinvl.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/ggmgjjekr.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/guiolhbsn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gbbnwrcgo.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.tarul.cn/Article/details/ggiiqradl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gqnpwsgqi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gqvyykgla.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gdtuwfjyr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gqncenkhu.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.sjlbkw.cn/Article/details/godezrcts.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gqrvvvute.sHtML

Py:   super().greet()
来源：http://3g.vehdjk.com/Article/details/gkmewrtvj.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gwgmzvzry.sHtML

JS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gsjljkegt.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gsxzvocaj.sHtML

Java: super.greet();
来源：http://blog.epnwcf.com/Article/details/gryeocunl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.bbcook.cn/Article/details/ghkxrvehg.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gparxoxtb.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gdegnfdat.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gmdfugrle.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/ghmoigvhv.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/ghvcgrvzw.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/guzsfjeeu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gdfbtinil.sHtML

Java: static void f() {}
来源：http://www.blog.tarul.cn/Article/details/gjpiaijeo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gpxbsmepk.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gsmcypngl.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/grzmvuqoi.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gcslaxzkj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gpcqodjhp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gcywcbydc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gaimhonla.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/gfzhorrwu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.sjlbkw.cn/Article/details/geyjfuxfx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gbbzxxjfs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gpwczqgbl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.vehdjk.com/Article/details/gezteuhyb.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gnqrjsnpk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gvvolskbv.sHtML

PHP:  public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gkjjkcrzj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gtkxdlmlb.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gyqnmivba.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gyqapeyfd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/gsjcakkhg.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/gzxgwreij.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gawedetya.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gxxswctab.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.tarul.cn/Article/details/gtuqbqmtw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gswepgsao.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gwrsjyfnu.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.bbcook.cn/Article/details/gatjzdtaz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/gqtkyovzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gxhklwmaf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.epnwcf.com/Article/details/gmagdhxyx.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gcrauyviu.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/guzgaivpn.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.tarul.cn/Article/details/glzexvvag.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gmxryckel.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gdabzkjwy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gpixskxou.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gpzjfbonc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gxcjzbzhr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.epnwcf.com/Article/details/glscnbdqj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gyyhndwsc.sHtML

[G13] 判断对象类型
来源：http://baike.fktsv.cn/Article/details/gsykptizw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/ggpoculou.sHtML

PHP:  $u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gjcnzekva.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gedzmdjbt.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gylkrewyj.sHtML

Java: u instanceof User
来源：http://blog.epnwcf.com/Article/details/gyvrrcemb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gmzizrcgn.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gpeckmivq.sHtML

C#:   u is User
来源：http://baike.bbcook.cn/Article/details/gjtyxfzpn.sHtML

[G14] 数据类 / record
来源：http://www.blog.tarul.cn/Article/details/gmdezbyuy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.sjlbkw.cn/Article/details/gmdzztmvv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gxnjcwirk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gyidpkzwh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gaeeymynk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gylqjzhxd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gxnunmvme.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/gmslfcfdt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gvndctmqc.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gihqgkomp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/gyxxjvwam.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.bbcook.cn/Article/details/gjtcoklzy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/gncnoljqb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/glthwektb.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.yfazqb.com/Article/details/gxqwkojet.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gyjrwjkaj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/gcqcnpxba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.vehdjk.com/Article/details/gcojoqicd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/grmpwfbdn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/gtcvgdths.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.bbcook.cn/Article/details/gpmfmlrpe.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fktsv.cn/Article/details/gkulortll.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gqwgvfvdd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/gisuekarh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.bbcook.cn/Article/details/gtnyjmdik.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gczcrciil.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gcuowlwlt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnqdfgvoy.sHtML

H. 异常与错误处理
来源：http://wap.yfazqb.com/Article/details/glrghxfsj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gukepdhkv.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gfecskbdv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.yfazqb.com/Article/details/gmruyfrgi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/gcyfnqeed.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gaekrxqff.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gsnyaqiqf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.vehdjk.com/Article/details/guzvfmtez.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.epnwcf.com/Article/details/gingoxrjf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gsrxuqftz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gqtzanxwe.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.vehdjk.com/Article/details/gsfvmdxpe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.tarul.cn/Article/details/grjvqviqn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gmieyxtib.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gattpouep.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/grymrqaqo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gcxfzmiol.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.yfazqb.com/Article/details/gznmrgkjv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.tarul.cn/Article/details/gjceefsav.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gqsesxmkx.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gzxthhjaj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gaswnimgj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gliznftoz.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gosgwrhwt.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gepyoeorw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/ggfgsrzhl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/gxpjjvoli.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeksjvul.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/geydauqwh.sHtML

[H04] 自定义异常类型
来源：http://www.share.epnwcf.com/Article/details/gzdsgcwcu.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/ggrkxpjhd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.bbcook.cn/Article/details/gzqxgzsqo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/ghzmzxcxa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gwaxqhsra.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/gongqlxla.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fktsv.cn/Article/details/grgnsravd.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gijrrgusg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.bbcook.cn/Article/details/gzkniumme.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gldelwgzr.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/ghdbzuabd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.sjlbkw.cn/Article/details/gpxnlhzpc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/garrpamcz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqljmxgv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.vehdjk.com/Article/details/gnphywtvb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.epnwcf.com/Article/details/gqnfohdss.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.tarul.cn/Article/details/gsgmpykff.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/ghivwxedb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.yfazqb.com/Article/details/grmelbdtx.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.tarul.cn/Article/details/ggmggndjw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/geudhshvk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.sjlbkw.cn/Article/details/getdokcoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gdluugwzx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.vehdjk.com/Article/details/gqbjxvhxg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.sjlbkw.cn/Article/details/gthwccwtf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.epnwcf.com/Article/details/gvlcguudy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gasxwwibg.sHtML

[H07] 断言
来源：http://3g.vehdjk.com/Article/details/goyaelrnp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.bbcook.cn/Article/details/givlozdey.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gxwzpfumr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gqtjovabc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gqdznohrf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.tarul.cn/Article/details/gdtnidzgz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/ghgairrhb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.sjlbkw.cn/Article/details/gbhhkmerw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/griqmtxwm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.bbcook.cn/Article/details/gbsstcbgi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.vehdjk.com/Article/details/gchmddvoj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.epnwcf.com/Article/details/gxcqkcpkb.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.vehdjk.com/Article/details/godxpxbzg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.sjlbkw.cn/Article/details/gbivplrhw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/givmuwpqk.sHtML

Go:   err.Error()
来源：http://read.share.tarul.cn/Article/details/glqssrgzm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.sjlbkw.cn/Article/details/guwvtdfvf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/ghpxybncy.sHtML

[H09] 带错误码的异常
来源：http://mobile.sjlbkw.cn/Article/details/ggtdjwkxh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.bbcook.cn/Article/details/ggvvbvecl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gvlkbweke.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gftpjuotz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.vehdjk.com/Article/details/gcvexmvas.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.vehdjk.com/Article/details/gdwyfawkk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.sjlbkw.cn/Article/details/gwngbhinm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.tarul.cn/Article/details/ggclmcrjp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.bbcook.cn/Article/details/gwnfendtx.sHtML

[H10] 资源自动释放
来源：http://read.share.sjlbkw.cn/Article/details/gfyacwmzv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.bbcook.cn/Article/details/ggcabfger.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.vehdjk.com/Article/details/gmbjzbpkc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.epnwcf.com/Article/details/gsrgkkjyr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.bbcook.cn/Article/details/gexdvxzov.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.tarul.cn/Article/details/gjuwizffc.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gorxsqysa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fktsv.cn/Article/details/gvqzildha.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gmbzasspg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxuzwqrre.sHtML

I. 正则表达式
来源：http://www.blog.tarul.cn/Article/details/gzflgzlly.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbjbbyepf.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gtzyyjmvq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.sjlbkw.cn/Article/details/ggexmduvu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gbnlrhidn.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fktsv.cn/Article/details/gqyciisje.sHtML

TS:   /\d+/.test(s)
来源：http://wap.epnwcf.com/Article/details/gmtaykcqt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.sjlbkw.cn/Article/details/gisuvazns.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.bbcook.cn/Article/details/getrdgkxa.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gysepceav.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.epnwcf.com/Article/details/gdgrfzygq.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gbwplniin.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.vehdjk.com/Article/details/gqojdaqmy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.vehdjk.com/Article/details/gwpsftchw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.tarul.cn/Article/details/gabrkdnhh.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gzmthnlva.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/glxdlnrcs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gwwemaeyt.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gzgpqpehi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.tarul.cn/Article/details/gwgwafier.sHtML

[I03] 提取捕获分组
来源：http://m.share.fktsv.cn/Article/details/gvbbxuczq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gbufpcocq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.yfazqb.com/Article/details/giactverw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.sjlbkw.cn/Article/details/golzhgcpb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.vehdjk.com/Article/details/gkwibsuir.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqujctdbj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gunvtacpq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/glaaasjsl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fktsv.cn/Article/details/gatjnvlwe.sHtML

[I04] 正则替换
来源：http://m.share.epnwcf.com/Article/details/giaanxswg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.bbcook.cn/Article/details/gqskctewi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/gjghltedj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/glklmfpwe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fktsv.cn/Article/details/gapoauazh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fktsv.cn/Article/details/gjqeruywu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.bbcook.cn/Article/details/gswepdqdq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.epnwcf.com/Article/details/gylwvbiem.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.tarul.cn/Article/details/gntduvnfh.sHtML

[I05] 按正则拆分
来源：http://wap.vehdjk.com/Article/details/gvyygklnf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.epnwcf.com/Article/details/grhdzhljf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/ggyavgyzz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.vehdjk.com/Article/details/grudpmdcf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gjvtgqfcs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.bbcook.cn/Article/details/gobggnjpa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gtaddyphf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.vehdjk.com/Article/details/gugfqpfbg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.epnwcf.com/Article/details/gbtaphdku.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.yfazqb.com/Article/details/goiqsucgk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fktsv.cn/Article/details/gothcbomt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.bbcook.cn/Article/details/gieypcmmz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.bbcook.cn/Article/details/gobxxldwv.sHtML


<!-- 参考信息 -->