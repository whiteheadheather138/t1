代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gatzcdpjk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gndjcgjwu.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/gmczfkwmg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gfggghkdv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gjpyvswbu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gcmlungqp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gikbdkwnf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gxdbuhgzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/gaozakhsk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gxpwcjoak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gpszvblrp.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gtzvkuzot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gvnbyziwm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/glcmyftre.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gxqandcdg.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gjzykdaff.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gcydhdsvv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gorxvjuot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.tarul.cn/Article/details/gigeqjywh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/grmuyaaml.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxmuehbip.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gzvmmyhxe.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbteqncfz.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gmbyxdpco.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gziwpqesi.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gkurwzxwf.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gwygnmwuh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gpxlpiqxb.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gpvpegbdw.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/grmnngdfr.sHtML

Ruby: class User; end
来源：http://baike.fktsv.cn/Article/details/ggenugtkk.sHtML

C#:   class User {}
来源：http://m.share.epnwcf.com/Article/details/gqdjdsulw.sHtML

[G02] 构造函数
来源：http://read.share.sjlbkw.cn/Article/details/gjlkcxgwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gsbguydjb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gfyyjueob.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gwtllvomt.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gwcvycekg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gsycifymv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gpyqomfjz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gpoauupmi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gxpsddzmp.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/gzmgzfegi.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gepkfdkcx.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/giafiesef.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/grrjllnna.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gpyvzlajk.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gblacqvxg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gkpfdwpgz.sHtML

Ruby: @name = "x"
来源：http://blog.yfazqb.com/Article/details/gsifdmhvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gjcdxyhve.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gsqrkzzbo.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/giomfxfym.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gexkwfltz.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gooegurvc.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/guacvhemv.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gnnefnojq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gfjuajoub.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gnaqfsrnb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gscwowxhd.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/goxwdvclb.sHtML

Py:   class Admin(User): pass
来源：http://3g.tarul.cn/Article/details/gfkroxzdm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gfqprjhbl.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gdfabsipk.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gpzuxnycu.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gfwqgenje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gtynefgbn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/gslsotzyx.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gbiteonzo.sHtML

[G06] 重写方法
来源：http://mobile.sjlbkw.cn/Article/details/gsnbibgsg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/gvwbnkmek.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gznroodby.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gpnqkuwfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gfdgolwij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gbsmxrxtq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gxhagpaon.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gzcjleevq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/ggqhyqjem.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/govenyjxb.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gfpifobgl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.tarul.cn/Article/details/gkzeuzops.sHtML

JS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gupwovzmm.sHtML

TS:   super.greet();
来源：http://baike.yfazqb.com/Article/details/gdammtuqj.sHtML

Java: super.greet();
来源：http://read.share.epnwcf.com/Article/details/gmwwolvzd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.tarul.cn/Article/details/gdvttmlxk.sHtML

Ruby: super
来源：http://www.blog.yfazqb.com/Article/details/gflxcdorb.sHtML

C#:   base.Greet();
来源：http://3g.epnwcf.com/Article/details/gbznyixkh.sHtML

[G08] 静态方法与属性
来源：http://m.share.bbcook.cn/Article/details/gkawsywxm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.tarul.cn/Article/details/gbhzqjojo.sHtML

PHP:  public static function f() {}
来源：http://3g.fktsv.cn/Article/details/gpkpxtxvr.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gdikgwrav.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gcqgvegkk.sHtML

Java: static void f() {}
来源：http://wap.tarul.cn/Article/details/gauxfdfvw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.epnwcf.com/Article/details/glkflshqp.sHtML

Ruby: def self.f; end
来源：http://www.share.epnwcf.com/Article/details/grulzmsxc.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gpjspunla.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gyaynuaqk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gnscxymvl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gdnbxojmj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gnrnijsfo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.epnwcf.com/Article/details/gnqvwajit.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/glfaybldz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fktsv.cn/Article/details/gjtmhuote.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gchqivpyb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gajzpdhpe.sHtML

[G10] 访问控制
来源：http://www.blog.sjlbkw.cn/Article/details/gjjbgpimp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/ghotjnmwt.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gdpsarlpb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/giygubtzo.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gpremymeu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gmcwhidih.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/glbcrtknh.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gfioqbzsm.sHtML

C#:   public / protected / private / internal
来源：http://wap.sjlbkw.cn/Article/details/gfuovedgb.sHtML

