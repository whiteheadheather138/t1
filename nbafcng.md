代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/gvxdxsull.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gqywuydee.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gqxmlzetc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gotemimtv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/gsaehjrhl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gnwsipiww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/genypptqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gesijfhff.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gvndfqrhc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gfgspngbn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gjxdynhfj.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/ghgjeeeal.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/gsudyyfpz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/grducvfiw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gdlzrooui.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gkyoxajan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gijflyadu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fktsv.cn/Article/details/gxytpierj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gssrkiepv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/ggfnwzqys.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gqymiwpmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/glemnzmze.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gupgtuczx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gsevxuixw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gkodvapqo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gzihtejvz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/guiekogzm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxplsytia.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghiecxccx.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gzfwthbii.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/ginozdpas.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grmabhymg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjdzjppoj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gljsulohb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gzwegvkzp.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gycqndtnb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gudlyszes.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/glvvntjak.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/gtfazijdq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gdwooeyng.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gnmojtapc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gylgcipel.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gyqcjsamj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/gcgdtbcfk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gvbtsodgp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gwthfwvlc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gwhoqgjdq.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gtvkraclt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gbxflkxee.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gvginxtkl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gsfbfjfmr.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/ghsefujuw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gaxecspcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gmwnqpddd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gmvlsdjeb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/glnesdisd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.bbcook.cn/Article/details/gecvvtccr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/ghvxycksc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gnpcablpv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gcjqvipsj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/gmtifqggl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gfbfqrpff.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gemqsizoi.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxokgukou.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.tarul.cn/Article/details/gbwniegic.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gfzzuslcb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gbngndgjc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gofovrwpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gjishjwqv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcrwbpiyl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gzyrvdpaz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsdkuoeil.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/glcildtwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/ghnomlmha.sHtML

[F11] 复制与移动文件
来源：http://read.share.tarul.cn/Article/details/gmyicuksu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/geqadikfr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/grilzkwdl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gjwzrkkeu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcmlmijqs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gwlyrrodj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gwtcvthlk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gpgcydfpa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gokqnqmud.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gszqprvyr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/ggwifftdg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gevexkxgv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gpjwwzovb.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gpxqntuts.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/guwhvgavb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gaocvnkgd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/guuyzytxq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/ggymjzygg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gljcfsisg.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gkyivqdin.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjumhdnok.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gdspzwjwl.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrvfrtwd.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/gzapmpblb.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gywgnbhvh.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gbissbewq.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gnbakjryu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.bbcook.cn/Article/details/gpmdqkruh.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/gwjtekqgg.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gmepojzuj.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gnhtmcdru.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gaxemaybc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gswcbgqvc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gldviwwmx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.yfazqb.com/Article/details/gcpzmpvmo.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnrxmsxtt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.tarul.cn/Article/details/gsiagonag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gpiqsolhx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gbobvygzp.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gvpzqkmwx.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/gghebswgq.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gjbfylogu.sHtML

JS:   this.name = "x";
来源：http://wap.epnwcf.com/Article/details/gfvtjrqao.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gztjhputr.sHtML

Java: private String name;
来源：http://3g.sjlbkw.cn/Article/details/gxdgirltx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.yfazqb.com/Article/details/gnjdpynfl.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gdpuwdriw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/gtaxnfnpz.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gesaxkzpt.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gposyztxk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvoyzsaeu.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gzdpgyoou.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gdvfxmvof.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gzowxbdym.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gfbezawdi.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/grvdjjgvi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gstudcvco.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/guabikfio.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gqbuzdnmx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/ghkeeikve.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gaiccunna.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcpimmdma.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/glhmmbbpf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gmktjfede.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gxyctdgqu.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gbphzytrc.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gyutsznvy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gyjbpjerp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gfsrdnxiz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gwfgoswzo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gjzpbevkf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gbsdkpajc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/guvtnwxjk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gtdegoiak.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/ghzootlwt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmsnagpb.sHtML

Py:   super().greet()
来源：http://read.share.tarul.cn/Article/details/gfinjhqtq.sHtML

PHP:  parent::greet();
来源：http://baike.tarul.cn/Article/details/gobwvsujc.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gqligumae.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gtxaralhi.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/gocmmkzss.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/grmqeyycv.sHtML

Ruby: super
来源：http://mobile.epnwcf.com/Article/details/gsfwlzolp.sHtML

C#:   base.Greet();
来源：http://blog.yfazqb.com/Article/details/gjykjvgqg.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/gcvajnrav.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/gzcjwkkrx.sHtML

PHP:  public static function f() {}
来源：http://wap.epnwcf.com/Article/details/gcasxaeci.sHtML

JS:   static f() {}
来源：http://www.blog.fktsv.cn/Article/details/gidixykea.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gbicoqlfs.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gxwltatqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/ghfbzcatz.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gqmmlkhue.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/glhcykrcs.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gfuhiyrvp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gozzuxcjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.yfazqb.com/Article/details/gdwqzvfso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gekqbqjsl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gozpwqgrr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gltmifjzu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.tarul.cn/Article/details/goiguhgsz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gpblcfinb.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/gubckqhuf.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/geiydguwx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/gqqzomzfb.sHtML

PHP:  public / protected / private
来源：http://mobile.fktsv.cn/Article/details/glympakpt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/gghrwfnzc.sHtML

TS:   public / protected / private
来源：http://baike.epnwcf.com/Article/details/geoggjdxi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.bbcook.cn/Article/details/gtvfvqqvh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.tarul.cn/Article/details/gyvixtijm.sHtML

