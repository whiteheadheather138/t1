代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gdeftcnxm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gjoheefod.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gwtxkfqwu.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvaxyachn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.sjlbkw.cn/Article/details/gxedvwymt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/glkobxcxy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfmapiwbj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/grimdkjfn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gezyvmzsy.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fktsv.cn/Article/details/gjgikundg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gkebmyhuk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxkfjnhwn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtjfdyuxr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gvdozupxg.sHtML

[F11] 复制与移动文件
来源：http://blog.epnwcf.com/Article/details/gugngdbwz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/giawncvwj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gffqjtyyi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gkqfcvnrx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gmdwyxpzw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.yfazqb.com/Article/details/gnzlvhilq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gqdjjtphw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gunvfzpcy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gnkgyettz.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gcxeamxdj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gnluigusb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/glfofotau.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/geumcxytk.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/ghsbbgugo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gsujnbdbi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gouaslzri.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gvmvavwla.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gvauiewqb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjmeshtol.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/ggthvdxml.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkazsklni.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gchlykgrt.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/giwlxxfpr.sHtML

PHP:  class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gzbykmhel.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gzlwmhjmi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gujukdmlz.sHtML

Java: class User {}
来源：http://wap.vehdjk.com/Article/details/gmsrptkjo.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gjuueqsva.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gpeuarcna.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/ghzbcuikb.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/ggapyrfcs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gjfinsrmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gnjltmwrj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/grpzsnhav.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gglcwkujj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/grxwwpwsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/goxiwliwq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gemazmiud.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gviebpcpc.sHtML

[G03] 实例属性
来源：http://mobile.sjlbkw.cn/Article/details/gvghjdyuq.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gaxkukizk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gvwuavgdh.sHtML

JS:   this.name = "x";
来源：http://m.share.vehdjk.com/Article/details/gctpkwfrg.sHtML

TS:   name: string = "x";
来源：http://blog.epnwcf.com/Article/details/glaompjse.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gliovcbou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.epnwcf.com/Article/details/gtadsksby.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gcmfzlwgb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gkwkhyhwr.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gyxsytvfh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gdqeornte.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gwbjtnohz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/ggvtsfyns.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gnddmqkod.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/giertiezg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gmthlemeh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.bbcook.cn/Article/details/gbrxibuoo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gpdnnkbgm.sHtML

[G05] 继承
来源：http://3g.vehdjk.com/Article/details/gzpzizseh.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/girlaxiog.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gxwkrdzwz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gukiirnrj.sHtML

TS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/ghhnlybiy.sHtML

Java: class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gwlqosqgf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gvnxdmutp.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.epnwcf.com/Article/details/gbaxvrsyo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gjduupwap.sHtML

[G06] 重写方法
来源：http://blog.tarul.cn/Article/details/gsmgczqoq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gntscrini.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gslilfjef.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gqeyzgbzt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gedqsvacc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gvvfawfec.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gmcrdykpr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gqjoymspq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/ghenbtaok.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gconuywxr.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gyjzlazmt.sHtML

PHP:  parent::greet();
来源：http://www.share.vehdjk.com/Article/details/gondhgtmj.sHtML

JS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gsgqspmdh.sHtML

TS:   super.greet();
来源：http://wap.vehdjk.com/Article/details/gylyruzox.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gchyukgqr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.bbcook.cn/Article/details/guoqjdeoq.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/goxskifob.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gwjojpdyg.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gckvwbvrl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/giwgxqwva.sHtML

PHP:  public static function f() {}
来源：http://3g.yfazqb.com/Article/details/geiaayfzv.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gjobcpoyu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxweexgyu.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/ghebumzyw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gvhkqrehh.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gxkuwbind.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/ghqjfdhnc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/geonxxxyh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/gwdstkgrj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.yfazqb.com/Article/details/gspjgxygy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.tarul.cn/Article/details/gwrddiesm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.bbcook.cn/Article/details/gnemcpqlo.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/grvundkds.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.yfazqb.com/Article/details/ghxitmqyc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.yfazqb.com/Article/details/gkeebblvr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gndecjoct.sHtML