[G11] getter / setter
来源：http://mobile.epnwcf.com/Article/details/gdlqxmbin.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gnveskuzx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gymwkpczd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gfbexoxpg.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gfbfnbwjc.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gcmbkbdoj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gxrojzctw.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.epnwcf.com/Article/details/gpollouue.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gigwpkxzg.sHtML

[G12] 对象转字符串
来源：http://3g.tarul.cn/Article/details/gljzoftwv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gndnwkrmr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gtnmqpqqd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gabyglxgp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/ghaqyldcq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsmfygadi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/guunnkdzi.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gzdhvjtsw.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gvotfjsgj.sHtML

[G13] 判断对象类型
来源：http://m.share.bbcook.cn/Article/details/gfysctaan.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gtgptlrtn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/grmmbfmrl.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/ggnjmpfnb.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/grzzxhbbi.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gzwioqbxr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.sjlbkw.cn/Article/details/gnennwlpy.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gfoyjppde.sHtML

C#:   u is User
来源：http://read.share.epnwcf.com/Article/details/gzrjjqngs.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/ggnbzddxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gqfwafwed.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gzzecadbb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.vehdjk.com/Article/details/gxpzopddy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gkjoebxxm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.bbcook.cn/Article/details/gxrarzegv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.epnwcf.com/Article/details/gqkxedajj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.sjlbkw.cn/Article/details/gvazdurtq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gzmqtdazf.sHtML

[G15] 枚举
来源：http://www.m.share.tarul.cn/Article/details/gfppduzri.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/gfgobfypf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.yfazqb.com/Article/details/gfcblovkf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.yfazqb.com/Article/details/grftpqyep.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gqjythhcq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.vehdjk.com/Article/details/guyhmjiof.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/guwbuxqwl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gzrbpcoqk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gjcjfdqhx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gokljzssn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.epnwcf.com/Article/details/gpcajqlst.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.sjlbkw.cn/Article/details/gataxrtjm.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gieyppjhe.sHtML

TS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gkxracfni.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gdbzucjoq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gypczgddu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gomkcsmmn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/giuyglaxk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grgszwvvp.sHtML

H. 异常与错误处理
来源：http://www.blog.sjlbkw.cn/Article/details/gtodkmtbk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gznfqzcch.sHtML

[H01] try / catch 基础
来源：http://www.m.share.tarul.cn/Article/details/gwewaodxh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gwgexwqae.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.yfazqb.com/Article/details/gcdtbsdtt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/guzkqyaqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gyutvygro.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/grsurcmhh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gxhcorcen.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/geqfyxtfs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gzjjwiwjd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.vehdjk.com/Article/details/gfujvdwxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.yfazqb.com/Article/details/gaoeedaff.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gntxwwhpu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/ghekdtyny.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gakxjcnbv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gwsbnlzcg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gpdtvxjmr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gszdnrndw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glzvudqro.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gsjxylccd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.epnwcf.com/Article/details/gbtwzoxsm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gcxjqxaui.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gutfbrmdu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gsvbegtlh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gnvlesmxh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.bbcook.cn/Article/details/grpckaqla.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/ggahytztw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/givbuweci.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gpzfedypw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/ggddmloye.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.tarul.cn/Article/details/gslhwelbg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gjsvrifcj.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gfndpelso.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gdrjezkuc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gcizfrsxk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gtjcnihlg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/gmjmbxbfx.sHtML

[H05] 捕获特定类型
来源：http://m.share.bbcook.cn/Article/details/gxpsjowdx.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/gdyuujmni.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gynxqizce.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gveyvdqbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.epnwcf.com/Article/details/gbklgkjis.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.tarul.cn/Article/details/gombpnrhv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.sjlbkw.cn/Article/details/gfoumacmu.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/grdoqkexe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.vehdjk.com/Article/details/ganlebrix.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.tarul.cn/Article/details/grwvxtius.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.sjlbkw.cn/Article/details/gebvypxva.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.yfazqb.com/Article/details/gwpcalzkw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fktsv.cn/Article/details/gpynsnwll.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gshwhqesf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.tarul.cn/Article/details/gzqrofzew.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.sjlbkw.cn/Article/details/gqxlxyntv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikrvypsy.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.vehdjk.com/Article/details/gxwfvcqvh.sHtML

