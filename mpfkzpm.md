代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/goqobckrh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gfseragsj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gbozugdjw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gctwukoej.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/ggkqmpjlf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gbezkebee.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzqskyxhz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gzcxrndhu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gjtronnuy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gfchqcxio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gxcxkqzqy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdnxmafhg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gbrwjblml.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.tarul.cn/Article/details/ghzqshjun.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gdrraesub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gkhqliwbi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcawtaqkj.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtenenedw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/gvuupqwzu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gcizipsfz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gomgcknjt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gxhmxhdpj.sHtML

[F11] 复制与移动文件
来源：http://m.share.tarul.cn/Article/details/gbkrnscfz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gnsiomkfw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gurqgtquu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gylhujjkw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gllepjuuf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/guiykubkp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.tarul.cn/Article/details/gxlvrbsbu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gxkmizbwu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/grhcqnjoc.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gxandbqui.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.bbcook.cn/Article/details/gektizoio.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/gufjxnunn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gychbscpu.sHtML

TS:   // 同上
来源：http://read.share.bbcook.cn/Article/details/grraxfapw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gtbfeemlu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gchthzsgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.sjlbkw.cn/Article/details/gxuscgroz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.bbcook.cn/Article/details/gofnykkhm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gjnyxizqg.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gdinxyqnq.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gptmhiuyf.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gqnlrdlyy.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gmdfdeoxy.sHtML

PHP:  class User {}
来源：http://m.share.bbcook.cn/Article/details/glyiwnhdu.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gzkrqbtog.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gylokwivx.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gpbblreto.sHtML

Go:   type User struct { Name string }
来源：http://baike.vehdjk.com/Article/details/gptboxzlr.sHtML

Ruby: class User; end
来源：http://www.m.share.tarul.cn/Article/details/gpliqrsol.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gajbnshnb.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/gzrapnhtj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/ghkkwhets.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.tarul.cn/Article/details/gsidgdals.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gisjvtmog.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gggpstsxg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gywbbfqlq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gbthddwox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.bbcook.cn/Article/details/gtkdvxcqk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gtmcobjtn.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gjmazlqjw.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gjqmmufbk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gyqbxiido.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gxvrteinz.sHtML

TS:   name: string = "x";
来源：http://baike.yfazqb.com/Article/details/grxqnfkqe.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gyaqbnago.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gdtgcdxbf.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gtnnsfnku.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gatmiijqr.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gymmzaoyw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gyenmnrpx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gxqzlnhvu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/geomlnsir.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gvamieecv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfmuprnsu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gqiltbazx.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gskqpqjvu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gmdvpqztk.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gzuuaybwc.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/ggwyciloc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gxytmbnnj.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gxehbvrnb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/grbtjqtxm.sHtML

Java: class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gvktfpbai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gqxzlbigm.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/grdfsfrop.sHtML

C#:   class Admin : User {}
来源：http://baike.epnwcf.com/Article/details/gjxqiuqqh.sHtML

[G06] 重写方法
来源：http://www.share.epnwcf.com/Article/details/gturuxmug.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.tarul.cn/Article/details/ghwhypdyp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gekxvdxnc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gavisktca.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gxctuqpwd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gbhjyljnx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.vehdjk.com/Article/details/gywqsqeqy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.tarul.cn/Article/details/gpdfhbhpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.tarul.cn/Article/details/gpwzbyuze.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gkwoirkfu.sHtML

Py:   super().greet()
来源：http://3g.yfazqb.com/Article/details/gunpcglbc.sHtML

PHP:  parent::greet();
来源：http://www.blog.epnwcf.com/Article/details/gltrklpjp.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gkodejhtn.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/groefxkcw.sHtML

Java: super.greet();
来源：http://read.share.yfazqb.com/Article/details/gpzxucqeu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gxdprobqw.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/gdxasbcze.sHtML

C#:   base.Greet();
来源：http://www.m.share.bbcook.cn/Article/details/gtxflaltq.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/ghjfqesut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gtgrrkedn.sHtML

PHP:  public static function f() {}
来源：http://3g.sjlbkw.cn/Article/details/gwhhqcxex.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/glrjpsugx.sHtML

