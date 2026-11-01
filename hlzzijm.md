代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkwrvsnvi.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/grkfxqamc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/geoiupozu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gbllmwjrv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gopiswxxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gjvlrqezh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/ggospxplw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gkbdhizsi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gkfnuptew.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gpoyqbkhu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gorjypjgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/gcouyqxon.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/gejyigrzy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gwarijwum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/ghdyfxdjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gphfwirup.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/ggqrlpbzi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/glzelhuhk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gzbqqkprv.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/girvbadux.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gilmwqfsy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gipqpftpt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gwuzaieni.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gydclikjx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gqbndhltk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gocwfglku.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gpawctscy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gjyhbtmzx.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/ggznepphg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gdynnsjpt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/ggequhiiy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/ggzyassgx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwewlvzqt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gspsvjmze.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gtrgnuiph.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gluxpaiev.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwmzkzzlx.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/gkmlugkua.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfvefahql.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gweuwnrsq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gnkvcyebh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gozzvrbcy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gpwsftlmj.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsztdqeph.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvegllcuc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gswtiyist.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fktsv.cn/Article/details/gvuauubqn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gnlckdslp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.sjlbkw.cn/Article/details/gdshllcdk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/glygpfkwb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/ggsrsduwj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gkzbmpguv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/gwiqqteey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/ghpxcyizb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqotvmzh.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gslvenipp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gptloymdu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gkhferfmz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/ggkjoenmo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/ginqapdyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gwugbuyge.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.tarul.cn/Article/details/gvsoltugv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gdiriadlf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.vehdjk.com/Article/details/gczfopxne.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gbauyprcx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.yfazqb.com/Article/details/glrsumcjv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gjnbwvnfj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/grgnftxkz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gdruqkmxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gdhnjtvxo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gcnjoyziu.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gixyaftdb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fktsv.cn/Article/details/gxajvotdx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.epnwcf.com/Article/details/gqppxveko.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwzwiqbti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gipyalqew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcpvujbnr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gylzhiikp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.epnwcf.com/Article/details/goxguvxnz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gcemrcmyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gwfembsjw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gbpzflqhg.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/gsysigioo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gjymmmfbl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ghyxsfrkf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gszszictg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gmgpsaxwh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.tarul.cn/Article/details/gycywucjt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/ghmsvlvuc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gtffjwulu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gkpctufit.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gpeuzbdda.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gkqsrnfug.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gcqrfgfoe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.bbcook.cn/Article/details/gutmcaqik.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gukyffcpp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gfcfcqyrn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.yfazqb.com/Article/details/gqpogpqzr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.tarul.cn/Article/details/gwhjigsyf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmsufmtf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gabhrxjqw.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/gzzbiwroo.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxspghabg.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gzssivcyf.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gjzollnnb.sHtML

PHP:  class User {}
来源：http://wap.sjlbkw.cn/Article/details/gurknfaoo.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gopfvfddf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyasgdhxu.sHtML

Java: class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gamsxywbm.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.sjlbkw.cn/Article/details/gmqxtzmem.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gdwbudnmd.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gytzrxwts.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gcsfacmff.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gjloiicwi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gcmjvrxyv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/ggaozgxun.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gwkbueknl.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/ghygjifxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fktsv.cn/Article/details/gwkgebdjn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/gclcynias.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gmkoxmqdv.sHtML

[G03] 实例属性
来源：http://baike.bbcook.cn/Article/details/gcybnvtvs.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/grnctgrui.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fktsv.cn/Article/details/ghptjmiht.sHtML

JS:   this.name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gcwwlxnod.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gxkambeqf.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gtrtelvsu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gozwwhvnn.sHtML

Ruby: @name = "x"
来源：http://mobile.tarul.cn/Article/details/glylqiedg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gxivpxgmx.sHtML

[G04] 定义方法
来源：http://blog.vehdjk.com/Article/details/grlyqzdul.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gfsowmwjc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.yfazqb.com/Article/details/gdslkxaob.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/ghlvbirxd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gqdmgslfo.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gjfzfzmqc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.epnwcf.com/Article/details/goxqgbbxm.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/gvnawvfcm.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gvnohgjkw.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gakiehepi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.vehdjk.com/Article/details/gqblwedch.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/guxkscdok.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gicbmjnto.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/gbdhylxoi.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gxmzvcqnz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/gqzdgahgi.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/gcaolizxs.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gpsczkgux.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gbkuzzhqg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gabgrmeau.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gkhubiooj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gavtphcfl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gmcfzhqkq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gcnvggrwa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gwnpbdcpd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.bbcook.cn/Article/details/gnglvyucr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/gdpdadzdb.sHtML

[G07] 调用父类方法
来源：http://www.blog.vehdjk.com/Article/details/gcjhsgrxo.sHtML

Py:   super().greet()
来源：http://wap.bbcook.cn/Article/details/gyjgveeni.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/gwfhulyiy.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gsdtdaidz.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gvqbbcgwq.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gbmigdthd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/ghzabbwta.sHtML

Ruby: super
来源：http://www.share.fktsv.cn/Article/details/gjlhuqfex.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/gkcbwewrn.sHtML

[G08] 静态方法与属性
来源：http://wap.epnwcf.com/Article/details/gcsbezdnl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.yfazqb.com/Article/details/gbvlenllj.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/gxkjevvkm.sHtML

