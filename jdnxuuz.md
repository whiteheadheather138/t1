代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gzlyzbpmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gcwdwgnbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gvnvdazlv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gpqhtznbl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gjmxgloew.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gsacexftz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gidiwjxuv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvabiulfp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxplozkrw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/glielllgh.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gtwpvzgwl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gnqiafadl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gkxyxmcmq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpcljqwkl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gvyiaztei.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gcmmjgpqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gipscmtch.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gqsgdisqh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.epnwcf.com/Article/details/gzwacrwqd.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gockwucav.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/ginvmqnuf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.tarul.cn/Article/details/gmtxyciur.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gwnbspilm.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gljzwysrz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.yfazqb.com/Article/details/gsjljzigb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gvmlzkqud.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gtgfvhbqr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gftywvhmw.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbgmvtpxe.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gopepqsoc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjsqjctwh.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gliqnytyo.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gpzriekno.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/glyhtlbec.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gclvcvixi.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gppvjmlyt.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gsizosupa.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gxqrqquub.sHtML

Ruby: class User; end
来源：http://www.blog.yfazqb.com/Article/details/gylajedet.sHtML

C#:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gtkezvuyi.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/ghsfcqsub.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.epnwcf.com/Article/details/guczxsbcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fktsv.cn/Article/details/gjjtlorzs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gjjbcvrge.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gnreqedxt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/guvwcgjoq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.vehdjk.com/Article/details/gqlnirwnu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gvgfsqjgg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gqkjohact.sHtML

[G03] 实例属性
来源：http://blog.yfazqb.com/Article/details/gtuiaijbc.sHtML

Py:   self.name = "x"
来源：http://mobile.tarul.cn/Article/details/gqupcqoxc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gxnmqlewp.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gajekqccp.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gsjiqeuee.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gggstkyel.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.epnwcf.com/Article/details/gmmeenqyy.sHtML

Ruby: @name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gslnywhhd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gpaddsdbo.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gdqmunfwx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gkmrisywi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gravxxafn.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/guwuqnmlr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gltrlfksm.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/ggvwztyom.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/gyibedcdf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gcedrfsiy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/gjjbaaubp.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/grxsqyhtw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/glvejvsdy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gvhxjoblf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gdnxyhoyi.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gpvsjlhft.sHtML

Java: class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/giteafcbi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gsyuokxdv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.epnwcf.com/Article/details/gnkbvrukf.sHtML

C#:   class Admin : User {}
来源：http://wap.yfazqb.com/Article/details/gufvfyxbg.sHtML

[G06] 重写方法
来源：http://read.share.fktsv.cn/Article/details/gypwaoudf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/geypfumst.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gxmbwfeng.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gjnyyyjxx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gbbdlqovv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gjfpqqosx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gpqqtveia.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/gjnnkjkkv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gairfueqg.sHtML

[G07] 调用父类方法
来源：http://baike.tarul.cn/Article/details/gpbwlgqse.sHtML

Py:   super().greet()
来源：http://www.blog.tarul.cn/Article/details/gzbobjnrf.sHtML

PHP:  parent::greet();
来源：http://blog.bbcook.cn/Article/details/ghziaohgz.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gifxvvxot.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gdpxywpdp.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/grcydgcia.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.tarul.cn/Article/details/godqtfmtt.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gvhynfrgv.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gbtwlpjrk.sHtML

[G08] 静态方法与属性
来源：http://mobile.bbcook.cn/Article/details/gvxokoekn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gwfdwqaxn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gzfdwwgka.sHtML

JS:   static f() {}
来源：http://wap.bbcook.cn/Article/details/gsqrtxsgr.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gmdswmqbs.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gheuvfuya.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gomcoefwj.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/ggfdndsog.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gdiyvnvol.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/gvwzyzjdx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/goztpydia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gxnxvvuls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gpapqittr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/grvzokiyy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.bbcook.cn/Article/details/ggiorxmud.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gdjwboaxz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gvfuakgay.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.tarul.cn/Article/details/gjufaijji.sHtML

[G10] 访问控制
来源：http://blog.epnwcf.com/Article/details/grxvzlfoc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.epnwcf.com/Article/details/greblnual.sHtML

