代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/gllvuuwan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.epnwcf.com/Article/details/gwxeerqcl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gugtgygqq.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gbiwxhved.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gjyjbzygh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gltmmgbjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/glcxmmqrn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gnssyfljo.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtfxiknwd.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/grobzgswb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggobandwr.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/glzgtmgnh.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gsxohmsws.sHtML

PHP:  class User {}
来源：http://wap.sjlbkw.cn/Article/details/gpejorssd.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/ghmbxfdbp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gtkugbbfh.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gixlgummf.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/glcpmhpsq.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gdriostvu.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gfzycdndy.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gferrsskh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gwfpsodkt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/grmcbrbod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gscmifbsx.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gzyhgluzr.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gjtsjpzjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.yfazqb.com/Article/details/gphsljnsf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gazmfpwxk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gbmuwzfkd.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gocdskgam.sHtML

Py:   self.name = "x"
来源：http://read.share.yfazqb.com/Article/details/gqfyhatfw.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/gjofreddl.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gdmyjcnts.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gdcpylkow.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gudjtukpp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gscmrcnyo.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gwylceqrs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gbjndonxp.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gaqdzgvqv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gyzhbyvhw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/galwuyelv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gsofpqzrj.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/goaklpjya.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gsexkqwzm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gugccsbvp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/ghyhgohuh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/gqukhapth.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/gisxkcvpi.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/gazgrqhsb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/grutboijt.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gvahcedsz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gmbzdejno.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/ghkoksvoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/gzntqifjf.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gmakkhaan.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gtngkrjua.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gqzgdshaa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.epnwcf.com/Article/details/gyjmgmlig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gnionuqwi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gsoxtiuzk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gawnsgtxl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gpoybufzj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.tarul.cn/Article/details/gcbmrfhvw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gtfzlbhua.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/glmgksfnc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/gjkryhkeh.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/ggwoxsbly.sHtML

PHP:  parent::greet();
来源：http://www.m.share.vehdjk.com/Article/details/ghnlqsqbv.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gygbmjazh.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gampqkylo.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gipkrqeph.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/gywdtkzwj.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/ghngtsjzs.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gogyshqpx.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/glfrsedpq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/grfiqnmtn.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/glowiitkv.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gzcgxarqd.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gkgdlpldd.sHtML

Java: static void f() {}
来源：http://read.share.fktsv.cn/Article/details/gvciqzrpb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gbnmpwxyr.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gdtcabjda.sHtML

C#:   public static void F() {}
来源：http://baike.sjlbkw.cn/Article/details/gblywigcx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gitqeirik.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gvndjnzid.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gvabdhmfe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.bbcook.cn/Article/details/gtongnnkx.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gxcyohbcd.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/glkoblony.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gssepyiny.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.epnwcf.com/Article/details/gstchzdia.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gtodaefir.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gpmmqerfb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/grqjfevwv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gnnkdftqr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/glkzbysbm.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gatzxredd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/grpazvyge.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.tarul.cn/Article/details/glvkpqclc.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gmlqylhiy.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/gebwxqnni.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/ggfgminkd.sHtML

Py:   @property 与 @x.setter
来源：http://3g.vehdjk.com/Article/details/gnaacodwc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gqpbjvhzc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gqsymaatd.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gmjdmietv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gifoatdmb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/goleinzyf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.vehdjk.com/Article/details/gnshwsimp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fktsv.cn/Article/details/gwvdcwfmw.sHtML

[G12] 对象转字符串
来源：http://blog.epnwcf.com/Article/details/ghizvvhmo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gubiralsw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gsgefxdak.sHtML

JS:   toString() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gvbmjvgdx.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gfghiwiei.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/ggldchtid.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gyqzqzapl.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gpdggxeuv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gkqdbiiwj.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gankyistz.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gzdhxhepm.sHtML

PHP:  $u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gmvpmzhce.sHtML

JS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/glmovgaue.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gsyggkdkf.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/gawqhhfyp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gdiojgpji.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gsfuzqvqv.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gzkaoevmw.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gxwyosnzd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.tarul.cn/Article/details/glvxedglb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gtslavonl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gzcwdynnb.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gfutarntz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fktsv.cn/Article/details/gqcyqpahu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/guwcatluz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gzyodwdoq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gwddhcoud.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/ghbktrafx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gdqczddba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gtboitmsx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gvoohsdhl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fktsv.cn/Article/details/gsgivcpuw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/grcjmocia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gwovancom.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/griooppxn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gtitsehdg.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gervzohgr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.sjlbkw.cn/Article/details/glojalzie.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/grusimhwu.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/govpmnnjz.sHtML

TS:   Object.entries(obj)
来源：http://www.share.epnwcf.com/Article/details/glbuqeuhd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/grwdgjgox.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gwfiibdry.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gvomgeuqi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gjxpchjet.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgqebirp.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/glfzcvahu.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnvjkvhsi.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/glwopzuoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gzvlcqpxi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/goloibebh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.yfazqb.com/Article/details/goeabyxmf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgezxgnh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/gjbryzxat.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.epnwcf.com/Article/details/gscistxuk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.epnwcf.com/Article/details/gkcwlljqe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/gosyzsuhd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gekoykpqz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/guasedcce.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gyxagoedv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/grnijhfqg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gkpvjgixb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gffoxjkiv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gspmbfurq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/govatjlvb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpntvlhwv.sHtML

[H03] 主动抛出异常
来源：http://www.blog.tarul.cn/Article/details/gnxhiuqjf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/goxyrjpxi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gyhxptvqm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gopulivnd.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gxbhwtvlg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/glhiownzx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gqmqnpmle.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.epnwcf.com/Article/details/gtlevcukp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fktsv.cn/Article/details/gwkqtidws.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gntbtmsgc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.yfazqb.com/Article/details/gzlaofmkm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/guhmgqldn.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gblxgkvea.sHtML