[G10] 访问控制
来源：http://3g.bbcook.cn/Article/details/gsdpuhsbj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.epnwcf.com/Article/details/gegwdmrfb.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/ggpwbnhiq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gqhgcoorh.sHtML

TS:   public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gbammfzbu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/gphntmjcl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gtmmknxtz.sHtML

Ruby: public / protected / private
来源：http://3g.yfazqb.com/Article/details/gxikwgayh.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.epnwcf.com/Article/details/gijcncajg.sHtML

[G11] getter / setter
来源：http://www.blog.yfazqb.com/Article/details/gtarhljcm.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/govxcwdqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gwzzcjqbj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gfevejhhu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gxamcnsmx.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gsmqfhpyh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gippxwnyd.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gtfakqwli.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gtjqaldrh.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gfoxlmjym.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gjpdnpyxp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gzqjgrotc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gmpdjlhsg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gutxqhviw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.epnwcf.com/Article/details/ggbkawoqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/goqmnzpyf.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gvxtktdbc.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/grnlssugf.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gpbvjxyas.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/ghejyesgf.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gqfiujvbq.sHtML

JS:   u instanceof User
来源：http://wap.sjlbkw.cn/Article/details/gopmccagr.sHtML

TS:   u instanceof User
来源：http://baike.epnwcf.com/Article/details/gdflwoylj.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gscuqahtf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/grkgkfmxr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.tarul.cn/Article/details/gylxbizkv.sHtML

C#:   u is User
来源：http://www.share.yfazqb.com/Article/details/ghbatguan.sHtML

[G14] 数据类 / record
来源：http://baike.yfazqb.com/Article/details/gmsyvzciq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gvrckehrg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gexpzqbay.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fktsv.cn/Article/details/gjtspkpah.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gdudaklsy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/giibxmuyf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gxdntntjm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.tarul.cn/Article/details/guktdjujc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gburaojzq.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gpjltzflh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/gbvxwwdln.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/giwkapqcx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.bbcook.cn/Article/details/ghxpmpvbq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gkxztksak.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.epnwcf.com/Article/details/gjwijmagw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/gfmjgdkxu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.yfazqb.com/Article/details/gbjmalfnw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.epnwcf.com/Article/details/ghuajkdzv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.epnwcf.com/Article/details/guekdubjn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gjyidrror.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/gssabjtrd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gpmmxrzau.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gxpfsoras.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gcslzcscj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/guiinxlpp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gsujjnunq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/glxhaakmy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grtaylvdv.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/gpstckwge.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grpivfigt.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gnsjnquee.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gbxusshcw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.bbcook.cn/Article/details/gbscexomq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gognexltq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/ggjaklbhb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gkydblokz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.sjlbkw.cn/Article/details/gyubbawxb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.vehdjk.com/Article/details/gkuhbhnwd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fktsv.cn/Article/details/gaswhasip.sHtML

[H02] finally / ensure 收尾
来源：http://3g.sjlbkw.cn/Article/details/gaibfjxsj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fktsv.cn/Article/details/gcaxcgaui.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gltvgeuhw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/godwzyclq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gvrmovxin.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gzouxtmzg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/gnjoigxsx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/ghefhdrze.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gvopccujn.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/gvgypufxe.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fktsv.cn/Article/details/geqfbuhez.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/grkebavot.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.bbcook.cn/Article/details/gejsjkrlp.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/ghkjqkvuf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.bbcook.cn/Article/details/gvbceytdu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/gulowcogf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.vehdjk.com/Article/details/gitvorhvu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gfsolasnz.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gximjnrud.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gaezlnfzz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gjkdkovjo.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.tarul.cn/Article/details/gguevjzcd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fktsv.cn/Article/details/gilzcboao.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/goevtppri.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gzhtyqvjy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gjvoxphma.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.yfazqb.com/Article/details/gbghzigxs.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gymsbgici.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gafndnjtd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gkltkrzst.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gfmaushin.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.epnwcf.com/Article/details/gpogegwyt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.sjlbkw.cn/Article/details/gzeequald.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.epnwcf.com/Article/details/gzfcbvjiw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/gljnsdvxq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.epnwcf.com/Article/details/gomdrdzmb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.epnwcf.com/Article/details/gznkfmkxo.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fktsv.cn/Article/details/gqymxzgta.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.tarul.cn/Article/details/ginjzepom.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/gbqlbgtgn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/guthwofjc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/ghewvmuxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.vehdjk.com/Article/details/gqwqbndjw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gijokbtjw.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/geszqhkdv.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/giehyyilx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.yfazqb.com/Article/details/glssmsiwr.sHtML

