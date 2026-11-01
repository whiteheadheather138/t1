代发 wailian999

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gjngfjkty.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/gjluxxowp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gtrlqixgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/guitjadum.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gujyhtpux.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/ginpomgsa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gnkmmxlrf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gnldsuqmg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/gfsqogyyo.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gzzhikakj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gkgidqsnq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.tarul.cn/Article/details/gjqbzalld.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gzegwdmpg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gfykzensf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gdwtbegak.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gymiqwxau.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gikrwpdok.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.epnwcf.com/Article/details/gmuklyddu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/gfwxdttck.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gusbloisl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gpkoxzftd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gsnxzzzmo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/ggslhaxnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gtikipwhl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/glnlbwwyc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gnghtjngm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gurhjpwiz.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/ghflmqnbx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gkydodhnb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.epnwcf.com/Article/details/gbsqapyxn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gevjbfmor.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gzatebfgs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/ghyfzujcv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gxmfwerud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsgwdiku.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/goiunrpju.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/gbygqknos.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gjitmeyzd.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gusiqnpzy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxumkijmp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/grfdyhqbe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/ghkfcvfqx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gjgqvldtd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gredsikih.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gbsmxcdjz.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gycmviphl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gdprtznhg.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gbowarcny.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gurqpenqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/golevxyls.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gyjxsptfb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gisqnzkww.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcypprimc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gfqjxpfna.sHtML

[F07] 创建目录（含多级）
来源：http://wap.vehdjk.com/Article/details/gtbplfonq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gnlrdcdeo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/ggfaomsae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gvfvprfjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gopzljmwa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gbejdtoor.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gipleoabk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/guylzdfbf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gqhlietfs.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/giuvoionn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gxevkqldo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.yfazqb.com/Article/details/gwltcbtrf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/goeaprsqn.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/grrfqyuli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gptkosius.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gjriaswkj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gpkahyibf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gfqommugn.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gbtqogqlj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gdnjagslp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gtithnppa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/gpmfdcubc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gpospubph.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gjrnchvmu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gydzhmxhb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmwkjgqoo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gzjoprfzz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gszelgivt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gniybrcce.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gdpehsddk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmjrpjswa.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxoxavoze.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gusbaqiry.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gmqyanrtd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggcshuimr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gzkoymkxw.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gkfppjotl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gwsghxuqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gvpkzbmcu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gzoferqrh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gmnrxsela.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gaulvosip.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/ghfihafyv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gkzcsdjen.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/goekpqgnu.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gdnlvnmcy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gqhzpasrx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.yfazqb.com/Article/details/gihbhhmqt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gcimtrplx.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gtyeodiwq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gprwmqpth.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fktsv.cn/Article/details/gutpfiwoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.bbcook.cn/Article/details/gsipxrlbm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gfbqsdmmw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gsoceirev.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gihulupvh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjfvzhprc.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gbuctjbrn.sHtML

Py:   class User: pass
来源：http://mobile.yfazqb.com/Article/details/gznlvduzj.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gspvaeent.sHtML

JS:   class User {}
来源：http://www.share.epnwcf.com/Article/details/giwjiejow.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/girbkngyi.sHtML

Java: class User {}
来源：http://blog.tarul.cn/Article/details/gaoiopfyw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/giaoqfxqv.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gzmxowghr.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gigtlfsss.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/gqsmtvbjw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/gugvpkkov.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.vehdjk.com/Article/details/ghajujhym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/ghexrqpxj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.epnwcf.com/Article/details/gcziehprm.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gkkbtoqub.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.bbcook.cn/Article/details/gnbdhubea.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gtnfkevsl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/gszzpmuvj.sHtML

[G03] 实例属性
来源：http://www.m.share.bbcook.cn/Article/details/gwhpibjzd.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gsmkrfahi.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gnwfhvhvg.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gjawgwpaf.sHtML

TS:   name: string = "x";
来源：http://wap.vehdjk.com/Article/details/giljqqsae.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gcjumnyve.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gauegtxgp.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gzjnxzfuj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gtbytqyud.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gfymkhugg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gqobnjbxo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gviznwrsi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/ghwqcfbzl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gfghzpcsm.sHtML

Java: String greet() { return name; }
来源：http://read.share.fktsv.cn/Article/details/gvqvtwzqm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gqzsqkwxf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/glgjxxhky.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gzbqknowr.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/giakpbegl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/giwldnhjt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/ggnsrwtkz.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gaulbmouc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gwvvalczg.sHtML

Java: class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gtrbspuuu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gbweggsqd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.tarul.cn/Article/details/gohjznpfs.sHtML

C#:   class Admin : User {}
来源：http://m.share.bbcook.cn/Article/details/gnkmjdxde.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/ggkkvlsmy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gjjasjpnc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gwqzhhmwj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gcvlajimc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gzhhvtlfc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gzvbwertz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.vehdjk.com/Article/details/gxeqphfyg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/gawwxrglu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gvxodbuoa.sHtML

[G07] 调用父类方法
来源：http://www.m.share.epnwcf.com/Article/details/gsyzijhhj.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gnzczbzbm.sHtML

PHP:  parent::greet();
来源：http://wap.yfazqb.com/Article/details/gnwprrvgu.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/glxrkonmv.sHtML

TS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gvftymgin.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/grbbmanhf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gpafwpqly.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gsmnrnhcv.sHtML

C#:   base.Greet();
来源：http://wap.sjlbkw.cn/Article/details/gtmpdrrsp.sHtML

[G08] 静态方法与属性
来源：http://3g.sjlbkw.cn/Article/details/gixeagocy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gbvuzvace.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaybwfkov.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/gohakqwkh.sHtML

