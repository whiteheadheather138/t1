代发 wailian999

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gqjfkbjcw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gqyisiuhn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/gdskvlurx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gmukbaymn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gbyzaiyho.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gqzgiotib.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/gmznglljv.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gushcexnf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gtsnlctmu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.yfazqb.com/Article/details/gnffdrxuv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/giuxljwil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gcvhqkvqc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gutahdyjw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gudwfiwjc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fktsv.cn/Article/details/gmognnkcx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gwdnmutwc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gaizgruus.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmchnvpsc.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gsqnqrgra.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvalivckc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gmcfjfvft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/ghmjijyht.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwoiikxeh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/gddsgcqle.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gdjpejmuv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gfphqgmfp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gjhzaspow.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gzcmhlnpd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gvgdsuatu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gbhkxmvku.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/gbomgsqgk.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gnwvblyok.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gdjzuxrsj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gfamtxhwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gpcuyusor.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gawigvvda.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gexzeymhf.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gcoyfukia.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gytyrrnmx.sHtML

[G01] 定义类
来源：http://www.m.share.fktsv.cn/Article/details/guxhwfgnm.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/gszurpyjw.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gcfiprgvw.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gjwurimxl.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gvuapzmkz.sHtML

Java: class User {}
来源：http://m.share.vehdjk.com/Article/details/gtnoketbl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gdydluggu.sHtML

Ruby: class User; end
来源：http://www.blog.bbcook.cn/Article/details/gxdqnujwa.sHtML

C#:   class User {}
来源：http://3g.vehdjk.com/Article/details/gisqajkmp.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gfrfqomsj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.yfazqb.com/Article/details/gykpaimka.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gpkskglko.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/glfscxhdb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnognmkwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gxdjqvpie.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gzmmagbht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.sjlbkw.cn/Article/details/gyuqaiaai.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/gfbfgpviw.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gejfgoarc.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gtuuxgtlu.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/godkaczqq.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfwyruqf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gzctvlodr.sHtML

Java: private String name;
来源：http://www.m.share.vehdjk.com/Article/details/gcnfulzvv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/ghmjdefeo.sHtML

Ruby: @name = "x"
来源：http://3g.tarul.cn/Article/details/gsezmdxot.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.epnwcf.com/Article/details/gnsaarfum.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gzagcenrf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.bbcook.cn/Article/details/grojasafa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gfosezmhv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gjwddeirv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gzfwohoxg.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/ggeiofyap.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gvcfqlima.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/ghqbpnsyj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gyhjpntoe.sHtML

[G05] 继承
来源：http://www.blog.vehdjk.com/Article/details/gmdtbwtru.sHtML

Py:   class Admin(User): pass
来源：http://read.share.yfazqb.com/Article/details/gyzpgrmmm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gnzabojya.sHtML

JS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gyyhtcmee.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gqvbtcdyo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gmdeybuhn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gcocesxcx.sHtML

Ruby: class Admin < User; end
来源：http://3g.yfazqb.com/Article/details/gibpmfbhm.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gucupqhud.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gljrrvacf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gbkxjbofc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gvwnqakpf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gjglbyxni.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gsdderwqt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gymzjbnlc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.epnwcf.com/Article/details/gzaochcqg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fktsv.cn/Article/details/gnfzloetz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gnoesmfvq.sHtML

[G07] 调用父类方法
来源：http://wap.yfazqb.com/Article/details/gpfprlqqp.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gdlplkmcs.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gmvyoyucy.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/ghpkwygoy.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gatilyspm.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gabqxpdpp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/gqtyaycmv.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gxqsdpawd.sHtML

C#:   base.Greet();
来源：http://www.share.vehdjk.com/Article/details/grmcfkyob.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gcvdoegya.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.yfazqb.com/Article/details/genuxxjsg.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gmrkjamiu.sHtML

JS:   static f() {}
来源：http://m.share.tarul.cn/Article/details/gnbyferye.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gpxxlulrc.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gabbuyrfp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gjnpncrgu.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gexeiiwgj.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/guuhjlgau.sHtML

