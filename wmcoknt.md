代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gjzxombca.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbsriulxk.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/gvsntcoyj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvtdcmtqc.sHtML

[F01] 读取整个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gmxiuabjd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.yfazqb.com/Article/details/gocexpnjx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsjqgneie.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/ggjrogoyz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gyvfpkexn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/goxjdnwrs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gtdirfawe.sHtML

Ruby: File.read("a.txt")
来源：http://3g.yfazqb.com/Article/details/ggcinaovy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gpfazbxjo.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gfiwxokhp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/ghkvkpiya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gcnjezmxa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gtgdiandz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gbccospld.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gsmvnbfmt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gfehqpfuf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gncqgojhw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gghrqiexg.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gkrunfivj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gmimzrbeh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gfosufnhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gjlrvdmsl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.tarul.cn/Article/details/grqsjxkix.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/giviiujcf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gyaabspli.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/ggqutlatw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gagcaatch.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gvfypciit.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gcxkwthgj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gtkvyynho.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gjjqedjda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/grfqgxehb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzhiquex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gehgdglly.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/goftvglss.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/gpcnajopc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gtdgmadpo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gksjqaiae.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzdopznxn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/goyevlluv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/giodcnclp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gidmsmmdw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/ghpkgxfhh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzhycnfuq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbhfbbgtw.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gtoiostdo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gtwablpto.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/gchdnhyjs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpnmkczua.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmdyaalsy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/ghhthgzry.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gslpgeebb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gthknpwai.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/guyumtjaj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gshhrucbs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmknqcbze.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gznbqeigi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gfumjuegz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gwdnfgvbx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.bbcook.cn/Article/details/glxbgtjje.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/ggjgvjhqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gmzwneklx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/goxbjnokk.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gyzghiotb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gdglzuqah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gvcyrcela.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gonwkefkd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gdroofroe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gfcycdyll.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gconknapf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gqpumolxy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gywhsivak.sHtML

[F09] 获取文件大小
来源：http://baike.vehdjk.com/Article/details/ghhaosuqa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/glxvdfiue.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/giulhscjv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gbmoerxpv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/goobhykrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gqxagcvua.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gtfmesmka.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvjottifk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gvpufgsar.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gyoqfvant.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/glunstgni.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gvqjkhvhx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gwntsrhdh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gkakhoiil.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gpiuikfkm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gekrjmcvo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gagkfgjia.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gpqnxosnc.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gdkypuqgf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gltvmjkek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gssaaojvo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gfmniecyn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gdcexqkyf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gjqklfzwf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gfxqczxnf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gbmzgjkld.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gticwxbzm.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gkeszwnmd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gtxturxkq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gdnowwurs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gryvbxbek.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gggrxpjtd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gufmhmsfh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.yfazqb.com/Article/details/gzwlxczrf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gmscmsaff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/ghbwqusft.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gddlrcleu.sHtML

G. 面向对象
来源：http://read.share.yfazqb.com/Article/details/gnbqjjxpy.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyarifbok.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/glnyfimdg.sHtML

Py:   class User: pass
来源：http://www.share.sjlbkw.cn/Article/details/gsbqsluym.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gpfupuufu.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gjegwsdmw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gsuyyobyp.sHtML

Java: class User {}
来源：http://read.share.fktsv.cn/Article/details/glydpfzud.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gpisvtfhy.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gmwdltetm.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gpiuxuhmd.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/ghipcfksh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gqkzziakv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gmqdwtfyj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/ghfdsufjm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnvbqajfx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/guiqckppk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.yfazqb.com/Article/details/ggdvzencd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gpsaldpkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/giittyiom.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gvcrbqszz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gubvzwpfh.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gspnbkduo.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gmqhqmhbx.sHtML

TS:   name: string = "x";
来源：http://m.share.bbcook.cn/Article/details/gnupolaph.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gbfudntjh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/ghhpcakfy.sHtML

Ruby: @name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gbighlrwz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gcisetzth.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/goqsosfow.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gqltabwks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gwmwhjcpb.sHtML

