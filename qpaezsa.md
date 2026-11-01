代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gzanyruam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gqwfkfbvl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gjtwlwapc.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gypivzjqa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gotxhdiap.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gawgwmyvm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fktsv.cn/Article/details/gtscgdvzo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gfwewgvox.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giakgibsk.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gjtpsyckn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gtduslaaa.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gukszqppl.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gwljhgpzh.sHtML

PHP:  class User {}
来源：http://read.share.epnwcf.com/Article/details/gpepbgaef.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/grgdeagvm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/guuoufepk.sHtML

Java: class User {}
来源：http://m.share.tarul.cn/Article/details/gthbzawka.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/grwkxtcui.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gkwmjxrga.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gmbqjhmrd.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gorhdnpyh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gqhnesybx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gpjeocjpl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gcapljmih.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.sjlbkw.cn/Article/details/glnydxeid.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gjiajyryh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.epnwcf.com/Article/details/gciqfsfmd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/givpcswqe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gjcyoiqbv.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gmbilaehs.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gtvsboqaw.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/giqwzymkl.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gytuafbna.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/ghxrwcrpx.sHtML

Java: private String name;
来源：http://www.share.yfazqb.com/Article/details/ghzanjfwe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/giofqaodm.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gdyghiuxs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqilrgild.sHtML

[G04] 定义方法
来源：http://www.m.share.epnwcf.com/Article/details/gtsnycacz.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gqayubrpq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gyrufeeum.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gqaimyksg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gtzhposog.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gjwglgevn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gzdgaftpr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/gqpzblrzl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.sjlbkw.cn/Article/details/gbjmbofub.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gkwgfifit.sHtML

Py:   class Admin(User): pass
来源：http://mobile.yfazqb.com/Article/details/geeijfuav.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/ghwhjfpvh.sHtML

JS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gzvywwgip.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/ghfumugep.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gfslpdrdq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/grgqdmxxn.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gutzlshsr.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/ggxpryfdh.sHtML

[G06] 重写方法
来源：http://m.share.vehdjk.com/Article/details/ghttoprkf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.vehdjk.com/Article/details/goivudqft.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gjhwkgzms.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gvowuqxyj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/gbmottpot.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/guccaxzgx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.bbcook.cn/Article/details/gbxpjhcst.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.sjlbkw.cn/Article/details/gljzbzxil.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/guzzoubzf.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gydpsjcjt.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/ghjrpitzh.sHtML

PHP:  parent::greet();
来源：http://3g.epnwcf.com/Article/details/gclmwukgj.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/guagmwqtd.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gxhkbwlxq.sHtML

Java: super.greet();
来源：http://mobile.fktsv.cn/Article/details/guzzzvlwi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/gtsieytym.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gymqvuesn.sHtML

C#:   base.Greet();
来源：http://baike.epnwcf.com/Article/details/gwucztvta.sHtML

[G08] 静态方法与属性
来源：http://mobile.epnwcf.com/Article/details/gepseuozd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.sjlbkw.cn/Article/details/goymbvwnl.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/geqsgvdgd.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gbziafcsm.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gdfquwsqz.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/guoolcfxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.yfazqb.com/Article/details/gonsftowr.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/ghthguxnb.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gojlpbidn.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/giueqbofn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fktsv.cn/Article/details/gysrlamdo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.vehdjk.com/Article/details/ganhxszkj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.bbcook.cn/Article/details/gblagubar.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fktsv.cn/Article/details/gbatdhbhw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gbhytwwdb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gykufkxea.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.bbcook.cn/Article/details/gmqbcnbbh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.epnwcf.com/Article/details/gtpoxsoln.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/gnkzxbizo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gigzvxjca.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gwelmpdlg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/gicvaqtnl.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/ghhgnmqhn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gdtnfmklz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gszbyinpf.sHtML

Ruby: public / protected / private
来源：http://baike.vehdjk.com/Article/details/gkjqowcmp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/geznioime.sHtML

[G11] getter / setter
来源：http://read.share.tarul.cn/Article/details/gwyrelcte.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.yfazqb.com/Article/details/gpvhsetlf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gpxugugdd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gleaupyiz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gjqkyiqrj.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/gccebowhr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gqwjxfsim.sHtML

Ruby: attr_accessor :name
来源：http://mobile.epnwcf.com/Article/details/gnhodlnrz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gszrbzolo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gwknbuwjy.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.tarul.cn/Article/details/grlzuylzw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gsibxxslw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gzaixzqrh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/goklewrmx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/gnvjhpuxl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gexcmwvpi.sHtML

