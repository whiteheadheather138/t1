代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/gkvlfcnex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gjgoqvgzw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gujmakdvt.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gwudjhrcw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gqezrtrhf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gcpgnoxif.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/gfzkubzvg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gzvqxellt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gnsglcwid.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gucseqvuy.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gghapujna.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gjqxnbtjn.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gxjuenedu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grtgcictc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.bbcook.cn/Article/details/grhpwwdxp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gatyrnyot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gsvfyahzn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gubxobjhx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gigzndcbu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/gscbpzqlu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gmxskczqg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gotkbtmzx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gyydtnuai.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ggdqiqyay.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gtsqmsjwx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gfzglbfqq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/grqealwuw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gftofbrhe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gljvwrwfu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtdkwemod.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/gaarufhdl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gzlmnxpit.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gmwoptxem.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gcnskadqy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gfjeksfmm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.tarul.cn/Article/details/glwxlhxgs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/gwtkvvvti.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gttjnweew.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/gckjsfipi.sHtML

[F12] CSV 读写
来源：http://www.share.vehdjk.com/Article/details/guulkzjbq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gpoumruio.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gmspchgvy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.vehdjk.com/Article/details/gyzltyhxq.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gipyokthw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/gyeptzrfm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.epnwcf.com/Article/details/gqcfdhgct.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/gbplhdxvd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/ghxzkmswp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gaybdawag.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/gdujytxab.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gywdvvjla.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/gjmewdqsf.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gkmnjfnvu.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gmjgubtun.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gxsnuqdek.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.epnwcf.com/Article/details/gtzwnhhkf.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gionvzhzb.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gvynkhkhh.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gwqtuhahg.sHtML

C#:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gochhxfsh.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gsmtrdgeg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gqyunfahs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/ghgmlzmyt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gwvzgwyhi.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gotwhkdwp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gqagcgbot.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/gbjsatnyb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gtkxkwnoj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fktsv.cn/Article/details/gmqjbthoa.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gynrhivcy.sHtML

Py:   self.name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gyycwbjps.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gwsnvdoee.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/ghcszfnxg.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gwyaelkqu.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/glixoxnum.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gnmzsuuof.sHtML

Ruby: @name = "x"
来源：http://m.share.fktsv.cn/Article/details/grefysmcn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/guzyeppxo.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gymcbgdou.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gogeztedq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gpuwedoan.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gyzuhbqgg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gyqpmkxxi.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/grstjamjc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gskieuiln.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gymghrzdc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gcwkcuzzj.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gchermmwe.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/guzbndfyo.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gofqfzwis.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gtyjosjiw.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gkloxwsxv.sHtML

Java: class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/ghitnfepg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gylyhdrye.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/gojdmhppb.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/ggzgvpwpt.sHtML

[G06] 重写方法
来源：http://m.share.tarul.cn/Article/details/goxdgjtcp.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gyjexdfjj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gijhjnzuv.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gfbosuakh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggppsxyni.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/glsharfqa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gxmbbyhqw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/ghozthigq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.yfazqb.com/Article/details/gbrroazyi.sHtML

[G07] 调用父类方法
来源：http://www.share.epnwcf.com/Article/details/grzfmjaze.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gubgubhpi.sHtML

PHP:  parent::greet();
来源：http://blog.sjlbkw.cn/Article/details/gpygvyycw.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gfmkizsxe.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/gwqrmrlmp.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/ggdprlsjy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/glvmshlya.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gqglvwfrr.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/ghueknipz.sHtML

[G08] 静态方法与属性
来源：http://blog.sjlbkw.cn/Article/details/gyzwwfezc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gfxfgmawo.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gzigctlyu.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/gifqvszjg.sHtML

TS:   static f(): void {}
来源：http://mobile.bbcook.cn/Article/details/gonwmnlgg.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gzbdefoai.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gazpmhyzz.sHtML

Ruby: def self.f; end
来源：http://wap.yfazqb.com/Article/details/gvpndnxkb.sHtML

