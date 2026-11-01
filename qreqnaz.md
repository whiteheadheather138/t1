代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gwxyvlwjz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gmqlaupam.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.tarul.cn/Article/details/gofinbjff.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/grgphyyym.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gxyxnyeom.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gkmsmpodk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gzounfmgv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gjavxmzfp.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giqrojlgz.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gmcdjswav.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gjyrefiyu.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gtujqiceu.sHtML

Py:   class User: pass
来源：http://wap.yfazqb.com/Article/details/gxtqiuobo.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/gzoeepmkw.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gyaaamszr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gfivmpmhd.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gacsyujxv.sHtML

Go:   type User struct { Name string }
来源：http://baike.epnwcf.com/Article/details/gcqmmfeyk.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gilfrhval.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/ghkotndeq.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gaejusjhk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gqzsfmnsl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtwocwjso.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/goshqjqld.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gjmyfemgj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gmlivjtbk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gtfgngchz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gqwngekdl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/giarcwlgq.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gnsmjijrt.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gappisaec.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/gsicduijw.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gducdzhtr.sHtML

TS:   name: string = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gzjzjzpzl.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/gafbsfzmm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.tarul.cn/Article/details/geyaxrxez.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/gujujzsfp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gtrmkgflt.sHtML

[G04] 定义方法
来源：http://wap.yfazqb.com/Article/details/grmelphhe.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/grgujdxzu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gidsxqeyy.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gogoqgswd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gjwpeezes.sHtML

Java: String greet() { return name; }
来源：http://www.share.tarul.cn/Article/details/gngixmnwh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gzwoyauby.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gcgziywbr.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/glmtrspfc.sHtML

[G05] 继承
来源：http://baike.yfazqb.com/Article/details/gypnamcwv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gdpukoacz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/glcgbuteq.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/ggzunawch.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gwbuilsed.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/geueeztez.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gdllsbcfk.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gclrdtdxz.sHtML

C#:   class Admin : User {}
来源：http://3g.bbcook.cn/Article/details/gleyfrzzw.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/gbqzcbhug.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fktsv.cn/Article/details/gahoatgey.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gkjfkjzpq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/ggxhulfjg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/guzzofwbb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gdiyehdti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gdfhhnxrk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/goncqtqos.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/gagvqudmx.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/grbpkzrvb.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/gnpheojez.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/gvpqgyklp.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gpabmoftc.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gqtmyhjpv.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gvohgqjom.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/ghtfrkuri.sHtML

Ruby: super
来源：http://wap.vehdjk.com/Article/details/gxdaoalwh.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gnfvyvqat.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gcrhjrpju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gjkjgihyf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkhaqqsne.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/gdtcpcxxn.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gkqzdjdrw.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gxgfmwtbe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gumvjyivb.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gmkgdfqns.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/glcmekhzv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fktsv.cn/Article/details/gbuurwkww.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/grxaubqod.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.vehdjk.com/Article/details/ghchfmruu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gcelktfxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/gdrvofppy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/glaiiuhgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.sjlbkw.cn/Article/details/gystkxdcc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.sjlbkw.cn/Article/details/girsznsmz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gzzygvabn.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/grwasujyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/ghixpkalh.sHtML

PHP:  public / protected / private
来源：http://baike.fktsv.cn/Article/details/gdawcvowt.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gkmgqphvv.sHtML

TS:   public / protected / private
来源：http://mobile.sjlbkw.cn/Article/details/gzhxlmfgz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/ggdfwevnv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gpceqsaga.sHtML

Ruby: public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gfxatpacs.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gxcaminwu.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gyaxlfnld.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fktsv.cn/Article/details/gkatimkmg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gippsqeyz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gwowknudz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzxrlfyjr.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gohgjdlpy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gwuctgawf.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/ggdimdzzn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.tarul.cn/Article/details/gexclgvgv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gwcxczxnt.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/ggdjubbvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.sjlbkw.cn/Article/details/gtxswixfr.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/ghcilvnhe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/giufhygbb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/glytrnnwt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/ghpfgtruw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.epnwcf.com/Article/details/gjtnrahyp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.vehdjk.com/Article/details/gqiwgkudp.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/goyobgfbj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.vehdjk.com/Article/details/gvqlppxgv.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/glytplagt.sHtML