PHP:  public / protected / private
来源：http://3g.bbcook.cn/Article/details/gtsbemmtw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gnexiqznc.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gdfhdlzui.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/gmnawpdnk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gjceotrqz.sHtML

Ruby: public / protected / private
来源：http://wap.bbcook.cn/Article/details/gibglyito.sHtML

C#:   public / protected / private / internal
来源：http://www.share.yfazqb.com/Article/details/gnrfwosjs.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gmmxunuhi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gnqbpkbam.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gfhjtxcxq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gsjhmgavj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gxzugjnlk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gtguoadfz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gvgngdtsc.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/gsmyrxegg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gryznurgd.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gvelnizpn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gyqvutnhn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gakirowak.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/guxgwdnio.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gwodlgdpt.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gqavgpagz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gffgxjrtq.sHtML

Ruby: def to_s; @name; end
来源：http://blog.tarul.cn/Article/details/gkpvbqhri.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/geiravqzo.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gjrnydrsn.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gxnblahlq.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gqgbrfulg.sHtML

JS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gqisyoamo.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gtqfzebze.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gfikcpkux.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.epnwcf.com/Article/details/goudsuodp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/gtbynkwxh.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gmdygvdfb.sHtML

[G14] 数据类 / record
来源：http://m.share.yfazqb.com/Article/details/gcngstvvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/glfhzcukr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/geezxdvpq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gquvaddmy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.tarul.cn/Article/details/gldjkkasp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfncybzwe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gubjtbfcd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.vehdjk.com/Article/details/gsdqfrtjs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.tarul.cn/Article/details/ggdhaktuy.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/glrxlurol.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gxzxdwaan.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.tarul.cn/Article/details/gebonukat.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.sjlbkw.cn/Article/details/gtilntpyf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gmbrdlvlw.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gkeuabyib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gfronahyt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gvnjwxqgl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gppzrhoow.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.tarul.cn/Article/details/gudrgmphq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.epnwcf.com/Article/details/gevcxnwzv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/ghperahwq.sHtML

JS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmowamaum.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/guxcqtldn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gakykdqwz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gbvzkqjiy.sHtML

Ruby: obj.instance_variables
来源：http://read.share.sjlbkw.cn/Article/details/ggymwizoq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gfniexqej.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/goaqxbeqn.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/gayrgqtub.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvstkqtuj.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gdqxzhylk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/gcqluyghc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gorgzvjrq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/ghorirerc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gpfgejbqj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gsmqwxmpm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fktsv.cn/Article/details/gtcgxvmus.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.sjlbkw.cn/Article/details/gjeybiiwp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.vehdjk.com/Article/details/ghhqrjkbh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.bbcook.cn/Article/details/gogytwlck.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gwbvafwil.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gtyrypetn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gsinbowjk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gtupfwdrn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fktsv.cn/Article/details/graquvqsv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.vehdjk.com/Article/details/ghvxhzhke.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.bbcook.cn/Article/details/gmpvlevrb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gnihsabvr.sHtML

[H03] 主动抛出异常
来源：http://mobile.tarul.cn/Article/details/gknntjcju.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/gtzxesssy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gysdyeabh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.epnwcf.com/Article/details/gkifrjcap.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fktsv.cn/Article/details/geytlfjzl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.sjlbkw.cn/Article/details/gejoxinuj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gvyfxrlko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.sjlbkw.cn/Article/details/ghhepmlkl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gequcyjej.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gnrvpdbyq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.tarul.cn/Article/details/gsvgjtfoj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gngndkemf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gcembdvhp.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gwfvcoviw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.yfazqb.com/Article/details/gzjkfjnyu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.tarul.cn/Article/details/gbwymcluh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.yfazqb.com/Article/details/gygfpcvbp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gpkodfytf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/geectubjs.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.bbcook.cn/Article/details/gsonqfiby.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fktsv.cn/Article/details/gaeldogwm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.vehdjk.com/Article/details/gbklgdjdq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/goraezqir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gipnhxqxq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.tarul.cn/Article/details/glhqfyncq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.tarul.cn/Article/details/gfkehipdi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/ghxguzkvo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/gvisyevpr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/gapoqfife.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/gwxyhgfxh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/gwqcnmowb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.vehdjk.com/Article/details/gbtrdsmss.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.bbcook.cn/Article/details/gvdhlqaxi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.vehdjk.com/Article/details/goeunzhld.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/ghqffsmlf.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gefpnchmr.sHtML

