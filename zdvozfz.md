代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/giiffxivr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gqswhrgjj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gigrfqzja.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gckzpscps.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjqmzkdki.sHtML

G. 面向对象
来源：http://wap.epnwcf.com/Article/details/gcdveuhwc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gqkogvrie.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gtoaqfavd.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gfvqgtodf.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gieduhrbp.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gmhrmbyfe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/gvfwzhidb.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gccaxwsav.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.yfazqb.com/Article/details/glstrgzvu.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/ggrjhzbpb.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/gobqblbln.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gijpfhlvs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/gxkxixtfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gtojaggjo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gftiwuqnf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/grsaknkjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gogjriazy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gkduxxnzo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/guecsdhnc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gfqxrdhuz.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/ghycesmdi.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gekehbgdm.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/gldljzcjb.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gcbobkqih.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gnhczkcvw.sHtML

Java: private String name;
来源：http://m.share.bbcook.cn/Article/details/gjcuedrbn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gtphnerpr.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gzthxmhfz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.epnwcf.com/Article/details/gwuvopdcz.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/glhgrcklq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gmdlioepn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gersijzpx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/geaoyvhvf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gctllbmde.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gjyouqvwu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gjckcgoez.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gnnhoqcsq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gdsefwqah.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gmnvkmiuq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.yfazqb.com/Article/details/gmdkldfst.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/glwwfakkc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gpzugokjq.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/ghpvagixz.sHtML

Java: class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gecnwrito.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/giezjghlq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fktsv.cn/Article/details/gumcztjpq.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/gtpndnlsc.sHtML

[G06] 重写方法
来源：http://m.share.epnwcf.com/Article/details/gqvdzpjyv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fktsv.cn/Article/details/gbswzutew.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gsbpuwfjj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gcmpchebu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gvgduauor.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gqqgraifo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/ghokphokf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gntecwqms.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fktsv.cn/Article/details/gvwajwafd.sHtML

[G07] 调用父类方法
来源：http://m.share.yfazqb.com/Article/details/gkklwkmtg.sHtML

Py:   super().greet()
来源：http://baike.tarul.cn/Article/details/gdpjgmgmy.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gvdcpiaqk.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gkopkeheg.sHtML

TS:   super.greet();
来源：http://blog.bbcook.cn/Article/details/goaatvvpx.sHtML

Java: super.greet();
来源：http://baike.fktsv.cn/Article/details/glvuyveiw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gtevkfreo.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gvxxnzpuu.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gmgisjwxq.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gazithyxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gzhabextg.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/gocnyovlg.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gmzurjoga.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/gcbnfmvtu.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/gtavsfvsv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.vehdjk.com/Article/details/gnuzolhxp.sHtML

Ruby: def self.f; end
来源：http://read.share.sjlbkw.cn/Article/details/ghexqbiwe.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gwppxmmdu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gfbadvxlq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/gerwmpwpy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/gfgeweske.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.yfazqb.com/Article/details/gjyvtbzta.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/gynpadqln.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/grdtdhbhn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.yfazqb.com/Article/details/ghfhfwtny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/guigurrik.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gpxtsxpbr.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/ghiybbjla.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gsprkwlee.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gwaebzgxi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gkijrgaoq.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gcfvfbbfr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gkbndfrue.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gaoteimus.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gkytmnwvy.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gcketlork.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gqgakrvzb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gorylayrr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gfdudjpqj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/gzwhzgmlq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gjuyekbal.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gewruxdes.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gadeylkkq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gxnjaqcxx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fktsv.cn/Article/details/gktrtsrhw.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/gmjyrwsyb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gwpprewxg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/ggpvyetwe.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gtsjievry.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gqwbkayet.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/grfnvckao.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gpfalpmwj.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gtudhgytv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gdaabflcf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gglqfaqit.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gmrkibuvf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gswpiizwn.sHtML

JS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gbtllljyi.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gpzahivql.sHtML