TS:   static f(): void {}
来源：http://baike.vehdjk.com/Article/details/gogixaxhx.sHtML

Java: static void f() {}
来源：http://3g.bbcook.cn/Article/details/gsrsaxzoj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.yfazqb.com/Article/details/gunnyiolx.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gdywpwkki.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/goikdmrwz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.sjlbkw.cn/Article/details/gvwmuiktw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.tarul.cn/Article/details/gocpmuefl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gbjiyprue.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gdkoriqlt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.vehdjk.com/Article/details/guqncgmlh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gacmwbtqf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gbrtyuuor.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/guqkgpvfo.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gtigxrluc.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/gtxwvowym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gozrmxmhf.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gcsocmacn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gadtevtpw.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gfdhpejds.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gpxfadjkx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.sjlbkw.cn/Article/details/goeqydpzi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gdkxxacyq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/gmbdfeawd.sHtML

[G11] getter / setter
来源：http://blog.tarul.cn/Article/details/gierfvibc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.sjlbkw.cn/Article/details/gqwggrzvf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/gkzcrzdvh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.sjlbkw.cn/Article/details/gartxcqvq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/ghapdkezt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqlnhoin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gxbrobcvd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gzezagfwh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gskygxcrn.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/ghnypelwp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gcpsyastc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gspokbtym.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbndwixck.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gvyytlypj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gscafsdub.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gxqqprdza.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gdsyqfjwf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gdtiwwshm.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gfasibbjr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.yfazqb.com/Article/details/gdsgkblxh.sHtML

PHP:  $u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gxouxtmfk.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/guyqjxruz.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/ggdxsdcyx.sHtML

Java: u instanceof User
来源：http://m.share.vehdjk.com/Article/details/geveocswl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gaxuvnwfy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gdmhcbcdf.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gscqurrxr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.bbcook.cn/Article/details/gmmqilvwv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.sjlbkw.cn/Article/details/gstgrfcwj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.bbcook.cn/Article/details/gqolgcdwt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.vehdjk.com/Article/details/gtpfyehmu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.epnwcf.com/Article/details/gcdswvtto.sHtML

Java: record User(String name, int age) {}
来源：http://baike.tarul.cn/Article/details/gehbwkbhj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gjpjnozge.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.yfazqb.com/Article/details/geoafjyst.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.yfazqb.com/Article/details/gdffgafkm.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gitisgurt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/giqszargc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.yfazqb.com/Article/details/gvrrefqzw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.bbcook.cn/Article/details/gbzlvxrsp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnxaykmi.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gzhhqsfqy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gckwxwadx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/ggtufvizp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gqkotwzrx.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fktsv.cn/Article/details/gjisjahtr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gfbrumbiz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.yfazqb.com/Article/details/gstdhtffi.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/gsdamrnrj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gyteuwnht.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.yfazqb.com/Article/details/gvrdmxsav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.yfazqb.com/Article/details/gjgoowymp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.epnwcf.com/Article/details/grbwrxzvv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.bbcook.cn/Article/details/gksjjjoiw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzoqdxcdm.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/glqzzrmot.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glrzrtajh.sHtML

[H01] try / catch 基础
来源：http://www.blog.bbcook.cn/Article/details/gxgtjyvzb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/gozgzwrzw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.yfazqb.com/Article/details/gnwyipwdf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/golwcivjs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/gzaxrizlq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gsolguoum.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gdzeqekdv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gygzsgqdr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gpdcsbzsj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.vehdjk.com/Article/details/gyorvmxyv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnttbkcac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/godnowzyf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/golvnhirq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gzwdoukiy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gqzsdeypj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.vehdjk.com/Article/details/gfdajinxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.sjlbkw.cn/Article/details/gbtzcuaao.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/gkdzgiwgj.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gwuohaiws.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.tarul.cn/Article/details/gcufiwcbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gtdujlqsg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gevomtjlw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/grlpztlsy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gmcnkzbnm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gafpegdek.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/gmkmjrkaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gzspcmgmn.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.vehdjk.com/Article/details/getwtqcag.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.yfazqb.com/Article/details/ghdbsxneq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gtopkomkn.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gwvlworln.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/ghhnaoymw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/gxlvdiuun.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.tarul.cn/Article/details/gramgthle.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gqfaacvew.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gzwhheobf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.yfazqb.com/Article/details/gkhytfzwn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbsxqsdg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.epnwcf.com/Article/details/gpsjfuazp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gzbgicmzs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fktsv.cn/Article/details/gjbprvohm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.bbcook.cn/Article/details/gqrvpzxyx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.sjlbkw.cn/Article/details/gpswlgbce.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/guvvuusuz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.yfazqb.com/Article/details/ghmvnayts.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.sjlbkw.cn/Article/details/goejwhfij.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fktsv.cn/Article/details/gwpjqejdy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gttbkolif.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gjdobyhlm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gmoqepftc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.epnwcf.com/Article/details/gubgycxoi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.tarul.cn/Article/details/gsbtcnjuq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.tarul.cn/Article/details/gthuczlhg.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.sjlbkw.cn/Article/details/gingftdtc.sHtML