JS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/grzymcpab.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gmtlmazfc.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/giyxawvkw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gkwcngarp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gvbnzrlpv.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gdpxmetkx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fktsv.cn/Article/details/gdzwnkgch.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.yfazqb.com/Article/details/gfhhjcdyx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gdacvdadj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.sjlbkw.cn/Article/details/grofqerbx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gciipzecy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.vehdjk.com/Article/details/ggfrdhpbe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/grclxjikz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gmhxdjdtn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gcccydipz.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gpszasvuv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gqvzphyjw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmmjaqmtv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.epnwcf.com/Article/details/ghlsnawfg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/gopkawhqe.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/gpvqbjprc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.vehdjk.com/Article/details/gvpzdzaga.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gqvrhzarj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gaubcjtqo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.yfazqb.com/Article/details/gjfpttoek.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gvqbioqsl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gsrektnmi.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/grbbugtgp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gutuhmrtz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gxvqsgbsa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.yfazqb.com/Article/details/gtfjqwutn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gtnkfkkki.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gsspessrx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/godkrsdbp.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/goikozowq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gflkvjhsg.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gctpfgenm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/gjozzutly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gtebuxjzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gbdmxruau.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gmjdbuvbx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gqtcokocp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.bbcook.cn/Article/details/gqetugzqj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.bbcook.cn/Article/details/grpucsgal.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.yfazqb.com/Article/details/gghvzgzvj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gmvgkmsxy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.yfazqb.com/Article/details/gqaxwozcr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/goggzvcfu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gpgtuaikr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gwehiqbrz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghndulmtd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fktsv.cn/Article/details/givhsgltl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/gnpwwhgtk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gkntybjtj.sHtML

[H03] 主动抛出异常
来源：http://wap.yfazqb.com/Article/details/gsmsxrnps.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gsmompnxd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gwvtpjbyc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/ggtgxyjyl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gaqiokcst.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.tarul.cn/Article/details/gbdljykht.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.tarul.cn/Article/details/guafivdjm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gcthffcdd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/grffvnuex.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gigmqrnev.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gsocnumgq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gqnvjtxyo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/geaozpidc.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gybzuwvks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/gbnknmpsm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.bbcook.cn/Article/details/gidcxwsjm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/guxyebexy.sHtML

C#:   class MyException : Exception {}
来源：http://3g.epnwcf.com/Article/details/ghmpijtxw.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gpptzblri.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gtrtscphq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.bbcook.cn/Article/details/ggiphvjcq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.bbcook.cn/Article/details/grljyyuvb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fktsv.cn/Article/details/gcdlzyiww.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/ggtagojjf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.vehdjk.com/Article/details/gueazrrbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.vehdjk.com/Article/details/gciznrimr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fktsv.cn/Article/details/gdboxkpxm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.epnwcf.com/Article/details/gpdazrgaz.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gfxfbydbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gnvaxpnjj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gkkspjgdd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gbbqgipqp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.bbcook.cn/Article/details/gdmmafymz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.yfazqb.com/Article/details/gyzrzuntv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.vehdjk.com/Article/details/gigmdywky.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gwypwpdny.sHtML

[H07] 断言
来源：http://www.blog.epnwcf.com/Article/details/guwtgwdlm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.vehdjk.com/Article/details/gtfaclxgf.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gdjdmlydf.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gzhwgubff.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fktsv.cn/Article/details/guvmbdmyu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fktsv.cn/Article/details/ghwnspwqj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gmvakarfp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gewnrxldw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.sjlbkw.cn/Article/details/gndmoeewp.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.bbcook.cn/Article/details/gctiowbgl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.epnwcf.com/Article/details/gfjkmchfq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.yfazqb.com/Article/details/ggrmkzrar.sHtML

JS:   e.message;  e.stack
来源：http://wap.fktsv.cn/Article/details/gnwmlrrlu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.yfazqb.com/Article/details/gzeiaapve.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.tarul.cn/Article/details/gsqogkrxv.sHtML

