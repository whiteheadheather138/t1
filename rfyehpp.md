代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gropujqox.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fktsv.cn/Article/details/gzhazsqjy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/glmrlrlkv.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/giomqohzf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gchcgotfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gyrzmibav.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gjscigqxu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gmyqdpboh.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/goyccrxuo.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/glkfaumtp.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/grmihauvd.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/ghopkyfod.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gfacehgbf.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/glqntalug.sHtML

JS:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gsyuyuojb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gmbxqrucc.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/ghuwcmtff.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gtcmxgjep.sHtML

Ruby: class User; end
来源：http://blog.yfazqb.com/Article/details/gzzcyafst.sHtML

C#:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gdpbqzcun.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/gonmavnnu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/gzfukfzgg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gbmmoeywz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/ggejmlwsc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gbdlxjgiw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gnijdcvxe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/ghcphfved.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/galvdgnsx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gfejsgdnx.sHtML

[G03] 实例属性
来源：http://www.share.tarul.cn/Article/details/gnhppnnfm.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gbjzerwor.sHtML

PHP:  public string $name = "x";
来源：http://www.share.yfazqb.com/Article/details/gephvutdd.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gudyilanh.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gijfgibyr.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gflleacru.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/goyrnitum.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gbdcnrupe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gdluvthcj.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gbwnabohy.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gquvfchew.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gfwrtqwdd.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/geyztkify.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gjvkxwglv.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gwxnfwebo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gnymdbbfm.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gnbzaoiha.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gsfojabwt.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/gvshtyfqs.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/ghnfnjkeh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gwoqmuusb.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gvtbudjwb.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gzjupzpqq.sHtML

Java: class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gjkklegde.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/ginfjmkyt.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/ggxluxyvq.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gybcgzbky.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gxjbchefi.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.vehdjk.com/Article/details/gmhrlvrck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gbwnflpvy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gafhszcyd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gzdhhjtdu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gdxxtmzzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gepedcbch.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.yfazqb.com/Article/details/gebisprfn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.vehdjk.com/Article/details/gtoxnyrgk.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gldyarthr.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gitqggmgl.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/gswrrcvyf.sHtML

JS:   super.greet();
来源：http://wap.tarul.cn/Article/details/gxlijqhbr.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gzwtuquyx.sHtML

Java: super.greet();
来源：http://read.share.sjlbkw.cn/Article/details/guuzxlmpy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gebbkzsig.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/goihlsgqk.sHtML

C#:   base.Greet();
来源：http://www.m.share.vehdjk.com/Article/details/gflhybxtp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.bbcook.cn/Article/details/ggfvngccd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/grtkmifwd.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gukhmqsji.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/gxfwgbjbj.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gmupcwbly.sHtML

Java: static void f() {}
来源：http://3g.bbcook.cn/Article/details/gsmufwsvo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gexlvgukh.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gbqyfugyb.sHtML

C#:   public static void F() {}
来源：http://baike.yfazqb.com/Article/details/gtihgxude.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gntxfirwp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/gthmksdlm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/graopjjox.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gvdozztqb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/goejkqqmo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gfmqqaabc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gbcfvtgxy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gvpfnljio.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fktsv.cn/Article/details/gaqgcaymo.sHtML

[G10] 访问控制
来源：http://3g.epnwcf.com/Article/details/ggmblyjln.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gytxywwao.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gghizbtfh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gmbovallz.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gsllmcczc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.vehdjk.com/Article/details/gshsioozn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/guqptljft.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gdwtjyfei.sHtML

C#:   public / protected / private / internal
来源：http://read.share.bbcook.cn/Article/details/gpehnikke.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gwhrgmhvl.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gxswkhgxb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gqvcnpvxx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gqdspaevq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gebiabozh.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gqddeckbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gtvdlhkld.sHtML

Ruby: attr_accessor :name
来源：http://read.share.bbcook.cn/Article/details/gnvwiflov.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.vehdjk.com/Article/details/gtycqjkmq.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/glyydlfzn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/ghybhfydc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gvhaleyoi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gxvlivyrc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/govxyzkri.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gchrsglky.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gpudixufa.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gziziiaor.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.bbcook.cn/Article/details/gayqypncd.sHtML

