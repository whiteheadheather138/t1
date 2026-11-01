代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/ggstmjnkg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gcassnfdg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/grjltfpfi.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcdvhlkdz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/gcljljdxy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/ghhqgmvmk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gkmkgozmm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/ggazdtflh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gjfgjkufv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/giqiuboei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gorxkttlw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gtytfxjha.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/gxlalhltw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gixptkitw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gyjzvjlsm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gnczadbfy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gkjeuejzf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnzmdcjmg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gpnavtmhk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gjoflditv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/graiiwqtc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfepmnxps.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gclpsnpta.sHtML

[F04] 追加写入文件
来源：http://baike.tarul.cn/Article/details/gslsldfxj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gihtaqtzo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gfdkhzrmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gjgghktoj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gealicggr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.vehdjk.com/Article/details/ghduhzskc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gfdjdfpqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/goznpfnrw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gkdebnjai.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gpwuhwsvi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gfhxuppvl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gbiczcqam.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqchqlmkk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzloyzidp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gobsdxuut.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gtoacaatk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gzzbifayb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gkakdrvaa.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gxxehozen.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/ggedjpvrr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/ganxieeha.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gjurdmqgw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/ghizzadsj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gwnhvusoi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gbnnazzqc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzrefolml.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.tarul.cn/Article/details/gwqtsvlbf.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gzzamtsax.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gniktdflj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gttdvpfja.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gevtiyznv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gelwzysag.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.epnwcf.com/Article/details/gvwleuzrh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/goutkzfzu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/glnizzqoj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/geeksrxcq.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/gqhbqkgxf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/gvcjvlorw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gtipagbnk.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gqtindzed.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/govuilovt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/givcxzeez.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/gsbzpasag.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gdngcinon.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gqrqbljde.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/ghlaujnbs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gpaqdxxit.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gndvhzwey.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gczrgfoku.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyrlzrzo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gmnaiitis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/gtxtbcduc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkuvbvlxh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/giymkmiiz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gyxuealmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gjdewsbti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.yfazqb.com/Article/details/gbndgajef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gboveoxni.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggnqyxilx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/ggcjwhuyj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gaewuxlqe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghwuvfmrg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gjpyrzapd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.yfazqb.com/Article/details/ggdehhefs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxammsiju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/gxtjkiwgd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfofodhdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ggkrtqqde.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.epnwcf.com/Article/details/gsyifxkuw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.yfazqb.com/Article/details/gqjjrxibn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gylgieqbz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gkmnmoger.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gkttejwxr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gyjyjnuyx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.vehdjk.com/Article/details/ghlklhrss.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gosrqdnqc.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/ggcsjjoqz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gxdmicmrx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.epnwcf.com/Article/details/gmluvvaot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gltudwnrc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.epnwcf.com/Article/details/gscxtgter.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdrjmfufi.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gtldgbvsu.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmngprveu.sHtML

[G01] 定义类
来源：http://wap.epnwcf.com/Article/details/gacdlzwoc.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gpjmphhlv.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gwdlhggcq.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/ganjvqzzs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gfcaguvne.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gqhuwowgz.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gjrzhafnm.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gkavwsusz.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/gsoelpxsj.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/gxuidyrag.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gxcihjljv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/gxgmdaypk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.tarul.cn/Article/details/gagyljdal.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gjalcgppl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/givimyvqi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gqitwfcwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gglordheu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gehavmnxt.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gqyvagzow.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gkoxxjijo.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gmpfrgqhf.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gwbcgqsbx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gluedbhgz.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/grpnxwhvq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/ggjnyvcxd.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gzsezotml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gjfmwaicv.sHtML

[G04] 定义方法
来源：http://www.blog.yfazqb.com/Article/details/ghdonopqc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gzlrbxxgn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gpczszkbn.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gnohyatvd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gqdebblru.sHtML

Java: String greet() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gocvltwrt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/ghjyrthff.sHtML

Ruby: def greet; @name; end
来源：http://baike.yfazqb.com/Article/details/gilvcngjt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/galcrvctb.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gmvucxmxp.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/gadrbutre.sHtML

PHP:  class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/guqpnixzs.sHtML

JS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/ghtozrmgp.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzxmtesp.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gujajfwyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.vehdjk.com/Article/details/gtuvjpimr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.vehdjk.com/Article/details/gytrhymbw.sHtML

C#:   class Admin : User {}
来源：http://blog.epnwcf.com/Article/details/gnjzcgncm.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gutjwqtoy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gygsuneby.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gjchhaszf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gkbydvoad.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gktfakdjv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/guhvktiof.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.yfazqb.com/Article/details/gxyfyhbzu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.vehdjk.com/Article/details/girbsdorr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fktsv.cn/Article/details/gtdpeswyg.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/gzhebdpty.sHtML

Py:   super().greet()
来源：http://m.share.bbcook.cn/Article/details/gpbwydxvh.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gjijkumjd.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gjdbngkcd.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gmrtywugl.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/grywtdyhq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/ghhgvnino.sHtML

Ruby: super
来源：http://3g.yfazqb.com/Article/details/glmdydsib.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gzetzpgyh.sHtML

[G08] 静态方法与属性
来源：http://www.share.sjlbkw.cn/Article/details/gpghktvau.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fktsv.cn/Article/details/gymrtjjkz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gukatstzn.sHtML

