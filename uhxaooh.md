代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/ghfauqeib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gljxfwkdf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.bbcook.cn/Article/details/gqobzehrc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gssvnuzlm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.bbcook.cn/Article/details/gphqoolto.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/gbniugbff.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpeimldmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gelfygspn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gfcjnukqr.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqsbjetig.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gzybzizbp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gelqfubmp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gushjskvg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gttlqbmbc.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gzehwmtfk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gfrfsrgqu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/ggncjabsm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gyepovbcz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/guwpzpfdy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gvygybesz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gmtqjgdru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvezvqtwk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gkflxcdlp.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpwsgxiq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gyljplwzg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gcsjdscli.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.epnwcf.com/Article/details/gkmjynrxz.sHtML

TS:   // 同上
来源：http://wap.sjlbkw.cn/Article/details/gbwnfiqow.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gsmrmwezh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.vehdjk.com/Article/details/gpvoscoag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gmjimeeko.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gcuujurrh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ghqoamdaf.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gfuduzegk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gatkunugu.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gpswdgrdl.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gmdsjzvov.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gedhlwpzu.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gvzsolxfj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/ghghohybp.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/ghfbekuua.sHtML

Go:   type User struct { Name string }
来源：http://3g.tarul.cn/Article/details/gzempwkjk.sHtML

Ruby: class User; end
来源：http://www.share.yfazqb.com/Article/details/gfokpphjg.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqkehiaph.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gktbjwjgt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/goehdnulr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gogvyhodn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gvkwjauai.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gxxggyhuv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gyhvzooqr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gzxjvvjyz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/gfatbcscc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gekjuosug.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/ggerdfavm.sHtML

Py:   self.name = "x"
来源：http://read.share.bbcook.cn/Article/details/gfiipihcu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/ghqkoybot.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gaddobznt.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/gsebickje.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gqwlrguyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.sjlbkw.cn/Article/details/gkjlthveu.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gcrybrvih.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gdcdspkgy.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gdshoihvl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gszwthulb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gtxqpudiy.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ggqskrlnh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gdzbdbxeg.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/ghgcgjbqr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gbdfwpqie.sHtML

Ruby: def greet; @name; end
来源：http://m.share.yfazqb.com/Article/details/gwdndgwiv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gxqvhxneo.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gcwvnngqh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gnalzsnqb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gtkrqglzq.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gzpqqeszk.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gwyeapvrv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gmibxrpgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gdrkqarzo.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gxghuvupx.sHtML

C#:   class Admin : User {}
来源：http://mobile.sjlbkw.cn/Article/details/gxhuywikp.sHtML

[G06] 重写方法
来源：http://blog.fktsv.cn/Article/details/gbtponivs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjdooccq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/geuiesytz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/goknpkrjp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.tarul.cn/Article/details/glcshcgdp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gatxokoce.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.vehdjk.com/Article/details/gtolzlyty.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/grepyqkhc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/gqfqclirl.sHtML

[G07] 调用父类方法
来源：http://read.share.sjlbkw.cn/Article/details/gebvdhgta.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gigdnnrwx.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gedkneuvv.sHtML

JS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gruohohea.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gybbuyawt.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gamrhdbph.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/gxxrabztt.sHtML

Ruby: super
来源：http://wap.fktsv.cn/Article/details/gzffynput.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gmcixcbbe.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gjkcotlpg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fktsv.cn/Article/details/geztizloa.sHtML

PHP:  public static function f() {}
来源：http://m.share.bbcook.cn/Article/details/ghoipeydp.sHtML

JS:   static f() {}
来源：http://3g.bbcook.cn/Article/details/gcemsdqns.sHtML

TS:   static f(): void {}
来源：http://wap.sjlbkw.cn/Article/details/grfvwvvic.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/gbbvozgla.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gngpsfhqo.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gzkkvmmiw.sHtML

C#:   public static void F() {}
来源：http://m.share.tarul.cn/Article/details/gkupjxiqa.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/grdbwpume.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/goxgejgrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fktsv.cn/Article/details/gitzcklnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gpacifjcq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/gdrmsljmh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fktsv.cn/Article/details/gsaemvvly.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.yfazqb.com/Article/details/gxrzywgft.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gllqnegzl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gcyiuypey.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/gaipoxsrc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.tarul.cn/Article/details/gholuebqd.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gsljadirr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.tarul.cn/Article/details/gopeiqust.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gmmuxbxkj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gafxzyqgy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/gountskij.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gwvgjxdbl.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gjyomgdwf.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/ggbayqiyf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.bbcook.cn/Article/details/gukncawzk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gwqpvemdr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gojvggivd.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gmrzxbxnn.sHtML