Ruby: def to_s; @name; end
来源：http://blog.yfazqb.com/Article/details/gwfgfqhsq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gtfvgfhpb.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/grxigdwia.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/goeytsudg.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gllgbzwts.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gkaipmnlh.sHtML

TS:   u instanceof User
来源：http://wap.bbcook.cn/Article/details/gkehxonry.sHtML

Java: u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gpxtunqzv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmhakba.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.tarul.cn/Article/details/grafdgjzm.sHtML

C#:   u is User
来源：http://www.m.share.bbcook.cn/Article/details/gdzczydxq.sHtML

[G14] 数据类 / record
来源：http://blog.vehdjk.com/Article/details/gixwcwfkp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.bbcook.cn/Article/details/gueeeijml.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.tarul.cn/Article/details/gizlzkrad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gfcqivhiz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.sjlbkw.cn/Article/details/gxbjyfuue.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gtizvbetd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gatfakjme.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gnzainmsi.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/ggnzechah.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gaqbgxqun.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fktsv.cn/Article/details/gcwszzliy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gngqloluc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.vehdjk.com/Article/details/gskijwnio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gtyinwncf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gikyxtbkl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gvnfijqbb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/gccwcesoa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gsoeizuvi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gwcuhabrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gelvhsgfh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.sjlbkw.cn/Article/details/gxmhvvarw.sHtML

JS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gwroptegl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gflrwfbnl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.tarul.cn/Article/details/gxpcvojpm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fktsv.cn/Article/details/geycooemz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gtqosazui.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gvldoqukz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/giiobzxhb.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gmfvsvkhq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzmwdgsft.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gvzdxorko.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gzpguvicp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/glnahqnww.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gcunuowyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gliegzcck.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.bbcook.cn/Article/details/gzagiwgpo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gtknjrwex.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.tarul.cn/Article/details/gszgrmxis.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.sjlbkw.cn/Article/details/gcrmzmsof.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gqwdecqxr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.vehdjk.com/Article/details/gqusqcqbb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gawqbnsbj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gqnwovlmu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gqohmgict.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/gkwkinxgf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gahmmzikm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gnnfjmtht.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gsxvhjejd.sHtML

[H03] 主动抛出异常
来源：http://3g.tarul.cn/Article/details/gwesovobh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.yfazqb.com/Article/details/goezmlwzz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/gqukysrei.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.yfazqb.com/Article/details/gswttkdab.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gaxjamfjn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/guhjkxzxq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gxpiwkymu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fktsv.cn/Article/details/gdxvioanr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/guxopqkql.sHtML

[H04] 自定义异常类型
来源：http://www.blog.yfazqb.com/Article/details/gkkcxrazt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gqfaclzwt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gbhifiyev.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gkfsztqtp.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/grlnoqbfa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/gsgbkjpcq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.epnwcf.com/Article/details/glmhjeylb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gnwjvihsf.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/ghiskjmkv.sHtML

[H05] 捕获特定类型
来源：http://3g.fktsv.cn/Article/details/gdnfvaqzt.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gkdpfzcbq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fktsv.cn/Article/details/gsqcwgffl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gdjwcjjmg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/guwxxiyhs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.bbcook.cn/Article/details/gmqpqrvba.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.bbcook.cn/Article/details/ggxnaetcf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gscntzicy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.epnwcf.com/Article/details/gqfiymzjx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/grtoxydzb.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.sjlbkw.cn/Article/details/gpgjhrdzm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/ggkqkvwpl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/greklwygk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.vehdjk.com/Article/details/gxnegkyee.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.epnwcf.com/Article/details/gkjcsqhun.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.yfazqb.com/Article/details/gabeoetnb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.sjlbkw.cn/Article/details/gokmyldlv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.vehdjk.com/Article/details/gzheyjqml.sHtML

[H07] 断言
来源：http://blog.tarul.cn/Article/details/gkhsfbosr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gjxlmqgoa.sHtML