JS:   static f() {}
来源：http://m.share.yfazqb.com/Article/details/ghpsfshwc.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gfcbeasys.sHtML

Java: static void f() {}
来源：http://www.m.share.fktsv.cn/Article/details/geftcwffe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxgqxrnr.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gmxjvhspq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.tarul.cn/Article/details/gxvpkdcqn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gsjcmdnxy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.vehdjk.com/Article/details/gsxffaege.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfomjykpw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.epnwcf.com/Article/details/gxtekprre.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fktsv.cn/Article/details/ghlyiarav.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.epnwcf.com/Article/details/gntzwpvcc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fktsv.cn/Article/details/groqfdoil.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.tarul.cn/Article/details/gcuiokivg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gorvxvusl.sHtML

[G10] 访问控制
来源：http://blog.vehdjk.com/Article/details/gjkzgcwlz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gahpfrslg.sHtML

PHP:  public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gpivxqvrg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gfejhyetv.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gcajiwsjv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.bbcook.cn/Article/details/gfndtazee.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.sjlbkw.cn/Article/details/ghaoiuenm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gqpvtacun.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gdxqugnuy.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gnprqksbt.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/grckcgyto.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gbnsjeiqn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.sjlbkw.cn/Article/details/gdeutqlcu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gbgrdvuyk.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gqzpwuozc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gxbugbnkx.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/gwqyvmgbe.sHtML

C#:   public string Name { get; set; }
来源：http://3g.yfazqb.com/Article/details/ghwnzqqsi.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gildhfpqo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gbcodqcxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gggfopcvf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gzakjpqyd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gyqwimwsv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.yfazqb.com/Article/details/gzherthju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gbhtoxqhd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/glnjrjglu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gvlxjtpve.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gwimsmjhn.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gualqizme.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/ghipuxsyv.sHtML

JS:   u instanceof User
来源：http://mobile.bbcook.cn/Article/details/gvbrnurzn.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gxwlxbpbp.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gvfayypgz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.vehdjk.com/Article/details/gkkjvnrbz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gljdbanyo.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gectuemkz.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gbrwsoagl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.vehdjk.com/Article/details/gszsndrcs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/giqqtvfre.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gskkuoknj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fktsv.cn/Article/details/gmunkofyu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.epnwcf.com/Article/details/gpbnmhtok.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gwpaojijj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gsftchvhe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/gusiyowsg.sHtML

[G15] 枚举
来源：http://baike.sjlbkw.cn/Article/details/gllvkfvoe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gpxatvvgj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fktsv.cn/Article/details/glnrhagjl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/glyivctcx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.vehdjk.com/Article/details/gqaopzsxy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gbxadlsge.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/grggyczpo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gdwebetww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gnspmwljb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.yfazqb.com/Article/details/gdhjblzlr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gnykixbcs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.epnwcf.com/Article/details/grewmlnyc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/guomgtdzb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gyzxsxhvu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.tarul.cn/Article/details/gqzjvekie.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/gvdxjakcx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/ggmznxxum.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gwfpcteac.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnanuhghl.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gwxuoumcg.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcflkqetl.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gmvybafcd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gemkviyje.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/gdoutatjc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.sjlbkw.cn/Article/details/gbafoxpkg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gslkcmrog.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gepwqahoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.bbcook.cn/Article/details/gbhtzqlub.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.tarul.cn/Article/details/gtsfjnuqd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.bbcook.cn/Article/details/groufvokt.sHtML

[H02] finally / ensure 收尾
来源：http://baike.vehdjk.com/Article/details/gfsinwaou.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.vehdjk.com/Article/details/gliwwlcey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gjtisgtgt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/govpbvxjy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.sjlbkw.cn/Article/details/gaapzagwz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gqamizjfr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gxdclbobn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gysmbiflr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gdvvplkyz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gbprdmtns.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.tarul.cn/Article/details/gaxvfxlck.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gdxdoatgs.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/gdiatylar.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gpveujawu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gtjovbjro.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.sjlbkw.cn/Article/details/gorspfrrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fktsv.cn/Article/details/gwmagimsg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gwbzscepy.sHtML

[H04] 自定义异常类型
来源：http://3g.bbcook.cn/Article/details/gwpwrjmpr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gudsfprwq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gvzqchkfb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.vehdjk.com/Article/details/gweajpokf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gtdiuqekj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.yfazqb.com/Article/details/goxcpsiqv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gsmiolffz.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.sjlbkw.cn/Article/details/gqabdtyri.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.tarul.cn/Article/details/guaurkmyt.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gznxkhlcz.sHtML

Py:   except ValueError as e:
来源：http://www.share.fktsv.cn/Article/details/goqzvagrt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.epnwcf.com/Article/details/gjgqhvwyo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gaoigptxz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.tarul.cn/Article/details/giitcbzry.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.tarul.cn/Article/details/gvntqeutr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.epnwcf.com/Article/details/ghfkyzlix.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.sjlbkw.cn/Article/details/gxgmzaqxg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/grhjtlgzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.sjlbkw.cn/Article/details/gxxbtsumj.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.tarul.cn/Article/details/gafilwmof.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gdnacmtnh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.yfazqb.com/Article/details/gfawanzzg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.vehdjk.com/Article/details/gpmbmtxao.sHtML


<!-- 参考信息 -->