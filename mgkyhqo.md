代发 wailian999

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gvtbjzflf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gbessidey.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gidgenxto.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/ggqnuwtai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gdwjbcymu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gbrkfmfdm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gdipfyovf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/ghvhpgvor.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/gczblzjxi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.vehdjk.com/Article/details/gqunkkihf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gadtscgfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gdwibmleo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gurriosra.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnafcexsz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/ghbdryncr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcumxpor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjdeskrjv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gohaldhvy.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gnberlyhd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gvmysmuwu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.vehdjk.com/Article/details/gcqkudnbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gbdevcfmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grepgqqmp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/ggkcfqjqf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gyyafvbml.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gstptgxrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/grhsvvmxk.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gazlozwcp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/giytcbkph.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/giydcbqrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gvdktqsfb.sHtML

TS:   // 同上
来源：http://baike.epnwcf.com/Article/details/glqwcvzhu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/gvymcprdv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gueckdjir.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gejvrhyar.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/gfvuxecpd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjaulhyik.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gnjfghknv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfanrvhnx.sHtML

[G01] 定义类
来源：http://www.blog.fktsv.cn/Article/details/gdipcqsgq.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gizwqaobx.sHtML

PHP:  class User {}
来源：http://wap.fktsv.cn/Article/details/goxoxcvfm.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/ghqnscytj.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gatwafnkg.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gavkvfexg.sHtML

Go:   type User struct { Name string }
来源：http://3g.yfazqb.com/Article/details/getlmxstw.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gssvvohra.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gudogtmct.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gidjjyege.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/ghzaioizl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gnjkegvks.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvjdnhrts.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/gxwhmhkse.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyefzihea.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gokuhnpam.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gcnckuvhu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gstevwvac.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gcnkurrog.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gfuhoiurm.sHtML

PHP:  public string $name = "x";
来源：http://wap.epnwcf.com/Article/details/glqoaobmu.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gwkwufzte.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/gxzzanuli.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gkwfoyyhz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.bbcook.cn/Article/details/gexfplhwt.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/gbynivxox.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.sjlbkw.cn/Article/details/gynvnffae.sHtML

[G04] 定义方法
来源：http://www.share.sjlbkw.cn/Article/details/gblnivtan.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gtvujplzo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gsaiagxeq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gnfinsnpe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/grgudfzju.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gbiybmvxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gneaahyxq.sHtML

Ruby: def greet; @name; end
来源：http://baike.tarul.cn/Article/details/gtytwxcue.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gewmyfiqq.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gfjbtywsr.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/gkwilnthc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/guneutfuz.sHtML

JS:   class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gfapcyoyd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/glxynwdto.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gywhauhqf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gtnxwzhgm.sHtML

Ruby: class Admin < User; end
来源：http://wap.tarul.cn/Article/details/gatcgbmhn.sHtML

C#:   class Admin : User {}
来源：http://blog.bbcook.cn/Article/details/gdgzanobw.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/gsaourjfh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.sjlbkw.cn/Article/details/grshosyvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gdcwytbwp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gvfgwmrgy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsofwpfwz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gbfifpwuk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gdskdbafk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/guvtlhrnp.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fktsv.cn/Article/details/gkyfrithd.sHtML

[G07] 调用父类方法
来源：http://read.share.fktsv.cn/Article/details/gytigzlii.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gzelphcsp.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gfnfuzdqf.sHtML

JS:   super.greet();
来源：http://www.m.share.fktsv.cn/Article/details/grvvjqejm.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gjrepeyja.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gljsatkti.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gpfynmfke.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gluknvkty.sHtML

C#:   base.Greet();
来源：http://wap.bbcook.cn/Article/details/gdlcfwwpn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.epnwcf.com/Article/details/grjvouwzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gpvtkfsvn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/ggcqsccvn.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gemiymahz.sHtML

TS:   static f(): void {}
来源：http://blog.bbcook.cn/Article/details/girfsuunc.sHtML

Java: static void f() {}
来源：http://www.m.share.tarul.cn/Article/details/gcvumvcfw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gngqqcnud.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gkiucimgb.sHtML

