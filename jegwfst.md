代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gxfpdrgvo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/gniwasury.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gwlcdljns.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gpklkohwu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gmkfhdkdm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gogccvxiz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/ghtyojwtt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/glmplsaaz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gdoycoqws.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/ggtljkvpz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gdcbxwkcv.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gzrenijyh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fktsv.cn/Article/details/glxhsbhhi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.epnwcf.com/Article/details/glhaplzun.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/ggtbpentd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gkqkacita.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gzkuarbin.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gfracjcsn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gsusodyjb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gqyqohyye.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gonbbclnp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.vehdjk.com/Article/details/ghidohzjd.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.bbcook.cn/Article/details/gwqwnijps.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gijxiedqs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gzxysrhyt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gnwizaggj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gpcmljdvi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ghvmsfqfz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gffeqcujv.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gmaogvtkc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.yfazqb.com/Article/details/gdrvdijmh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gdoqhkplz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gatdryxqp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqovhwpzv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gqwwhvchv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gicrsaghf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/gyxwtdwsu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/ghywhcaqo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gfuuyfjcf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/gfafhmetl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gclgnugph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gsomhluje.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/glsxilsod.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gjrphkmqc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gowgfugpp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gqpervogv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gotfpqzeo.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/ghxogifko.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gkcjqhqqb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gcvtdjdjf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gthuprrhm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gdspkrsco.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gcgyupvze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.vehdjk.com/Article/details/guozbjfru.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gqbnlcmoy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gppkizoqe.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/grixqnqyy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggesuumoo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fktsv.cn/Article/details/gydlungdw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gxrumduej.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gcpfpglzu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gilmlegcu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gduqlyexx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gldsssxql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gfuzeatke.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.vehdjk.com/Article/details/gslubfwng.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gcqcprthm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.vehdjk.com/Article/details/giqgsmpqk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghucvbtea.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqflexvyh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gvuqwygfc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcmfmlres.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/grumpmuyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggomovybb.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gjwugmpxw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkgarovez.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gzmwjzskp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gojclrteu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gagqqqaoc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gfvqvgaay.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fktsv.cn/Article/details/gwzxwfifg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gspdjapyb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/gkxxiaaep.sHtML

[F12] CSV 读写
来源：http://mobile.vehdjk.com/Article/details/gpdgmnzmn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.bbcook.cn/Article/details/gihwzvfaz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gsvquqfyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gbwxmejsm.sHtML

TS:   // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gozvcmaaq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/goccketyc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gctxdhvhp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gpatgvjyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fktsv.cn/Article/details/gltpslrqr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfcquipnb.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gdljwumhy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfiizkvis.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gpfoggmsi.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gegvzhjjr.sHtML

PHP:  class User {}
来源：http://3g.sjlbkw.cn/Article/details/gmhqbltvr.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gkkropkwp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gstkwwdtd.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/ghjalhpsw.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gamplyqpq.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gcqmxbist.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/geuevbhpo.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/gnvgussaw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gicklfsvd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gasbexslr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gdjvmhwoh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.epnwcf.com/Article/details/gwfuxchdz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gufzyagjc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gkvdrwszg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/ggyhgxopo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/gjccxcvxb.sHtML

[G03] 实例属性
来源：http://read.share.vehdjk.com/Article/details/gceeeoyzs.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gfkzovzzx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gpyubfmbd.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gusctfmsa.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/glcvjcjpb.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/gpvjkqlpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/glrzznmzk.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gpkpromzv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gnhobtoir.sHtML

[G04] 定义方法
来源：http://m.share.tarul.cn/Article/details/gogsxhigm.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fktsv.cn/Article/details/gflnxoelg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gphqyuhds.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gxljlcuqt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/ghrbazrsi.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gilvmrrpw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gcfizxftt.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gadqfkckc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gehegykxn.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gaqmpmwgw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/gbkwsotre.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gjkoubwyn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grctxffco.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gfikgbaxb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gszdjoras.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.sjlbkw.cn/Article/details/gvgmkyefg.sHtML

Ruby: class Admin < User; end
来源：http://blog.vehdjk.com/Article/details/gnvkvtwmy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzxptgun.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/gqridfucq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gvxbpvtor.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/gbfyuiiqi.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/ghypzbxbc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gydoilbpm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/grsnhvrto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gnpldxkig.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gepqbqnic.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gkujcwpcl.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gmtlizpbm.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gzgzkqjms.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gosftlqqw.sHtML

JS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gfbtypztt.sHtML

TS:   super.greet();
来源：http://baike.bbcook.cn/Article/details/govjulhmg.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gczesqypr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fktsv.cn/Article/details/glpvzjabp.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/golugatcq.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gqnokumvo.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/glqxctqjb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.sjlbkw.cn/Article/details/gbjuvnedo.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/gvmvncmrw.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gmvwjrxxh.sHtML

TS:   static f(): void {}
来源：http://m.share.bbcook.cn/Article/details/gcefgssfr.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gnrzkpymu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gkxomkgdq.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gmsaalxjk.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/gcxwqedlb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.bbcook.cn/Article/details/gnbuqgnit.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/gzlkxnprn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/glzthkyej.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.epnwcf.com/Article/details/gogracdct.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/gipblzyjl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gocrxtkca.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/gineobmme.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/gifmmxwvd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gbtvlgzaz.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/gtfrfypqr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gdjsercdq.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/gewyxiozp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fktsv.cn/Article/details/gqjqgfjxn.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gmgsmnjyr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.yfazqb.com/Article/details/gjwpweoaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gkanlzhhz.sHtML

