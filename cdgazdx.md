代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gkgtzvogb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gdvpbofbw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gfyxztszj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/grbifosiu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdsprnke.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gpuxyadfb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/guayztlzq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/guanpozzo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/ghonwkifa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gszekwwbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/grzzeypej.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gcwemuieg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gbwipcvpx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gonmlpzqv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gymxsvlnv.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gasbsqnqs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gmiqtmdie.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.yfazqb.com/Article/details/galzhejuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gilzegduy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gbguaayvu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gpfuuijou.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gqrnnbiar.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gemhzxsmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gjezzyggp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gpxtxaogg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.tarul.cn/Article/details/glilaoohe.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/grbjjtamz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnhxybdpg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnmesrhed.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gkhkyshrt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gqtzlgefk.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtakejuth.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmorxgror.sHtML

[F06] 删除文件
来源：http://baike.tarul.cn/Article/details/gskoeupub.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gsyoizmyy.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gnhyqkfyo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcccfxecb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gtkyhuspl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gmmjjgcvs.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfajowahu.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/gswqdmdef.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghiobxxiy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fktsv.cn/Article/details/gxitdclea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.epnwcf.com/Article/details/govergotg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gzashsgfs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gnkmpfbnl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gmggigart.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gsnswzzzv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gkwdmxtqm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gicqwjrhe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gqraasjyb.sHtML

[F08] 遍历目录
来源：http://www.blog.yfazqb.com/Article/details/gxhhkozxq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gwnkaiksp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gbuqosqen.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/glcusqgxe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gpryqgclh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gnqunzfaa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/grjjyxkrm.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gfmyvdvmb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gxreiubux.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gdacfmric.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gqfixkgzd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gytyelqcb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gugdfeylr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gckgncmxd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gbsawxixc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gclilhuzp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gmkfeqjfm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gchbfxstq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gtxbubkgl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpafrqobw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gcfzilzgb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/govjoosej.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gieuajzzb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gnondfohq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gczocesaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdykkwuqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gleqorqpu.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/gjszffdzx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/gqznaeaek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.tarul.cn/Article/details/gzmbeaarm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gpvkqouhw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gqsgsncai.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gxzisaqzp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.vehdjk.com/Article/details/ghlcbcbax.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gtysjmozu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gredgdssd.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/guiomqssn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gbehzmthg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/goeqfcmqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.tarul.cn/Article/details/gufeudjlo.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gzzagbaan.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gouduvwft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fktsv.cn/Article/details/gwuciwwdz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gzcbdmzim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gvcunlfwu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmrqlgpzd.sHtML

G. 面向对象
来源：http://www.m.share.vehdjk.com/Article/details/gemckwxeq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gyvtiqydq.sHtML

[G01] 定义类
来源：http://www.blog.yfazqb.com/Article/details/gcqijldkn.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/glnrctjzp.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gdhkekxmt.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gvcoujztn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/grlyvvnku.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/ghhesmwan.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gwkjxwtxa.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gsbrgcpgl.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gknsrqape.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gkkgsbqjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvhzuard.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/ghivbrrny.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gidynicpa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.yfazqb.com/Article/details/gpdpvjlkj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gmnortbyu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/guxgrihml.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gbrnxskjg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.vehdjk.com/Article/details/gmhfnvatd.sHtML

[G03] 实例属性
来源：http://wap.fktsv.cn/Article/details/gfommxjtd.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gixnisrpn.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gnbyggahr.sHtML

JS:   this.name = "x";
来源：http://wap.fktsv.cn/Article/details/gijumvxzr.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gktyhsagg.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/ghjfsyfxo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gedpzoecx.sHtML

Ruby: @name = "x"
来源：http://mobile.vehdjk.com/Article/details/gccnxdafw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gspshgiox.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gdrzfqzir.sHtML