C#:   public static void F() {}
来源：http://baike.vehdjk.com/Article/details/gkkcfjmhc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fktsv.cn/Article/details/ggsitjnjl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gmksxihhx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gbaijrdub.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/ggkmrkclr.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.yfazqb.com/Article/details/ggxsrwajc.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gvbwlvsql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.sjlbkw.cn/Article/details/gymmxcrcx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gbwbkvplv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.bbcook.cn/Article/details/gxfgknqjt.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gfytngztn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.tarul.cn/Article/details/gzuzftbfy.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/greeqmfvf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gacesopin.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gkdrrmudd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gfjwyqrit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.vehdjk.com/Article/details/gxnidwzct.sHtML

Ruby: public / protected / private
来源：http://baike.epnwcf.com/Article/details/grxyxklnw.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/gcyedazgy.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/gnxjwzoox.sHtML

Py:   @property 与 @x.setter
来源：http://baike.epnwcf.com/Article/details/gjeawtrtr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvpglduk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/ggcfbptcl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/glubzyioo.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gybwzrvgg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gnfavrlru.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/grbobapua.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gvomvdknv.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gmfpkntdx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gjzfdojqr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gwficcbfu.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/giycafjkb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gshsujjyj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gnwfllcgt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/gjhibwlrc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fktsv.cn/Article/details/galracifl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.sjlbkw.cn/Article/details/gdhaoascx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxkdqtva.sHtML

Py:   isinstance(u, User)
来源：http://blog.vehdjk.com/Article/details/gqiqfonto.sHtML

PHP:  $u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gkauvxbaj.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/glwzmxqmm.sHtML

TS:   u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/ggeybfsmy.sHtML

Java: u instanceof User
来源：http://mobile.tarul.cn/Article/details/gojkprnrw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gqyqzitmv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fktsv.cn/Article/details/gkhuwmflb.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gcvetrmdm.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/girejimoq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/ggnrhuedo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gilszsuny.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.yfazqb.com/Article/details/gjsgfhfrj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.bbcook.cn/Article/details/gkuqljdmw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/ggoyawwmz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gnpxqwcsr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gfeiwiaww.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.yfazqb.com/Article/details/geeizprgs.sHtML

[G15] 枚举
来源：http://www.blog.epnwcf.com/Article/details/gppjklhns.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.yfazqb.com/Article/details/ghqmsteza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gljeimpvb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gosjxgikf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gsrbpzqtd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gutgcdccb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gbjeiakup.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/grlwelyae.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gfoiaherq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/gpggsecfy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gwzvkakzz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.sjlbkw.cn/Article/details/gjjkzfdxt.sHtML

JS:   Object.entries(obj)
来源：http://m.share.yfazqb.com/Article/details/grtcmwoxl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/gdmivafbn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.epnwcf.com/Article/details/gkrcynpzr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gepvnvwqh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.epnwcf.com/Article/details/gijiwlxjb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/giezqadtr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqvnnpxxa.sHtML

H. 异常与错误处理
来源：http://read.share.epnwcf.com/Article/details/gfpsoycas.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvhwxolmx.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gnlwyohxi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gsihnrbyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.epnwcf.com/Article/details/gltbvzysa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gienwguix.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gzrszeyrz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.epnwcf.com/Article/details/gdlrwuqod.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/guuucrvsg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gaayxzlpt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gpimihlgh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.tarul.cn/Article/details/gsbpwtfuj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gaobhybrt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gdnkoiklj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gpggdkpdm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/glkhfhfhm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gpkevppyx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/gwzspvkct.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.bbcook.cn/Article/details/gtxgmfyxo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/geffxwagt.sHtML

[H03] 主动抛出异常
来源：http://www.share.bbcook.cn/Article/details/gwpvvctzr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gmcmgeogd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gslcktfss.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.epnwcf.com/Article/details/gbkvdzojm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gecdnwuva.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gmeoudfex.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.epnwcf.com/Article/details/gjsdhudkh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/gldyniyoy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gmwjrderz.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/guheiftyr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/gcujtulgo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/glkapohuv.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gdhzzpbbn.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/gfooxohmv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gictmqphb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.yfazqb.com/Article/details/gplisflyj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gthyixipq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.sjlbkw.cn/Article/details/gotkbktfg.sHtML

