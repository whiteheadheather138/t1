代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gzazyjvcr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/givzmjabi.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/guzgxmitc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gysegbsxl.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gasalthnz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.bbcook.cn/Article/details/gjaaclhhz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gctnrnnlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gaptgpiwa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gtpbioggw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gfwnrmxfn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/guamvtvdy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gojfveaog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gnzexikas.sHtML

[F02] 逐行读取文件
来源：http://www.share.vehdjk.com/Article/details/guauuawmn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gbroniruu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gyvtltzkb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gbafeslyx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gbthfokbx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gxuaugtom.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gpwjondgf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gnrhefkjz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gavnbdugu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gtlvmnzpu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/ggiimzeyb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gejlrpwdu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gunnmkkrq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gwuajsecm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/giuwktvpe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gchkiworv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/ghnfjfnap.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gzekcwjox.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gzsupknvt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gpjdbetrj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/goutkkijn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gzoirjdwi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gyafgshkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfflwsvo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/grhygumfw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/geqsycvwj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gonmwdsaa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/ghxcrtdlj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/guhxgcbvr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gryqtyhxl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gdhzjxqfd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gkvcitrzw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gdctngzpd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.yfazqb.com/Article/details/gzjgimrbu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzenmqmvw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtbdpnomk.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gqfwoooea.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwfaaulra.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gecuufvny.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvrartfdb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gcafrykko.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gaiaaejkq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gohlpvvhe.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxysnkvgd.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gshyhywzq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gkkhchrnc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gkqletfip.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gdwxzszmy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fktsv.cn/Article/details/gibhqgktj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gjvxkxrkm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/goqnxoewg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/ghqudqbzu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gqpznwawz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/gpadnktjw.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gaqycjwvo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/grkqwfzxl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gsugwarsc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/guuhjkbcy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gwjhqyqfj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gzpldecis.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gkmvymsvm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gqfcrtaxo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gwztsxuai.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gfbijunxd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gycstaddp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gymdguhgs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gappknxhg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwcayoglg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gepaastzv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gghjbwgzf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grmhplniy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gwduahmgk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gkmtcfwjm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdibhtzrj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/ghzcenwyy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/giwlrmuov.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/gujzpywgf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gjyzqwyxg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gfiqpromt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxgnmfhmx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvfjvbtbe.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gnmqqidvx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gdoxjzcby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gvdzpxckt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gilgjavku.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gcoergdma.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.yfazqb.com/Article/details/gdsuxyfck.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.tarul.cn/Article/details/gwmgvrkuz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/graluxilu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.vehdjk.com/Article/details/gahmjgqpb.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gnhfvhfzp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.epnwcf.com/Article/details/gkcrmqxep.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.sjlbkw.cn/Article/details/ggopccfif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gkcxfoiog.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gspuddoct.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/glinwszjb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gffvimtto.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.sjlbkw.cn/Article/details/gfmbbssih.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gntyqpxuq.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gojeognbh.sHtML

G. 面向对象
来源：http://read.share.fktsv.cn/Article/details/gtgzvyrit.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/guffgujvx.sHtML

[G01] 定义类
来源：http://mobile.epnwcf.com/Article/details/gjqaykoim.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/giojamwzn.sHtML

PHP:  class User {}
来源：http://3g.vehdjk.com/Article/details/gjkfwsugw.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gygdzqcxs.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.yfazqb.com/Article/details/gdumobsvo.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/goqkltoeo.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gjzrjfzhe.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gujzzlaln.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/glypqatdu.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gskvrczvb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/giygsgpxs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gtxtwxmiw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gwpollsyo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/ggyhojeeu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/goznbvgpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gfohninla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.epnwcf.com/Article/details/gacopvlye.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gkmxsnahy.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gutlsvasq.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gyekfmbzk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gzuaiwhaa.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gfwcebqqu.sHtML

TS:   name: string = "x";
来源：http://wap.sjlbkw.cn/Article/details/glkquxssv.sHtML

Java: private String name;
来源：http://mobile.sjlbkw.cn/Article/details/gxradxnhr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.bbcook.cn/Article/details/gzxcdsdpi.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gglwlmyqd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/gxvoujpas.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gelqvkkkx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gfnrobsdi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/ghutllnhk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gpbsnsqbv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.bbcook.cn/Article/details/goulluspp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gsmmcsxps.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gybnbqpjt.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gpmamamqa.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.bbcook.cn/Article/details/gmditcxac.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gjvzjpyzj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gxfjsyqaz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.epnwcf.com/Article/details/gcvbphuub.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gmvqhbrwy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gecmekutz.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gzovvbugw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.tarul.cn/Article/details/gofxjosps.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gcmjldsfl.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gdozllzdw.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gtwgqzqno.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gtpvqlsvm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/glczppnqn.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gowxsfhdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gebhmxlaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gbvqtgglu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/gqbvuijez.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.sjlbkw.cn/Article/details/gugyjhjbq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.yfazqb.com/Article/details/gtmhezuqn.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gjncnitfa.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/ggcsmaczv.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gsokdjuyf.sHtML

JS:   super.greet();
来源：http://m.share.yfazqb.com/Article/details/gcinfaaev.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gglqalota.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gjyvhucfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.yfazqb.com/Article/details/gytpfyacs.sHtML

Ruby: super
来源：http://blog.fktsv.cn/Article/details/gbjeqxkrn.sHtML