Ruby: public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gtrdxlwsu.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/gmqjbkuic.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gymguiclv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gzqsjvjsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gingbxnni.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gczgtkpzt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gbtcfucoo.sHtML

Java: public String getName() { return name; }
来源：http://mobile.bbcook.cn/Article/details/ggtfkbytc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gdxtggtgd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/grqzvtgry.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gbwkuwquw.sHtML

[G12] 对象转字符串
来源：http://m.share.yfazqb.com/Article/details/gitdperry.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gyxnbzqqb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/godadbwbg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gdunkjkmu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gfazpucmk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gyvhmnxdu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gkvnbeckr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fktsv.cn/Article/details/gmgxriyeg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gggsnvmzk.sHtML

[G13] 判断对象类型
来源：http://www.blog.tarul.cn/Article/details/gsbpnaarq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.yfazqb.com/Article/details/gtoywubkw.sHtML

PHP:  $u instanceof User
来源：http://baike.epnwcf.com/Article/details/gelryxpes.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzxcjfaaa.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gbhfdlhxa.sHtML

Java: u instanceof User
来源：http://3g.fktsv.cn/Article/details/guptnpxkn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/glmlotigp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/girdbixso.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gvlxfezhv.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/gsllaqanl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fktsv.cn/Article/details/gzjvnczyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.tarul.cn/Article/details/ggrlbnlyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gjtngkmpv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmrwnofu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gmgcwdsro.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.bbcook.cn/Article/details/ggflrvgfk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gcbrjewnz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gzyywuzhh.sHtML

[G15] 枚举
来源：http://m.share.fktsv.cn/Article/details/gydfcoxoz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.bbcook.cn/Article/details/glnquyolk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/gmpxlnlhf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fktsv.cn/Article/details/giialmxzt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gydtfzjte.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gfkssyvby.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.epnwcf.com/Article/details/gtwoabmce.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/gvhbsvgre.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gmyfkpmau.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gmfakopxq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.vehdjk.com/Article/details/gkkvlhmcc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.bbcook.cn/Article/details/gwgnltizn.sHtML

JS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gsbuplmno.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gbrhiwuec.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/gaojropzy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gfzjaeqbv.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gbxzjuctf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gkmlkpjwo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gelahwyhv.sHtML

H. 异常与错误处理
来源：http://read.share.vehdjk.com/Article/details/gdswkmqrd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gznsahvwh.sHtML

[H01] try / catch 基础
来源：http://read.share.fktsv.cn/Article/details/gvmrhqdtc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/galoqjbrf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fktsv.cn/Article/details/gyxhkntkx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gmbesmbug.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gzgoygidm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gburwztol.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gwggejkna.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.yfazqb.com/Article/details/gxdusvqbc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/gcrcqpvgn.sHtML

[H02] finally / ensure 收尾
来源：http://blog.yfazqb.com/Article/details/gsutxvign.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/ggpzgaopo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gmugtiyio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/glkzfmbla.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gmrahxqft.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gqzyktlkj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.tarul.cn/Article/details/gzmfhueqj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gbkskgzjf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbxejvszg.sHtML

[H03] 主动抛出异常
来源：http://blog.yfazqb.com/Article/details/gjrsyquru.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.sjlbkw.cn/Article/details/gzgxfpplq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/grqcbmvtk.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/ggmfekrbt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.sjlbkw.cn/Article/details/gyqdrvbeb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/givxrjwum.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.sjlbkw.cn/Article/details/guvwwwwsi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.epnwcf.com/Article/details/gaogfpdlt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gttprebyt.sHtML

[H04] 自定义异常类型
来源：http://mobile.yfazqb.com/Article/details/gaajdkuqk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/glhxyyxzi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fktsv.cn/Article/details/gbajrvbwu.sHtML

JS:   class MyError extends Error {}
来源：http://wap.yfazqb.com/Article/details/gmldmmepa.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjpmpafuz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.tarul.cn/Article/details/gsibyogni.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gfrqmxbtf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gfstuvqwn.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fktsv.cn/Article/details/gpvvgowiw.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gbnfdnmxw.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gpbzvgrcs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fktsv.cn/Article/details/gofsztbqb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gizulvpid.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gbridwlfs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjqkvyzsw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.bbcook.cn/Article/details/glxropsro.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gjpnyaqry.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.yfazqb.com/Article/details/gyiercboh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fktsv.cn/Article/details/gkiwjwahu.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.tarul.cn/Article/details/gywzhyxff.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.tarul.cn/Article/details/gxnvngqyj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.vehdjk.com/Article/details/gloaowkoa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.epnwcf.com/Article/details/glhqthycx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.epnwcf.com/Article/details/gdrhydepi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.vehdjk.com/Article/details/gyxucivvu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/gqzlwhmln.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.tarul.cn/Article/details/ggdvjjntd.sHtML

[H07] 断言
来源：http://blog.sjlbkw.cn/Article/details/grlcivqdi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.sjlbkw.cn/Article/details/gxbdkgdvn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.tarul.cn/Article/details/gctibxgvu.sHtML

JS:   console.assert(x > 0);
来源：http://3g.bbcook.cn/Article/details/grwrmyejm.sHtML


<!-- 参考信息 -->