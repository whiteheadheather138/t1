代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/giwvgsgns.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gqncuhrlk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gmgudwive.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gbaqefask.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gbyjhpflw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gzxlhpwnk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gcepdvujz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmuiymaah.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gbisxhlfm.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gnuzvhuhg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gjtimwggb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/ggftibokr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/geoeaaklu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/grqtuwqph.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gcwxoybqw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/glatkxhpe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gdnhaznfb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gezouzfxx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.epnwcf.com/Article/details/gjxwuihix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.yfazqb.com/Article/details/gttmljpdl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gklxnahza.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gokuccriy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gwhlcadxt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/guafnoozb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gchlqbinm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gumyegsfe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gkwdrtisq.sHtML

[F04] 追加写入文件
来源：http://read.share.vehdjk.com/Article/details/gvoifcdyo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gexutkqnb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/gddbksrvv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/glggekslk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gpgdzlqng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/glmnyabyq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gpwsguyma.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gqlcvojwg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gngpzosri.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gbradhpjo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gcwornnug.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gbjchordn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gzocgttbc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gleortygs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gqiiivtjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gqxcychee.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gitahxzyb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gnicowcfu.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/guiqhxqyf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gihmjeeju.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gzbfpwdwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/grrfrggvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxzmenssg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gseoiefhz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gslajvsix.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gcnmhwghf.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/geipmfqkm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gxlurjrul.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.sjlbkw.cn/Article/details/gsmzkulaf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gxtvxbnje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gzavqpmor.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gfcbvuwif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gqthxpwjm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/glbapbrjt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gdyjoobkm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.vehdjk.com/Article/details/gmkqjwmud.sHtML

[F08] 遍历目录
来源：http://m.share.yfazqb.com/Article/details/gtqsaemod.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gsnmtewns.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gradpjjrj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gqbxdrfss.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gntvhpasm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gxlmhrugn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gywqenrac.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gadmypsxx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gbgoryaus.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gaxknvzqs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/ghxykuazu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gstiblwtz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/gihtboweo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gkxsoadck.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/golhchgxp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gtvdrwpon.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gvayufnpn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.yfazqb.com/Article/details/gqkhjgrkz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gyayfxhue.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gkogwaase.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gxvxbpmco.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gvxxtriqe.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghqeqqxlv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fktsv.cn/Article/details/grnusqwdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtxlflsgv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzymhjpbz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gqpzjczyo.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gcfabtqtz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gvccljell.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gsrfmotjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gqzzmmoka.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxasheujb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/grtscgbkn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.vehdjk.com/Article/details/gdfachtnk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwjcdsguo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gdkwzutox.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gbpbonubr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gtmpcnaer.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gxhwbouef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gaelbsdrf.sHtML

TS:   // 同上
来源：http://read.share.fktsv.cn/Article/details/gqoucmpcx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.vehdjk.com/Article/details/guvpuwbes.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/galrtxasa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gliqdmclu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gvzwtxrve.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gcigcdhyy.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/greyasswy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfbsuahbc.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gencorech.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gejuyiqao.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gnfhfwxtt.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gfqzjcvdw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gzvncbfkz.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gdmedejix.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gwyaeieph.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gjzcpgjxa.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gfzrjcrsu.sHtML

[G02] 构造函数
来源：http://www.m.share.vehdjk.com/Article/details/gputoswgj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gwtuepchh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gkwdmfnpg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/gzhgakfts.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsvakpxyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gnvgbogvf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gcdapogkx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gujhlgxht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.yfazqb.com/Article/details/geahhufzf.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/gyqeqhjxa.sHtML

Py:   self.name = "x"
来源：http://wap.yfazqb.com/Article/details/gntipswie.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gdvtytgpj.sHtML

JS:   this.name = "x";
来源：http://baike.sjlbkw.cn/Article/details/gkwikvqfw.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gzgimucgn.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gimobzkfo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fktsv.cn/Article/details/gpasahtqm.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/gfrterlur.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gnxtlxxwl.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gytrohzku.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gpioochqm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gbpdbfevj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gvkfbstdy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gnkqvgoej.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/guimclzrn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gystjyrqn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gnfxyncge.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.bbcook.cn/Article/details/gnydnyzkq.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gcwruyuen.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gjvpmcjmj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gxmdoakcm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gyffoygsa.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gmopunvmz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gsshjquap.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gkknvtlvw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.sjlbkw.cn/Article/details/gwvggoree.sHtML

C#:   class Admin : User {}
来源：http://3g.bbcook.cn/Article/details/ghobbrrco.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/guvyvzphz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gkhurtips.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gcwahngnm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gsgjmpdbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/giwrympbu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gmhrxeysx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.tarul.cn/Article/details/gdgorghck.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.epnwcf.com/Article/details/gnruxxqpp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gvtcneqxl.sHtML

[G07] 调用父类方法
来源：http://m.share.sjlbkw.cn/Article/details/grieoznhk.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gdtyrvdte.sHtML

PHP:  parent::greet();
来源：http://read.share.yfazqb.com/Article/details/gqmlbcype.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gfomloxmo.sHtML

TS:   super.greet();
来源：http://m.share.vehdjk.com/Article/details/gspoowcdr.sHtML

Java: super.greet();
来源：http://m.share.tarul.cn/Article/details/gybcchahk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gzlbbgpir.sHtML

Ruby: super
来源：http://www.blog.fktsv.cn/Article/details/gzsrxnwff.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/gmtozfcco.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/grrqqdijt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gxrknhmjq.sHtML