PHP:  assert($x > 0);
来源：http://wap.yfazqb.com/Article/details/gmtgagyht.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.vehdjk.com/Article/details/gqxyfwdha.sHtML

TS:   console.assert(x > 0);
来源：http://blog.tarul.cn/Article/details/glynirhjs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.tarul.cn/Article/details/ggqklamzz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.bbcook.cn/Article/details/guswlmnlr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gxgudpkfr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.bbcook.cn/Article/details/geedltvec.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.epnwcf.com/Article/details/gbjibkoxy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.epnwcf.com/Article/details/gihyrygqa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.sjlbkw.cn/Article/details/gvzeilxnz.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.tarul.cn/Article/details/gaxaqbysp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.vehdjk.com/Article/details/gqgskggkh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/gphfgncvb.sHtML

Go:   err.Error()
来源：http://www.share.yfazqb.com/Article/details/gwvsvkqsd.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.bbcook.cn/Article/details/gqmnvwhiu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.bbcook.cn/Article/details/gplteakgy.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gzbedcgbg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/gbrhanwhd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.yfazqb.com/Article/details/guoamzrdj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/gimzdkwwb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.bbcook.cn/Article/details/grqhljhjp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.epnwcf.com/Article/details/gqdphcyvz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gztrdhqzk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.epnwcf.com/Article/details/gmisavoss.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.yfazqb.com/Article/details/gpeetdhfs.sHtML

[H10] 资源自动释放
来源：http://mobile.tarul.cn/Article/details/gjsnlapwb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.tarul.cn/Article/details/gfaglmgnf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.yfazqb.com/Article/details/gnbjllvvm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.tarul.cn/Article/details/ghbskcday.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.sjlbkw.cn/Article/details/grmvzbctx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.tarul.cn/Article/details/gdbjadzzu.sHtML

Go:   defer f.Close()
来源：http://baike.bbcook.cn/Article/details/gyshawilb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.epnwcf.com/Article/details/gcbqqehow.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhhhcmnr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gazvrrmdm.sHtML

I. 正则表达式
来源：http://mobile.tarul.cn/Article/details/gdoqpisgj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpxnnvpti.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gomemnfyp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gwopfjlvb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.epnwcf.com/Article/details/gzzxhbkba.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.yfazqb.com/Article/details/gmzaobdrh.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.vehdjk.com/Article/details/gefsrvojy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gqfhjdwaw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/glkvzsxsd.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gcsghanly.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fktsv.cn/Article/details/gtdqpjylw.sHtML

[I02] 提取所有匹配
来源：http://m.share.epnwcf.com/Article/details/gbjdeoivc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.sjlbkw.cn/Article/details/gibcboydd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.epnwcf.com/Article/details/gknuxxcyi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.epnwcf.com/Article/details/gvjdupypm.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.sjlbkw.cn/Article/details/grquvtwgh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.bbcook.cn/Article/details/gsoffkfvn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.sjlbkw.cn/Article/details/gzxtlqpez.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfztavzti.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.epnwcf.com/Article/details/gxvylksrd.sHtML

[I03] 提取捕获分组
来源：http://www.share.tarul.cn/Article/details/gpheizcks.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.yfazqb.com/Article/details/gedenlaim.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gcrprnfnq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.yfazqb.com/Article/details/gxgfgejws.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.yfazqb.com/Article/details/gdqvngrbl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.yfazqb.com/Article/details/gjcodudly.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.vehdjk.com/Article/details/gbmrqkhit.sHtML


<!-- 参考信息 -->