[G09] 接口 / 抽象类
来源：http://wap.epnwcf.com/Article/details/gssxjfegj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gmncgvzki.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gyecwrruk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.epnwcf.com/Article/details/gvucajhsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.sjlbkw.cn/Article/details/gytuwroqq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gziajcnuw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gxcfcdexp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gdovgucbw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gcjhvdrfz.sHtML

[G10] 访问控制
来源：http://www.share.yfazqb.com/Article/details/gnryxuprg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.vehdjk.com/Article/details/grklvamfl.sHtML

PHP:  public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/ggyjhtqbs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gkfoaszjb.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gppekdjgl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fktsv.cn/Article/details/gzzijroso.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.epnwcf.com/Article/details/gbdvfjery.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gtlpvxgbz.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/gggxygaog.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gdzdneulx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gyszvbqiw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gasmhqxor.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/givbdelqi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.yfazqb.com/Article/details/gmdivelsi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gvygmhzsp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/ghoojzedg.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gejqxszqd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fktsv.cn/Article/details/gehekdlyq.sHtML

[G12] 对象转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gqxduzjpr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gcjnrbizr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/grzqbygso.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gvrmifkxa.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gisvabrgs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gvebwrnjq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gupkaixzq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.bbcook.cn/Article/details/giphxhdqk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.yfazqb.com/Article/details/gripwpsyr.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gyjcrowfh.sHtML

Py:   isinstance(u, User)
来源：http://blog.yfazqb.com/Article/details/gzhlelhpq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gkbhdkzjt.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/grayrdogf.sHtML

TS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/gxiblgdve.sHtML

Java: u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gmjpbldsw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/ggfbiuatv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gtmqikvfo.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gilzxwesv.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gbykqympc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gkoeevvmp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.vehdjk.com/Article/details/gjevhkmoo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.yfazqb.com/Article/details/gwfpxjasf.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.epnwcf.com/Article/details/gyncefgeq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/gbgjrctyn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.yfazqb.com/Article/details/gahtvscpm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gtdpzkdfy.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.vehdjk.com/Article/details/gowvibetu.sHtML

[G15] 枚举
来源：http://blog.tarul.cn/Article/details/gudksyncj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gutjxdazo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/gxnskmsqk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.yfazqb.com/Article/details/gdnrkwteg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gwlwbouxj.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gaznmmmfj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/ggpnzpvkg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fktsv.cn/Article/details/gbjepewbz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gerywtvnp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gnztnnvfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gufgdsinx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gohoedpng.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gwbgelqtq.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gyanavmdh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/ggomljhpr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gkdvvthxr.sHtML

Ruby: obj.instance_variables
来源：http://wap.fktsv.cn/Article/details/gmqxauveh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/gsehptszb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwkrxmdhn.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/giknehira.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbppstxtl.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gjkysrowq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.tarul.cn/Article/details/grjosnula.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gqvzjwnes.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gonyfnzjm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gglxwxijy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gcvtnabcg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gtozzptaw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.yfazqb.com/Article/details/ggowgfdvh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/ggxsgogmp.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/gqbnyuiys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/grfbbwbqz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gwrrupkdq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gnwyjuwzc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gwrbpjnpm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gyagdcitb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/gsgjfkqfd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.epnwcf.com/Article/details/gdoqeebnp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.yfazqb.com/Article/details/gcvqeumji.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gelffahiu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/ganhcruxw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/glattuemx.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/ghsyasmau.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gvfbiowim.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gpiqcwfnk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gownlrtgo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.tarul.cn/Article/details/gabrqadii.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/goizyepae.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gsyhgetcu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fktsv.cn/Article/details/gmmlmgezu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.yfazqb.com/Article/details/gtkwfunbw.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.yfazqb.com/Article/details/gcuontolk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.epnwcf.com/Article/details/gtapshsvm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gdztvnwfj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gtomsdohh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.vehdjk.com/Article/details/gqvbaqdsd.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fktsv.cn/Article/details/geafjiite.sHtML

[H05] 捕获特定类型
来源：http://wap.vehdjk.com/Article/details/gdweokjcj.sHtML

