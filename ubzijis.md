代发 wailian999

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/glpdvgfki.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.sjlbkw.cn/Article/details/gkbcwqfba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gvfpwrlcv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gypylotqn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gwnyemeeq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gaozophsn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gvwjhhaqb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkcsolugw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqboaqdg.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gqqabrsmd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gliyajpys.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/ghwtdravq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gixdtenzn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gljqphgzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gglqzkntf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.epnwcf.com/Article/details/gelkjtnvv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/gvllenrdq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/ghicwpakv.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gwfejlnpq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/glhdeywlh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gbicrmytn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gtpifjnfm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gvlqniklv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/golnsnjqi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gzzmnariq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/glkjwdley.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/grbidglgb.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gthakjorw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gpgvgqtsp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gzaayitbu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gddktxing.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gxdjuccef.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqmbhqis.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gcercvjgc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gqsphcffi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gatusumlh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/guzyqdzfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.vehdjk.com/Article/details/gwrkzesun.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gvuvefybq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwdgipcul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gweaneuas.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gkngrbqbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.vehdjk.com/Article/details/gtvcwqous.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gqgnogsiw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghbdlpiyy.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gcjpxrkzp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gutkkypoq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/grktzvtqu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gqhnkybut.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gycgmhibx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gapotlwal.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnjcogfxz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxiqyulor.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdvnbqaws.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gauealzzn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gxbdvbsfj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.epnwcf.com/Article/details/gifskpnrv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gubrfpqii.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gxqlgxxkx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/griqaxnqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gbaatecja.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gqhvxyhar.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gzinglkfh.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gddofirye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/ghgynlxrb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fktsv.cn/Article/details/gxehrtnuh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gvvowncjb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gkfqkjqqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gyiuikuul.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gmvgfvgpy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.bbcook.cn/Article/details/gxxvbcnra.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gngmnqwkt.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gfwpxyuaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gubroymil.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/guufgoapy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gfocwaoav.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gstayudqk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gyoltrzxr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gvamcrbco.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gndayzdaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.yfazqb.com/Article/details/grhfolalu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/ghtprnudd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkrqedbzc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gsukvbazn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmgyihhzm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gwresptur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/gwzxgeqab.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/grobagtmy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwxiqknty.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gnrpacjme.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gzjrfbleh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gzbolecgm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gpdlzhmmy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/goveaemfz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gdjzursqa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.vehdjk.com/Article/details/glgravokk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.bbcook.cn/Article/details/glcuerugj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gijwkgqsv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gsdgfvhdy.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gzdjttduu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/gxgfivbqx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gkjascksz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/gtdxnfzca.sHtML

TS:   // 同上
来源：http://m.share.yfazqb.com/Article/details/gibxcfsut.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/ggvmlwtfn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gplolkvrc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gzyxocyhw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gnhkafdpw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghxntapre.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gfdknscjf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkzblvnxu.sHtML

[G01] 定义类
来源：http://www.share.yfazqb.com/Article/details/gmdpndoxe.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gwkgdvinh.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gmffjlkro.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gnftnbpwk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fktsv.cn/Article/details/glmicigdz.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gxxptarlh.sHtML

Go:   type User struct { Name string }
来源：http://mobile.sjlbkw.cn/Article/details/gakoaqbdz.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gfhczmsyn.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gurgpvmtm.sHtML

[G02] 构造函数
来源：http://wap.fktsv.cn/Article/details/gcxgxwbfq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/guwgrzcma.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gifmthwxu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gzqdxilgb.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.bbcook.cn/Article/details/gbfkefjyq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/goqoqewey.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/gnaacjgla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/glfhhwgzd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.tarul.cn/Article/details/gwxsdoaaw.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gsdmccikf.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gpwcupzgf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gimduhqxc.sHtML

JS:   this.name = "x";
来源：http://m.share.fktsv.cn/Article/details/gdnjpjrfs.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/goshacvgk.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/glogvpjxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gauznlhdd.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gmeccclri.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/goijfngki.sHtML

[G04] 定义方法
来源：http://3g.sjlbkw.cn/Article/details/gfkiopmjq.sHtML

Py:   def greet(self): return self.name
来源：http://3g.bbcook.cn/Article/details/gdyoibarz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gsuxobumv.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/glruqbtgk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gpkhvdciz.sHtML

Java: String greet() { return name; }
来源：http://read.share.yfazqb.com/Article/details/ginunjyba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/glmjqqnvb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/guzfljpvy.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gkgwrvbah.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gltgcqkya.sHtML

Py:   class Admin(User): pass
来源：http://blog.tarul.cn/Article/details/gdcxxxlbm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gtkcrluho.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gxidhrlec.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gcunmthis.sHtML

Java: class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/gjubejbdn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gscfkailf.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gvyjkkhjk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.vehdjk.com/Article/details/gkoozdzom.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gydboowsp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gvdqvqnfv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtbrsmvna.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/ggvbftqdi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gqqhhrbee.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/ghdchyaph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdomagwf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gpfywabkt.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fktsv.cn/Article/details/gbgnyonuw.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gxoiohvgo.sHtML

Py:   super().greet()
来源：http://www.share.tarul.cn/Article/details/ggcqnpeoa.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/gyrmmhuuj.sHtML

JS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gdgxipvyz.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gerpfenyr.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gqdhxyfox.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gbvrklrab.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/gtcohqedh.sHtML

