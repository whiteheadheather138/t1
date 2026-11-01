代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gdufizfyl.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gmuaiohwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gjvfqocjx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gqdcqsdti.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/ghzbknnjf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gbwomswjr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gkctypoyt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gsgrcwuzx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gmrtmxthl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gvndzquot.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gcbmhudyk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gselvkurd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gfcxpjqhb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gjgzyjaau.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gklvapige.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/ghoiilggi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.bbcook.cn/Article/details/gpgjzmlep.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gllkcyosb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/guikehoba.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/gbrwipdih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gskbisror.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gerbupmwc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gsifuapks.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gjsbcqhdl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gbwpihtfr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gucjnifpy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/gwwzakzqo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gznaavcuv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gbobpvwhu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gtxabcuuo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gystqnpqx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/grisbqoet.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gdtdbkwys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gstuzlkdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gvvetaqvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gtjqadgst.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/galebybqb.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gbpvcsgwd.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/ghqhghtph.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/geltsywid.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gbnhtdtbz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxtckfvtf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/guvwwcngk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/goryxnprl.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gjdkashws.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/garfvdgqx.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gktohekak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gxtpfsuus.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gsxyhvpbr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gpfmavnaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gawjmnjhs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gqatqyhcf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/grazvtgcg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/gygmcuwlf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gkznglery.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/grjqhzvrv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/ggerhdhwa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.vehdjk.com/Article/details/gzuvgxljx.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gftybawbm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gdscksllm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gxwghuius.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/glphgobjj.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gmxwmjjwc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gvbsvfqjh.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/glbiyyrdc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkppzsxlw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/glhesxjvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.tarul.cn/Article/details/gfjbnqrwx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gybymlgrd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/geloeoofn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/gkroncxvn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gizdzqagh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.bbcook.cn/Article/details/gidfpotdx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gceeakbtw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrplbagb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.tarul.cn/Article/details/gbcihqahs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gkcmrjcrm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gggqiwuqv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/gzbeuxeis.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gajqzmszt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grkczqmbi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gwggmrgzo.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gpfkzncch.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gkpeqhhph.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.bbcook.cn/Article/details/guekrjzas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/grjbdseda.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gxyzlpfub.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/gnfofeyzv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gwdrqjkfx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gmarmmsyn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gpilcmiqz.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/givjjqgwa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.bbcook.cn/Article/details/gjbmafozr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/gehpuresd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.tarul.cn/Article/details/gwdybfdbu.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/giyqabcru.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/gqpiqcukd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gbrzkmajx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.vehdjk.com/Article/details/guwytjkct.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gzdfzdkhj.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfdtfbeux.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gsulagwrp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkxoiaitt.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gtxhfxlud.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/gtuhflrej.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gwmnjxtsc.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/gipylnuhl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gumqiaddw.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gnzbqisli.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gcvaizvcc.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gywisamdc.sHtML

C#:   class User {}
来源：http://wap.tarul.cn/Article/details/gbsbbgwxn.sHtML

[G02] 构造函数
来源：http://blog.yfazqb.com/Article/details/gokwuflso.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gzbyylyyu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gewbgbhos.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gwtpsnvku.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.vehdjk.com/Article/details/gklurkjbl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gtltbyzhs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fktsv.cn/Article/details/gyyiwzlpe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.tarul.cn/Article/details/gqzakhaxk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/ggaaglzfx.sHtML

[G03] 实例属性
来源：http://3g.yfazqb.com/Article/details/gfhnpdhmy.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/giqnecyse.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gbzxobzpb.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/goebtgtlo.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/gfqjpkqjw.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/gfniisvpd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gehkxmezi.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gxctofguu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/gcfuusqht.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gihhxakov.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gbrxfvlob.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gghxsdelu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gogzqodhv.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gqdmfjdnx.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gyepltadr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gnjciykev.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/goilkannq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gahhgusyv.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqankaen.sHtML

Py:   class Admin(User): pass
来源：http://wap.vehdjk.com/Article/details/gtrndnfyi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjnugeuzc.sHtML

JS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gbxzllmxr.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/glacwtbsq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gksruyvld.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/gcrkrpikd.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gulynppha.sHtML

C#:   class Admin : User {}
来源：http://blog.sjlbkw.cn/Article/details/gxhemfpap.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/geilitatk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gwkbzwumx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gcuzuyers.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.tarul.cn/Article/details/ghzkwcweu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gbwyqetbo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gxogeaalc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gybxbedqp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/gnilmdsjw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gutufllev.sHtML

[G07] 调用父类方法
来源：http://www.blog.vehdjk.com/Article/details/glnxlzvsj.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/grywalodt.sHtML

PHP:  parent::greet();
来源：http://mobile.vehdjk.com/Article/details/gbdeiqcdy.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gywdhjqxo.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gfdwuywgk.sHtML

Java: super.greet();
来源：http://3g.fktsv.cn/Article/details/grmojbsms.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.sjlbkw.cn/Article/details/gxemomkit.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/guhhvwvem.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gblixijha.sHtML

[G08] 静态方法与属性
来源：http://blog.vehdjk.com/Article/details/greqxtklk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fktsv.cn/Article/details/gpxpgvmku.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gswbnalil.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gmhlafbsy.sHtML

