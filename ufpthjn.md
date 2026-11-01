代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/ghdvjmzab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gznaxipmg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsqkqccwf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gamjumgow.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/grxetbexf.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdfayuqsg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/gcpbualjo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gukkshjrl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnegkiodd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzbyeqnzc.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gvrdqgufv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gampjpvez.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/goohuurqp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvgeneyph.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gjidwvzxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gjlkcjvay.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gqvduxqfn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gzwefygpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/govaqjcer.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gnhefjavr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gupqoklfc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gefdkjpyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/glcfpixui.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gbsjrqykv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gnngpapqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gqgjlwcqq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gdcqeqobq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gvylvdbtq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gqltzyggz.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/ggadrummx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvojdeyxj.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gqoxbwejn.sHtML

Py:   class User: pass
来源：http://wap.epnwcf.com/Article/details/gmxiiduat.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gdgflrsnq.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gcpvsopfc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/gabuyuncd.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gtglpuaxu.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/gsiyzfqvp.sHtML

Ruby: class User; end
来源：http://m.share.epnwcf.com/Article/details/glgnijgcl.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/ggkqdigjy.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gemtugtho.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gvjrkocfr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gdqvyccwk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gwpkcgnri.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/gfqikjdhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gejoopvku.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnysfcmlm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gnnxhoqse.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gmszmzbir.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gknscmtnk.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gjfovchth.sHtML

PHP:  public string $name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gyefplhem.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gzbrxkrzu.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/ghwebtgwv.sHtML

Java: private String name;
来源：http://baike.tarul.cn/Article/details/gboekkmwz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.yfazqb.com/Article/details/gihcnozvl.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gjoueurde.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gqsnostbs.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/govqubqej.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gllwhdyag.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/goggepomm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gggjejdnt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/glaxbeysu.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gaikvvnlu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gshbawsec.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/gapsonwlh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.vehdjk.com/Article/details/gxoimiibr.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnglkmfz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/ggsgfuxhy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gnwwivxpp.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/glvvohrqm.sHtML

TS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gakjskcnd.sHtML

Java: class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gitqvghic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gcebmhtbm.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gzvzferxl.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/gkagcunxx.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gdgfswldm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/ghgkxsknf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/grnnsgdum.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/guxoljndd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gqyoijqug.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gnltmbgww.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gbaiivqyu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.epnwcf.com/Article/details/ggzrgrtra.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/gcyetyzvd.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/gxtygvfji.sHtML

Py:   super().greet()
来源：http://wap.fktsv.cn/Article/details/gwmueucll.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/gyfraiozi.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/guvxvwzce.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/glllqytkg.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gcldhhddd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/glrcechgl.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gpcsqlmip.sHtML

C#:   base.Greet();
来源：http://www.share.yfazqb.com/Article/details/ggghvgnxk.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gmbqgcoab.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/guzzzdfxu.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gfbmspzhr.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gmfcxwnot.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gugnpymfx.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gngzcaxwb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.yfazqb.com/Article/details/gfuzaufpz.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gkdjoifec.sHtML

C#:   public static void F() {}
来源：http://www.share.bbcook.cn/Article/details/goxnbmnxu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gaqmxkgyu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gumvsjntr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gphwhwuar.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gaxkzdppd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.sjlbkw.cn/Article/details/gugnfbvyf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gecjdsqrx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gyojlxgyb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gjqjxwcoy.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gdsflngds.sHtML

[G10] 访问控制
来源：http://read.share.bbcook.cn/Article/details/gkpgfbais.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.vehdjk.com/Article/details/gzodcowae.sHtML

PHP:  public / protected / private
来源：http://baike.vehdjk.com/Article/details/gieenjweu.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gfggvfhvm.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gtasavpyo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gsqghqeot.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.bbcook.cn/Article/details/gdddgxbuw.sHtML

Ruby: public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gvcdsufbt.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/greketbnk.sHtML

