代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gqpzikoji.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gptexiuvb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gqkdyjalx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.sjlbkw.cn/Article/details/glbgyphsp.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gsjuosazj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkdhkbxtw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gmybhyzra.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/glanxwmss.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gfejkyqgk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gfueynjiv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/gwkecejou.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnekfhmqf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gkwqmlhit.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gmbxjmgmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gteknsibx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gucngrvxy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glwrgynsy.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gohmiuplt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gbvgulees.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gprthmhhg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gdbnsopob.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gtkwrwivp.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gbeigqenj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guyzaktkb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gmhxuqera.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gseafpfhz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gelpcukyc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gnexrbkkp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/gjxvjffxc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gyzdyipjh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/galufsdpo.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gceaocxrk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/grvbqehbp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gfbcfhabi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gnhgdgyxe.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gytnuljhk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gclqvdqsg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/geiqqbmch.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gapfxdjqs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/gmymuzpyx.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gauyvwyyp.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gzdwonajz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbklhnuaf.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/glkczrvbp.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gvzqnyzgd.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gohcqcfjh.sHtML

JS:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gilvqpdxq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/glrdlsesn.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gslvrxyyb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gwhrhaptw.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/grnzbrsgw.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gyttozpkf.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gqfvankoy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gxbtlerfs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/gdwjjqbjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gfcshuoil.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gpncdcbxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glezcfglz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/giuacgggp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gshhkrnmp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/ghbzzevrz.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gqqslrjkr.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gcgiaoxkh.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/grqkdbiav.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gmhlnikes.sHtML

TS:   name: string = "x";
来源：http://read.share.tarul.cn/Article/details/gpxmfgyex.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gxsxfshvv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/grijdixaz.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/ggyyakfnu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gygetfpyv.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gyjdwecvl.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gzzsodsgo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gicbqgeri.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gbocjhyio.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvznjekc.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gcejerkmh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gggfvbbcj.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gdcailzan.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gtuudotvw.sHtML

[G05] 继承
来源：http://wap.fktsv.cn/Article/details/gjlmvuvwa.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fktsv.cn/Article/details/gtfsvhmtd.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gcjfbbedp.sHtML

JS:   class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gpciqczrd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gatyzrrdb.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gjklbujzf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gkghnxfub.sHtML

Ruby: class Admin < User; end
来源：http://mobile.yfazqb.com/Article/details/gcpehwmhj.sHtML

C#:   class Admin : User {}
来源：http://3g.yfazqb.com/Article/details/gcxvfugev.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/gnxqcaqnv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/geksnrlhz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gzzwoyeoz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gcpqszsxk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gyulwxmam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gwivyjgzd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gnsrfzhaf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.epnwcf.com/Article/details/gpokqafzc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gibtckzok.sHtML

[G07] 调用父类方法
来源：http://www.blog.epnwcf.com/Article/details/gzqufkeho.sHtML

Py:   super().greet()
来源：http://blog.fktsv.cn/Article/details/gqmkqcepx.sHtML

PHP:  parent::greet();
来源：http://wap.bbcook.cn/Article/details/guzmwazrh.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gcutjndox.sHtML

TS:   super.greet();
来源：http://www.share.yfazqb.com/Article/details/gyksqlhhf.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/geqivzcup.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.epnwcf.com/Article/details/gqbxwoeyn.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/ghacaiges.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/gdlzbuucy.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/gmdqbsftb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.tarul.cn/Article/details/gazotpaxe.sHtML

PHP:  public static function f() {}
来源：http://www.blog.bbcook.cn/Article/details/gvwjxubcp.sHtML

JS:   static f() {}
来源：http://mobile.bbcook.cn/Article/details/gpceuohit.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gyqjybkeg.sHtML

Java: static void f() {}
来源：http://baike.fktsv.cn/Article/details/gneybghau.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gibubyete.sHtML

Ruby: def self.f; end
来源：http://3g.fktsv.cn/Article/details/gzybyutph.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/ggdygferp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.sjlbkw.cn/Article/details/gtmbqikth.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.bbcook.cn/Article/details/grqdlckzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/gwwelvdco.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.bbcook.cn/Article/details/grmtroitz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gpqmzzzly.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/gbznyxuka.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fktsv.cn/Article/details/gevfilutf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.tarul.cn/Article/details/gsxjjifiw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.tarul.cn/Article/details/gfgehryjy.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gajvlghte.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.tarul.cn/Article/details/grslpiisb.sHtML