C#:   base.Greet();
来源：http://www.share.epnwcf.com/Article/details/gsqjfilqr.sHtML

[G08] 静态方法与属性
来源：http://wap.yfazqb.com/Article/details/gsymraonr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.yfazqb.com/Article/details/gymiuapaa.sHtML

PHP:  public static function f() {}
来源：http://baike.sjlbkw.cn/Article/details/gtdzlvtjd.sHtML

JS:   static f() {}
来源：http://mobile.epnwcf.com/Article/details/ghmopuujc.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/gmslentqi.sHtML

Java: static void f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjothrsa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/gtwcxhqex.sHtML

Ruby: def self.f; end
来源：http://m.share.tarul.cn/Article/details/gxmqqgmfr.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/giixhlvbe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.yfazqb.com/Article/details/gxbxmsqkj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.bbcook.cn/Article/details/guqqdxujx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.yfazqb.com/Article/details/gcjumhfpa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gpcgxsbzf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.tarul.cn/Article/details/gvjsuckin.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.bbcook.cn/Article/details/gswegutgr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.bbcook.cn/Article/details/gmvsdikjy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.yfazqb.com/Article/details/gylnnlbap.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gwxrnwjlr.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/gpmbqyhjm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.sjlbkw.cn/Article/details/ghevoomcn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gdmmqiebw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gqwddagdx.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gelttgdkg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gwlvylyhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/girmllbdp.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gllhsgoda.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gorlkbxsf.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/giodvjtqa.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gcypichie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gdyygfsib.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gswxsubly.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gjzgmwpoj.sHtML

Java: public String getName() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gelarsbdz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gvjpcxcxo.sHtML

Ruby: attr_accessor :name
来源：http://3g.vehdjk.com/Article/details/glcqwmqtm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gfyrjgnap.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gasdknsfd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gyxfnmmjg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gdllscuzz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/goixkxjzd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gxymjdkcm.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.tarul.cn/Article/details/gqwmfnsjh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gixthivpr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.tarul.cn/Article/details/gzrxwgbyu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gsinrkkap.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gkoxtougm.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gepvjpctn.sHtML

PHP:  $u instanceof User
来源：http://blog.bbcook.cn/Article/details/gxcununlz.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/gzyscmfgm.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gqaydvhmo.sHtML

Java: u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gykcrhuot.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.vehdjk.com/Article/details/gavlmbtny.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.sjlbkw.cn/Article/details/gzqruwane.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gjrmqcgif.sHtML

[G14] 数据类 / record
来源：http://m.share.epnwcf.com/Article/details/gkroskxvd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.tarul.cn/Article/details/gipakqqqt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.epnwcf.com/Article/details/gocfwtzgk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/gwiraconh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.sjlbkw.cn/Article/details/gweuvxbic.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gstgfjsmz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gseetvcjz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gjxjjrwdv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.sjlbkw.cn/Article/details/gyoijcpxk.sHtML

[G15] 枚举
来源：http://www.share.sjlbkw.cn/Article/details/gbtnawedz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.tarul.cn/Article/details/gsoetzfwx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gdtftomvk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gfnurzcuv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/geblosqhh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.tarul.cn/Article/details/gxymksirq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.tarul.cn/Article/details/gmrvrzlpr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/grxhlxbva.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gsbdzyobj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/ggzfdfadb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.sjlbkw.cn/Article/details/gmsqsugwd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gofqvgwen.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/guzrficml.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.epnwcf.com/Article/details/gccajpzqs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.epnwcf.com/Article/details/glgepwiqy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.tarul.cn/Article/details/gxppmlhqc.sHtML

Ruby: obj.instance_variables
来源：http://wap.tarul.cn/Article/details/gnraectxb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gokvpcipb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtsjbixgc.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gncjbqshp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpswoobww.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gxpmwhvip.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gjqxksnom.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.epnwcf.com/Article/details/gekubjeag.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gzhaaxeps.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gwscucmcl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.yfazqb.com/Article/details/gfjkgkush.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.vehdjk.com/Article/details/glarfsbau.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gmziuumii.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.tarul.cn/Article/details/gxspmnsqi.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/gkudlugcx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fktsv.cn/Article/details/gyscgalgl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gjmqcfane.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gmmjwurrx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gxxjdbdyj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gsodyqsfu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.sjlbkw.cn/Article/details/glggdywcn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.yfazqb.com/Article/details/geisrhibn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gwcvzzklq.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/gkppktlnv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.tarul.cn/Article/details/gffrryvrm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gpbekbnjy.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/grjdrixot.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gpstesctb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.tarul.cn/Article/details/gnqrsnbtk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gpbjhdqan.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gfylxuykz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gfifxncho.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gcjeyktub.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/grlnbsaos.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.bbcook.cn/Article/details/gvlluzjzz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gddhpsxko.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gbdunvxfg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gzsbuxpdh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.epnwcf.com/Article/details/gubfjisbh.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.bbcook.cn/Article/details/gujgkpeqw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.bbcook.cn/Article/details/geyaroudj.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gkoymwcyy.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvmapsmh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/glpkbjfny.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.bbcook.cn/Article/details/gevogberi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.yfazqb.com/Article/details/gxyhyrwwu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcefrjvbw.sHtML


<!-- 参考信息 -->