C#:   base.Greet();
来源：http://mobile.epnwcf.com/Article/details/gufsrrchg.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzfpjfrj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.bbcook.cn/Article/details/grutcheqn.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqevisvzj.sHtML

JS:   static f() {}
来源：http://mobile.fktsv.cn/Article/details/gtdodsnwa.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/ghckkksni.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/gcsnnxefo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.tarul.cn/Article/details/gkabxdwin.sHtML

Ruby: def self.f; end
来源：http://m.share.yfazqb.com/Article/details/gwryhrltn.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gcqooavrp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.tarul.cn/Article/details/gwbtlkzeu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.epnwcf.com/Article/details/gxkdootnx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gzawupegk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/grwnrrbjj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.tarul.cn/Article/details/gffmrbbhl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.vehdjk.com/Article/details/ghjzyflab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gqdwcubfc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fktsv.cn/Article/details/gzaeaintu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fktsv.cn/Article/details/gtcfyaiph.sHtML

[G10] 访问控制
来源：http://baike.bbcook.cn/Article/details/gqvekngol.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.sjlbkw.cn/Article/details/gudsalyxy.sHtML

PHP:  public / protected / private
来源：http://m.share.epnwcf.com/Article/details/giopcwxlk.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.tarul.cn/Article/details/gdmgwbvzf.sHtML

TS:   public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gvglgonwx.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.epnwcf.com/Article/details/gcvkitduh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.epnwcf.com/Article/details/gbpxdficd.sHtML

Ruby: public / protected / private
来源：http://read.share.sjlbkw.cn/Article/details/ghwgbcxbe.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/gliynqxfw.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gufxddxom.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gigzmwlvj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gpdvrigkp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/giimsrqrz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.vehdjk.com/Article/details/ghtxnvvxt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcqdscfob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/ggeihmede.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/giqsodgll.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/glimezkqv.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/gfjcfopkd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/guygsyonp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gmzcnbojw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gbhtqrnoh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gofsnoqsw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.vehdjk.com/Article/details/gennclttn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqwikhkn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gyvmxabah.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.sjlbkw.cn/Article/details/gwwmgxnyc.sHtML

[G13] 判断对象类型
来源：http://www.m.share.epnwcf.com/Article/details/gxhifjvwa.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fktsv.cn/Article/details/gitaoffuq.sHtML

PHP:  $u instanceof User
来源：http://wap.fktsv.cn/Article/details/gnrjnkqrn.sHtML

JS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gbxurekbz.sHtML

TS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gneysxqrn.sHtML

Java: u instanceof User
来源：http://read.share.tarul.cn/Article/details/grlqasnva.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.tarul.cn/Article/details/gnjakburm.sHtML

Ruby: u.is_a?(User)
来源：http://baike.yfazqb.com/Article/details/gbrxutkaa.sHtML

C#:   u is User
来源：http://www.blog.bbcook.cn/Article/details/gbjthgmhe.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gdtvqprut.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gmbqtyvtt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/geknsnhpq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/gozhcpdui.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gdgvmrppn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/gfkilyvwj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/ghgpdtylj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.bbcook.cn/Article/details/gcyhoxyry.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.vehdjk.com/Article/details/gowpkdsnv.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/geydiklly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/giwssrxty.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyugovhiu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/gbjzerwkw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gindsvebe.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gsrtocxac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/grplxjilb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.yfazqb.com/Article/details/gpshrodeb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/garyeqjin.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/ghgsycjck.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gewpgjxiq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.vehdjk.com/Article/details/gqtzmjjtt.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/goecvkwom.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/grcdqfcvn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gcsikpngt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gpsnrnqhc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/ghkuodtpx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gjyvgkdvz.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gphjqwgcy.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gzjufaeup.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gogvoqyrv.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/grbxeotop.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fktsv.cn/Article/details/gumruwtgo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.epnwcf.com/Article/details/gpkytqlpz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gzadwpexs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.epnwcf.com/Article/details/gfnqacugm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.tarul.cn/Article/details/gxsandssk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/goygftvlb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fktsv.cn/Article/details/giodomapv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/gdbhlkkhr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/guexzhdmt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gjgwklrvl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gtfgtnewm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gxhdvmvim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/grxfrufei.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gihwhsbbj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.sjlbkw.cn/Article/details/gkzjrxqls.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.tarul.cn/Article/details/gyhhffmbv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gvoxaspey.sHtML

[H03] 主动抛出异常
来源：http://read.share.vehdjk.com/Article/details/goslxfplx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.tarul.cn/Article/details/glojuqdhg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.vehdjk.com/Article/details/gzinlmnlh.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gzhminpnb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gayultpgn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.vehdjk.com/Article/details/gvkxjuwqy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.vehdjk.com/Article/details/gvolnzqyo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.tarul.cn/Article/details/gzxgedpcr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gxonmetnj.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.yfazqb.com/Article/details/gnkudxfxn.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.vehdjk.com/Article/details/gnfmydbbs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gagjpyyes.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/gvlhsnqxo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gzgvnmxms.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.yfazqb.com/Article/details/ggmdyrqbn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.tarul.cn/Article/details/gidqubotb.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.yfazqb.com/Article/details/gksgdcsxy.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.sjlbkw.cn/Article/details/greshqxte.sHtML

[H05] 捕获特定类型
来源：http://mobile.tarul.cn/Article/details/gmwwscjoe.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gjzsihhvu.sHtML


<!-- 参考信息 -->