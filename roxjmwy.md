代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gaisaxdjo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gersxxoqa.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gaisoweyn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjqxvebqa.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gkmdzyeux.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/gnouhsiqw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/goqzagufm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gxthlmngr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gdaygeelt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gainclhes.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.tarul.cn/Article/details/ghisirerf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gydvrptkk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gzqczmzsv.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/glyxrxxgi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gyvwlduye.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gighjqlmp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gavadwhva.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyucjbndd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/ggbkwpbko.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/godtnkmtt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/grutsudhk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gszblrhwr.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gttovtbrv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gxdovcnkt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gycuzmibc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gnswujkyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/glpqaguck.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/goqxdfaxk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gforhtwaq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gdhyzrqhy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/goqldtisc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gtsfkmrpo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gipotmlhs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gcwbktxgi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/grgbnmqkb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gvgvwoxqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/gsvdunxad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gielbjadr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gfaimclqd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gixzpcijp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.yfazqb.com/Article/details/gkcfzsiou.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gvonthfeh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gjdvmtzor.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmuepmttf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gssusfoqq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gbsikykqi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gttwiovuy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gfutubert.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gisdpbjsi.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gsyetuqqn.sHtML

Py:   os.remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gabkovnlb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gwofeuuyt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/giwgagcpy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkjqmlmhw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gxjsbfkgl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gsgtljiyd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gznokhjys.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/giiqceysr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gyrgomnlg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.tarul.cn/Article/details/grusqxhqj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.sjlbkw.cn/Article/details/gbtsjxmqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gvcuwohmn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gkkuetuvo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/grtugrlxg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gjrgftyyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gilixwcnm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gsorllzzu.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gzlccstan.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/ghubflnao.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gvpxmzmcr.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gplhftwob.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/gevumvzvd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/groshnimq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gpxcnlzdj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/gasyopiow.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gjidwegml.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gwdqodrgp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gqzxtyyag.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gwdkoblly.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gxassuwzu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gkmaoolgl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/ghlnsrvup.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fktsv.cn/Article/details/ghzqfywwq.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gqjogekng.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gxvphnomk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gvqpsaglh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gspnhganl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gkrqreozx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gvrioibza.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gukuedsqi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gzdghwdre.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/grrvqrvyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/giniztqxn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpohptgwz.sHtML

[F11] 复制与移动文件
来源：http://baike.yfazqb.com/Article/details/geoyioial.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gilzpebyk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gdknxgbqr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gbtumpfsb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnpmfhhxf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/grqhfbuoi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gpjbpgxlm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/grzjjfwhd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gstaappzr.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/glagiipkz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/guortpxhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gpttzopmy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gryvnzalj.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gbjudqyoz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.epnwcf.com/Article/details/gjxwviggv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.yfazqb.com/Article/details/gmprwveor.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gybynqnpj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gonytelsg.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gynzsvsfi.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/geggyppzm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gygmglxhy.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gkarkeasd.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/goklzumus.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/grtvkyrup.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gtbohzgth.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.yfazqb.com/Article/details/gkzrcafgn.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gvdutgvnm.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/garwrvrre.sHtML

Ruby: class User; end
来源：http://read.share.tarul.cn/Article/details/gcgsdupfy.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gluehfezi.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gybjrcjcq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gmjsnvsno.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gnhdqhzfq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grmqdndti.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.epnwcf.com/Article/details/ghymemxxr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gdcvbgieq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/guiomjmht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/geivzkzyv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gtuvvzojf.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/ghcjyshsx.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gjnplvsxw.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gnxyapfoz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gpscohxhe.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gunpbjgwe.sHtML

Java: private String name;
来源：http://www.m.share.epnwcf.com/Article/details/gjlipyqps.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.tarul.cn/Article/details/geueygruz.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gysypjhsg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gzwzlbxyj.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gldklxkho.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gykucijyw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gjvqhqihr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gbfzajaqq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gimmaxmks.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gxjoddlov.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gvoaglnif.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gyyjusknp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gteupscnk.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gkyvyzxeo.sHtML

Py:   class Admin(User): pass
来源：http://blog.epnwcf.com/Article/details/gojgnewdm.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/gapapjzca.sHtML

JS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gzgrzocvt.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gsjasxyzf.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gxasohiwc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gikacvbqd.sHtML

Ruby: class Admin < User; end
来源：http://wap.sjlbkw.cn/Article/details/gqgfxqxwh.sHtML

C#:   class Admin : User {}
来源：http://read.share.tarul.cn/Article/details/gxinezcob.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/gzfcfcrzu.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.yfazqb.com/Article/details/ggwuktrpq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gudnnuwvm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gpdsfuwcn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gyxaelkvj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gekyqxjde.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gkbjbapky.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gfekukjyn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/gbhsuwrfa.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gcneyobnc.sHtML

Py:   super().greet()
来源：http://mobile.tarul.cn/Article/details/gmtjiruzk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gprbrgmhy.sHtML

JS:   super.greet();
来源：http://www.m.share.yfazqb.com/Article/details/gbohsymny.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gvmltfour.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gpbapmwxa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/ghxgnjnvs.sHtML

Ruby: super
来源：http://wap.epnwcf.com/Article/details/gocbjcimd.sHtML

C#:   base.Greet();
来源：http://m.share.epnwcf.com/Article/details/gksosrafb.sHtML

[G08] 静态方法与属性
来源：http://blog.epnwcf.com/Article/details/gsppszdsi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/ghsfgncfi.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fktsv.cn/Article/details/guetscdig.sHtML