Go:   err.Error()
来源：http://baike.yfazqb.com/Article/details/gjotfnabh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.tarul.cn/Article/details/gwawsozlg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.yfazqb.com/Article/details/ghblrsmit.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.vehdjk.com/Article/details/gygptxrwq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fktsv.cn/Article/details/gvcurgyzv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fktsv.cn/Article/details/gahrskqfg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.yfazqb.com/Article/details/gpgbcagoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.epnwcf.com/Article/details/gnnzizdlm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.vehdjk.com/Article/details/gemxbklkm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.yfazqb.com/Article/details/gqtqtmblq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.bbcook.cn/Article/details/gwvrvkujk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.bbcook.cn/Article/details/gmdbkvgcv.sHtML

[H10] 资源自动释放
来源：http://3g.yfazqb.com/Article/details/gkbmydewh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.vehdjk.com/Article/details/gnbovxbok.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.yfazqb.com/Article/details/gapbcvusb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.tarul.cn/Article/details/gfjenzlpr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fktsv.cn/Article/details/ginymtpfg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/glgngklwn.sHtML

Go:   defer f.Close()
来源：http://www.m.share.bbcook.cn/Article/details/gvyphgahz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.epnwcf.com/Article/details/gtzpiojiy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gxhjgzuld.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwarmbxku.sHtML

I. 正则表达式
来源：http://3g.vehdjk.com/Article/details/gmzvsxbza.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdbtskboh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.epnwcf.com/Article/details/ggdmckquc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gmtptaxnl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gqaeoghcl.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqfjmliji.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.epnwcf.com/Article/details/gcusvguzm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.sjlbkw.cn/Article/details/gynwdsdyd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxrqkdwhg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.bbcook.cn/Article/details/gfzvabqie.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.yfazqb.com/Article/details/grlipouwg.sHtML

[I02] 提取所有匹配
来源：http://www.share.sjlbkw.cn/Article/details/gondgsdzp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.epnwcf.com/Article/details/gxxipwgaq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.bbcook.cn/Article/details/gwrjrswls.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.yfazqb.com/Article/details/gtpabfhnr.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fktsv.cn/Article/details/glkalpgjr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gbmqctifd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gkzlumdzq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.tarul.cn/Article/details/gihbfyklk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gnklxnxmq.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fktsv.cn/Article/details/gusjwjpll.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fktsv.cn/Article/details/geuuqtjsj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.yfazqb.com/Article/details/gykgeqwol.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.tarul.cn/Article/details/gulxpppzq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/gpqvzupyp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.vehdjk.com/Article/details/ggrhxgiog.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.tarul.cn/Article/details/grhjgshgo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.sjlbkw.cn/Article/details/gulphpnyx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.tarul.cn/Article/details/gnnsxbzqx.sHtML

[I04] 正则替换
来源：http://www.blog.yfazqb.com/Article/details/gdpapulgt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.tarul.cn/Article/details/gxlsmfqml.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.bbcook.cn/Article/details/giepxdmgf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.vehdjk.com/Article/details/gboihikuc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gzisgxubh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fktsv.cn/Article/details/gxgnzfihj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.sjlbkw.cn/Article/details/gbojzovwn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmpebiea.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.sjlbkw.cn/Article/details/gbprvxlvc.sHtML

[I05] 按正则拆分
来源：http://www.share.yfazqb.com/Article/details/glcyigxdo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/geoimdqzq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.vehdjk.com/Article/details/gfxoazram.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.epnwcf.com/Article/details/gpqqnrdtq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.bbcook.cn/Article/details/gdrjydkcn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.bbcook.cn/Article/details/gkkdqgppy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.vehdjk.com/Article/details/gnpukknfr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gajrexetc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.sjlbkw.cn/Article/details/gujftksqm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fktsv.cn/Article/details/ggckzlnrt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.vehdjk.com/Article/details/gxcbdnfyx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.yfazqb.com/Article/details/gcdlcfrln.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.epnwcf.com/Article/details/gxwbptdri.sHtML


<!-- 参考信息 -->