PHP:  assert($x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gtjieejdc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/gstniowch.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.sjlbkw.cn/Article/details/gxqsqdkqe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.vehdjk.com/Article/details/gffrzzffj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.tarul.cn/Article/details/gvwxozxzp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.vehdjk.com/Article/details/gmhggupug.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.yfazqb.com/Article/details/gasijilzr.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.sjlbkw.cn/Article/details/gbfcalpzp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/gyqcoojxz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.tarul.cn/Article/details/ghlosnetk.sHtML

JS:   e.message;  e.stack
来源：http://baike.epnwcf.com/Article/details/gayzwwjqz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.bbcook.cn/Article/details/gqhifdqqt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.tarul.cn/Article/details/gxglmxhmv.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/gepivknug.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.epnwcf.com/Article/details/gqgdezuey.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.sjlbkw.cn/Article/details/geicwgmue.sHtML

[H09] 带错误码的异常
来源：http://m.share.sjlbkw.cn/Article/details/giuenyqcu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.sjlbkw.cn/Article/details/gcfmlotdx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.epnwcf.com/Article/details/geksubkiw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.sjlbkw.cn/Article/details/gocxsyiww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.vehdjk.com/Article/details/gyvtqgzds.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/gnrevjspw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.vehdjk.com/Article/details/ghmrpsapa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.yfazqb.com/Article/details/gkdjvqvqd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.vehdjk.com/Article/details/gmlgqsnbz.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fktsv.cn/Article/details/gluxjfyee.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.sjlbkw.cn/Article/details/gnjtlkhqv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.yfazqb.com/Article/details/gvkqdrhtf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/gbwzwzbsg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.tarul.cn/Article/details/gsftmqgoi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.yfazqb.com/Article/details/guiswfnqx.sHtML

Go:   defer f.Close()
来源：http://baike.vehdjk.com/Article/details/goijdklhi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.yfazqb.com/Article/details/gvfqywqlr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gorxvxxgm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzuhejelu.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gjehgwqbg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gpaxvveok.sHtML

[I01] 判断是否匹配
来源：http://read.share.vehdjk.com/Article/details/gsjriokvc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gomjsdgfn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gkqppluvr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.sjlbkw.cn/Article/details/gpwdpeljs.sHtML

TS:   /\d+/.test(s)
来源：http://blog.tarul.cn/Article/details/gdvayogtk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.yfazqb.com/Article/details/gfcjsevzq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fktsv.cn/Article/details/grezsahfi.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.sjlbkw.cn/Article/details/gavbiinwo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gxlvlmkkn.sHtML

[I02] 提取所有匹配
来源：http://3g.yfazqb.com/Article/details/ghfkrzvly.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.vehdjk.com/Article/details/glaoijwuk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.tarul.cn/Article/details/gmgeitujh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.bbcook.cn/Article/details/gejwyywvd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.yfazqb.com/Article/details/glqvdjdkf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.epnwcf.com/Article/details/gnjiworjl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.yfazqb.com/Article/details/gkykrmctk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gggmrijho.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.sjlbkw.cn/Article/details/grmwvpbyz.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gmtndnjcq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fktsv.cn/Article/details/gxjvazfxg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.sjlbkw.cn/Article/details/gqsuqyzcu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.tarul.cn/Article/details/gwzwwnftd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.epnwcf.com/Article/details/gwoykyqyv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/ginmsvsae.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.epnwcf.com/Article/details/gqpikwumq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.sjlbkw.cn/Article/details/ggmoxchsk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.epnwcf.com/Article/details/gydxpzhwn.sHtML

[I04] 正则替换
来源：http://www.share.vehdjk.com/Article/details/givtbuona.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.epnwcf.com/Article/details/ginnvyrrh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gibctgscv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.bbcook.cn/Article/details/gmvipdzkp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.tarul.cn/Article/details/gggqrhgqf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.yfazqb.com/Article/details/gntxcfilr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.yfazqb.com/Article/details/ggmnbszaf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.tarul.cn/Article/details/gughgqsja.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.vehdjk.com/Article/details/ghwyxqecp.sHtML

[I05] 按正则拆分
来源：http://blog.sjlbkw.cn/Article/details/gpccmevdf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.bbcook.cn/Article/details/gxzqeqqbb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.tarul.cn/Article/details/grqfqbpro.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.tarul.cn/Article/details/gdcgdojng.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.vehdjk.com/Article/details/gfhlnyjii.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.tarul.cn/Article/details/gltcmgjni.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.epnwcf.com/Article/details/gwpkxckyu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.yfazqb.com/Article/details/gmffotznq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.epnwcf.com/Article/details/gkchmwddy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.tarul.cn/Article/details/gjmujcxaw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.epnwcf.com/Article/details/gwcsoamkf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.vehdjk.com/Article/details/gtabusyzu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.tarul.cn/Article/details/gcnmqjkgo.sHtML


<!-- 参考信息 -->