Java: public String getName() { return name; }
来源：http://wap.fktsv.cn/Article/details/gczuopwha.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gcarhavpm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fktsv.cn/Article/details/gunhikpog.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.sjlbkw.cn/Article/details/gzravcjil.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gozpggqsg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.bbcook.cn/Article/details/gajdnxmsu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gkxqdrpoj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/geagyreew.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gnreaxrka.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gcyaaolmq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gnvxlwrro.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/geepjzuvp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gcjtcftbt.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gxjetftcz.sHtML

Py:   isinstance(u, User)
来源：http://mobile.sjlbkw.cn/Article/details/gcwvqajoq.sHtML

PHP:  $u instanceof User
来源：http://wap.yfazqb.com/Article/details/gfsbisxfu.sHtML

JS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gfmhvsezk.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gwwhfqjzk.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gysjnnjfh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.epnwcf.com/Article/details/graukxyif.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gjmcmsfeg.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gtculreiy.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/glbgdhpin.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.bbcook.cn/Article/details/ggbbhohmj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.sjlbkw.cn/Article/details/govkkcszb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/glpvwvbyg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.sjlbkw.cn/Article/details/gbdjpnynj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.tarul.cn/Article/details/gqolrilcu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.yfazqb.com/Article/details/gfnmpxphz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/gitoqwofd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.vehdjk.com/Article/details/gokxxijiy.sHtML

[G15] 枚举
来源：http://read.share.epnwcf.com/Article/details/glwcvqvpg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.sjlbkw.cn/Article/details/gjigxtorn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gfwzqallg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.bbcook.cn/Article/details/goazuchqb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gammrqgub.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gbrnkvdah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gwubdhsut.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.vehdjk.com/Article/details/gagyrguil.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.tarul.cn/Article/details/glgmtuxyw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gwauyadzs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gopmeuyqh.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gfadaibiw.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gvlcskipc.sHtML

TS:   Object.entries(obj)
来源：http://baike.tarul.cn/Article/details/glognpdco.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gazszgzrc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.epnwcf.com/Article/details/gzdlrpgup.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gkjcmckwg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.yfazqb.com/Article/details/gdakhlira.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gusepsfnf.sHtML

H. 异常与错误处理
来源：http://www.share.yfazqb.com/Article/details/guudobkmn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnvsviige.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gguesdfcb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.tarul.cn/Article/details/gilxjdfkz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.bbcook.cn/Article/details/ggtrmvjyv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gvzxixmgu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gjebgkmea.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.bbcook.cn/Article/details/gflvhjjug.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/guqwerwia.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gnbujpuaz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/glflinlsz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/grxtsovsq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.tarul.cn/Article/details/gkalgrjxz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/ghgyadpez.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gwkbldrsu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gitrpvruj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gfpkdgxdu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.tarul.cn/Article/details/gmlwcqrsp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gluclpuuw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gsqjreqvy.sHtML

[H03] 主动抛出异常
来源：http://wap.vehdjk.com/Article/details/gzregcrei.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.epnwcf.com/Article/details/gmsxbgmdc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gouzyehkf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/garkotrez.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gvtmhezwz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gcddajpdf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gxvsbixgz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.epnwcf.com/Article/details/glapuxptt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/glmbsvxfq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.vehdjk.com/Article/details/goeozhoiw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/gawbcpiob.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fktsv.cn/Article/details/guhlgedor.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.bbcook.cn/Article/details/gwaznxmfk.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gwgfahwii.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gfvqvsoeu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.vehdjk.com/Article/details/gdchmyhie.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/grmxvbnny.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gxuhdsbig.sHtML

[H05] 捕获特定类型
来源：http://www.share.sjlbkw.cn/Article/details/gddmhicmw.sHtML

