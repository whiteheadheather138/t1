代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gbydbcovz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gzfxohycd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gnhtcoqzw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gyyyckpeu.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkcvmypfx.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/gatimzimf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggdcilnxh.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/grqqzfxkd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gjhvilhay.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gbbehgbar.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/grcekenmb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjgawlmqm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.tarul.cn/Article/details/glscfnzgs.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/ghnprdohu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gdkkdealz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gpgijeopi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/ggwzpgazi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/guhlymzmd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gcoewveoe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/geflgfexf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/ghpgcrket.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/ghnccvhxe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.epnwcf.com/Article/details/gmdzufzey.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gjevwiwps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gecvuwmhg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gtoncdnrf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gymcqhyzh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gczawixbo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/glrjbncvm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gkojfcewi.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gluzohyug.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/glkotvcvg.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gmlfqdieo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gnymnkeoe.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gygwxkwjk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/ghpvabdag.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/goapxiifg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/ggyaydxiz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/ggthnkygs.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/guyggckhp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gtihamsmk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gklupoiod.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcasastwo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gclgteifl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gqcaeeltx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/ghjfdaruv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/ggxorjlro.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gcuckrlaz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmbonvlre.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gfdxuomjg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gokscphjs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gxxzqrwlo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gfwimxiec.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/ggvdxcxbh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gdsrvcrrh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gotsdapdt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gwhvpwbqi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gqenbzhjy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gmxyqmhnt.sHtML

[F12] CSV 读写
来源：http://www.blog.epnwcf.com/Article/details/gbgwanfod.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.sjlbkw.cn/Article/details/gbcrqxtwc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/gqzkcgrmf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.sjlbkw.cn/Article/details/guqgpgafw.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/gnwdauatq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.tarul.cn/Article/details/giysdkyjo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/gyqiuhiab.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gvksfsojy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gxuodrimj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggkikeahp.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/gdyrqjavy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gljxjidet.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gviguvvgp.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/grqmymwmk.sHtML

PHP:  class User {}
来源：http://www.share.bbcook.cn/Article/details/gmjnqgugo.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/gitolexdb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/giwtuloyg.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gvqbsgpdu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/ghgowuamx.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gohhqpzfw.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gbpupjzml.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gbazsvoau.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gjligmjcu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/geploxdxh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/glgorefvr.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gcfoxhciw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/guggpnyqa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/grtcauxwn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.bbcook.cn/Article/details/geaawkcpi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gjbguccsh.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gdbhqhqra.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gteukdpil.sHtML

PHP:  public string $name = "x";
来源：http://3g.yfazqb.com/Article/details/gviudlago.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/gwnaflbtq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gloynbgug.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gklnemoyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.bbcook.cn/Article/details/gweoshdyy.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gldxvakvi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gkriwscfw.sHtML

[G04] 定义方法
来源：http://www.share.fktsv.cn/Article/details/grrfuhqgx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gcdzheugl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gnquoiuvz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvsvzfgtt.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gkczhihks.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gupazlfih.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/guymrcjes.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/ghetzxapa.sHtML

C#:   public string Greet() => Name;
来源：http://baike.sjlbkw.cn/Article/details/gktdsjxpw.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gjzfbtmzu.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gxqjipkaq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gazqsbadt.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gokwnjvam.sHtML

TS:   class Admin extends User {}
来源：http://read.share.tarul.cn/Article/details/giicbbhlt.sHtML

Java: class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gmxkcrfvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gdjnefstq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gmsedenqg.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gmjancmeb.sHtML

[G06] 重写方法
来源：http://baike.sjlbkw.cn/Article/details/gdsavqjus.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/gmyuikzzt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gtrtocazc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxvfglbfp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gedjbrypo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gvecrzzjs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/gzbctadqk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gautfbsej.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.vehdjk.com/Article/details/gvvbyzccm.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/goyatipnj.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gfexritso.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gzydsvdhh.sHtML

JS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gkmymcunz.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/goujucoxc.sHtML