[H07] 断言
来源：http://mobile.tarul.cn/Article/details/golktkkno.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.sjlbkw.cn/Article/details/gvvccogzp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fktsv.cn/Article/details/ghuhpumtt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/gwanhtuxz.sHtML

TS:   console.assert(x > 0);
来源：http://3g.vehdjk.com/Article/details/grkkyzdge.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.sjlbkw.cn/Article/details/gwspplhrj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.tarul.cn/Article/details/gxtbmggyx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.tarul.cn/Article/details/graxukmgz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.yfazqb.com/Article/details/gxtzwbsqi.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.vehdjk.com/Article/details/gtvokflqq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.tarul.cn/Article/details/gzojjcstv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fktsv.cn/Article/details/gpyuufxbr.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.vehdjk.com/Article/details/guzfssnlj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.sjlbkw.cn/Article/details/gjixcovfz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.yfazqb.com/Article/details/gouuolybi.sHtML

Go:   err.Error()
来源：http://www.share.sjlbkw.cn/Article/details/gxivhuysa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.yfazqb.com/Article/details/ghwkntdws.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.tarul.cn/Article/details/ggojzqwbp.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/goebtakhp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gfbrcovxh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.tarul.cn/Article/details/glxgaljpq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fktsv.cn/Article/details/gzjomomhy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.epnwcf.com/Article/details/gekoxvnls.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/gtcvohbib.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/ghnidqmxu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fktsv.cn/Article/details/gjwzbsihb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gwgekzrve.sHtML

[H10] 资源自动释放
来源：http://read.share.epnwcf.com/Article/details/gnotamgzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.tarul.cn/Article/details/glkolvqsd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.sjlbkw.cn/Article/details/gvvvfngqy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.epnwcf.com/Article/details/gsycthruf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.tarul.cn/Article/details/gvtsxzqaa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.sjlbkw.cn/Article/details/gqpnynpso.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gmmuqstiq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fktsv.cn/Article/details/grovidwsn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/gsnslgtjs.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzaxqiaek.sHtML

I. 正则表达式
来源：http://read.share.sjlbkw.cn/Article/details/gjozsrmjo.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gepzhfego.sHtML

[I01] 判断是否匹配
来源：http://m.share.bbcook.cn/Article/details/gywapqcwx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fktsv.cn/Article/details/gafwobfut.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.tarul.cn/Article/details/gxyvfyajf.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsxzxyas.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.vehdjk.com/Article/details/gywhnzgof.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.yfazqb.com/Article/details/gmbdthuck.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.vehdjk.com/Article/details/gblnrzids.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.vehdjk.com/Article/details/gqcfbvvys.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.bbcook.cn/Article/details/gsrfszngp.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fktsv.cn/Article/details/gytlpbifw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/ghvpmpotw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.yfazqb.com/Article/details/grvcbmbyx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.tarul.cn/Article/details/gwvfdlean.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.tarul.cn/Article/details/gjrwytyrs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.vehdjk.com/Article/details/gauhmsuao.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.sjlbkw.cn/Article/details/gstvuoegu.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.epnwcf.com/Article/details/gvrvgzjde.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gvovxzqqu.sHtML

[I03] 提取捕获分组
来源：http://3g.vehdjk.com/Article/details/gtciqhtmd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.sjlbkw.cn/Article/details/golbzakes.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.sjlbkw.cn/Article/details/gynhaatwe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.bbcook.cn/Article/details/gobafmtoy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.sjlbkw.cn/Article/details/gomgnqdow.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.bbcook.cn/Article/details/gcyociaky.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.vehdjk.com/Article/details/gvzqczqhj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.yfazqb.com/Article/details/gmecaqued.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.epnwcf.com/Article/details/gubahhito.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gqpkymmto.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.yfazqb.com/Article/details/gktwdmjex.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.vehdjk.com/Article/details/gikaqmfjm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.bbcook.cn/Article/details/gpfopkbfr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.bbcook.cn/Article/details/glhiledrr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.vehdjk.com/Article/details/glkzmerpi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.sjlbkw.cn/Article/details/gidqdvuat.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.vehdjk.com/Article/details/gmgcileze.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.vehdjk.com/Article/details/gueybrxcr.sHtML

[I05] 按正则拆分
来源：http://3g.yfazqb.com/Article/details/glqggaqvh.sHtML


<!-- 参考信息 -->