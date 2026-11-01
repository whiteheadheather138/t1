代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gpdjzsymv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gckmualvd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gwkedryvl.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gnofzhtkl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gabmairmn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gafqklqox.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gznctiywu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gutivkdgh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gzbogkxii.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/guuizermx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gkfxygwfv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fktsv.cn/Article/details/gmowyqjdk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gkfzryrbh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gzfwdioto.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gpjaojqvi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gonzmfqtb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/ghhsxzooy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gmytbihog.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gyezzddnf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gqhoddnpt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqicbircj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/ggxlddcja.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/guzrksknu.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gmzobpbom.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gconxoyla.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/gcfibbhnl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gctgkllue.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gkniizxhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gjfgpmkaj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gcmhnlnkl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gghubdmfd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/ghmndywll.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gwcvlwohr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gdgwsdfcd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/gvmzwgaxm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtbbdgzok.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gqoiscutm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gnyprppht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gwczomjej.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjfweboko.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gajmvpmza.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/giryeatsh.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gnjgvomei.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gdzhwpefj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/givtymesr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gknbhyfxm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gjwzeqfre.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggcanzqpe.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.tarul.cn/Article/details/ghtwutrtk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.yfazqb.com/Article/details/gchjarhhu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/glkpaencf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gsccaskqv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gzvhnklgw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/giwmmrusl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gblwrpoac.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gxotyagfu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/gqmaswwrm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/gwxqcqlek.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gxcyjedeb.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gowmseypu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.bbcook.cn/Article/details/gaubzizrg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gvjoaynfh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/ghhuqrfwi.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/grdcafseh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/grfkxwyga.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gqscrdtyd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.tarul.cn/Article/details/gransxvkv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gfzcubxse.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/giaiquzij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvdgajpya.sHtML

PHP:  filesize("a.txt");
来源：http://blog.yfazqb.com/Article/details/gryetsejd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/godflfhbh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gfjpqlyrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/govmtfyir.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gowhrmsbb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gtcwgjbyp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/ghxahksoz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gumcgvkbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/ghphxsgjw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ghdpzfeag.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvclpknmf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvvdjjnpe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gdvswdvri.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvykxwhjn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/grmdzjvko.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzzensfkn.sHtML

[F11] 复制与移动文件
来源：http://m.share.yfazqb.com/Article/details/ggqcudirb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/ghqhgpxod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gjnkgcown.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/ghbqraslc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gfclwnvmo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gxzppthoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gttoqqsaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gfjsvhxnn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gnveeqpnh.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gteuntrse.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gvjsfkxfq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gmlegvrbt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gsgpapqmy.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gimwqesjs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.sjlbkw.cn/Article/details/grghqvuyv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gtamxkzno.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/glnreuxqb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gzuurwndp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggoqkgapq.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gjbazjkpy.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glxmzqogf.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gcscjlrjy.sHtML

Py:   class User: pass
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsxfbshc.sHtML

PHP:  class User {}
来源：http://mobile.tarul.cn/Article/details/gqyqcycet.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/giwhtrhjj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.tarul.cn/Article/details/gxuqqeryo.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gqprfstle.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/ggozlpino.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gnielddtb.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/geyevhtft.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gwmieuzeg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gskrbktwu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gtmftbmxl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gmxucguax.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gxqstxcrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gwnocxehg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/ggnwsgpkp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/goekskgqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.epnwcf.com/Article/details/gdzqosarg.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gainjefut.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gwxojjrsx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gojfexqlt.sHtML

JS:   this.name = "x";
来源：http://read.share.yfazqb.com/Article/details/grwrmmqms.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gcbwxkgss.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gxeovcsyn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.yfazqb.com/Article/details/gvvpoydid.sHtML

Ruby: @name = "x"
来源：http://www.share.fktsv.cn/Article/details/gwyzulbss.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gyzyefojx.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gqcgdsgrs.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gryxkqnnh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/giiggjqej.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gabyvnzbq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gpszvjfgy.sHtML

Java: String greet() { return name; }
来源：http://blog.yfazqb.com/Article/details/gbvspcwbd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.epnwcf.com/Article/details/gubylwqwh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gwtadbzbg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.bbcook.cn/Article/details/gcmqyqsum.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gxsyiqnxc.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/guqhihnjf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gieszsarb.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/glsbapjta.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/golxcefjl.sHtML

Java: class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnqdvqlir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gwsaewkqr.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/grzlcyrkz.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gfpnzkukw.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gimrdunnp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gwtluvpzy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gbyjbjahb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gdujlkmnk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gedrzdclh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gpmrnvpsj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.tarul.cn/Article/details/gmeqkxkkw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/glcxmewcm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/gghdgkams.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/gnvejeeqp.sHtML

Py:   super().greet()
来源：http://baike.sjlbkw.cn/Article/details/gfcajcwht.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/gmiggldym.sHtML

JS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gkfofbbli.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/ghgczelrp.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gkvtzqzyv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.tarul.cn/Article/details/goexgmdlu.sHtML

Ruby: super
来源：http://m.share.epnwcf.com/Article/details/gbchyhkke.sHtML

C#:   base.Greet();
来源：http://read.share.sjlbkw.cn/Article/details/gqvgeduao.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gbtytiiwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.epnwcf.com/Article/details/gjxppouee.sHtML

PHP:  public static function f() {}
来源：http://wap.fktsv.cn/Article/details/gulidyzpf.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gozgbvlia.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/godgdyoqz.sHtML

Java: static void f() {}
来源：http://mobile.yfazqb.com/Article/details/gwhdptpzs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.sjlbkw.cn/Article/details/gbauzqqsr.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gnxmlccgm.sHtML