JS:   static f() {}
来源：http://baike.sjlbkw.cn/Article/details/gdmmrfmfp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gkjpiyllu.sHtML

Java: static void f() {}
来源：http://blog.fktsv.cn/Article/details/gmuvvtgim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/gfutyzibw.sHtML

Ruby: def self.f; end
来源：http://www.share.bbcook.cn/Article/details/grezlrkhm.sHtML

C#:   public static void F() {}
来源：http://www.blog.vehdjk.com/Article/details/gsckgowma.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gpngdwemt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gwodolgoh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.epnwcf.com/Article/details/ghzguqfsf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gfvggqxbn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.bbcook.cn/Article/details/gfjhtfnda.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fktsv.cn/Article/details/gilsvpcso.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gfjxqomxj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gbjvgutkz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gzabljdce.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/grnsjbfls.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.sjlbkw.cn/Article/details/gggwsaxdc.sHtML

PHP:  public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/galeeiyqv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.epnwcf.com/Article/details/gvygqwbby.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gmrzdrxbo.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gatzmgaiy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/glmvydtkm.sHtML

Ruby: public / protected / private
来源：http://www.blog.tarul.cn/Article/details/gcadpcrjf.sHtML

C#:   public / protected / private / internal
来源：http://3g.vehdjk.com/Article/details/gqzhewyxy.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gjtoimmph.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.bbcook.cn/Article/details/gdgbkasnm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbxfgtuvt.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gfigafoun.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gzazyenwi.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gqbfnrlcg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/gjgxvgixa.sHtML

Ruby: attr_accessor :name
来源：http://www.share.sjlbkw.cn/Article/details/gzfacnclr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gmqbonqve.sHtML

[G12] 对象转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gbfwtagsy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gaacjdmge.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gcinjdnkq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gucuhckws.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gjwghlolq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.epnwcf.com/Article/details/ggyocqrvh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gjwcawmoa.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gnomsnzvl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.yfazqb.com/Article/details/ggnyfodhg.sHtML

[G13] 判断对象类型
来源：http://wap.sjlbkw.cn/Article/details/ggozjnkdz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gcykehykk.sHtML

PHP:  $u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gmuttfhzy.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gmhexnpcu.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gopoqusin.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gbsqgkkbo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.sjlbkw.cn/Article/details/gksccfplf.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/giqgmgywr.sHtML

C#:   u is User
来源：http://3g.bbcook.cn/Article/details/gbbnxuotd.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/guyiatlwt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gsdvugekb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gvjoieloa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gaaicbste.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/ggpfujnen.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.yfazqb.com/Article/details/gxpjkkrxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.bbcook.cn/Article/details/gyilcnalb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.bbcook.cn/Article/details/ghzqtgyaj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/glupvogvv.sHtML

[G15] 枚举
来源：http://wap.epnwcf.com/Article/details/gxbyhwlsx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fktsv.cn/Article/details/gslrrnsis.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.epnwcf.com/Article/details/gemozlagq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.bbcook.cn/Article/details/gfmgcqhlr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.bbcook.cn/Article/details/gjtjhszvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gwfonddqa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gxyvuramq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.tarul.cn/Article/details/gsukmhqlb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.bbcook.cn/Article/details/gblkessop.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/gwvdymlbm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.sjlbkw.cn/Article/details/gxlgzxxcw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gwrelcsar.sHtML

JS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gjughzsuj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gfnkhxsyz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gmozkkpyz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.epnwcf.com/Article/details/gcbgbzsmn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gassnwvrw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gzydvndxt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdhwvvrra.sHtML

H. 异常与错误处理
来源：http://m.share.tarul.cn/Article/details/ggtxpedzm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxyvwoujj.sHtML

[H01] try / catch 基础
来源：http://wap.bbcook.cn/Article/details/giglrkeca.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fktsv.cn/Article/details/ggcccjzdz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fktsv.cn/Article/details/getcejtfm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gjxzmyosz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/guszggory.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.epnwcf.com/Article/details/ggxgxodiu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.yfazqb.com/Article/details/gsezpgwaj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.tarul.cn/Article/details/grrxtcrje.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gptgsxadz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.yfazqb.com/Article/details/gclxtlzvd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gndteehim.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gnvklywjm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/ggkqdgugk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/geggneehb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gcblmvaan.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.epnwcf.com/Article/details/gzszfhgpj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.bbcook.cn/Article/details/guprsnpxg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gyzofkyxu.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/gfqrzfgju.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gcofdaibv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gfaqmhzpv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/ghatzgoqt.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fktsv.cn/Article/details/glkblsgtm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gptivzkbg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.tarul.cn/Article/details/gbxicrsvx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gyngwglfv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gelkubshr.sHtML

[H04] 自定义异常类型
来源：http://wap.tarul.cn/Article/details/gbvtjheqz.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.tarul.cn/Article/details/giatpdrfi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.vehdjk.com/Article/details/gxwdqmgys.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.yfazqb.com/Article/details/glalpvssl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gviotfizr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gmuftmrzz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fktsv.cn/Article/details/grnwvuajs.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.bbcook.cn/Article/details/gtstnopmt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.vehdjk.com/Article/details/gsfypvmuu.sHtML

[H05] 捕获特定类型
来源：http://www.share.fktsv.cn/Article/details/gnruulevj.sHtML

Py:   except ValueError as e:
来源：http://3g.yfazqb.com/Article/details/gnojicurl.sHtML


<!-- 参考信息 -->