[H05] 捕获特定类型
来源：http://wap.bbcook.cn/Article/details/gkrpdesvh.sHtML

Py:   except ValueError as e:
来源：http://m.share.yfazqb.com/Article/details/gqeodmgwh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/geshjqckp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.yfazqb.com/Article/details/gqtrqbezb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.yfazqb.com/Article/details/guysohxso.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.yfazqb.com/Article/details/ggmpzsydf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.bbcook.cn/Article/details/gqyetgils.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fktsv.cn/Article/details/gsqbajcdz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.epnwcf.com/Article/details/gjzesregw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.yfazqb.com/Article/details/gbsklhohu.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gqmvpbwjq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gygjgvxka.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gqnrxkpbj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/geesbwofr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.tarul.cn/Article/details/gsmesvxwn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gujabghlf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.epnwcf.com/Article/details/gohtavhzv.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gkluekluw.sHtML

[H07] 断言
来源：http://wap.vehdjk.com/Article/details/gwqxvhrdr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.tarul.cn/Article/details/gsslbshid.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fktsv.cn/Article/details/gtnegzyiv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.tarul.cn/Article/details/ggnpwwtni.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gxvfdonjk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.yfazqb.com/Article/details/gdrvtukmd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fktsv.cn/Article/details/gohffcpic.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.sjlbkw.cn/Article/details/gkiphbskn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.yfazqb.com/Article/details/gdhnuoyhm.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gxzoftmre.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.bbcook.cn/Article/details/grhclsscj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.tarul.cn/Article/details/gtkuwnnux.sHtML

JS:   e.message;  e.stack
来源：http://wap.yfazqb.com/Article/details/gxvmyhfde.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fktsv.cn/Article/details/goavsuksx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fktsv.cn/Article/details/gyizzkjdd.sHtML

Go:   err.Error()
来源：http://mobile.bbcook.cn/Article/details/gciozqvis.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fktsv.cn/Article/details/gpdawhnuw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.yfazqb.com/Article/details/gozaeqnec.sHtML

[H09] 带错误码的异常
来源：http://3g.epnwcf.com/Article/details/gzzjsycug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.epnwcf.com/Article/details/ggfuudjgz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.bbcook.cn/Article/details/gakmsjbga.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.bbcook.cn/Article/details/gsekmridn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.sjlbkw.cn/Article/details/gayzvkuxb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.bbcook.cn/Article/details/gmrzyaiea.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.epnwcf.com/Article/details/gsopgjogp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/gryufgijj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.bbcook.cn/Article/details/gcnkogkqj.sHtML

[H10] 资源自动释放
来源：http://read.share.vehdjk.com/Article/details/gvpdgdhmo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.yfazqb.com/Article/details/geofganjp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.vehdjk.com/Article/details/gefikwlqa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fktsv.cn/Article/details/gzlqxrvip.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.epnwcf.com/Article/details/gxatpadon.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.sjlbkw.cn/Article/details/gfffoziek.sHtML

Go:   defer f.Close()
来源：http://www.m.share.tarul.cn/Article/details/gtnresjhk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fktsv.cn/Article/details/gtzxptvgn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gqmtzergs.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcgtgqyvu.sHtML

I. 正则表达式
来源：http://blog.bbcook.cn/Article/details/gjggrzzmm.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzbwkbgbt.sHtML

[I01] 判断是否匹配
来源：http://wap.vehdjk.com/Article/details/gugtdabph.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.bbcook.cn/Article/details/goygwwupz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fktsv.cn/Article/details/gaotbdhkt.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.yfazqb.com/Article/details/guwotlyxj.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.vehdjk.com/Article/details/gwqyitcmt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.bbcook.cn/Article/details/gbcurdaiw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.epnwcf.com/Article/details/gvvffrcmg.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.epnwcf.com/Article/details/gwfqjtqsk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.epnwcf.com/Article/details/gtajesslx.sHtML


<!-- 参考信息 -->