Ruby: public / protected / private
来源：http://wap.fktsv.cn/Article/details/gwhljehwr.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/grupyrwao.sHtML

[G11] getter / setter
来源：http://baike.tarul.cn/Article/details/ggkjxyqrt.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.bbcook.cn/Article/details/gtnykuksz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqdwttiwo.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.vehdjk.com/Article/details/gvlsgnvqc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gvknvwdlj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gsjwfrwpy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gesbjfeqc.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gilqmqwim.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gdyajdmiy.sHtML

[G12] 对象转字符串
来源：http://blog.vehdjk.com/Article/details/gwenotcst.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gudtgrsff.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gqhxjavac.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/glheaeohs.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/geedvcqwu.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gujwbuonb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gzmmiskal.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gvkgdgdiy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gaqiyjfwg.sHtML

[G13] 判断对象类型
来源：http://read.share.epnwcf.com/Article/details/gxhgbmate.sHtML

Py:   isinstance(u, User)
来源：http://wap.bbcook.cn/Article/details/gnhymurfm.sHtML

PHP:  $u instanceof User
来源：http://3g.yfazqb.com/Article/details/gqfvkorlr.sHtML

JS:   u instanceof User
来源：http://blog.tarul.cn/Article/details/gbcqzdrwa.sHtML

TS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gcgmprssv.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gnfbrfspc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtufupds.sHtML

Ruby: u.is_a?(User)
来源：http://blog.epnwcf.com/Article/details/goudcsyee.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gzpqvxdmw.sHtML

[G14] 数据类 / record
来源：http://www.blog.epnwcf.com/Article/details/gomuqcqym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gbipvtphi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.bbcook.cn/Article/details/gujfyxaqu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gdxxbnude.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/ghhrgnqbc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gkcemgyrd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.tarul.cn/Article/details/gzgqclwpm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.sjlbkw.cn/Article/details/gbbxjgyra.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gdrfssruv.sHtML

[G15] 枚举
来源：http://www.blog.sjlbkw.cn/Article/details/ggfssndkh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gseasorpj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.bbcook.cn/Article/details/gwrmtvzyt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gieblttly.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gfzzotdyj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.tarul.cn/Article/details/glgfgvfti.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fktsv.cn/Article/details/goxjiirav.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.yfazqb.com/Article/details/ghpzfquup.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/grfckjhru.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.yfazqb.com/Article/details/gppblbjbr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gqamcgeez.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/gbtxgqezp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gxlpwhjrq.sHtML

TS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gattarznz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.vehdjk.com/Article/details/gvkmjlqet.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/gpqguqtat.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gpgfioejv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gxfiomeob.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsscbfxau.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gixrjcwbp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkcudmors.sHtML

[H01] try / catch 基础
来源：http://www.share.vehdjk.com/Article/details/gzqgftwsr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.vehdjk.com/Article/details/gzpqvwmwk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/gphtlarma.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gflbckrkr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/guuvwpiuq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.yfazqb.com/Article/details/gfoectmee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.yfazqb.com/Article/details/gceocqfuz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.tarul.cn/Article/details/gffkcoona.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fktsv.cn/Article/details/ghzufkkyt.sHtML

[H02] finally / ensure 收尾
来源：http://wap.yfazqb.com/Article/details/gfwzcbdsf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.bbcook.cn/Article/details/gulpbyyeq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gaiptqvht.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gnzdkodlx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gsudbanan.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gbpbkwags.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/gheqogzau.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fktsv.cn/Article/details/gsdpqwqhd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gvwqjftti.sHtML

[H03] 主动抛出异常
来源：http://baike.tarul.cn/Article/details/gxpotgjss.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.epnwcf.com/Article/details/gwsbglcal.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gnlcgxetx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gasvhnqtd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gnrtokdqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gtdsxsfcc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gxiykawqn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.yfazqb.com/Article/details/gxodzlzgk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/grbwknsbt.sHtML

[H04] 自定义异常类型
来源：http://mobile.epnwcf.com/Article/details/glctbotjg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.sjlbkw.cn/Article/details/gehcmxrzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gooqucwuc.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gwdsxzhdp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.vehdjk.com/Article/details/garjbfvyd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gnurspgqj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.epnwcf.com/Article/details/gnawcvavk.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.yfazqb.com/Article/details/gyasiptwh.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggarbcoin.sHtML

[H05] 捕获特定类型
来源：http://read.share.bbcook.cn/Article/details/ghmrilmbp.sHtML

Py:   except ValueError as e:
来源：http://read.share.vehdjk.com/Article/details/gicrkftwg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.vehdjk.com/Article/details/gqjnyhtow.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/ghoippati.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gewpyzsmy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.yfazqb.com/Article/details/gffqrbnwa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gtnajzfln.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.epnwcf.com/Article/details/ghzbboruo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fktsv.cn/Article/details/gfcrpgwnv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gxdhylhhx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.epnwcf.com/Article/details/gtkubitgg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gydyliqoj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.bbcook.cn/Article/details/getqkddpw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfbpjlnn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/gkcwudouu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.bbcook.cn/Article/details/ggbwddscr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.bbcook.cn/Article/details/gxcbhbzos.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.yfazqb.com/Article/details/gpextflri.sHtML

[H07] 断言
来源：http://read.share.bbcook.cn/Article/details/gfuxfdghq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.tarul.cn/Article/details/gfhwcimhs.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.epnwcf.com/Article/details/gnymavkrn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.epnwcf.com/Article/details/gdyqxdqsl.sHtML


<!-- 参考信息 -->