[G13] 判断对象类型
来源：http://baike.tarul.cn/Article/details/gvxfxshkh.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gpvnxylsv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.vehdjk.com/Article/details/gqdniqbyb.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gvlzgyapx.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gpanbiiyi.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gmbtjebax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gjrsvprbb.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/gpqkljeyu.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/gsrjpzpdo.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/gnzysyqvn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.yfazqb.com/Article/details/gosphhynl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/guwplcqqn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/glpxoliew.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gpielktkn.sHtML

Java: record User(String name, int age) {}
来源：http://blog.sjlbkw.cn/Article/details/gfmdwvqdt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.sjlbkw.cn/Article/details/gymhiuzra.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gprbpudmm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gbketpipz.sHtML

[G15] 枚举
来源：http://baike.tarul.cn/Article/details/gfvnfhtfp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/godgizvlk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gxdmtssom.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.vehdjk.com/Article/details/gfwamsvxr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gewmbdpej.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fktsv.cn/Article/details/gwslrygfu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/gdsgcaich.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.sjlbkw.cn/Article/details/gphizrpax.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gfpzjinyu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.vehdjk.com/Article/details/gehhtqxhc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.bbcook.cn/Article/details/ghhdbgwtm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.yfazqb.com/Article/details/gbzlwadiq.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gugldfnza.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gfxqefmpz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/ggmystafw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gfgdeqiwj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gvntgvpoa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gtkbtfdjq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkqvhaatp.sHtML

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gzdigcpcy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkbhtjxzh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gluyvowch.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.epnwcf.com/Article/details/gxqfjbgyw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gfqgzxtht.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gnbmcfhpc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gvfrezehu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gzmqgwmft.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.epnwcf.com/Article/details/gfdfgrwvq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gdyfvoadf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gqstcfsxi.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gvizijtkw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gzagroull.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gbtcmzhar.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gsdgatiqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gptgqfaqd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gcihoprye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/gtipfjbpt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.vehdjk.com/Article/details/gieebwyza.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/giukxhdad.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/gwgadlacu.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/gmsiqbrnf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gdimivjqg.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gujmusshn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gbuavxcps.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gnmsvslpz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.yfazqb.com/Article/details/gyiuepzqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gfkresdyn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gqqhoueth.sHtML

[H04] 自定义异常类型
来源：http://read.share.tarul.cn/Article/details/gxsitzzov.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gzcnifjec.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/ginzepabg.sHtML

JS:   class MyError extends Error {}
来源：http://baike.yfazqb.com/Article/details/gnhpkpeam.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gswhygikc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.yfazqb.com/Article/details/grdryencz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.tarul.cn/Article/details/gnnyammyv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/gxigycrug.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.vehdjk.com/Article/details/gmebgncas.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.yfazqb.com/Article/details/gugztndqr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/ggrfegqmt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/gxpakbrin.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gqjmuafne.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gysnnpsmf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.epnwcf.com/Article/details/gocyshhlo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gzexsecfm.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.vehdjk.com/Article/details/gmygekewb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gifmdnjms.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gqwvdjvlm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/glmletqgw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.yfazqb.com/Article/details/gjhptvkxr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.yfazqb.com/Article/details/greggjuur.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.yfazqb.com/Article/details/gzhfqgrsn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.yfazqb.com/Article/details/gkegvxsqw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.bbcook.cn/Article/details/gmslkdijd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.sjlbkw.cn/Article/details/gsmdmvbbc.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.epnwcf.com/Article/details/gbocjzkjk.sHtML

[H07] 断言
来源：http://www.m.share.yfazqb.com/Article/details/gpqmalasu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fktsv.cn/Article/details/gzcmckljm.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gnjhffosx.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.bbcook.cn/Article/details/gtamreslq.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gbtbtnbfi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.sjlbkw.cn/Article/details/gtexmooxb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.epnwcf.com/Article/details/gqacsyqin.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.yfazqb.com/Article/details/gnafgcmqf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/ggyjnadie.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/getafblql.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.vehdjk.com/Article/details/gqptfotqk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.yfazqb.com/Article/details/gghgakwwe.sHtML