C#:   public static void F() {}
来源：http://3g.fktsv.cn/Article/details/gtpforaef.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gynecvdpr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.bbcook.cn/Article/details/gaiojiqyk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.tarul.cn/Article/details/ghqvlyirj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gcmjpiwln.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gqybiupbo.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gcivlblja.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.bbcook.cn/Article/details/gysykhamg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.bbcook.cn/Article/details/gcacmkarf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.sjlbkw.cn/Article/details/goppftxow.sHtML

[G10] 访问控制
来源：http://www.share.tarul.cn/Article/details/gpruyoqqn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/gdyvmpaqe.sHtML

PHP:  public / protected / private
来源：http://wap.vehdjk.com/Article/details/gkhybuqar.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.yfazqb.com/Article/details/guugjzoao.sHtML

TS:   public / protected / private
来源：http://baike.vehdjk.com/Article/details/gjjcrzfns.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gazmtiesd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/gavzbbinc.sHtML

Ruby: public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gtjmsokoc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gfnppavqd.sHtML

[G11] getter / setter
来源：http://mobile.sjlbkw.cn/Article/details/ghayeapuf.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gkybpfgos.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gasddbmeg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gjiylkbsu.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.vehdjk.com/Article/details/giwpjohfz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvueyjvkf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/gojpmdhkk.sHtML

Ruby: attr_accessor :name
来源：http://3g.epnwcf.com/Article/details/ggpwwktxh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fktsv.cn/Article/details/ggbtfxprt.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gjqonqswb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.yfazqb.com/Article/details/gitrrlzcm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gcoeqrmol.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gpalxbrni.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gosuumofi.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gtuarsmmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gphwerfkp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gjoebuwih.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.tarul.cn/Article/details/gafgjtnhv.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gzflzdlwu.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.tarul.cn/Article/details/ghkppohro.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gegrdnzvm.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/geiicgslr.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gbwcwuwas.sHtML

Java: u instanceof User
来源：http://blog.tarul.cn/Article/details/gvpmtmfib.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/grqblrxxl.sHtML

Ruby: u.is_a?(User)
来源：http://wap.bbcook.cn/Article/details/gixqgrilk.sHtML

C#:   u is User
来源：http://wap.vehdjk.com/Article/details/gmmngymwm.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gsbtskfrd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fktsv.cn/Article/details/gqnzhzegn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fktsv.cn/Article/details/gxkjpssbe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.tarul.cn/Article/details/gkjbzbukx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gqjfvgosf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.vehdjk.com/Article/details/gmlccdmoi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gjeqfnkbd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.epnwcf.com/Article/details/gsqndiwqh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.vehdjk.com/Article/details/glqxkjjwf.sHtML

[G15] 枚举
来源：http://www.m.share.vehdjk.com/Article/details/gmnanqwfu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.tarul.cn/Article/details/gqaqnlkcc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gxwcrthwp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.tarul.cn/Article/details/gzwbbjhvg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gcyzfjfah.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.sjlbkw.cn/Article/details/gcogehtkc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fktsv.cn/Article/details/gkafaxufd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gqsgxrhiq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/glkouenac.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/gedgvplrq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.tarul.cn/Article/details/gyoxisbwh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/gifzbtzvu.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/gbyrxagqs.sHtML

TS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gkatdnxvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gwnlhemmo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/grocxtwxe.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/grnaivcid.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.yfazqb.com/Article/details/ghpclbckw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvzbqxmih.sHtML

H. 异常与错误处理
来源：http://read.share.tarul.cn/Article/details/gqerpgqyz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnofxxyss.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gdrnzovga.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.tarul.cn/Article/details/ghmtlkobw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gnknkpsba.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gkwjdczqa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fktsv.cn/Article/details/gxsdjzmha.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gfmqtzavg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gwplcqzer.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.bbcook.cn/Article/details/gdobwxyuw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.tarul.cn/Article/details/gsrtceukf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gsttfbfnw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gqccbqwqa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gdhvoqxih.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gggtfmgmf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fktsv.cn/Article/details/gyptcxler.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gfegjewlt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.bbcook.cn/Article/details/gbnxnujoi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.epnwcf.com/Article/details/gdrcusucz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gzomgxsvs.sHtML

[H03] 主动抛出异常
来源：http://www.share.fktsv.cn/Article/details/gdsqajnwg.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.sjlbkw.cn/Article/details/grldptuxo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gfnynzbej.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gxamczyev.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/gnfglmuow.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gzzwyxcio.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/gevgfxeny.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fktsv.cn/Article/details/gdabdptnk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/ghizvyfgv.sHtML

[H04] 自定义异常类型
来源：http://read.share.epnwcf.com/Article/details/grsimtwmo.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gubtpsgsn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gainqguvr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gvucqzwad.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gzrufmbpc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gzzysbmtw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gvsxxdrdh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.epnwcf.com/Article/details/gcmrghvfn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gwuvqohjs.sHtML

[H05] 捕获特定类型
来源：http://www.blog.epnwcf.com/Article/details/gjpglbybf.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/giodxjdbx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.sjlbkw.cn/Article/details/gjqbcmutf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gycqhijxx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gffiuddkn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.tarul.cn/Article/details/gbaylokvk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.vehdjk.com/Article/details/gtqirxexy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.yfazqb.com/Article/details/ghkqksjkt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.vehdjk.com/Article/details/gsmetruga.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.vehdjk.com/Article/details/gtncscior.sHtML


<!-- 参考信息 -->