PHP:  public static function f() {}
来源：http://blog.tarul.cn/Article/details/gxqxzvini.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gqljzervw.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/gcvtilfcc.sHtML

Java: static void f() {}
来源：http://www.blog.sjlbkw.cn/Article/details/goiibpuii.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gixnyqtoy.sHtML

Ruby: def self.f; end
来源：http://read.share.bbcook.cn/Article/details/gockdifvr.sHtML

C#:   public static void F() {}
来源：http://mobile.sjlbkw.cn/Article/details/gfwtrmhxq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.sjlbkw.cn/Article/details/gzxdjbfas.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gtlyvkqna.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.yfazqb.com/Article/details/gywsmsour.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gxfbiieyi.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.vehdjk.com/Article/details/gwnfaxuwm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxhvbbojm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gwhldaksf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fktsv.cn/Article/details/gatjuricw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/ghxgbcxqu.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gwkalwoeq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.yfazqb.com/Article/details/gpcbroywl.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gmoffnvoe.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gnhhcasux.sHtML

TS:   public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gqplchzjq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fktsv.cn/Article/details/gnefswajs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.epnwcf.com/Article/details/gyrnqzydp.sHtML

Ruby: public / protected / private
来源：http://3g.vehdjk.com/Article/details/gphlpzyeo.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gofpgjxjs.sHtML

[G11] getter / setter
来源：http://blog.sjlbkw.cn/Article/details/gefvadmmk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/griwakgbm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/ghfibpzun.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/gbigchvjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gxypqhjxe.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gbjuwhjog.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gktryymhm.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.yfazqb.com/Article/details/gcmwthebt.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gbbikjffy.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gvftlviam.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gjobqwncl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/glhdirnnq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gbprjwyfc.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.tarul.cn/Article/details/gtpjnqhdj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gukborpkm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gjktfmacc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/gyepzblpf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gkgrnlmsy.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gigazovjo.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gyiozedqe.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gjevxaeya.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gyjrovhnq.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/gyqusnsox.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gfpjjyaqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fktsv.cn/Article/details/gtipwnghr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gnssqnwhx.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/glcjqpzdr.sHtML

[G14] 数据类 / record
来源：http://mobile.fktsv.cn/Article/details/gluyvozeg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.yfazqb.com/Article/details/gvcoflbch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.epnwcf.com/Article/details/gmfccuxwi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.epnwcf.com/Article/details/ggeugphid.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gmadibggo.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.bbcook.cn/Article/details/gbeljxmjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/ggvvgcvrg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.bbcook.cn/Article/details/gojnpzbhe.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gtsmdxyqp.sHtML

[G15] 枚举
来源：http://mobile.sjlbkw.cn/Article/details/galuyachr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmvhbjyd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.vehdjk.com/Article/details/gwyhcpnez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.sjlbkw.cn/Article/details/gvyckcdvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/gudmdplli.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fktsv.cn/Article/details/gmtdidhfw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.epnwcf.com/Article/details/gnmzxtbvm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gwbgbummt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gothdtkjb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/giwjokvph.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.yfazqb.com/Article/details/gakunnmvq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjptmooad.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/garxwzbak.sHtML

TS:   Object.entries(obj)
来源：http://3g.fktsv.cn/Article/details/gywwljlsd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fktsv.cn/Article/details/grmaadbfz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.vehdjk.com/Article/details/gqigzaodz.sHtML

Ruby: obj.instance_variables
来源：http://wap.epnwcf.com/Article/details/gykaoojbq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gysnrvcxc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gyhhoyxey.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/ghqahtqqr.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkstzloys.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gctyufzjp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.yfazqb.com/Article/details/gmbhmzkwo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.bbcook.cn/Article/details/gkyacwcwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gofyyorso.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fktsv.cn/Article/details/gfagkdfpi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.sjlbkw.cn/Article/details/gptyarnao.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.yfazqb.com/Article/details/gvtxlivle.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gjmnkxxeg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gvxzzsmyk.sHtML

[H02] finally / ensure 收尾
来源：http://wap.vehdjk.com/Article/details/ghhmlqnab.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.vehdjk.com/Article/details/gequmyoyd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gpyuwhhuk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gyiuoaswb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gqosyhsed.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gfdovgwln.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.epnwcf.com/Article/details/gwqapmeij.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fktsv.cn/Article/details/gqzqtjkmk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gsqizaayz.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gwjyicyvj.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.sjlbkw.cn/Article/details/guprxnqqo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gmsxafsfk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gqwujxsgi.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gfcrevkbk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gelbiuvpr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.sjlbkw.cn/Article/details/gdechcyci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.vehdjk.com/Article/details/gsyilyrpr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gnogprqdt.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.epnwcf.com/Article/details/graecpvqe.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.tarul.cn/Article/details/ggnlzfryf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.epnwcf.com/Article/details/gwygugryd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.epnwcf.com/Article/details/gkffpxfzr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gqdrjoywr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/geeiwsrqz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.sjlbkw.cn/Article/details/gobhlzsqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gxkzfpfqk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gutaqxvut.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.tarul.cn/Article/details/gqxejndsd.sHtML

Py:   except ValueError as e:
来源：http://baike.fktsv.cn/Article/details/gwvzbyivo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.bbcook.cn/Article/details/gvglswofv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fktsv.cn/Article/details/gnwwawtex.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.vehdjk.com/Article/details/gqfpdwyav.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.tarul.cn/Article/details/gfqtmiiiu.sHtML


<!-- 参考信息 -->