PHP:  public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/gyjkexsgc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.bbcook.cn/Article/details/gqdpwymjj.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gidbocqwm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.yfazqb.com/Article/details/gwgaecauq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.epnwcf.com/Article/details/gjgvagsjy.sHtML

Ruby: public / protected / private
来源：http://mobile.tarul.cn/Article/details/gmfriyzsq.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gflzqbxnq.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/geldlusel.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/ghilkizta.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/ggzlelhzt.sHtML

JS:   get name() { return this._name; }
来源：http://3g.bbcook.cn/Article/details/gcixzbgpj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gxhsowpjb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwjxkaqb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gwkarsnle.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.bbcook.cn/Article/details/gzczdokvs.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/gqdtvjibg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gbteiedpt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gesxhrjvh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gmfpymsii.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlxtihui.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gckpkflxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gjmofqnyu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gxmgcqxjx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.vehdjk.com/Article/details/gclyircsr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gzbtstaaj.sHtML

[G13] 判断对象类型
来源：http://m.share.sjlbkw.cn/Article/details/gkqmwbkgm.sHtML

Py:   isinstance(u, User)
来源：http://m.share.sjlbkw.cn/Article/details/ghupduznn.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gtprakxne.sHtML

JS:   u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gwwocnzqa.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gdmcsomjt.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gcdnjazwm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.sjlbkw.cn/Article/details/gyqtrppnx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gbqxxnbhz.sHtML

C#:   u is User
来源：http://wap.yfazqb.com/Article/details/gygepsxvo.sHtML

[G14] 数据类 / record
来源：http://3g.tarul.cn/Article/details/glqytvtcq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/givgvsuvn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.bbcook.cn/Article/details/gcwddeovc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gpxcrbukt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.vehdjk.com/Article/details/gnczgbzrc.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gcgnzrvfd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fktsv.cn/Article/details/gnpfklepl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/gfqeinopl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/gozzptkdk.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gqyrjwdua.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fktsv.cn/Article/details/gzbukfphf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/goliatost.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fktsv.cn/Article/details/ghnamzmwd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gqnykcwnk.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gjmdfbxac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/grwqpaerl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.sjlbkw.cn/Article/details/ghzcibfcc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gzjazwnpg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/gsndwxvag.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gimuvmzxm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/gymrwpvrq.sHtML

JS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gfzlahryy.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gjiqpeqho.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/groopgucn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/grgquhjdl.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/ghxpvbjjj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/godkqallr.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtasgixfg.sHtML

H. 异常与错误处理
来源：http://m.share.yfazqb.com/Article/details/gpwuzjlth.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmenonteq.sHtML

[H01] try / catch 基础
来源：http://baike.yfazqb.com/Article/details/gykwmsfvz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fktsv.cn/Article/details/gzmqgmzop.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.tarul.cn/Article/details/gcccmgpmh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/gnbajaaad.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.epnwcf.com/Article/details/glxjwcecs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gvcvpbxgc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gqtffupxn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.epnwcf.com/Article/details/gtawyoydk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.yfazqb.com/Article/details/gkzivbskq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gyfkzzcfb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/gultinqce.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gpwzoqkuv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/ghquysqmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.vehdjk.com/Article/details/gflxhwmcn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gxalasyzc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.epnwcf.com/Article/details/gxmftflmg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gllxyuure.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gvhxflqux.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gnyrnwfha.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fktsv.cn/Article/details/gpsxfnnww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gtljubokn.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.yfazqb.com/Article/details/gesiuslzf.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gqzpmtfts.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/gvnmizxho.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gdykiljgn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gkmsibebw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gpzjkjayo.sHtML

[H04] 自定义异常类型
来源：http://www.share.sjlbkw.cn/Article/details/gdqwlapqs.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.vehdjk.com/Article/details/gqbvytroa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gpxtzgbjx.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gswurpoug.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.epnwcf.com/Article/details/gtjggrrtv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.epnwcf.com/Article/details/gnqejupbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.bbcook.cn/Article/details/gntopjdkd.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gnxwtapgp.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.yfazqb.com/Article/details/ghpvmrzpe.sHtML

[H05] 捕获特定类型
来源：http://wap.fktsv.cn/Article/details/ghcukdctg.sHtML