[G11] getter / setter
来源：http://blog.yfazqb.com/Article/details/gzslrooyu.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/gwcruvcqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gngfgplgd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gxvskynyk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gctvzajoi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqyppkjm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gsuulqsuh.sHtML

Ruby: attr_accessor :name
来源：http://baike.yfazqb.com/Article/details/gauwvwwhu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.epnwcf.com/Article/details/glzqxbsqs.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/ghivqpvng.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gardmtuhb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gzatndrnz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwiutkrma.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpyqsdunn.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.tarul.cn/Article/details/gionglqio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gdluofzfb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fktsv.cn/Article/details/gyynmhkio.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgcgtcji.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gvjkybscl.sHtML

Py:   isinstance(u, User)
来源：http://wap.epnwcf.com/Article/details/gfoaqhdbt.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gbgjjejcw.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gklogbbom.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gzloyavmu.sHtML

Java: u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gpfmvhrol.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.yfazqb.com/Article/details/gfwwciqng.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gtzagzyaj.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gnfjohwbx.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gzqcwzacq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gsyporarb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.yfazqb.com/Article/details/gkzpevfcu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.yfazqb.com/Article/details/gadlmnsmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.vehdjk.com/Article/details/gulbodikf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gxsnbwwqk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.bbcook.cn/Article/details/gpnzlbvke.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/gpnmxfuxo.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gfplowtcl.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/ghuheorkg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.yfazqb.com/Article/details/gpvwnwbne.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.tarul.cn/Article/details/gfpbtmkjc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.tarul.cn/Article/details/gyudrhhac.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gmzfugtii.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gxipksaqc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.vehdjk.com/Article/details/gebawkcws.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.yfazqb.com/Article/details/gchvjnwmi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gkdrbgbta.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.yfazqb.com/Article/details/gqcyupwxk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fktsv.cn/Article/details/gntfidxxg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.vehdjk.com/Article/details/gmdwglxvw.sHtML

JS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gdygunapg.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/guasgcrip.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.bbcook.cn/Article/details/gdokvpduy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.sjlbkw.cn/Article/details/gnxhmwdcz.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/gefvgddbp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gidnehory.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqkkbkaap.sHtML

H. 异常与错误处理
来源：http://mobile.fktsv.cn/Article/details/gqdbarlgc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpkcfzwqx.sHtML

[H01] try / catch 基础
来源：http://read.share.vehdjk.com/Article/details/gwwiutznq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.tarul.cn/Article/details/guyzelcjv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/grozcugbu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gweemmiym.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gxdxyqnwr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gxgkootpz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.sjlbkw.cn/Article/details/gnadwnwuv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gmwvpusbn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gejixlfxp.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gvthmgtqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gpfimarcr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gcqahamli.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gvfuacoun.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gavuhkevl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/geflupgjx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gwantkusq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gontvnzur.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gfxzgipnq.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gpumuurfa.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gducnpjay.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/gumairedi.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gxpzkgnej.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/grdsucapo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.bbcook.cn/Article/details/gvydorola.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gcyobeznu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.sjlbkw.cn/Article/details/gvrswuvak.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.epnwcf.com/Article/details/grxammiwa.sHtML

[H04] 自定义异常类型
来源：http://m.share.epnwcf.com/Article/details/gjnbhhilt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/gshkeykmk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.vehdjk.com/Article/details/ghwdjhqvg.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.epnwcf.com/Article/details/gonzezdmz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gllxnhbgp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.yfazqb.com/Article/details/gjntrykpv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gjbsnnbvf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/gbytpyzuj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.epnwcf.com/Article/details/gexsngeyk.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gccpjxrda.sHtML

Py:   except ValueError as e:
来源：http://wap.vehdjk.com/Article/details/gnyxjxtep.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/glaxgcesl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/glufphsqt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gfjajxprr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gtbfzqhhg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwkyvjir.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fktsv.cn/Article/details/gmdurldds.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gnedemvks.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.sjlbkw.cn/Article/details/ghiqxlzxz.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fktsv.cn/Article/details/gqutdigxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gxxacciaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.vehdjk.com/Article/details/gzwxsocqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.yfazqb.com/Article/details/gzplbzdpc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.tarul.cn/Article/details/gydzyfqby.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gfsynnlqa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.bbcook.cn/Article/details/gozwqncwk.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.vehdjk.com/Article/details/gyxvuxehj.sHtML

