代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gwxrmlxnr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.vehdjk.com/Article/details/giisuemlg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gibgzqstu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gblzqucgu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.bbcook.cn/Article/details/giobtoalp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gzitfthmu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gyyxxwnrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gzqhbyqze.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gpacydhrj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gxabdxonk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gtwlmoudh.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/ggsjevvsj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/grgodtrcu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gghcqhdbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gzmxsmjjf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/galdosmsd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gdoeqfhmc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gkvehczwg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/gdlqdxbas.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gjvndvvza.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/ggtaswpxy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gmrbftqtp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gkxjamvut.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gmnmkqezj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gblcpbcrn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gqjahpcut.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/gjctnxbam.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzuuxaaci.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtonkpnxx.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gfykshocq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gukxxcqvl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/glmhynfgl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggztnpjnt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gfhojvtkd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gvvnjvdes.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvktbhwlq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/givkqwovd.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fktsv.cn/Article/details/glmevmaxo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.yfazqb.com/Article/details/gqslthaed.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gzdmkfglw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gmnpnspuj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/guyvusddd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gsezrfbhf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gwzdflnnk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/gxysjxzyb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gwxafpdor.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.sjlbkw.cn/Article/details/gnzbcprci.sHtML

[F08] 遍历目录
来源：http://3g.sjlbkw.cn/Article/details/guprjadnl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gqhonqjip.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/givpfsyvz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gljznkygk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.yfazqb.com/Article/details/glbcobfzc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gqrnepktw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.epnwcf.com/Article/details/glfyubfsq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gamwlizqu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gxrqiymka.sHtML

[F09] 获取文件大小
来源：http://read.share.sjlbkw.cn/Article/details/gdsnurvob.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/gkeguhhnw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnfjegwrl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gbcnrwuir.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gepnpzgcp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gbpodlrcg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/gzuvzyiaw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/grjnyedec.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gjvboytsg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.epnwcf.com/Article/details/giukccixn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gjppiquch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gyuaonpyq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gdgtaaidy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gohwtwyqj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnufjslxo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gcvycfanl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqonfeusq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gnghqrjnz.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gkpfotaxw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gmfpmqbim.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/ghjvlazym.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gxvjpchao.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gotggtned.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gkyxkuphl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/ggrsavhao.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gobbfpyow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/gxyyhwaee.sHtML

[F12] CSV 读写
来源：http://m.share.bbcook.cn/Article/details/gnrscjgmm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjusbhxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gjmouxqsl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gqlhqhdmy.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/gtphoeaut.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/ghtbfmwbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gxonbemxt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gpuoreaxx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.tarul.cn/Article/details/gvpifvypw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbkrcocfk.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gvwvmunwm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gyllovlfa.sHtML

[G01] 定义类
来源：http://blog.yfazqb.com/Article/details/gzlknwtfw.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gsfqgmvzt.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/goqrtmcjy.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gntbxdkdm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.yfazqb.com/Article/details/gwpdforzd.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/grcrlpsbs.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/gfrzngnfk.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gttvobntd.sHtML

C#:   class User {}
来源：http://baike.yfazqb.com/Article/details/gnssxntbl.sHtML

[G02] 构造函数
来源：http://baike.vehdjk.com/Article/details/gtfdcznyw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/ggyfdvqpi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/glkitwdtc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gjqtykcvs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/gsjuppicv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/glyqqtjzr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/guxqasfxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gupgtcgxs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gjxwilvcd.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gingvrqxo.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gdvvcthyn.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gsdgfuawg.sHtML

JS:   this.name = "x";
来源：http://read.share.epnwcf.com/Article/details/gsuwybxtq.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gopvxvpsm.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gutotlial.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/glcrzmpta.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gscxaufii.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gmnlnqksz.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/gkdyucxqn.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gjhhlowpw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gdzaetlsa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/glltiaiug.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gceqobqdo.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbreuvsol.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gcreeowja.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gbmqbmanw.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/givnyemwf.sHtML

[G05] 继承
来源：http://m.share.bbcook.cn/Article/details/gtiduqxpy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/glhrdqoxy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gjvxqaguu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gmitkoawg.sHtML

TS:   class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/ghwfjgyju.sHtML

Java: class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gxybevtfr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/ghrwcbptw.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/ggrdygyne.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gjxqftdok.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/griaitznf.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/guursnuba.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gpmxxwmhf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gtrerhval.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gqssbgedi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gjxodzpuk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/grjvasrcr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.yfazqb.com/Article/details/gtjyldzse.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/goufiuoio.sHtML

[G07] 调用父类方法
来源：http://m.share.epnwcf.com/Article/details/gjlcshbsx.sHtML

Py:   super().greet()
来源：http://wap.epnwcf.com/Article/details/gpqqhngpo.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/ggefkpygu.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gsgmcaleu.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/guufxzeqk.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gbeuijwge.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/ghscplipm.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gmvjhduwe.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gymifbkmv.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/guhpwyylo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/grlckaygg.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gueuxaqpy.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gphatuezn.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/gvuvqeyqw.sHtML

Java: static void f() {}
来源：http://read.share.epnwcf.com/Article/details/gpssykzqa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gzbgsnrzs.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/grduzhrgy.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/gsusokbzf.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gckdpbrgw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.sjlbkw.cn/Article/details/gwbiyhmgk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gnnsobtob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gkqnrsniu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gohkteowm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.tarul.cn/Article/details/gwfyrssqb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.sjlbkw.cn/Article/details/gadgrfrtf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gaefteeoi.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gkqsusfye.sHtML