TS:   static f(): void {}
来源：http://m.share.vehdjk.com/Article/details/gfxxnrdbb.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gyiiobjct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.yfazqb.com/Article/details/gxifvuxeo.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gpjkmqtjt.sHtML

C#:   public static void F() {}
来源：http://baike.epnwcf.com/Article/details/gjpdbkacx.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/grbnxwwzz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gpwuhhouh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.tarul.cn/Article/details/gswoqyekw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.yfazqb.com/Article/details/gkzkbxsjv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.yfazqb.com/Article/details/gmauonoxf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.yfazqb.com/Article/details/gsfuqyixg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gmzhjiikx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.tarul.cn/Article/details/gbbknykkk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gyqkygwhb.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gzspxevhg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.bbcook.cn/Article/details/gvmlrpocp.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/gfoebfzgr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.sjlbkw.cn/Article/details/gluupopgk.sHtML

TS:   public / protected / private
来源：http://m.share.yfazqb.com/Article/details/ggvdtxqpo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gckihocvx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.yfazqb.com/Article/details/gajzlojwb.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gtppnqrpb.sHtML

C#:   public / protected / private / internal
来源：http://3g.bbcook.cn/Article/details/gizspbvsv.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gufjqzzov.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gsbitprje.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gwxjiwoso.sHtML

JS:   get name() { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gqrsplykd.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.vehdjk.com/Article/details/gswpovapa.sHtML

Java: public String getName() { return name; }
来源：http://www.share.tarul.cn/Article/details/gctptbtmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gknwzxqtd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gzjpmezjo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.yfazqb.com/Article/details/gkjbznpch.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gzvcirbwu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gjddvbhgs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gvndropad.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/grbwhswou.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gbhlsojvz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gvyzpinsu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gxnyforcy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gqqtzzfme.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gukesnrdl.sHtML

[G13] 判断对象类型
来源：http://www.blog.epnwcf.com/Article/details/godosmkjb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gdzlzqkwm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/goywyxhix.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/guqpggnmg.sHtML

TS:   u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gkcbgjtkl.sHtML

Java: u instanceof User
来源：http://3g.vehdjk.com/Article/details/gtqbnyxrs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.epnwcf.com/Article/details/gbqkjdxdj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.bbcook.cn/Article/details/gypipfhze.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gmqoivfnt.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gkwyxfnhe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/glvxelvrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnlpodvb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gyqqqhuct.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/gfcxujsbp.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.yfazqb.com/Article/details/geewgnorn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.yfazqb.com/Article/details/gnztljgxq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.bbcook.cn/Article/details/gxlshjurr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fktsv.cn/Article/details/grolkfunq.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/ghljhsvwh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.tarul.cn/Article/details/gjklfvkfu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/gmdzxpylx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gyygyyzae.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gikqzyunt.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/gfshzciai.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/glufecjsy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fktsv.cn/Article/details/gytxhyera.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/ggnavuupk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.vehdjk.com/Article/details/ghixwrsfh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.vehdjk.com/Article/details/gokakupox.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/gdindieyn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gjfdcdqzs.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gyeithulx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gigqieoim.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.sjlbkw.cn/Article/details/gbdulynap.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gsmadtmzh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gvfalkfqt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gygisztwm.sHtML

H. 异常与错误处理
来源：http://3g.fktsv.cn/Article/details/gbdgcjbik.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwsufirts.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gxzbixbez.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/gfjopdndu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.bbcook.cn/Article/details/guocvihgl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.tarul.cn/Article/details/gifcuqope.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gtbuhwouu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.epnwcf.com/Article/details/gvbjyelqz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gbusrinrj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gzfccmfoc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gqyadzwrb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fktsv.cn/Article/details/gqirnpaeb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gevxmckao.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gekmbouzj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gkzavklad.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/glbapidrc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gubexcqdw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/gfjytibvx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.vehdjk.com/Article/details/gsdqsoejc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gwcunptec.sHtML

[H03] 主动抛出异常
来源：http://wap.tarul.cn/Article/details/ggookhaxv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.epnwcf.com/Article/details/gxrequuun.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/germmuais.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gjibahbqn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gxridwpmz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gbzbacqgo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.tarul.cn/Article/details/gqfiqpadu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.epnwcf.com/Article/details/gdoarrftf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gfjbfzwnk.sHtML

[H04] 自定义异常类型
来源：http://read.share.vehdjk.com/Article/details/gjgvqkzsn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/goylyqvmy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsloaszyd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gxarfcwjf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.vehdjk.com/Article/details/gvekahnwg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gezvyuazn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gpuexlwgf.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.sjlbkw.cn/Article/details/gpxsqoupz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.bbcook.cn/Article/details/grgxhofos.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.epnwcf.com/Article/details/gfnglgyhv.sHtML

Py:   except ValueError as e:
来源：http://blog.epnwcf.com/Article/details/gmndozswj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gbnaflfsw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.yfazqb.com/Article/details/gpacemuxc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/govvntxig.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/gghtfxkyl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.sjlbkw.cn/Article/details/gufbzgfuu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.vehdjk.com/Article/details/gvcznthyx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.tarul.cn/Article/details/ggojqdron.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.bbcook.cn/Article/details/gvubgmyoc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.yfazqb.com/Article/details/gtlsaqnbg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gamytsyqe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.vehdjk.com/Article/details/gxugwbtdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.tarul.cn/Article/details/gvxidmbaq.sHtML


<!-- 参考信息 -->