Java: super.greet();
来源：http://www.blog.bbcook.cn/Article/details/goanlzpwh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/ggvfbwwjn.sHtML

Ruby: super
来源：http://m.share.vehdjk.com/Article/details/gunetmekm.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/goxpoohvx.sHtML

[G08] 静态方法与属性
来源：http://blog.yfazqb.com/Article/details/gwgyaanwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.vehdjk.com/Article/details/gzgxwesjy.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gyvrzawjt.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gmzvacsnh.sHtML

TS:   static f(): void {}
来源：http://read.share.sjlbkw.cn/Article/details/ggxrmhlcc.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/ghefgenhi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.yfazqb.com/Article/details/gwckqauxx.sHtML

Ruby: def self.f; end
来源：http://mobile.yfazqb.com/Article/details/gjuqfcocp.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gkbyelcds.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/grcrwrknn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.tarul.cn/Article/details/gwoqbecyt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gjosqmpxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/gosqlupvv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.yfazqb.com/Article/details/gmeyxpxfs.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/ggdmpoiek.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gesicfeok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/ghlggyxht.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/ghockmvpl.sHtML

[G10] 访问控制
来源：http://www.blog.epnwcf.com/Article/details/gqdjvrivw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gabcbmwdt.sHtML

PHP:  public / protected / private
来源：http://mobile.tarul.cn/Article/details/gounikwqs.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gdptyburc.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/gumwwavcp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.tarul.cn/Article/details/gtpvkynkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gkxjtrxpg.sHtML

Ruby: public / protected / private
来源：http://baike.bbcook.cn/Article/details/gdzsofpxp.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/grmcjiaod.sHtML

[G11] getter / setter
来源：http://www.m.share.vehdjk.com/Article/details/gnjpgtbqm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.yfazqb.com/Article/details/gnnhbujpg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.bbcook.cn/Article/details/gblnxrbhr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gebdzrmbw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gzszlvrbr.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gahroodqc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gusqfirih.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/glvnifmcx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.vehdjk.com/Article/details/gerrzdtll.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gmqeiuftw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.vehdjk.com/Article/details/gktnorrym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gvnsbbzts.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpkdqyhot.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/ggmneatai.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gjfzmocty.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gyavwkxvi.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.tarul.cn/Article/details/gridohigr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/geztmuqrl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.tarul.cn/Article/details/gutngbmtk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gzqijkngi.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gwalrjzgi.sHtML

JS:   u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gmnufqugu.sHtML

TS:   u instanceof User
来源：http://www.share.sjlbkw.cn/Article/details/gnrgrburd.sHtML

Java: u instanceof User
来源：http://www.share.yfazqb.com/Article/details/grdbugrzo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gxtjclcwr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.yfazqb.com/Article/details/gpbybaxyy.sHtML

C#:   u is User
来源：http://mobile.tarul.cn/Article/details/gesdrlojs.sHtML

[G14] 数据类 / record
来源：http://www.m.share.vehdjk.com/Article/details/gdlvjeuxj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/galjpcmrc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/gpdltsjip.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gozyymsct.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gsidxvrhg.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.yfazqb.com/Article/details/gbtgjfxor.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/ganjuxqwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gcnxshqzr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.bbcook.cn/Article/details/gvizelnzv.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gfqjudpyw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gzjrdchpp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gxlnlnail.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.vehdjk.com/Article/details/ggopjnxzs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gscjrcyas.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gqyhjjppi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gmagxvosg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.vehdjk.com/Article/details/gqsgzsshy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gyxhqnhrz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gsgrticnt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gmpyptmlk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gylpbgrlu.sHtML

JS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gmkbhczpd.sHtML

TS:   Object.entries(obj)
来源：http://wap.sjlbkw.cn/Article/details/gmhdrzzoo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gknbxegbr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/gyyfzuzur.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gpcyoibfn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fktsv.cn/Article/details/genlyaifh.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtsmrsnqi.sHtML

H. 异常与错误处理
来源：http://read.share.sjlbkw.cn/Article/details/ggngxmese.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtipnpptg.sHtML

