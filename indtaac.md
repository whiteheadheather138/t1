代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gceqyvhxi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gitmxosed.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gpsnpjbhy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gxcvcliyb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/ghkdqtzzt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gnwscwgtg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fktsv.cn/Article/details/gbtdgchxe.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gqvvjkamj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.tarul.cn/Article/details/gtlbmkwfp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gtdbijaex.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gcweqgzta.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/gcfnrgtev.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gpdkcegnf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/glqthrdev.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gtpfsfvbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gchukmsqn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjxkvuxod.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/grfullmls.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxmxjswmg.sHtML

[G01] 定义类
来源：http://mobile.vehdjk.com/Article/details/gzdyadmgw.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/glykoagwz.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gijqvpycq.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gjkocnkrs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/gcisshwhj.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/ggrejmhfp.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gkthxcixp.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gyeehnxoq.sHtML

C#:   class User {}
来源：http://read.share.vehdjk.com/Article/details/gxnhbxzbp.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gaoxerruq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.tarul.cn/Article/details/gkvkqmtkn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.sjlbkw.cn/Article/details/gkevisxfb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.yfazqb.com/Article/details/gankxrfzx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gjqgomgxo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/grpbjwpal.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gwiuwupse.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.bbcook.cn/Article/details/gcyaehvxa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gggkzfcon.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gyfsurhji.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gxfcapevg.sHtML

PHP:  public string $name = "x";
来源：http://blog.vehdjk.com/Article/details/gvtphhvzv.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/ghxbsxduk.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/gvdeygsln.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/gwghxqjpq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gecnkdcoy.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/ghbpmwycz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gmndmznzk.sHtML

[G04] 定义方法
来源：http://mobile.sjlbkw.cn/Article/details/gfnglqpgf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gwgvadazp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gprwhucmu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/grcihqgvs.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gjedjsljt.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gwsgclhiy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/gjbifhwut.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gdiqlzyyr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gvwlsmrli.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gbjpnwbes.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gegskztmg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gytxrcfjj.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gjqvehpnt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gfehzvcky.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gzizppuhu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gaueofkvr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.bbcook.cn/Article/details/gbdbbbrai.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gqnvjygwk.sHtML

[G06] 重写方法
来源：http://m.share.bbcook.cn/Article/details/gnuojthvq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gqytvnmyl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gkxzqdfnq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gukqpnotn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gfxqneyep.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/ghorkbelt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/glhotifdr.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fktsv.cn/Article/details/ggaunsaab.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.sjlbkw.cn/Article/details/gtfuyufqm.sHtML

[G07] 调用父类方法
来源：http://m.share.fktsv.cn/Article/details/ghlzeksdw.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gjqlgoqwy.sHtML

PHP:  parent::greet();
来源：http://www.m.share.yfazqb.com/Article/details/gtwybgbfw.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gilqrcahv.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gvdskkhgg.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gmdasyppj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.vehdjk.com/Article/details/ghujfjudu.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gnbmizvne.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/gkqukzpvv.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gbljrnfju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.vehdjk.com/Article/details/gmdlozams.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/govrhdbau.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gwpyuvhzq.sHtML

TS:   static f(): void {}
来源：http://baike.fktsv.cn/Article/details/gviixjvmo.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gcfjnuhoz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fktsv.cn/Article/details/gqcyxzuhe.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gfckxcjlw.sHtML

C#:   public static void F() {}
来源：http://read.share.sjlbkw.cn/Article/details/gjdpvbrth.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gkigtuygf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/ggklnteqh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.epnwcf.com/Article/details/gxcjehudn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.sjlbkw.cn/Article/details/gcpuxrabl.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.yfazqb.com/Article/details/gjjaqsdlz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.yfazqb.com/Article/details/gvgbjoxnj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gcjyoemxl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/grslmbtnv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gsqkbmrps.sHtML

[G10] 访问控制
来源：http://wap.tarul.cn/Article/details/ggeyhqdij.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gukqxsopr.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gbdqbcgbb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.epnwcf.com/Article/details/grgdndrqh.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/grjikedqd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.epnwcf.com/Article/details/gipeenqco.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gnzgdaczz.sHtML

Ruby: public / protected / private
来源：http://3g.epnwcf.com/Article/details/gukzjpech.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gubzsnsbo.sHtML