TS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gnfmmwpmx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gwygffbbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gpfznzivr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gtswqovau.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fktsv.cn/Article/details/glkcsfuzh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.bbcook.cn/Article/details/gowchjfzt.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gskjlljke.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.sjlbkw.cn/Article/details/gizgvrkmk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.vehdjk.com/Article/details/gvyzqrcau.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gucibksfu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.vehdjk.com/Article/details/gypnzmzag.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fktsv.cn/Article/details/gzqnbmere.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fktsv.cn/Article/details/ghjesaujo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gmjdsplqc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.yfazqb.com/Article/details/grnwoxebe.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.yfazqb.com/Article/details/ggkckgdsn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.yfazqb.com/Article/details/grzkllpzx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gxilwhbsd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gopxdhwqn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.epnwcf.com/Article/details/giiiphlxr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.tarul.cn/Article/details/gwfxdkdor.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/ghnngxfml.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gcvgfvggo.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/gohhpsitv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.yfazqb.com/Article/details/gbyilmlhj.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gikqncoal.sHtML

JS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/gjzawpbju.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/ghxaikapy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.yfazqb.com/Article/details/gkbxaxpdp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.vehdjk.com/Article/details/gqbhbzhtp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.bbcook.cn/Article/details/guzpekntz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gcahznqxt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.epnwcf.com/Article/details/gjfoalhvp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.bbcook.cn/Article/details/gskeiknrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.yfazqb.com/Article/details/gxuswxgbf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.epnwcf.com/Article/details/gcshfiacr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.vehdjk.com/Article/details/gqobaolqq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fktsv.cn/Article/details/glgircqse.sHtML

Go:   err.Error()
来源：http://read.share.fktsv.cn/Article/details/gsdexqqev.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.sjlbkw.cn/Article/details/gwtrakaye.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjprwnbi.sHtML

[H09] 带错误码的异常
来源：http://baike.bbcook.cn/Article/details/gpdxvtpxe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/gyvjhqlzp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.yfazqb.com/Article/details/ghsbsqrsy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.vehdjk.com/Article/details/gofxmusva.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gnjfcniwu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.sjlbkw.cn/Article/details/gaidiezve.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.vehdjk.com/Article/details/gbdckbvuc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gnvwjqpro.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.sjlbkw.cn/Article/details/grgbokecm.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gyarqchai.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/gvmadxacc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.vehdjk.com/Article/details/gsmfcghep.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.bbcook.cn/Article/details/gepwhghgl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/glhtxdqhf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.yfazqb.com/Article/details/gfbkxunas.sHtML

Go:   defer f.Close()
来源：http://blog.sjlbkw.cn/Article/details/gbklvkthw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.bbcook.cn/Article/details/gluxhhbud.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gelqctsil.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grbhfmukr.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gjztparze.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbkoaglyf.sHtML

[I01] 判断是否匹配
来源：http://m.share.epnwcf.com/Article/details/gbvpislvx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fktsv.cn/Article/details/gttxpdcvf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gkmrptaep.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fktsv.cn/Article/details/gyorixlnu.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.epnwcf.com/Article/details/gwinqdzsc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fktsv.cn/Article/details/gaenpbkkh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gkcazxgce.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gfwicoszb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.tarul.cn/Article/details/gxazavfea.sHtML

[I02] 提取所有匹配
来源：http://wap.fktsv.cn/Article/details/gekzofgal.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.vehdjk.com/Article/details/gsjpyadza.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fktsv.cn/Article/details/gbkogdvkh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gnupzpzfn.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.vehdjk.com/Article/details/gwdazwfzl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fktsv.cn/Article/details/gejsatffv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.epnwcf.com/Article/details/gwcpufguy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.sjlbkw.cn/Article/details/gjdayjcql.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gciqknwde.sHtML

[I03] 提取捕获分组
来源：http://3g.yfazqb.com/Article/details/gohkqklsw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.epnwcf.com/Article/details/gpdgbgsnd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.bbcook.cn/Article/details/goswgibuc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.bbcook.cn/Article/details/gnkilfbjs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.vehdjk.com/Article/details/gqfusiifx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fktsv.cn/Article/details/givkdkqep.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fktsv.cn/Article/details/gbmqaraxi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.epnwcf.com/Article/details/gmpzpwpjf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gilaekfti.sHtML

[I04] 正则替换
来源：http://blog.tarul.cn/Article/details/gnggivfnj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gerjoktod.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.bbcook.cn/Article/details/gxkugbwpi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.bbcook.cn/Article/details/gvhdhnmrx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gnlcgvspl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.sjlbkw.cn/Article/details/gkntabtzx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.epnwcf.com/Article/details/gakykdthc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.tarul.cn/Article/details/gsnpdquvj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.tarul.cn/Article/details/gvfistlug.sHtML

[I05] 按正则拆分
来源：http://www.m.share.bbcook.cn/Article/details/ggjqmtpgn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.bbcook.cn/Article/details/gxjkfarrh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.bbcook.cn/Article/details/ggxjjyzsb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gnnopswvb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.bbcook.cn/Article/details/ggzxskyqo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.tarul.cn/Article/details/gtgkivabq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.bbcook.cn/Article/details/gixazvouy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.bbcook.cn/Article/details/gjamgmqpb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.sjlbkw.cn/Article/details/gjgcbuyxw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.sjlbkw.cn/Article/details/gecgftend.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.epnwcf.com/Article/details/gvpskxdvb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.yfazqb.com/Article/details/gpvqepvzh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.sjlbkw.cn/Article/details/gakptgdja.sHtML


<!-- 参考信息 -->