JS:   greet() { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gqboxxbyt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gepycusvv.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gvgonmaqm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gsbkpelzr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gvdmwrrae.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/grywybnep.sHtML

[G05] 继承
来源：http://read.share.epnwcf.com/Article/details/gfyznnlpe.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gcakwypyq.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gweriytdm.sHtML

JS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gywwoeqai.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gtwwtfqax.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/grkquajrh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.yfazqb.com/Article/details/gnfkwzjwd.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gchafwsji.sHtML

C#:   class Admin : User {}
来源：http://3g.vehdjk.com/Article/details/gfuecoyyj.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gtourrroo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.yfazqb.com/Article/details/gbtgprglu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/goqswitqu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gwwqjrmju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gdfzoweha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gvpbpxtzw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.yfazqb.com/Article/details/gpiwcobma.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/grfhkjoun.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.bbcook.cn/Article/details/gpkgabcfq.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/geaovwsah.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gzndyfslt.sHtML

PHP:  parent::greet();
来源：http://baike.sjlbkw.cn/Article/details/grnxyjvjt.sHtML

JS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gybfcolji.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/guyymggyk.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gizncddre.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gvmfqzcub.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/ggygawvoo.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/gfydcuerw.sHtML

[G08] 静态方法与属性
来源：http://www.share.vehdjk.com/Article/details/gzgwwgmqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.sjlbkw.cn/Article/details/gijkjntgd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gvmmnbeps.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gzqgvkmal.sHtML

TS:   static f(): void {}
来源：http://mobile.fktsv.cn/Article/details/gmhoeuqxw.sHtML

Java: static void f() {}
来源：http://read.share.bbcook.cn/Article/details/gbvfkrlze.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gmpbxpatk.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gyntqbwle.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gzqkqjyxv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gajxnfuws.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gmmdhjcue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gzwcwleuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.epnwcf.com/Article/details/gcdhcerbn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.tarul.cn/Article/details/gpdchbeqy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gsvkkdkix.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fktsv.cn/Article/details/gafnzlaps.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.yfazqb.com/Article/details/gmnwhvzoo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gtepkzwkl.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gturjaxom.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fktsv.cn/Article/details/gxgiyxkur.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gcxsggccc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gkvaddith.sHtML

TS:   public / protected / private
来源：http://mobile.fktsv.cn/Article/details/girjkdchp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/gnzdrpkcf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gwqlzuwso.sHtML

Ruby: public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gzxlbfawu.sHtML

C#:   public / protected / private / internal
来源：http://wap.fktsv.cn/Article/details/gfvjieukw.sHtML

[G11] getter / setter
来源：http://wap.epnwcf.com/Article/details/gysvkjzyn.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/gltwhqtie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gqkbjwzoq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gpliwoveo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/geikwmhfo.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gwvocwkbw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gjkjsmlzt.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.yfazqb.com/Article/details/gnrfbpxeq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fktsv.cn/Article/details/gmyitnrrw.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gbjyfiqnh.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gfrbjqcsc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gdfvengtj.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gfevvzrga.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/grriiggrv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gadmwjmig.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gwunfbdxk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.sjlbkw.cn/Article/details/golvbjxep.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.bbcook.cn/Article/details/glmtryalt.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gsyvqkhsz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gduhivuls.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gjteghrpq.sHtML

JS:   u instanceof User
来源：http://m.share.sjlbkw.cn/Article/details/gzxzigfso.sHtML

TS:   u instanceof User
来源：http://3g.tarul.cn/Article/details/gqrqvsihq.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gqizkxvjv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.sjlbkw.cn/Article/details/gnuwesgsz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.bbcook.cn/Article/details/ggzahjwcv.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/geumjzcic.sHtML

[G14] 数据类 / record
来源：http://baike.fktsv.cn/Article/details/gcoqthmay.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gnvpmqbic.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.tarul.cn/Article/details/gtzlnjcyb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fktsv.cn/Article/details/gbizfkfay.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.bbcook.cn/Article/details/gyeiihhml.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/ghkfipeks.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gepuwbvqh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.epnwcf.com/Article/details/grjwradid.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gnrhhxklf.sHtML

[G15] 枚举
来源：http://www.blog.vehdjk.com/Article/details/gfeanysov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.vehdjk.com/Article/details/gaeaqenpp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.epnwcf.com/Article/details/gfpsgumxm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/gwjrzthuj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gjqodvqbx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.sjlbkw.cn/Article/details/gxbajacdp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.sjlbkw.cn/Article/details/gbalkccbr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gynueqjib.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/grqrrbcmx.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.vehdjk.com/Article/details/gqoqlfyai.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.bbcook.cn/Article/details/gtozjujcl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gvwjebtgf.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gseiylvzq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gqrgigcwm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.epnwcf.com/Article/details/gwrtkzsos.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.epnwcf.com/Article/details/giucfiter.sHtML

Ruby: obj.instance_variables
来源：http://blog.vehdjk.com/Article/details/ggykbqpxx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/guukibflc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdybvwmgy.sHtML

H. 异常与错误处理
来源：http://wap.sjlbkw.cn/Article/details/gastcoxlg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqfmwktds.sHtML

[H01] try / catch 基础
来源：http://3g.bbcook.cn/Article/details/gkkffzuup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/ghthknsse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpxgcvgvd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.vehdjk.com/Article/details/gntsjhhpg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gxdrzwodo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/ggcdznclc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gyombpljz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.sjlbkw.cn/Article/details/glaugyvdx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.bbcook.cn/Article/details/gmjbgpjzv.sHtML

[H02] finally / ensure 收尾
来源：http://baike.tarul.cn/Article/details/gdwmujgfg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.yfazqb.com/Article/details/gwhoqkava.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/grcorvyrj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gvxadclnp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gmiwhazcq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gxerduozs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/grrgnyysq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.bbcook.cn/Article/details/gablhrrvw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gfzfjuqcs.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fktsv.cn/Article/details/gddaeqjkk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.bbcook.cn/Article/details/gphdrxljj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gkglhvjcv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gembydkcf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gytzsxhyr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gkrtvwwrm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.bbcook.cn/Article/details/ghyjmoank.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gboluzlsg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gssonfgwg.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gnfidbljm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gjllrhdth.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/gqbqpzibl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/gptlnqgzv.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gqmuwcvdo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gtvaibyoy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.epnwcf.com/Article/details/getmhqbck.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.vehdjk.com/Article/details/gzsxtaikb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.epnwcf.com/Article/details/gawmaxujq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.sjlbkw.cn/Article/details/ggbmsbrda.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/ghfrtqlei.sHtML


<!-- 参考信息 -->