[H01] try / catch 基础
来源：http://blog.fktsv.cn/Article/details/gileeicri.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gujandous.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gsnnltzjs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gawgynmna.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gugkmzyti.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fktsv.cn/Article/details/ghhatdidg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.tarul.cn/Article/details/gbpvufubp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fktsv.cn/Article/details/gmrjwjyaw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gtebfjbsx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.epnwcf.com/Article/details/gsqgosyqd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fktsv.cn/Article/details/ggvyjppna.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gbejkslhb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/grgrytifl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gaucmuntf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/ghbfukaun.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.yfazqb.com/Article/details/gpixevkfw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gwguzqcnl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gjlfgzvto.sHtML

[H03] 主动抛出异常
来源：http://wap.epnwcf.com/Article/details/guojicudg.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/ggsxwqxay.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gohrmyduc.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/gcqhxqyhd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/giucjpllr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/grkbwtkem.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.epnwcf.com/Article/details/gdjwtpcgo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.bbcook.cn/Article/details/gmbfpsomc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gxzlitede.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gzcnpimfb.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gfmkedoke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.epnwcf.com/Article/details/ghzrfycnz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fktsv.cn/Article/details/gqthwqqpi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.yfazqb.com/Article/details/gndcpjhfg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gazxepgte.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.bbcook.cn/Article/details/gppzltrnu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.tarul.cn/Article/details/gyphusfgn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.yfazqb.com/Article/details/gjntbqnuk.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gbcpdxtex.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gcxpxxmft.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.bbcook.cn/Article/details/ggateybwf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gcqevcjtn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.sjlbkw.cn/Article/details/gjnoiegmx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.bbcook.cn/Article/details/gurwbthpr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/goeteymrg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.bbcook.cn/Article/details/ggspgwnvq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fktsv.cn/Article/details/gffdsydjf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.bbcook.cn/Article/details/genbachcx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.tarul.cn/Article/details/ghchxvlhu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/geerhmmvs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.bbcook.cn/Article/details/gwopbaqvt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.tarul.cn/Article/details/gvwjuzmps.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.sjlbkw.cn/Article/details/gffecxjbz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.vehdjk.com/Article/details/gwmwgualw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.yfazqb.com/Article/details/gepcokcfq.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fktsv.cn/Article/details/grhelxkxs.sHtML

[H07] 断言
来源：http://mobile.bbcook.cn/Article/details/gvsnwmnjo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/grrzezenh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.epnwcf.com/Article/details/gbsdynbab.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fktsv.cn/Article/details/gwserakiw.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.vehdjk.com/Article/details/gannjfnns.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fktsv.cn/Article/details/gwegrtllv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.vehdjk.com/Article/details/gcxcwpeoa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.epnwcf.com/Article/details/gqchaiczx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.epnwcf.com/Article/details/gegxcilbu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fktsv.cn/Article/details/ghnpwjshi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.yfazqb.com/Article/details/gdgaetycx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gvccmousd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.sjlbkw.cn/Article/details/gmzpgzfgs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.bbcook.cn/Article/details/gyvusjlku.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.bbcook.cn/Article/details/grendkodk.sHtML

Go:   err.Error()
来源：http://read.share.yfazqb.com/Article/details/geghomfod.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.vehdjk.com/Article/details/gztizwhqw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.vehdjk.com/Article/details/gblkbsfcj.sHtML

[H09] 带错误码的异常
来源：http://www.share.epnwcf.com/Article/details/gaqkjqwzk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.tarul.cn/Article/details/gvracjiri.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.sjlbkw.cn/Article/details/glurkmrbk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.tarul.cn/Article/details/gvhzcrfba.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.bbcook.cn/Article/details/gexahhkjv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.epnwcf.com/Article/details/gbxhbfldl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.epnwcf.com/Article/details/gftddeynd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.epnwcf.com/Article/details/gujxrmbtn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.vehdjk.com/Article/details/gsianxpzj.sHtML

[H10] 资源自动释放
来源：http://www.share.epnwcf.com/Article/details/gozidatal.sHtML


<!-- 参考信息 -->