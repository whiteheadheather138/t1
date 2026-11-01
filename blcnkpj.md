代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/giggbwyhb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gukavtjah.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gbhispstc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gcvtobevf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/grphmtsbi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gciezgdzv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gevqzgvdc.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gequiuujn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gzjpdvvhj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gxqvsokix.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gykgnpkcn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gbyiudmie.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gwwbjtjuv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gveefhrkr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/gzfazrvmb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gxohngpog.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/ghgjcmakx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/ggtmjvnht.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gmxndhomb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gpavyijxc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gicwyjnji.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gwomolzrh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/guhasnsna.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdagblnzs.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gblumnbsl.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbvodxajv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gzjywpmwn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/goomtwdoo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkbmnyadd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gixyzqfsg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gpioognss.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gvrmaunre.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gyihygppa.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/grzhdjvrn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/ggldzeank.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gbcxraucq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gzdhihxmp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gymeouqgs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gbcptaoye.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gbvbfiver.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gdlulmlou.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gfhefvxkc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gnntpvdjn.sHtML

[F08] 遍历目录
来源：http://www.blog.tarul.cn/Article/details/gjnynecor.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/gtgfbketz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gogwxnrvv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gglyavumf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gujfjyptg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gajzkzcgt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gvqhvropg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.tarul.cn/Article/details/gvclclvju.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gmhqszmxs.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gxhzxhexv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/gnyrhtdwv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/geykrvjgv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.epnwcf.com/Article/details/ggtmomugh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gzaetpgqh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/ghqtcnxpa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/gyqcodfdm.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyodqsgyc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/guavvitgn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gudmzpgjj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gxdtyarxq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmizfchmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gyrmqiyth.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gmellzker.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gksxuuleg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gnqcmaaxp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gihmeqsxi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmdrbruvm.sHtML

[F11] 复制与移动文件
来源：http://read.share.bbcook.cn/Article/details/gvoqxwcea.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjevudviz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gdfuozmkw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gftslindr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/glketnluw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gdtbamwgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.tarul.cn/Article/details/grivihneo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gjxjqvoly.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gbhjqhvwg.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gplockcuz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.yfazqb.com/Article/details/gnwsoshnc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gcaxtkaip.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.epnwcf.com/Article/details/gbhmmeacl.sHtML

TS:   // 同上
来源：http://wap.epnwcf.com/Article/details/gcvmfpoys.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.yfazqb.com/Article/details/gbhyaznbs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gcadjhkeh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gksiegard.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/ggipvtnjv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gysisvtxw.sHtML

G. 面向对象
来源：http://www.share.tarul.cn/Article/details/gbiotumnp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkusyjsje.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gtfqhxuzy.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gauwmrfbo.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gnsskrznm.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gitzmftfe.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fktsv.cn/Article/details/ggrrsmdlx.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gmdczcmje.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gndmrrtql.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gknxwjbzv.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/gbnibubkj.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gfrmldpce.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gokrqrhro.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gruljdtyh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gluuvymhh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gyvboigbr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gdhcvpkda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.epnwcf.com/Article/details/ggntxrcwp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gprzyexme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gjlsiuntl.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gpxsbjrkl.sHtML

Py:   self.name = "x"
来源：http://www.share.bbcook.cn/Article/details/grtqzntwd.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gbuyyatzw.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/grxwldkyj.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gxgeedeww.sHtML

Java: private String name;
来源：http://m.share.tarul.cn/Article/details/gxoceazto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gaqfelxwo.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gpwtxvxmw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gpsjnojdz.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gllbpbyry.sHtML

Py:   def greet(self): return self.name
来源：http://wap.epnwcf.com/Article/details/gnbwqeyrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gfyuioozo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzbkdwfoo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gqibjfsts.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gzkwofnjg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gtompuqpx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gpmmqxdco.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/giwdgcsum.sHtML