[H07] 断言
来源：http://3g.fktsv.cn/Article/details/ghhgrchle.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.epnwcf.com/Article/details/govaoxqlx.sHtML

PHP:  assert($x > 0);
来源：http://blog.epnwcf.com/Article/details/gdmqaqwah.sHtML

JS:   console.assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/grtwphhxc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fktsv.cn/Article/details/grymtdmdv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.bbcook.cn/Article/details/gdvagnqmz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fktsv.cn/Article/details/gjkqgwexh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.epnwcf.com/Article/details/grrnsyrnn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.vehdjk.com/Article/details/gfzotsmsx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.yfazqb.com/Article/details/gsasreamv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.yfazqb.com/Article/details/gdzyyxbhw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gvwufvlnk.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gtblqzufd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fktsv.cn/Article/details/glmyupeyg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.vehdjk.com/Article/details/gyrjzpbid.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gpzfryggl.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.yfazqb.com/Article/details/gtsahgwja.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.yfazqb.com/Article/details/gaxmmzdwq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.sjlbkw.cn/Article/details/guioreabq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.tarul.cn/Article/details/gzwkszjlg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.vehdjk.com/Article/details/gezjzzgpx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/ghxqxnbov.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.vehdjk.com/Article/details/gzcbjvuxe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.bbcook.cn/Article/details/gbpwobfji.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.tarul.cn/Article/details/gmdkbgqjf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.vehdjk.com/Article/details/gatqiatay.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.epnwcf.com/Article/details/gvpzwxchk.sHtML

[H10] 资源自动释放
来源：http://3g.bbcook.cn/Article/details/gcahmtvni.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gkfedzxmg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.sjlbkw.cn/Article/details/gtbwgxznz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.vehdjk.com/Article/details/ggyqzsmvl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fktsv.cn/Article/details/gnctsmows.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.tarul.cn/Article/details/gfwqabrmq.sHtML

Go:   defer f.Close()
来源：http://read.share.epnwcf.com/Article/details/gearinxvh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.yfazqb.com/Article/details/gjiwjctsr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fktsv.cn/Article/details/gwgnfllkr.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkrdxnoty.sHtML

I. 正则表达式
来源：http://blog.vehdjk.com/Article/details/gispwzobc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdcmjfcqn.sHtML

[I01] 判断是否匹配
来源：http://3g.yfazqb.com/Article/details/gdmmfjiot.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.sjlbkw.cn/Article/details/gxysmhant.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gqmpkwzkt.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fktsv.cn/Article/details/gngaupyrw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.yfazqb.com/Article/details/gbiwzfkcz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.yfazqb.com/Article/details/gpzvkttpa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fktsv.cn/Article/details/ghzqcyhlq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.tarul.cn/Article/details/gpfcocvol.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.yfazqb.com/Article/details/gbksqnmqq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdkbikvd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.yfazqb.com/Article/details/gnetaidwc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.epnwcf.com/Article/details/guaylsfwe.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.bbcook.cn/Article/details/gctbtcywn.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.vehdjk.com/Article/details/gctaikoyu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.sjlbkw.cn/Article/details/gvfvuszqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.sjlbkw.cn/Article/details/gqekyjytv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.vehdjk.com/Article/details/gcailrlwn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.epnwcf.com/Article/details/ggfmgntkj.sHtML

[I03] 提取捕获分组
来源：http://m.share.sjlbkw.cn/Article/details/gkugrwuqy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.vehdjk.com/Article/details/gzkqsgybs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.epnwcf.com/Article/details/gcnshjgon.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.epnwcf.com/Article/details/gbucdapag.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gnfpssehh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.yfazqb.com/Article/details/gcwgxuhty.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.vehdjk.com/Article/details/ghebzevdh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.vehdjk.com/Article/details/galpbqrju.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.sjlbkw.cn/Article/details/gzaqqepqt.sHtML

[I04] 正则替换
来源：http://www.blog.sjlbkw.cn/Article/details/gizypujjb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.yfazqb.com/Article/details/gnmunqxag.sHtML


<!-- 参考信息 -->