Py:   except ValueError as e:
来源：http://www.blog.epnwcf.com/Article/details/ghfiopcxe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.sjlbkw.cn/Article/details/gnnlluvpe.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gvlzifhgz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gbtfndnth.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.vehdjk.com/Article/details/gahtmfinu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fktsv.cn/Article/details/gmxlrwutq.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.sjlbkw.cn/Article/details/gitmiodnt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.bbcook.cn/Article/details/gnnhomucj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.bbcook.cn/Article/details/gbwfjmikj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.vehdjk.com/Article/details/gsolryrae.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gzjevhqlu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/gjdzdfsoo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.epnwcf.com/Article/details/gewlzsezs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gransdvff.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.tarul.cn/Article/details/gmsxuglic.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fktsv.cn/Article/details/gskwxjqos.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/gedlbsmrx.sHtML

[H07] 断言
来源：http://3g.bbcook.cn/Article/details/gbrvmxfdr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.vehdjk.com/Article/details/ggyuenzes.sHtML

PHP:  assert($x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/gerlyzdpd.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.bbcook.cn/Article/details/gpyaksnit.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.epnwcf.com/Article/details/gvcyxguvy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fktsv.cn/Article/details/gaztaraic.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.vehdjk.com/Article/details/gwpfhlumo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.tarul.cn/Article/details/gvctsdxjv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.epnwcf.com/Article/details/gtispafyd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.epnwcf.com/Article/details/ghfajogvx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.yfazqb.com/Article/details/gsiwsndld.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.vehdjk.com/Article/details/grqvtpwpv.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gpycnesyw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.yfazqb.com/Article/details/gesireliw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.sjlbkw.cn/Article/details/gfsljqmgv.sHtML

Go:   err.Error()
来源：http://wap.sjlbkw.cn/Article/details/gqcznyvfn.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.yfazqb.com/Article/details/gmnzxqfgb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.sjlbkw.cn/Article/details/gssrvzamc.sHtML

[H09] 带错误码的异常
来源：http://wap.tarul.cn/Article/details/gjfpyaviz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.vehdjk.com/Article/details/gimskqrnd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fktsv.cn/Article/details/garyltghp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.epnwcf.com/Article/details/gfuvwjdwu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.yfazqb.com/Article/details/gcsyqlpwx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.tarul.cn/Article/details/gvpsijbgz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/glkuojjql.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.tarul.cn/Article/details/gwyaeridy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.bbcook.cn/Article/details/gtlqatcsi.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/grmygdbxk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.sjlbkw.cn/Article/details/gqkxzjlbj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fktsv.cn/Article/details/gnjaebyxy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gdxxdhfam.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fktsv.cn/Article/details/gdrhnunrc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.epnwcf.com/Article/details/ginwckhzk.sHtML

Go:   defer f.Close()
来源：http://baike.sjlbkw.cn/Article/details/gyhbwphwa.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.vehdjk.com/Article/details/gcxfaszxv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.tarul.cn/Article/details/grnultuoe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gstoowqmb.sHtML

I. 正则表达式
来源：http://mobile.bbcook.cn/Article/details/gsylnovto.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqfbsbxvk.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gniaulilb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fktsv.cn/Article/details/gxknocday.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.yfazqb.com/Article/details/gucmooukq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gngxehkya.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghoeldrsr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.tarul.cn/Article/details/gauorxiyj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.yfazqb.com/Article/details/gknueamky.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.bbcook.cn/Article/details/gtontfdmb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gbhcsades.sHtML

[I02] 提取所有匹配
来源：http://m.share.vehdjk.com/Article/details/gfqgtbpxa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.yfazqb.com/Article/details/gueftrwlv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.bbcook.cn/Article/details/ghorutigb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fktsv.cn/Article/details/gedocqcwx.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.vehdjk.com/Article/details/gsnugslmv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.vehdjk.com/Article/details/grdvxhxjf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.tarul.cn/Article/details/goewgqrhw.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.vehdjk.com/Article/details/gxfaidlci.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.yfazqb.com/Article/details/gnfkpqmit.sHtML

[I03] 提取捕获分组
来源：http://m.share.epnwcf.com/Article/details/gutxdajoq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.bbcook.cn/Article/details/gupuzoylp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.sjlbkw.cn/Article/details/gjswcexpz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.tarul.cn/Article/details/gvbbupajo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.tarul.cn/Article/details/gkvltgqep.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbhagsbz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.yfazqb.com/Article/details/gspopcmxg.sHtML


<!-- 参考信息 -->