[G11] getter / setter
来源：http://mobile.yfazqb.com/Article/details/gsztazqst.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/ghuozqthe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gdznniqgc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gkoiefoqh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.yfazqb.com/Article/details/gydzqzzel.sHtML

Java: public String getName() { return name; }
来源：http://3g.epnwcf.com/Article/details/gckflnsvr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/goybprkmq.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/gqfrbduhe.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gzwnbzawd.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gfqgjuffa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gmegqosrs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/grekvquyk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gkqissujv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqdhrmiau.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.tarul.cn/Article/details/gwtvygdhn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/ghtnhqlma.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gpmrrdpqa.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.vehdjk.com/Article/details/grfmfmrjd.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/grufrstin.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gmzchjmtk.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/giwhnjuqo.sHtML

JS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gficmtuhf.sHtML

TS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gdxmkolyd.sHtML

Java: u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gsltvmjdm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gikzoleif.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gwuhjtxsd.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gigpebqgq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gxufkulpm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gspugnllc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.epnwcf.com/Article/details/glznsqpxj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.vehdjk.com/Article/details/gjgwkviev.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gufphbkjl.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.epnwcf.com/Article/details/gdnnuqwnw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gjtifpnus.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.yfazqb.com/Article/details/grffslafh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.sjlbkw.cn/Article/details/ggpxpskyp.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/gmmjggoph.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.vehdjk.com/Article/details/geomdaqql.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gmnrubkze.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/gzyisyaqq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gwrpvpyvs.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.sjlbkw.cn/Article/details/gsqfxiiyh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.sjlbkw.cn/Article/details/gzdickteh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/gasdqfrvx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gkjhoiezd.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/gcxccbhok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gwtcaxfxf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gfhqvqahd.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gqyuzcsri.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/goajjskkt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/grebfgbqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/getmqebmd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/gsjpgkfbz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gwnfmeilu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gavgiueoo.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gibiluqeo.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gqdejpgst.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/ginbdkawk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gffkwvpta.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.bbcook.cn/Article/details/gaxzkeuuh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gmlldsqog.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gnkslgvxg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.epnwcf.com/Article/details/gbstltzny.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.tarul.cn/Article/details/gwpjnqcgw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gvhbzcxdl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.epnwcf.com/Article/details/gvhvhhubj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gwmbyxlyl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.epnwcf.com/Article/details/gspfuxlwk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gsqiqedtb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gmlikacsz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gqtioinbn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gfnztciys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.tarul.cn/Article/details/gwclsummx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gbclqhvke.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gbevalyqa.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gcnrgxbjj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.sjlbkw.cn/Article/details/gmqhljzvp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gajvljfen.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gihqcjxnc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gfzcrkqbo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gouruihhl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gcixjoaov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gdzdwmxej.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/ghekswtfx.sHtML

[H04] 自定义异常类型
来源：http://www.share.bbcook.cn/Article/details/gfknmzwpy.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.vehdjk.com/Article/details/gufkofhuw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/ggqxmtkus.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gsyumohvw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.sjlbkw.cn/Article/details/gbmodteqi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.tarul.cn/Article/details/gtyeqrray.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gdlhrimbs.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.bbcook.cn/Article/details/gewomcefg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.tarul.cn/Article/details/gamjgiroj.sHtML

[H05] 捕获特定类型
来源：http://mobile.yfazqb.com/Article/details/glxkdaobi.sHtML

Py:   except ValueError as e:
来源：http://www.blog.yfazqb.com/Article/details/gzawgtoge.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gooffykdl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gxqhcfync.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gddmnxxuu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/gustpytso.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gosemxgjx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/giotqnzss.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gxyevpcwf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/ggiycjefp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.bbcook.cn/Article/details/gskvqfzsb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/ghawoukwv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/ghocpouoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/gghtyityn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gzgwpgqfe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.tarul.cn/Article/details/gqybbsjfg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gkryutszl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gemyxsfwa.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gzhcrbppm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.vehdjk.com/Article/details/guioxyeez.sHtML

PHP:  assert($x > 0);
来源：http://blog.tarul.cn/Article/details/gzslaivqq.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gxohgskqr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.yfazqb.com/Article/details/gtfqdduwm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/gxasjcqdu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.epnwcf.com/Article/details/gxquzehnn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.bbcook.cn/Article/details/gvbkeghms.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.yfazqb.com/Article/details/gxapllanz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.tarul.cn/Article/details/gjyynzzyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.sjlbkw.cn/Article/details/gvbrlsvgs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.yfazqb.com/Article/details/gotscunme.sHtML