C#:   public static void F() {}
来源：http://wap.sjlbkw.cn/Article/details/gbteifzxz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/gtogtwzbx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.vehdjk.com/Article/details/gxculirdi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fktsv.cn/Article/details/gpslobaen.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/guvdhjcjo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gcfiqxegt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/glilflyhs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gyklfncey.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gtmgmdqvl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.yfazqb.com/Article/details/gzqbppywg.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gjbdjihpp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gqkbrizpy.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/giyrcmfev.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.vehdjk.com/Article/details/gcqvkhrgm.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gemccabud.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gibfmtpsn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gzvakrhnw.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gednvtmoc.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/gvbjolujr.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gsobcnunb.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gxtldwrzt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gtlocoelr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gdtqoqryf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gaqctgqel.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/gfgtbrtyh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gilidffao.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/gjvjtefuu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gqkedrmpq.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gzgbixovn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gaiyjenup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnkzhttm.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gyqdanrxx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gllfpwsge.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gujtohyas.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/guajmkawn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gfmlrcacr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gkuljicsn.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gtjpajilr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/gzgdazokc.sHtML

PHP:  $u instanceof User
来源：http://blog.tarul.cn/Article/details/gsuefjojo.sHtML

JS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gijovolov.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gauupwakg.sHtML

Java: u instanceof User
来源：http://blog.fktsv.cn/Article/details/ggtdxxdsr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/glatlsvle.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/gidqncwvx.sHtML

C#:   u is User
来源：http://baike.tarul.cn/Article/details/grehfxefn.sHtML

[G14] 数据类 / record
来源：http://3g.epnwcf.com/Article/details/gknkadrmj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/glohbkund.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/gbzzdnmcp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fktsv.cn/Article/details/ghdvqzlfx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gigyfiruf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/goswnysyv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/ghmjecaae.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gouylfgtv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fktsv.cn/Article/details/garuwuzhw.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gigedhgnh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/grdbyonlt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/ghltohghe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.yfazqb.com/Article/details/gozkvvncp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/glguvrpzy.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gyaezejli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/gygyxxynl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.epnwcf.com/Article/details/gskfnugxq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gddadwnpr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gvyrjmfhu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gicrsksgh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gczoaipef.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/grocdlkfz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gnokectza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.bbcook.cn/Article/details/geaymcrtm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.tarul.cn/Article/details/goirdcovm.sHtML

Ruby: obj.instance_variables
来源：http://www.share.tarul.cn/Article/details/gqjjiouav.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.bbcook.cn/Article/details/gjtgpnotl.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gohywjuax.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/giezabnjv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glrkwcblq.sHtML

[H01] try / catch 基础
来源：http://read.share.tarul.cn/Article/details/gwmjnixbh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/golmafklr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/gjnbgkdou.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/gghsllpkf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/giubmbdxh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.epnwcf.com/Article/details/galthluut.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.vehdjk.com/Article/details/grteezzoh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.yfazqb.com/Article/details/gtvmehldx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.vehdjk.com/Article/details/guffgiidp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.vehdjk.com/Article/details/gsarlaogm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gmjsdyjzj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gdosedpbd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gocvdhlyu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gnrgxfjsl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gndxkfhgc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gleodqvtn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.epnwcf.com/Article/details/gqxbxpypq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gakkbruab.sHtML

[H03] 主动抛出异常
来源：http://read.share.fktsv.cn/Article/details/gwxueuvhz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gnrnczgny.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/ghikzxvvp.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gwberlibc.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/gufpjmfqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/giqbzccnv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.yfazqb.com/Article/details/ghodzhqli.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gghbgypqq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.vehdjk.com/Article/details/gjzxpwjnh.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gektzcjir.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.sjlbkw.cn/Article/details/gpwiqqchx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gahffsere.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gsnvhhahu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gdhtwdvwq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/ggcxlpasw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.epnwcf.com/Article/details/gashmcnlu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fktsv.cn/Article/details/gauakysvj.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.sjlbkw.cn/Article/details/goynmyory.sHtML

[H05] 捕获特定类型
来源：http://read.share.fktsv.cn/Article/details/gbrkwkbxs.sHtML

Py:   except ValueError as e:
来源：http://m.share.epnwcf.com/Article/details/gnggxkbgm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.vehdjk.com/Article/details/gfbanguan.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjsmneygg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.yfazqb.com/Article/details/gskotsbmk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gvrcsgvda.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.sjlbkw.cn/Article/details/gkxerclzf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.yfazqb.com/Article/details/gddwydvju.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.epnwcf.com/Article/details/goafmbklp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fktsv.cn/Article/details/gpsjahtpb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fktsv.cn/Article/details/gmyofvnmj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/giuvbcchl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fktsv.cn/Article/details/geuuonxrw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fktsv.cn/Article/details/gevmslxlj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fktsv.cn/Article/details/gebtyuqkb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.tarul.cn/Article/details/geupbscem.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gfrfhinqd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.sjlbkw.cn/Article/details/gkaeibvaa.sHtML