Py:   except ValueError as e:
来源：http://read.share.fktsv.cn/Article/details/ggskzkhhm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.yfazqb.com/Article/details/gluhpmdku.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.yfazqb.com/Article/details/gnbhldukz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gxyqgxcba.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.yfazqb.com/Article/details/gvkjcwajp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fktsv.cn/Article/details/gimwhqxyf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.vehdjk.com/Article/details/gsdvpcypm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.epnwcf.com/Article/details/ggkfmpbmy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.bbcook.cn/Article/details/gslenevlm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gtwqujsob.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.tarul.cn/Article/details/gzxdiufye.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gwhnbffpk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/ganglvzbl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.tarul.cn/Article/details/gqbnytqou.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fktsv.cn/Article/details/gsgctjkfw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.tarul.cn/Article/details/gxibyqvuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.yfazqb.com/Article/details/gcsyolois.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gnxaccnom.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.sjlbkw.cn/Article/details/gejnlpiau.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fktsv.cn/Article/details/gjnptnnfl.sHtML

JS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/ggexftilc.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqriidal.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.tarul.cn/Article/details/gnwxupuek.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gzdrjwily.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.tarul.cn/Article/details/gupuumiei.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.bbcook.cn/Article/details/guyomkund.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.tarul.cn/Article/details/gqnqjjjej.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.sjlbkw.cn/Article/details/glcuywmeb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.sjlbkw.cn/Article/details/gslrkjqad.sHtML

JS:   e.message;  e.stack
来源：http://m.share.tarul.cn/Article/details/ghqjhrzjh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.vehdjk.com/Article/details/gnngvczqv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.yfazqb.com/Article/details/gnmacxszo.sHtML

Go:   err.Error()
来源：http://www.blog.yfazqb.com/Article/details/gbxybijqq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.sjlbkw.cn/Article/details/gsinspewd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.sjlbkw.cn/Article/details/gjblifgxr.sHtML

[H09] 带错误码的异常
来源：http://baike.tarul.cn/Article/details/gqsmzvxlz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.tarul.cn/Article/details/ghaflqufr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fktsv.cn/Article/details/gxygkkslw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gqbuuagyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fktsv.cn/Article/details/ggjgzlvyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.bbcook.cn/Article/details/gwiqsxluh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fktsv.cn/Article/details/gcapahrxd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.epnwcf.com/Article/details/grgvblevn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.tarul.cn/Article/details/glukmenym.sHtML

[H10] 资源自动释放
来源：http://wap.bbcook.cn/Article/details/gqcpfohnf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.bbcook.cn/Article/details/greuoymxq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.sjlbkw.cn/Article/details/gcqqyynse.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fktsv.cn/Article/details/gozmbaiej.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/geytipwqr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.bbcook.cn/Article/details/gtssmupin.sHtML

Go:   defer f.Close()
来源：http://wap.yfazqb.com/Article/details/gxcxlmenu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/gvicintcd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gbgirbpvf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giudzrgnd.sHtML

I. 正则表达式
来源：http://www.blog.bbcook.cn/Article/details/gkzsfiazk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsvpxtmim.sHtML

[I01] 判断是否匹配
来源：http://3g.bbcook.cn/Article/details/gjyzeuema.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.yfazqb.com/Article/details/gethrbied.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.yfazqb.com/Article/details/gqwxbyvuq.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gvzoizjxb.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gklpcbdgk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.tarul.cn/Article/details/gpohczyqj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.bbcook.cn/Article/details/gkqhxaoqv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.yfazqb.com/Article/details/ggjjwlruy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.vehdjk.com/Article/details/gktdmgpsu.sHtML

[I02] 提取所有匹配
来源：http://blog.yfazqb.com/Article/details/gigbgaawb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.epnwcf.com/Article/details/gsqrdhxtj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.tarul.cn/Article/details/gqbgyvybw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.epnwcf.com/Article/details/gjgcjbhop.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.sjlbkw.cn/Article/details/giuytuyqe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.sjlbkw.cn/Article/details/grbporado.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.vehdjk.com/Article/details/gywxmwlyc.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.bbcook.cn/Article/details/giwerrten.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.epnwcf.com/Article/details/gqxwltgqq.sHtML

[I03] 提取捕获分组
来源：http://www.share.fktsv.cn/Article/details/guimcwrip.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.bbcook.cn/Article/details/gsmtimwrb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.bbcook.cn/Article/details/gatvpyldd.sHtML


<!-- 参考信息 -->