TS:   static f(): void {}
来源：http://baike.epnwcf.com/Article/details/goxmcmpjt.sHtML

Java: static void f() {}
来源：http://3g.vehdjk.com/Article/details/gsjwuwhol.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gdkhzeiil.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gployjfkj.sHtML

C#:   public static void F() {}
来源：http://blog.epnwcf.com/Article/details/gklurmuhy.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.epnwcf.com/Article/details/gobblxnyb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fktsv.cn/Article/details/ghhgvoedx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gucdbplao.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gwapbbcaa.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gpyxygxqb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.tarul.cn/Article/details/gevgtjoxs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.tarul.cn/Article/details/gwpvxjemh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.tarul.cn/Article/details/gfaueybew.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.sjlbkw.cn/Article/details/gbncktbtu.sHtML

[G10] 访问控制
来源：http://baike.fktsv.cn/Article/details/gxmciqkyz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.tarul.cn/Article/details/gpjpzgnqz.sHtML

PHP:  public / protected / private
来源：http://3g.tarul.cn/Article/details/gzhkqdrhw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.yfazqb.com/Article/details/gjwxaeqal.sHtML

TS:   public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gyoaddjcm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gnovfmony.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gtmmwxcja.sHtML

Ruby: public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gllelmart.sHtML

C#:   public / protected / private / internal
来源：http://blog.sjlbkw.cn/Article/details/gpduegzxj.sHtML

[G11] getter / setter
来源：http://baike.sjlbkw.cn/Article/details/gtolujilo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gsyxciclu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/gwrjrqhqg.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/ghqkoktji.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.tarul.cn/Article/details/gtmpjclmq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/ghldbvctz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gciznftza.sHtML

Ruby: attr_accessor :name
来源：http://blog.bbcook.cn/Article/details/gwcgtmrtn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.tarul.cn/Article/details/gsyptrteh.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/geqkxyblf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/guaqlkmxe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.yfazqb.com/Article/details/gbsujhfhr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gixexixyh.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gwjarymxw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gioxdqfvh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gcjjmotbb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.vehdjk.com/Article/details/gcrgtswdu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.yfazqb.com/Article/details/gaamggfzx.sHtML

[G13] 判断对象类型
来源：http://3g.tarul.cn/Article/details/gdcgxbhsw.sHtML

Py:   isinstance(u, User)
来源：http://3g.epnwcf.com/Article/details/gjzecdihv.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gvvfkcwgg.sHtML

JS:   u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gymhnqkqn.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gwgzkyrek.sHtML

Java: u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gjcgxnryz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.bbcook.cn/Article/details/gtfzqktra.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fktsv.cn/Article/details/gqbcgstak.sHtML

C#:   u is User
来源：http://m.share.epnwcf.com/Article/details/gmrcoibag.sHtML

[G14] 数据类 / record
来源：http://blog.yfazqb.com/Article/details/gzlkvalri.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.vehdjk.com/Article/details/gcflmnvlv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.vehdjk.com/Article/details/gnhnjhuns.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/guugpicwt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gyqlgkwue.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/ghtmtxizg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.vehdjk.com/Article/details/gpzkmvosp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gshpxbcnk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/glrbcdbzr.sHtML

[G15] 枚举
来源：http://www.m.share.epnwcf.com/Article/details/gmvfqnjby.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.bbcook.cn/Article/details/gjqtiulrj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fktsv.cn/Article/details/gctawzifp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fktsv.cn/Article/details/gvycpsxdn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gzsosikhe.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/ggbczkwsx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.bbcook.cn/Article/details/gpqhenoxz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fktsv.cn/Article/details/gtecczzfx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.vehdjk.com/Article/details/gseoaunvt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.vehdjk.com/Article/details/gwwsthoph.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gogdgmdmc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.tarul.cn/Article/details/gsshjynvs.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggkbbojfd.sHtML

TS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gzylpxfbr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gcyxoiupf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.yfazqb.com/Article/details/gwmlxwxbd.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gssaxrdaa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gqhfrzlxe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsvrbbiod.sHtML

H. 异常与错误处理
来源：http://m.share.bbcook.cn/Article/details/gojlipvtn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gaaevglqh.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/golfoeqeq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.vehdjk.com/Article/details/ggofmonge.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/ggxjgoanf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gzqnbuffk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gmdxmawlv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.tarul.cn/Article/details/gucwzydbv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.tarul.cn/Article/details/gdooejqbq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/gubjikzfh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.bbcook.cn/Article/details/gdszufear.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/ghjjpsjbf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gfzvfroda.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gordctszq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gipzhmuqd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkkpwslwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gzmpsbcjd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fktsv.cn/Article/details/ghsmjlaav.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/glowogxjy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.vehdjk.com/Article/details/gopvbzrrk.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/gxzmkwezd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gybdlprgk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gywvjqgnm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gwmgabsiw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gfewwndof.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gvhfbtxxt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.vehdjk.com/Article/details/gzczdhsro.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/goewqbisc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gwvbedonh.sHtML

[H04] 自定义异常类型
来源：http://wap.sjlbkw.cn/Article/details/gkfkcxhxp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fktsv.cn/Article/details/gpjacacqd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gikkdeadb.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.sjlbkw.cn/Article/details/gadscylpf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gjejnzhyh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gdiopbokq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.epnwcf.com/Article/details/gbhsxbvyh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.yfazqb.com/Article/details/genbegsms.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqswhlvcp.sHtML

[H05] 捕获特定类型
来源：http://3g.tarul.cn/Article/details/gzvzusttr.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/guvsflfeo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.tarul.cn/Article/details/gqxsffaio.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gxqidimdz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/ggxbqoqbp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fktsv.cn/Article/details/gjhvohkyc.sHtML


<!-- 参考信息 -->