JS:   static f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggrpvkwxt.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gcyakdgai.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gjayjzydu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/ggqklnnmf.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gcunnlwnv.sHtML

C#:   public static void F() {}
来源：http://www.share.yfazqb.com/Article/details/gefpvmaue.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gxfknxcoi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gjfhgcixq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.epnwcf.com/Article/details/gkyfycvcb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gyrzxmhiu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/geqihkbhv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gwhmpsldz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gzgcbdnbk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.sjlbkw.cn/Article/details/gygyfjica.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.yfazqb.com/Article/details/gcfifxpkg.sHtML

[G10] 访问控制
来源：http://www.share.sjlbkw.cn/Article/details/gmchtswtt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.epnwcf.com/Article/details/grksxfvdz.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gktmnvzzm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.sjlbkw.cn/Article/details/gslthuojg.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gjlsvfbmg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/gebqkkkqk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gtfptoanz.sHtML

Ruby: public / protected / private
来源：http://blog.yfazqb.com/Article/details/gwrfxzddb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.yfazqb.com/Article/details/glnmmcejr.sHtML

[G11] getter / setter
来源：http://read.share.vehdjk.com/Article/details/gzqztdbpz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/gozbscpjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxfrlpzle.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/goiwpdaly.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.tarul.cn/Article/details/galaxpckt.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gzmvxtwcv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gqkxfjhbo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gsbunkglf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gnewbtmtx.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gzwcyfyir.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gqpggccpq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/ghajawxok.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gioxmwzfi.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gosvkpqim.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gttjwfsef.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gpugurtpu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gyuxnzfdh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gdfesggry.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gowbterxq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gbaotvmob.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/grktqroby.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gkfakzgdc.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/goslbdtlv.sHtML

Java: u instanceof User
来源：http://wap.yfazqb.com/Article/details/grkyjpqop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gkojodhbq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.epnwcf.com/Article/details/gnqpkwlut.sHtML

C#:   u is User
来源：http://blog.epnwcf.com/Article/details/guofzqyds.sHtML

[G14] 数据类 / record
来源：http://read.share.yfazqb.com/Article/details/grizghnrq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.yfazqb.com/Article/details/guxdsfqep.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.tarul.cn/Article/details/gfhbxmzyl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gnycxucxm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.vehdjk.com/Article/details/gujsqxnkh.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqqyiugha.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fktsv.cn/Article/details/gksdwqdld.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.vehdjk.com/Article/details/gpvglwvct.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/grbspggnd.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/ghbgzdzmx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.sjlbkw.cn/Article/details/gyvvdzotz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.sjlbkw.cn/Article/details/gmgutskdz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/ggskvkqjm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gbkncizgc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.sjlbkw.cn/Article/details/gohmpuzam.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gzplfcqht.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.sjlbkw.cn/Article/details/gmquysgqf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/glfmbaynn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gkunjbbjb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gpgtxxbrm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fktsv.cn/Article/details/gyrdwqdxz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gklzdhneo.sHtML

TS:   Object.entries(obj)
来源：http://baike.bbcook.cn/Article/details/glpyxrkal.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.bbcook.cn/Article/details/ghyxqxhot.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.tarul.cn/Article/details/gjacoqlvt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.epnwcf.com/Article/details/geilokaeg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gfrvuhrzh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gutidcrwr.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gqmwgsmpq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggscasfgg.sHtML

[H01] try / catch 基础
来源：http://m.share.fktsv.cn/Article/details/gizhusvsj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fktsv.cn/Article/details/grqaulprh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.vehdjk.com/Article/details/gcfshqjvx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/ggpztvddu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gktbxrckc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gclmvibkm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.yfazqb.com/Article/details/ghrconqlw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/gegtjyuzl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gqovjrtdx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.vehdjk.com/Article/details/gscxvzirw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gtvcpknmt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gqolzkvju.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/ggplzczbz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gnevmslvs.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.epnwcf.com/Article/details/gqxessiwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gruyaykgo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gqtsyszzo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/ghppowtmj.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gcmgjbmiq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/ggtzubozq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gxsgoqnhm.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.yfazqb.com/Article/details/gzceglonh.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.epnwcf.com/Article/details/gpgszbdyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gydecmkgp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.sjlbkw.cn/Article/details/gnmzpcokl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/guqeyaftg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gauduohgp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.sjlbkw.cn/Article/details/gubpbwcvr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gpehnjruk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gpsrgiwzo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.bbcook.cn/Article/details/genakwwaa.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gpkvhluog.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grqsyfzuy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gjvwntqtg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.yfazqb.com/Article/details/gozmzcsti.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.yfazqb.com/Article/details/gepdpxoct.sHtML

[H05] 捕获特定类型
来源：http://blog.vehdjk.com/Article/details/gateywxnh.sHtML

Py:   except ValueError as e:
来源：http://read.share.bbcook.cn/Article/details/gnrwzguol.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.bbcook.cn/Article/details/gvlixibao.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gnweruhtb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fktsv.cn/Article/details/gxhnanxvo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fktsv.cn/Article/details/ggvorcgow.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.epnwcf.com/Article/details/grrqrifop.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/ggfukrbgg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/gkzyvczoo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gvbjcarzy.sHtML


<!-- 参考信息 -->