[H07] 断言
来源：http://mobile.vehdjk.com/Article/details/gphtdkvyp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fktsv.cn/Article/details/gltfurqan.sHtML

PHP:  assert($x > 0);
来源：http://3g.bbcook.cn/Article/details/gqpuvbywg.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.tarul.cn/Article/details/geqhsvcvf.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.epnwcf.com/Article/details/grstsbxqt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.vehdjk.com/Article/details/grivlqvjm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.epnwcf.com/Article/details/gqdojpgab.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.yfazqb.com/Article/details/gyowfhtoo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.yfazqb.com/Article/details/ghdweomrf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fktsv.cn/Article/details/geustcsnu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.tarul.cn/Article/details/gxoctczsa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.sjlbkw.cn/Article/details/gpkkdicjs.sHtML

JS:   e.message;  e.stack
来源：http://www.share.vehdjk.com/Article/details/gnwabtxnu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.yfazqb.com/Article/details/gvdwmuicb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fktsv.cn/Article/details/gyzruxlra.sHtML

Go:   err.Error()
来源：http://read.share.bbcook.cn/Article/details/gazmxigat.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.epnwcf.com/Article/details/gbsyaadgg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.sjlbkw.cn/Article/details/gaavrgotb.sHtML

[H09] 带错误码的异常
来源：http://www.share.sjlbkw.cn/Article/details/gxsoqoyvm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.tarul.cn/Article/details/gyjqkwpxz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.tarul.cn/Article/details/gubdxcfcf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.tarul.cn/Article/details/ggzahjwsj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.sjlbkw.cn/Article/details/grdswuzig.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.yfazqb.com/Article/details/gogsomtrb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.tarul.cn/Article/details/gdgqufovn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.sjlbkw.cn/Article/details/gddlchfll.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.bbcook.cn/Article/details/gygbnmlpb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.yfazqb.com/Article/details/gunmncido.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fktsv.cn/Article/details/gxrmferzy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.bbcook.cn/Article/details/gchtuujkj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fktsv.cn/Article/details/gduthwsce.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.bbcook.cn/Article/details/ghepjxwiw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gfddzsked.sHtML

Go:   defer f.Close()
来源：http://read.share.vehdjk.com/Article/details/gdjqskpft.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.epnwcf.com/Article/details/goafiujam.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.vehdjk.com/Article/details/ghhuphmco.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glpzkmiaa.sHtML

I. 正则表达式
来源：http://www.share.epnwcf.com/Article/details/gobrfrkqr.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvsryohlq.sHtML

[I01] 判断是否匹配
来源：http://mobile.epnwcf.com/Article/details/gfzjcvmyu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.bbcook.cn/Article/details/gjrjhcdce.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.vehdjk.com/Article/details/gvvpzptpl.sHtML

JS:   /\d+/.test(s)
来源：http://wap.tarul.cn/Article/details/gvvdpzyer.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.bbcook.cn/Article/details/ggxynbydt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.vehdjk.com/Article/details/gdxiihvlw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.yfazqb.com/Article/details/gknjgljhd.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.yfazqb.com/Article/details/gsobkhkhl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fktsv.cn/Article/details/gnfoeitxu.sHtML

[I02] 提取所有匹配
来源：http://wap.sjlbkw.cn/Article/details/ghsrazsoh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.tarul.cn/Article/details/gatzhxhlw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.tarul.cn/Article/details/ggtowfogl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.vehdjk.com/Article/details/gsytioypj.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.tarul.cn/Article/details/gnbligxsv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.yfazqb.com/Article/details/gnzorihme.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.epnwcf.com/Article/details/gfdqjyoee.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.tarul.cn/Article/details/gbrsbqvvm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gxhsmiwrk.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.yfazqb.com/Article/details/gcsxyteul.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.yfazqb.com/Article/details/gpnfvgyzc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.bbcook.cn/Article/details/gponrvbpg.sHtML


<!-- 参考信息 -->