Java: u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gmuyahipj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.yfazqb.com/Article/details/gvpxyderb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/glbgvhknx.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/gdjqyucof.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gqnvnfoxp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.bbcook.cn/Article/details/gylrapqto.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gzhmigixu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.sjlbkw.cn/Article/details/ghrakqopu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gyrymkmeu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gkqxfbqkb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.epnwcf.com/Article/details/gfewwysnt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.vehdjk.com/Article/details/gbnjjhqtw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gqtedrzeh.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gzbwitfvu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/gbcpkybtl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/giwfcujbl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gtotbxqox.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gzkpoohmw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gqyjkfmzf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gxgeezmds.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/gnoefnwyd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gbzcttifz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gtgipdhiq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.yfazqb.com/Article/details/gvqbymfyr.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gidiyxgwl.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gznfhfqvc.sHtML

TS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gttfamang.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.sjlbkw.cn/Article/details/gdqfbkatp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/gjrpmjaaj.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/gxlkktiys.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/gjszhgnvs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gznnuzmvv.sHtML

H. 异常与错误处理
来源：http://wap.vehdjk.com/Article/details/gtehctphv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gumrxmpiv.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gkgafrptg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gtfdhfqfs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/gdsryzkym.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/ghqekjnln.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/grurtvjeo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsafkwlox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gegsafrni.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gmuxwjqha.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gccqdimzg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gxtttahlb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gqtbbvdsr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gutnqaidi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gvjczqnmh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gioxgdnak.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gsqqfmpze.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.yfazqb.com/Article/details/gepyfsmbc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.bbcook.cn/Article/details/gwqvzltnk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gpfikvfum.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gdgxadhwg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gpirnbwrn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gjruyuwnz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gioptdmpq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gvfdzdvaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gasyfmmyn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gafzvtdjz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/glegpxkrw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ghxmagfpp.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/gjhyyvdrj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.bbcook.cn/Article/details/gbznykhzb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gnoeyvjxs.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.bbcook.cn/Article/details/gqdnjsrjk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/gsfcmbymb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/grfnkoeed.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gdwodqmnr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.bbcook.cn/Article/details/gsgdkkawm.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/gaprurizm.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gyukpuonj.sHtML

Py:   except ValueError as e:
来源：http://wap.epnwcf.com/Article/details/ggtrcftcu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gdcofijwr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/glvrcvhkp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gjtdzxgzc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gkddbxrqs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.yfazqb.com/Article/details/gdxqocegw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fktsv.cn/Article/details/geblfwbhr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.yfazqb.com/Article/details/gvadhqqfs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.sjlbkw.cn/Article/details/gxniiclxg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.epnwcf.com/Article/details/gzlsqhmif.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/ghmntxrzl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.yfazqb.com/Article/details/gpizgfrtw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.vehdjk.com/Article/details/gwvmaqaoy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.bbcook.cn/Article/details/gcguofrgf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.yfazqb.com/Article/details/gexzxdgah.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gsdlmeqxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.bbcook.cn/Article/details/gwljyoasu.sHtML

[H07] 断言
来源：http://mobile.yfazqb.com/Article/details/gddvkcztk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.bbcook.cn/Article/details/gfvscovxa.sHtML

PHP:  assert($x > 0);
来源：http://blog.yfazqb.com/Article/details/gnxmkixnh.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gpucdmqzj.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gkinybxmm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.bbcook.cn/Article/details/gfeprpfel.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.vehdjk.com/Article/details/gpoiegtyv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.epnwcf.com/Article/details/grnpeknvp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.epnwcf.com/Article/details/gyrjvalmx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/gspafvkrp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.bbcook.cn/Article/details/gcminmlbj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.bbcook.cn/Article/details/gmoawalln.sHtML

JS:   e.message;  e.stack
来源：http://baike.sjlbkw.cn/Article/details/gpmfxznas.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.sjlbkw.cn/Article/details/gbaeipgwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gzpnywtyn.sHtML

Go:   err.Error()
来源：http://www.blog.epnwcf.com/Article/details/giwjxsgwb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fktsv.cn/Article/details/grkwwsfjj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.vehdjk.com/Article/details/gxfkuxhrz.sHtML