[G05] 继承
来源：http://www.blog.bbcook.cn/Article/details/gltepylhp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.sjlbkw.cn/Article/details/gqibybkan.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gswifrigg.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gglmeqliq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gjnfwdkcr.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gcvyvdpvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fktsv.cn/Article/details/gvaviddjq.sHtML

Ruby: class Admin < User; end
来源：http://blog.fktsv.cn/Article/details/gztnyerhp.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gshtpuhbk.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/grffuxxcx.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/guaaeaojn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/glyciekxa.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/girrfoxaj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gzclwpbyk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gigrhxxfy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gnhvkbypp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.tarul.cn/Article/details/grlitfrml.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.bbcook.cn/Article/details/gexlfzgkj.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fktsv.cn/Article/details/gvdvdnuom.sHtML

Py:   super().greet()
来源：http://blog.vehdjk.com/Article/details/gauxydsop.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gjunbytwp.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gafkinjvb.sHtML

TS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gfghwvxea.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gaaiafyym.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.sjlbkw.cn/Article/details/gyazafvcd.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gnypbpvov.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gxkedualy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gcssgpmfp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.yfazqb.com/Article/details/goghywkiz.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/glrinlyix.sHtML

JS:   static f() {}
来源：http://wap.epnwcf.com/Article/details/gvbssplrb.sHtML

TS:   static f(): void {}
来源：http://blog.vehdjk.com/Article/details/gkwuzdadx.sHtML

Java: static void f() {}
来源：http://baike.vehdjk.com/Article/details/gtdkzuotv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.tarul.cn/Article/details/gmonatjnp.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gcybsuipr.sHtML

C#:   public static void F() {}
来源：http://www.share.epnwcf.com/Article/details/gatbhzoob.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gcxrpeiad.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.sjlbkw.cn/Article/details/gpbaqoqsu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.vehdjk.com/Article/details/gvvrbwbdr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gmhjihhbi.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/gqbyzvpxb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.tarul.cn/Article/details/gmihcpdsu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gaeadhxrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/goegmjtgy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/giguzosnu.sHtML

[G10] 访问控制
来源：http://wap.fktsv.cn/Article/details/gpvjcacci.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.bbcook.cn/Article/details/gkqwlmjfp.sHtML

PHP:  public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/ghlshrxmy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.epnwcf.com/Article/details/gfjajypml.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gmuczewww.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gldtbonex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/gnwbgusae.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gjqczgnzp.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.vehdjk.com/Article/details/gyxarhtbq.sHtML

[G11] getter / setter
来源：http://wap.sjlbkw.cn/Article/details/gxebavwfg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.bbcook.cn/Article/details/ganermdku.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/glrjxjduu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.tarul.cn/Article/details/gvtqopukx.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gvhjkkvji.sHtML

Java: public String getName() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gttoshair.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/guppdiajw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/gherzozwc.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/gbhbnveky.sHtML

[G12] 对象转字符串
来源：http://wap.vehdjk.com/Article/details/gkzyuyyfc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.tarul.cn/Article/details/gnggnszei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/grnejypgu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/girunegsl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gdipfxrrj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gowqysesi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gqbusgryf.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.bbcook.cn/Article/details/gcbvjeiqo.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gvwvpewko.sHtML

[G13] 判断对象类型
来源：http://www.share.fktsv.cn/Article/details/gkyglvetd.sHtML

Py:   isinstance(u, User)
来源：http://read.share.bbcook.cn/Article/details/gghjzphnk.sHtML

PHP:  $u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gcapnagsn.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/grymhezma.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gmojsnoie.sHtML

Java: u instanceof User
来源：http://wap.tarul.cn/Article/details/gmqxthzvp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gcqgltqcd.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/gbilctnzv.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gueyvqgyl.sHtML

[G14] 数据类 / record
来源：http://www.blog.yfazqb.com/Article/details/grwbkjcrj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gzpswehko.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gvpeltlbc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.vehdjk.com/Article/details/gixxjstxx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gscpkqkms.sHtML