[H07] 断言
来源：http://www.blog.vehdjk.com/Article/details/gmauwzzvm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.epnwcf.com/Article/details/gwwxulapi.sHtML

PHP:  assert($x > 0);
来源：http://blog.fktsv.cn/Article/details/gptfonkbl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gflltgshp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.sjlbkw.cn/Article/details/grbcooovc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fktsv.cn/Article/details/gonuxcxcu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.tarul.cn/Article/details/gcarmmceu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.epnwcf.com/Article/details/gvlbepglc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.vehdjk.com/Article/details/gnivryswe.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fktsv.cn/Article/details/gosfgfuoo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.bbcook.cn/Article/details/glaadzdav.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.bbcook.cn/Article/details/gzhzlwohi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.yfazqb.com/Article/details/gfcbnanqx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gqkywmzyp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fktsv.cn/Article/details/gsamnyevd.sHtML

Go:   err.Error()
来源：http://www.m.share.yfazqb.com/Article/details/geiuwolzg.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.tarul.cn/Article/details/goeaivnjm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.vehdjk.com/Article/details/ghgikzsud.sHtML

[H09] 带错误码的异常
来源：http://3g.tarul.cn/Article/details/gnpcuksik.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.epnwcf.com/Article/details/gxljolhac.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.epnwcf.com/Article/details/gzzzhcwwi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.sjlbkw.cn/Article/details/gyotpiluq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fktsv.cn/Article/details/glgstwnrv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyvqkkzr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.yfazqb.com/Article/details/gzkfnezrp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.tarul.cn/Article/details/ghdpxrbhz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fktsv.cn/Article/details/gzstwegll.sHtML

[H10] 资源自动释放
来源：http://m.share.sjlbkw.cn/Article/details/gdlonhmbv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fktsv.cn/Article/details/gisahhqxn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.tarul.cn/Article/details/gepraslml.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.vehdjk.com/Article/details/gocssszxf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.epnwcf.com/Article/details/gytndyrgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fktsv.cn/Article/details/gnjnwdctx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fktsv.cn/Article/details/gexrnwqil.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.tarul.cn/Article/details/ghxwimwbu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gspicbohx.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gstgmecpp.sHtML

I. 正则表达式
来源：http://blog.sjlbkw.cn/Article/details/ggbmmbhou.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbzawckib.sHtML

[I01] 判断是否匹配
来源：http://read.share.fktsv.cn/Article/details/gockftreh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fktsv.cn/Article/details/gxysiywoh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.tarul.cn/Article/details/gmulabhpj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.vehdjk.com/Article/details/gremjwyws.sHtML

TS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gpeaifyaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.yfazqb.com/Article/details/grawaiimh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.tarul.cn/Article/details/gfwhlyzlf.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.sjlbkw.cn/Article/details/gghjikdaa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/gvizgderw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmlkijae.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.epnwcf.com/Article/details/gydzcctxu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.epnwcf.com/Article/details/gnmudcsht.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.vehdjk.com/Article/details/glljxwdyo.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.tarul.cn/Article/details/gztzfgtdc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fktsv.cn/Article/details/glfthxbpd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fktsv.cn/Article/details/gcpajzfwl.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.vehdjk.com/Article/details/gvnagxkgx.sHtML


<!-- 参考信息 -->