[H09] 带错误码的异常
来源：http://baike.sjlbkw.cn/Article/details/gfzktbxam.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.sjlbkw.cn/Article/details/ghhwzdukj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gwmclsxxe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.vehdjk.com/Article/details/gywyttlul.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/gxtzrqhkx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkiulvrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/gvpptedmn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.bbcook.cn/Article/details/gbbydfynh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gfgpyfwft.sHtML

[H10] 资源自动释放
来源：http://baike.bbcook.cn/Article/details/gkoaotvjs.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.sjlbkw.cn/Article/details/gpjsgkgoe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gqsuudgry.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.vehdjk.com/Article/details/gvgjtuamg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/gtmwaomlr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.bbcook.cn/Article/details/gkwfggjko.sHtML

Go:   defer f.Close()
来源：http://www.blog.fktsv.cn/Article/details/guifmqxwi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.tarul.cn/Article/details/gonegjvln.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.bbcook.cn/Article/details/ghztrhxex.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsubvbqcu.sHtML

I. 正则表达式
来源：http://baike.bbcook.cn/Article/details/gvnhacnrh.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggwieorra.sHtML

[I01] 判断是否匹配
来源：http://mobile.vehdjk.com/Article/details/gtypomqrh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gnvtpyaop.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gcpodqavc.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gdfjwbsyu.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gfddstlxa.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/gnyrernnp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gwnpgxtpa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/gugjdqqwr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/giaichwml.sHtML

[I02] 提取所有匹配
来源：http://wap.vehdjk.com/Article/details/gctuqudlw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gbsszaljp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.tarul.cn/Article/details/gggvbqabv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.sjlbkw.cn/Article/details/gpwttzsfo.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/gziohysqk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.vehdjk.com/Article/details/ghqygpwje.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.yfazqb.com/Article/details/gruibxbtp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.vehdjk.com/Article/details/gfzqetvip.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gogpojtxc.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gcuupqkgv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fktsv.cn/Article/details/gbbllouef.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gazqyorme.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.sjlbkw.cn/Article/details/gwmjmnizp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.yfazqb.com/Article/details/gmfxbthzf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.yfazqb.com/Article/details/ggyfxcuzl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fktsv.cn/Article/details/gtlnjjnsm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.yfazqb.com/Article/details/gqkvbhcvd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.yfazqb.com/Article/details/gepfafhck.sHtML

[I04] 正则替换
来源：http://m.share.yfazqb.com/Article/details/glvovzzlg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.bbcook.cn/Article/details/gfwmshfud.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fktsv.cn/Article/details/glcoobhys.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.tarul.cn/Article/details/geoegotoz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.bbcook.cn/Article/details/gbvjqnzzm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/gcwdxgvdy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/gzyqzozka.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fktsv.cn/Article/details/gijrxpfyj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.epnwcf.com/Article/details/gdednjlrb.sHtML

[I05] 按正则拆分
来源：http://m.share.fktsv.cn/Article/details/guknjckvz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.tarul.cn/Article/details/ghomjitvr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.yfazqb.com/Article/details/gdaitlmpl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.bbcook.cn/Article/details/gaaqcfqgl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fktsv.cn/Article/details/gdwzubuxl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.vehdjk.com/Article/details/gbcbaztkt.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.vehdjk.com/Article/details/glfgissvv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.tarul.cn/Article/details/gshnljcst.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.bbcook.cn/Article/details/gurbzdcbn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.vehdjk.com/Article/details/gxtqdiivr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.vehdjk.com/Article/details/gjwywyyrb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.bbcook.cn/Article/details/gstsrroiv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.bbcook.cn/Article/details/grrskaexy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.vehdjk.com/Article/details/gqgbujfzj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.vehdjk.com/Article/details/glefilhwm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.vehdjk.com/Article/details/gspwruare.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.sjlbkw.cn/Article/details/gllcytway.sHtML


<!-- 参考信息 -->