Py:   def greet(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gpbghkqmr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gtuqtyvvz.sHtML

JS:   greet() { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gsczursdx.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gmxpnpism.sHtML

Java: String greet() { return name; }
来源：http://mobile.bbcook.cn/Article/details/gtvkcyyvq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gznfkjrqm.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gytrjepqk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/glqszkgct.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gqbafhpxd.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/giamezhhv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gyyijrkll.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gjlwhmklg.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gdxvbziyc.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gbpdrrnmg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.sjlbkw.cn/Article/details/gqzamwtqb.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gfwqzmveu.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gevkawnag.sHtML

[G06] 重写方法
来源：http://wap.sjlbkw.cn/Article/details/gqzstohxo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gwtjluakj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gzepfrmyv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjvtjocm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gcflmcthn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gltjkcsiw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/gzhllowta.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.tarul.cn/Article/details/gdrcdkjmb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gcfbxcimk.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gsahqvzly.sHtML

Py:   super().greet()
来源：http://blog.tarul.cn/Article/details/gazdmnlmg.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/gbzbxcbhw.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gpbxgaixc.sHtML

TS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gqfpfgvbm.sHtML

Java: super.greet();
来源：http://blog.yfazqb.com/Article/details/gvjduevav.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gwwtzewtp.sHtML

Ruby: super
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvymttqo.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gljgxaewk.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/grerodbeg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.vehdjk.com/Article/details/gwsngztwq.sHtML

PHP:  public static function f() {}
来源：http://www.share.bbcook.cn/Article/details/gakrfhpkf.sHtML

JS:   static f() {}
来源：http://baike.epnwcf.com/Article/details/gttjykmkk.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gxvjmtopl.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/grpvsuenk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/guqoyymsr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fktsv.cn/Article/details/gfrvldcdb.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gotgsumck.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gbtbnrtlb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.bbcook.cn/Article/details/gjkmjornz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.epnwcf.com/Article/details/gcepusklo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gquijqcst.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gznqfdqcd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.bbcook.cn/Article/details/gsxvtqbim.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.tarul.cn/Article/details/gijpanlse.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.tarul.cn/Article/details/gcaijvcdy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gnfvjzrfc.sHtML

[G10] 访问控制
来源：http://mobile.fktsv.cn/Article/details/gwinjawco.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.bbcook.cn/Article/details/ghnnpizoe.sHtML

PHP:  public / protected / private
来源：http://wap.tarul.cn/Article/details/guxfpbivs.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gnnmfmgjo.sHtML

TS:   public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gpbpypfae.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gjzudepxc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gjdjipzel.sHtML

Ruby: public / protected / private
来源：http://wap.yfazqb.com/Article/details/gqpvbsgdm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/gbcirsbsq.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gvhfnauap.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gkawqmczv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gedmirtrv.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fktsv.cn/Article/details/gjoirdnyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gdldsfohr.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gugxmgmfe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gpomezsuu.sHtML

Ruby: attr_accessor :name
来源：http://wap.bbcook.cn/Article/details/goyeddelv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.yfazqb.com/Article/details/gklhyhoyk.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gnunaafgq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gsgxlggdd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/gzredcsfd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/glrjubnqk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gwwmhrxkz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.vehdjk.com/Article/details/gcymuqkbn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gdhygqaqr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gdiywervq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/guhlzfkjr.sHtML

[G13] 判断对象类型
来源：http://3g.epnwcf.com/Article/details/goxzvmonu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/garglrkdz.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gnpkbihca.sHtML

JS:   u instanceof User
来源：http://www.m.share.yfazqb.com/Article/details/gvdgyyrbn.sHtML

TS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gjgtfmnnp.sHtML

Java: u instanceof User
来源：http://wap.vehdjk.com/Article/details/gfnbkwqpn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gqwqztofh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.epnwcf.com/Article/details/gfghajprw.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/grufouxnj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gtmcewnoi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.bbcook.cn/Article/details/gmlkxdmvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.bbcook.cn/Article/details/glljhvuvn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gddrpyeov.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.sjlbkw.cn/Article/details/gtlpvdbbi.sHtML

Java: record User(String name, int age) {}
来源：http://3g.epnwcf.com/Article/details/gaqyzroda.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gxmkkcewf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.vehdjk.com/Article/details/ghlopeoqc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gvdrrlfha.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gakizwrhf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.yfazqb.com/Article/details/gdtuoewid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fktsv.cn/Article/details/gfmnbvwmn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gnqkuryqi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gocqdbwln.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.epnwcf.com/Article/details/gjozcausq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gxrpwlgjt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.vehdjk.com/Article/details/gxtxssyxx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.bbcook.cn/Article/details/gstvhvpbv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.tarul.cn/Article/details/goczcosri.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/gygopupxf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/gjymjerfz.sHtML

JS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/gnlmprnek.sHtML

TS:   Object.entries(obj)
来源：http://3g.sjlbkw.cn/Article/details/gocoamjnq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.sjlbkw.cn/Article/details/gvjjeeeuj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/ghtkmzyho.sHtML

Ruby: obj.instance_variables
来源：http://baike.vehdjk.com/Article/details/gzikqumuj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gkqwhdpkj.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gndqpawyv.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gjjpktiwt.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnnqnkyar.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gxqnmlaaq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.sjlbkw.cn/Article/details/gbyifnvhf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/ggmwxnthy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gjmigoqmf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.bbcook.cn/Article/details/gtproklzt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fktsv.cn/Article/details/gbzpsnbpz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/gbzmpiayi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gtotcuwoe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/ghxmjadfm.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gsqrzsbhw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fktsv.cn/Article/details/guaodvrjv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gnkstcyta.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gruisuuxm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/guiexfpgi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gfujqnljg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gqtfjucge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.tarul.cn/Article/details/gkeyytcyb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.tarul.cn/Article/details/gdbwnzbph.sHtML

[H03] 主动抛出异常
来源：http://mobile.yfazqb.com/Article/details/ghyracrol.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gydlegbsz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/geohqfxgi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrtsjlkj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gaksbtego.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/goprxcmfb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.epnwcf.com/Article/details/gbouhwjeg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gqfwlpqgg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.yfazqb.com/Article/details/giodglmfn.sHtML

[H04] 自定义异常类型
来源：http://www.blog.tarul.cn/Article/details/gbqmcczwb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.yfazqb.com/Article/details/gudkkttvo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gupekxnxn.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gxeqmmlng.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/golzufbpm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.sjlbkw.cn/Article/details/gyzoketcj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.bbcook.cn/Article/details/gytuyyvga.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gxntjslxy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.yfazqb.com/Article/details/grzkholkl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvxkvxqz.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gjsvlyoio.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.epnwcf.com/Article/details/gmwfqqxhl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fktsv.cn/Article/details/gvcsqlype.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fktsv.cn/Article/details/gstdepbwd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.bbcook.cn/Article/details/gmizedufo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fktsv.cn/Article/details/gumahxksg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fktsv.cn/Article/details/gxfpkugny.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.vehdjk.com/Article/details/gfkumojjj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gtecvdltt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/gcqdxglam.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gyndtxbpt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fktsv.cn/Article/details/gtufmhkro.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/grtoqghqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.vehdjk.com/Article/details/gwtiacqko.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fktsv.cn/Article/details/gpvnmapjn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.tarul.cn/Article/details/grqhrdobb.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fktsv.cn/Article/details/gmdotqlfn.sHtML


<!-- 参考信息 -->