Py:   except ValueError as e:
来源：http://baike.tarul.cn/Article/details/gbgjtzudq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gwerfkyfx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.vehdjk.com/Article/details/gyyqunaqg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gybufdwrr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfbpgnywk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.sjlbkw.cn/Article/details/gtrsdtazu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gydjznbsz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.sjlbkw.cn/Article/details/gcbfcmvqn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.bbcook.cn/Article/details/gnwjfxbeg.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.epnwcf.com/Article/details/gzrmfmmtf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gjwfoqecy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/grqimxwkz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.yfazqb.com/Article/details/gjhrjsxfw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.yfazqb.com/Article/details/gpbyplwxm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.bbcook.cn/Article/details/gclenuoux.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.vehdjk.com/Article/details/gobwuoucl.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/gehebsxed.sHtML

[H07] 断言
来源：http://baike.bbcook.cn/Article/details/govsmgvon.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.vehdjk.com/Article/details/gqmeijzma.sHtML

PHP:  assert($x > 0);
来源：http://baike.bbcook.cn/Article/details/gmhwwicjs.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.yfazqb.com/Article/details/gwpuphovr.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gxhsyolkn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.tarul.cn/Article/details/gtyimffho.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.bbcook.cn/Article/details/gdvznqmbx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.epnwcf.com/Article/details/gutdmqfmn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.sjlbkw.cn/Article/details/glwhhsvxz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fktsv.cn/Article/details/ghufpkauj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.epnwcf.com/Article/details/glwtflucy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.bbcook.cn/Article/details/gpahdkteu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fktsv.cn/Article/details/gtfkrzgwo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.tarul.cn/Article/details/geukgyolq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.sjlbkw.cn/Article/details/gqaumjdyz.sHtML

Go:   err.Error()
来源：http://wap.fktsv.cn/Article/details/gcokcmwjb.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.bbcook.cn/Article/details/gtkedeylo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.tarul.cn/Article/details/goqgywobf.sHtML

[H09] 带错误码的异常
来源：http://read.share.bbcook.cn/Article/details/gnxqtnqyj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.yfazqb.com/Article/details/gvyimpuud.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.tarul.cn/Article/details/gaydqqhgl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.bbcook.cn/Article/details/gihvtscos.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.epnwcf.com/Article/details/gtcudvjgl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.tarul.cn/Article/details/gmihyqwmh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.yfazqb.com/Article/details/ggkhuwcwa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.tarul.cn/Article/details/gqxjtjvve.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.tarul.cn/Article/details/ggtwffhrf.sHtML

[H10] 资源自动释放
来源：http://read.share.yfazqb.com/Article/details/ggqdxwgib.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fktsv.cn/Article/details/gnydmqbbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.vehdjk.com/Article/details/ggjotvvwb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fktsv.cn/Article/details/gkxwhjrcz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.vehdjk.com/Article/details/gcqehefvd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.sjlbkw.cn/Article/details/gzpydmqiu.sHtML

Go:   defer f.Close()
来源：http://m.share.yfazqb.com/Article/details/gonxpwixt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fktsv.cn/Article/details/giwvpzzty.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghgaartjn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gznziasap.sHtML

I. 正则表达式
来源：http://mobile.sjlbkw.cn/Article/details/gmgowbjui.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdqdcpcle.sHtML

[I01] 判断是否匹配
来源：http://3g.tarul.cn/Article/details/gyubktpft.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.bbcook.cn/Article/details/gscotsljd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gzyncepwm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.vehdjk.com/Article/details/gkemoumcs.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.tarul.cn/Article/details/gbagizodg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.epnwcf.com/Article/details/gjhewcaeo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.vehdjk.com/Article/details/gwdrlwhxn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.yfazqb.com/Article/details/ghdnpcimr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.sjlbkw.cn/Article/details/gsbcnlvis.sHtML

[I02] 提取所有匹配
来源：http://www.share.yfazqb.com/Article/details/gwwgowuef.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.bbcook.cn/Article/details/gxanggjxv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.yfazqb.com/Article/details/gadygzmyu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fktsv.cn/Article/details/gtkysvwap.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.epnwcf.com/Article/details/gdahgjapm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.tarul.cn/Article/details/gaqiliwjw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.sjlbkw.cn/Article/details/gykxvavpz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gsjkfybzx.sHtML


<!-- 参考信息 -->