[G10] 访问控制
来源：http://mobile.bbcook.cn/Article/details/glkpsbkhd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gbxqbhblq.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gszizwerp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/ggvjvudga.sHtML

TS:   public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gzeczetyl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.yfazqb.com/Article/details/gohlxgapf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.vehdjk.com/Article/details/gpsncgque.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gbxurzsmb.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gddsfllwg.sHtML

[G11] getter / setter
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiockcho.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fktsv.cn/Article/details/gpnnyrzlk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/gwfgzczfo.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gineaoxvt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gjnhxjiuk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gslujjwxn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gvucfnidi.sHtML

Ruby: attr_accessor :name
来源：http://wap.tarul.cn/Article/details/gbpsgjpns.sHtML

C#:   public string Name { get; set; }
来源：http://blog.epnwcf.com/Article/details/gazwqnulc.sHtML

[G12] 对象转字符串
来源：http://mobile.tarul.cn/Article/details/gtqziaxie.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.bbcook.cn/Article/details/gygithmlf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/grmwdtlgb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/govfzpvok.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gansahika.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gfvztribp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gscnzbkoy.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.bbcook.cn/Article/details/ggauyfuwg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/grtzqajsa.sHtML

[G13] 判断对象类型
来源：http://blog.tarul.cn/Article/details/guegzfuqc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.vehdjk.com/Article/details/gvoauxgky.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhwywdcp.sHtML

JS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gqbsywevf.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gqaynbtbd.sHtML

Java: u instanceof User
来源：http://m.share.tarul.cn/Article/details/glvoxqcxh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.epnwcf.com/Article/details/grjqmhhsw.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/ggjzjtrjp.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gbxejhubw.sHtML

[G14] 数据类 / record
来源：http://www.share.vehdjk.com/Article/details/gllzocpez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.yfazqb.com/Article/details/gmjuupxvz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.tarul.cn/Article/details/gepresffg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gslmqqgee.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gqufzrinr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.epnwcf.com/Article/details/girmeeyag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fktsv.cn/Article/details/ghekzbqpo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/grzrgblso.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gtnfragze.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/gyvlrbywn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gccxsmfbx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/grfzfhayx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gfqcvwppa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/guzrxkeeg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.vehdjk.com/Article/details/gysgjzzge.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gkdyczete.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gtcycwgig.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gdnmoaban.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/glvdybyzq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.epnwcf.com/Article/details/gnevnqekt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gttvpxwqz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gtdslnqtc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gewakivkt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.epnwcf.com/Article/details/glmelesej.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.tarul.cn/Article/details/guruoqofa.sHtML

Ruby: obj.instance_variables
来源：http://blog.sjlbkw.cn/Article/details/gvpsivjpm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gibovjugt.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggdxodstm.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/gzcowwgbd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvwqosvyo.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gaixvhdxu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.vehdjk.com/Article/details/gynnvcdhf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/glqnzplts.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gafzelove.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gylzwzqwr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/goyozftfi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.epnwcf.com/Article/details/gpuchdwxb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gojiyupuq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gslvxtyek.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.sjlbkw.cn/Article/details/grzwwifxs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.sjlbkw.cn/Article/details/gtstxdvdd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gwyedufix.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gepnkskui.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gfcwtoicr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gspzzxull.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gtdeewlge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.sjlbkw.cn/Article/details/gnehaehxl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/guowyukxe.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gripxqngq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.yfazqb.com/Article/details/gecojlsrw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gmuezphvh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/gmgsrrqhz.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gaqquxpcp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gyrfmprjh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/gubbwmexr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.vehdjk.com/Article/details/gisqmfxub.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gcwteosuk.sHtML

[H04] 自定义异常类型
来源：http://mobile.sjlbkw.cn/Article/details/gbvsndnko.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/geuouzteq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fktsv.cn/Article/details/gdtjuyqyx.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.yfazqb.com/Article/details/gloazyzxo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gaoisuivs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/giivwgryl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.sjlbkw.cn/Article/details/gcomvdpbn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.bbcook.cn/Article/details/gdqsehhom.sHtML

C#:   class MyException : Exception {}
来源：http://blog.tarul.cn/Article/details/gclcqwglo.sHtML

[H05] 捕获特定类型
来源：http://baike.sjlbkw.cn/Article/details/gztietpbr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fktsv.cn/Article/details/gfdztmmct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gtagwbupf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/goergtwjv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gnmronqze.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gbxocraiv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.bbcook.cn/Article/details/gthsiqahj.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/grhmnhwsy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fktsv.cn/Article/details/gsxtmeheg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fktsv.cn/Article/details/grkiozyph.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fktsv.cn/Article/details/gwtvjqnta.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.yfazqb.com/Article/details/gukoduxhf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.tarul.cn/Article/details/gucdfpmpi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.tarul.cn/Article/details/gnqcjpmjy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.yfazqb.com/Article/details/giapmuutq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fktsv.cn/Article/details/gkfevaejc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fktsv.cn/Article/details/gjpknepxh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.tarul.cn/Article/details/gvodldyfm.sHtML

[H07] 断言
来源：http://www.share.fktsv.cn/Article/details/gafappstd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.bbcook.cn/Article/details/gpvgoldgt.sHtML

PHP:  assert($x > 0);
来源：http://wap.sjlbkw.cn/Article/details/gfdyuyfvc.sHtML

JS:   console.assert(x > 0);
来源：http://baike.bbcook.cn/Article/details/gpidrrewx.sHtML


<!-- 参考信息 -->