JS:   e.message;  e.stack
来源：http://blog.epnwcf.com/Article/details/gpakuipio.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.sjlbkw.cn/Article/details/gqyowdlki.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.tarul.cn/Article/details/gbpxzzqom.sHtML

Go:   err.Error()
来源：http://mobile.epnwcf.com/Article/details/gonxmesfw.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fktsv.cn/Article/details/gsvnpbunz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fktsv.cn/Article/details/gspuslfki.sHtML

[H09] 带错误码的异常
来源：http://read.share.vehdjk.com/Article/details/gcudfqzgn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.bbcook.cn/Article/details/gqanfzeoe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gkamztdii.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.yfazqb.com/Article/details/gsykpvaix.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.yfazqb.com/Article/details/gtobnaogq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.bbcook.cn/Article/details/ghiehetxw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.bbcook.cn/Article/details/gauganoqm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fktsv.cn/Article/details/gmbcgafth.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.tarul.cn/Article/details/gisyhlasn.sHtML

[H10] 资源自动释放
来源：http://baike.vehdjk.com/Article/details/gukjcuhwb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.vehdjk.com/Article/details/gkcxkavje.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.epnwcf.com/Article/details/ghoxkgsdh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.tarul.cn/Article/details/gwlwvbgkj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gwsqgajen.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fktsv.cn/Article/details/gksigvxfk.sHtML

Go:   defer f.Close()
来源：http://www.share.vehdjk.com/Article/details/gpjdxkarb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.vehdjk.com/Article/details/gykltnhlw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.vehdjk.com/Article/details/goakkmkgw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqidopowb.sHtML

I. 正则表达式
来源：http://blog.epnwcf.com/Article/details/gtizgvhay.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfihimfve.sHtML

[I01] 判断是否匹配
来源：http://m.share.sjlbkw.cn/Article/details/gzwiavybt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.bbcook.cn/Article/details/gvdtumhkr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.yfazqb.com/Article/details/gydrdmjrj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.yfazqb.com/Article/details/gtbjoexca.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.epnwcf.com/Article/details/grcusolbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.sjlbkw.cn/Article/details/gpuipgdjt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/gwhfccajd.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.epnwcf.com/Article/details/gjihjzywi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.yfazqb.com/Article/details/gagyonhzh.sHtML

[I02] 提取所有匹配
来源：http://3g.epnwcf.com/Article/details/gqqrveclb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.epnwcf.com/Article/details/gmnzqcqbm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.bbcook.cn/Article/details/ghgofmblo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.yfazqb.com/Article/details/gezbcujpj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.sjlbkw.cn/Article/details/gkkiqfuib.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.sjlbkw.cn/Article/details/gwusoobst.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gnhckvnsf.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.yfazqb.com/Article/details/gkcjszija.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.yfazqb.com/Article/details/gujwbpxig.sHtML

[I03] 提取捕获分组
来源：http://www.share.yfazqb.com/Article/details/goyhsbgzu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.sjlbkw.cn/Article/details/gvtprjbus.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.epnwcf.com/Article/details/gbvsxjrlh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/glfudkjgm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.epnwcf.com/Article/details/gctsbsllu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.vehdjk.com/Article/details/gtsnzekyd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.bbcook.cn/Article/details/ggyiffzin.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.vehdjk.com/Article/details/gxqzmqtvu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.yfazqb.com/Article/details/gonujqlah.sHtML

[I04] 正则替换
来源：http://www.m.share.tarul.cn/Article/details/geubyhnle.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/guqraazjh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gvzgcwocc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.sjlbkw.cn/Article/details/gysdctoye.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.vehdjk.com/Article/details/gxulmzeiw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.yfazqb.com/Article/details/gcrdbsfvk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fktsv.cn/Article/details/gtjsvhhnc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.yfazqb.com/Article/details/gkgpkryqo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fktsv.cn/Article/details/geusgknoq.sHtML

[I05] 按正则拆分
来源：http://baike.epnwcf.com/Article/details/gucnslooq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.bbcook.cn/Article/details/ggqphuijh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gfwxsrcrl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.vehdjk.com/Article/details/gnvjvvzgd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.vehdjk.com/Article/details/gsixhbajw.sHtML


<!-- 参考信息 -->