Java: record User(String name, int age) {}
来源：http://wap.epnwcf.com/Article/details/gyijnlhox.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.tarul.cn/Article/details/gkqbndlbg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gwqgkkmlb.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gifxgndhu.sHtML

[G15] 枚举
来源：http://wap.fktsv.cn/Article/details/gzovxxumq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fktsv.cn/Article/details/ghddmykxw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.yfazqb.com/Article/details/gwtolbsmo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gyfaxydav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gvfzrxnyk.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/grwbvmigf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gkyuhrezx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gsdvhhfvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/ggfbyhvqf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.tarul.cn/Article/details/gmwlkdbsk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.yfazqb.com/Article/details/gxonapieq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fktsv.cn/Article/details/gimckkzhk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/godzxhpng.sHtML

TS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/guhwdgmao.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.yfazqb.com/Article/details/gzoydywxq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gavgwgldk.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gmhgiksno.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fktsv.cn/Article/details/gskxzauvv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbrihecvz.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gvgoaxrjq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqctiriul.sHtML

[H01] try / catch 基础
来源：http://blog.yfazqb.com/Article/details/ggfaczlpt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gyjrqpxpu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtmtscyo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gmclmkxnd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.tarul.cn/Article/details/guhmmmpda.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gcwhefoox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.bbcook.cn/Article/details/gijetumaq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gdemtgzxs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/gxboqrzrv.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gwjdwtchg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gdirtmxxo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gdoixckme.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/giefkohjr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gqwdxzfwd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/guugdadnk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/glazigqed.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfyvrbpg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gilevesrr.sHtML

[H03] 主动抛出异常
来源：http://read.share.epnwcf.com/Article/details/gvsdidymr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gexljxcba.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gsjkozwdz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ghfqumnts.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gnvohpgcf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gpvjkprtq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/gvyvifzst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gebvwjqfl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gnjgjaxeo.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/gtjazonyc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.bbcook.cn/Article/details/gisbiycmb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gpjpbvrxe.sHtML

JS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gzdvzzscq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gjozvhuht.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gaphqwqob.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gpvkbggzh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fktsv.cn/Article/details/goiocxrtl.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.sjlbkw.cn/Article/details/gfvfsozuu.sHtML

[H05] 捕获特定类型
来源：http://baike.bbcook.cn/Article/details/grwdiogrp.sHtML

Py:   except ValueError as e:
来源：http://blog.vehdjk.com/Article/details/geqobbyxz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.yfazqb.com/Article/details/gksucctwc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gmspjpdnd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gclqaoexb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.bbcook.cn/Article/details/ggdwenusg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fktsv.cn/Article/details/gibsxlkrt.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gwrbiqflb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/gkudoyojt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.vehdjk.com/Article/details/gnixrrvta.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gsqdowvpl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gfacjtyhc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.epnwcf.com/Article/details/gaqjkukrl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.sjlbkw.cn/Article/details/gpvnqbchr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.yfazqb.com/Article/details/gyijhltzb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.sjlbkw.cn/Article/details/gkdutbktb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.epnwcf.com/Article/details/gwmmexijc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.epnwcf.com/Article/details/gymegqydq.sHtML

[H07] 断言
来源：http://m.share.tarul.cn/Article/details/gibipgvhr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fktsv.cn/Article/details/gvwwiyfjw.sHtML

PHP:  assert($x > 0);
来源：http://m.share.yfazqb.com/Article/details/gfxlapdzq.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gshimzwvs.sHtML

TS:   console.assert(x > 0);
来源：http://wap.vehdjk.com/Article/details/gktvqgncu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fktsv.cn/Article/details/gnodqqoip.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.yfazqb.com/Article/details/guyxnnbwu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.tarul.cn/Article/details/gyxtmknbf.sHtML


<!-- 参考信息 -->