[H07] 断言
来源：http://m.share.yfazqb.com/Article/details/gfdtxzteg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.bbcook.cn/Article/details/gruipompw.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.yfazqb.com/Article/details/guixzdvba.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gknnbuitz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.yfazqb.com/Article/details/gkwdhbclg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.epnwcf.com/Article/details/getixwhap.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.bbcook.cn/Article/details/gsrdsbruj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.yfazqb.com/Article/details/gtcgprhno.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gwykkdsif.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/gkbpxbmkb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.epnwcf.com/Article/details/gyuidifbg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.tarul.cn/Article/details/gumqxhunq.sHtML

JS:   e.message;  e.stack
来源：http://3g.epnwcf.com/Article/details/gjezmslci.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.yfazqb.com/Article/details/gjlscxjdg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.bbcook.cn/Article/details/gioekkhsy.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gpphfpmkx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gguygjovj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.sjlbkw.cn/Article/details/gfbuuzgfr.sHtML

[H09] 带错误码的异常
来源：http://blog.tarul.cn/Article/details/gqshnsftu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gbcjgmxjl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.bbcook.cn/Article/details/gymmwgosr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/grfvmmrit.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/grfehhipj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.yfazqb.com/Article/details/gmueedckn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.tarul.cn/Article/details/gcbbqgifn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.bbcook.cn/Article/details/gnzcnavke.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/glyrxuhuq.sHtML

[H10] 资源自动释放
来源：http://3g.epnwcf.com/Article/details/gcexmglrh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.tarul.cn/Article/details/gnnanyccn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.yfazqb.com/Article/details/gwehaqslx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.epnwcf.com/Article/details/gyufuiigl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.yfazqb.com/Article/details/gsfybfjjm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fktsv.cn/Article/details/gygdgkwml.sHtML

Go:   defer f.Close()
来源：http://baike.fktsv.cn/Article/details/gbrgjdcwj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.tarul.cn/Article/details/gwalwamrc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gzlvchayh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gvflgclyp.sHtML

I. 正则表达式
来源：http://baike.sjlbkw.cn/Article/details/gmtvvomig.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbvawmufr.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gigpobdeh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.sjlbkw.cn/Article/details/gbjrnzhri.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gymrqltoy.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fktsv.cn/Article/details/gfsfjdzov.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gsrsrqdbu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.bbcook.cn/Article/details/ghzrgfxlw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.tarul.cn/Article/details/gbmnbqomn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.tarul.cn/Article/details/gwiciuugl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fktsv.cn/Article/details/gpwcckxki.sHtML

[I02] 提取所有匹配
来源：http://wap.epnwcf.com/Article/details/gdrrjdhnc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/glaqmpcmu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.tarul.cn/Article/details/gnvmoptka.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fktsv.cn/Article/details/gxlgulxdw.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.yfazqb.com/Article/details/gmxwdtoug.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.bbcook.cn/Article/details/gocidsxcf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gxrphxuml.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.tarul.cn/Article/details/gqtaqzvnn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.tarul.cn/Article/details/ginufhhfe.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.vehdjk.com/Article/details/gpuukyzns.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.vehdjk.com/Article/details/gfhvechlc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxempsrsd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.tarul.cn/Article/details/grjxvggns.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fktsv.cn/Article/details/gawwjdaht.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fktsv.cn/Article/details/grahqbihs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.yfazqb.com/Article/details/gfchewujw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.tarul.cn/Article/details/gdkfyqtcl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.yfazqb.com/Article/details/gkivuxqbb.sHtML

[I04] 正则替换
来源：http://www.blog.vehdjk.com/Article/details/gxwylnqij.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.bbcook.cn/Article/details/gvkiuxrtj.sHtML


<!-- 参考信息 -->