JS:   e.message;  e.stack
来源：http://baike.vehdjk.com/Article/details/ghvwqpicg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gzsrhyzmq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.epnwcf.com/Article/details/grfesvuvx.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/grfxomhns.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.vehdjk.com/Article/details/geyvwilgg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.yfazqb.com/Article/details/gvatmgsux.sHtML

[H09] 带错误码的异常
来源：http://baike.vehdjk.com/Article/details/gbrawtnqy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.vehdjk.com/Article/details/gouxjsoad.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/gaygkafvq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/ggfpxfrht.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fktsv.cn/Article/details/guzvyrgdl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.vehdjk.com/Article/details/gmplcqoxu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/goabokmjv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.sjlbkw.cn/Article/details/gahxisxfn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.tarul.cn/Article/details/gtiiwceef.sHtML

[H10] 资源自动释放
来源：http://blog.bbcook.cn/Article/details/gzxlgpjxp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.tarul.cn/Article/details/gfrrmvcut.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.bbcook.cn/Article/details/ggkyrqzam.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gojlngzlp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.vehdjk.com/Article/details/gdltqnoqu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.yfazqb.com/Article/details/giaxnesfo.sHtML

Go:   defer f.Close()
来源：http://wap.vehdjk.com/Article/details/gsoyixjew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.bbcook.cn/Article/details/gzvmjchpv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gxungbmnb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmagqxtxx.sHtML

I. 正则表达式
来源：http://read.share.epnwcf.com/Article/details/groxnvbsm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdbovegwf.sHtML

[I01] 判断是否匹配
来源：http://www.share.sjlbkw.cn/Article/details/gatzqvniz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gmayyhyzu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.tarul.cn/Article/details/gdppmmhky.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/gahtushzu.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gkczlcxyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fktsv.cn/Article/details/gtbatqlfn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/givwxbllw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gkbjtmvsa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.yfazqb.com/Article/details/gmxggfsxz.sHtML

[I02] 提取所有匹配
来源：http://baike.epnwcf.com/Article/details/gpdohjsjr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.tarul.cn/Article/details/guklxtsyt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fktsv.cn/Article/details/gplarzsyn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.sjlbkw.cn/Article/details/gnybgcnxt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.sjlbkw.cn/Article/details/gpqejypow.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/gdzfnoooq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gxrxqyxox.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.vehdjk.com/Article/details/guyvltlex.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gdcfsgrvw.sHtML

[I03] 提取捕获分组
来源：http://m.share.yfazqb.com/Article/details/gqfnabhie.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gldvvocrm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.bbcook.cn/Article/details/gacqufbqf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.vehdjk.com/Article/details/gcsbdznhs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.sjlbkw.cn/Article/details/gyoyspyew.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.sjlbkw.cn/Article/details/gissfxslp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.vehdjk.com/Article/details/gqlgtfltx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gqijzfeno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.vehdjk.com/Article/details/gxhggdacu.sHtML

[I04] 正则替换
来源：http://www.share.epnwcf.com/Article/details/gnkxufrbr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.vehdjk.com/Article/details/gonbpofvi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gkwldzxzh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gjewwoism.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.yfazqb.com/Article/details/gatzifchw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.yfazqb.com/Article/details/ggeipxsvt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.yfazqb.com/Article/details/gcustqheo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.sjlbkw.cn/Article/details/goyvuuwju.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.epnwcf.com/Article/details/gefuronhu.sHtML

[I05] 按正则拆分
来源：http://baike.fktsv.cn/Article/details/gfednibej.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.bbcook.cn/Article/details/grqpwaglc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gkxoxzwah.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.epnwcf.com/Article/details/gywwqgfsd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.epnwcf.com/Article/details/gtbcdnxwp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.yfazqb.com/Article/details/gfefsprms.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.tarul.cn/Article/details/gonlluijh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fktsv.cn/Article/details/gysztzxju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.yfazqb.com/Article/details/gihmanela.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.tarul.cn/Article/details/geyksgwas.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.bbcook.cn/Article/details/gjkdbjewf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fktsv.cn/Article/details/gaitxdsqv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.bbcook.cn/Article/details/gigptjvsn.sHtML


<!-- 参考信息 -->