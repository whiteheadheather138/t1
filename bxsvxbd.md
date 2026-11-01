代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gajcsybqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gwyqyyicy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gphojwrtk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.vehdjk.com/Article/details/gxsufyueh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/glilunfur.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gblkjduuy.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gozyratqv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gtpfcdrjp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gusfjsaix.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gcabdkdws.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gygyzqhev.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gwyrbxeal.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gerugasew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gmsschfnu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gsmqmswzc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gicbaqtap.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gtsavzpjh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/grebdbczi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gesjtnoir.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gteujzdbm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gptssnlph.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gxivqeqxm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gvvjnavan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gtfjqinex.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gfdabcczx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gloumjqly.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gldmjtxmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbivevpaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gmksxsjqa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gcghbkzar.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/goiteuzwv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfjovyjnq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjcboqioq.sHtML

[F06] 删除文件
来源：http://baike.vehdjk.com/Article/details/gpulzrthl.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gspltnsja.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gqwywswyb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkilblqyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gkvhijvoj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/golubdfna.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gotarhddm.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpaxjjwgb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gtevdcbas.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gvcufwjhe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.yfazqb.com/Article/details/gwhqiuvaa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/goqikhpcv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gbmrpegrp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gpcdfbyzt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.epnwcf.com/Article/details/gmoyikbun.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gatidtwdb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gcsuektgz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/glypnkqxc.sHtML

[F08] 遍历目录
来源：http://3g.bbcook.cn/Article/details/gzbszayux.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gedfglflo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gywvuqayq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gpzymgzbm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gjivcjnck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gbsdegnck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gyatjzuho.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gkskvzxct.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gzyrtyzda.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gavtiiwqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvjrirkkr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gxjibstzv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gybzpqust.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gcytrewgc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/ghbyttmez.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/ghfholifl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/grnghtxfi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.tarul.cn/Article/details/gflyarelk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gwhcucxtv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gsvcbeqhl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/golrpgkmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gvpviipwy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gdgdcgjgs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/gurrmjpqk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/goaoqsoee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/ggroukgqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gqmqaffrl.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gndjoepsa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gghixofwr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gfmnfdufz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gfoksgtkv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gwizoxeri.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/guxsxvceg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gtkbyvidj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gwcfjryll.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqhytrww.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/gkwmmooss.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gphuekqeu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gaijxszof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/ghrctyybd.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gwqpouofx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gxumfcpgw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gwggiidqd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.tarul.cn/Article/details/goyfwzlng.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gpgqeqpuq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/giflrwbzk.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/gkzkumcwq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gshuvubvx.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/ggixpjbiv.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gczfbmctg.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/guqltnjnk.sHtML

JS:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gowdhnkbk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.epnwcf.com/Article/details/glfrjhkhq.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gkdszvdaq.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gfvfhhqrm.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gvcginkuc.sHtML

C#:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gbvrfrqge.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/ghpoespkm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gfrmhzxcs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/gqznhnbct.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gtitfoicb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gumpcalsh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gkkohclqq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gjqtdejni.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gszluknni.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.bbcook.cn/Article/details/gkwwqycyz.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/gqjrofmkw.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gndcqzubw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gnwmrpfjj.sHtML

JS:   this.name = "x";
来源：http://baike.yfazqb.com/Article/details/ghsnsrlat.sHtML

TS:   name: string = "x";
来源：http://wap.yfazqb.com/Article/details/gejznttbc.sHtML

Java: private String name;
来源：http://www.share.fktsv.cn/Article/details/givofpbho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gsralvsag.sHtML

Ruby: @name = "x"
来源：http://wap.fktsv.cn/Article/details/gadijmvro.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gqmtciccp.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gmswdygya.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.sjlbkw.cn/Article/details/gbqjkswny.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gubozzysi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gyyvqlcxa.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gttywmans.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gimtlgbks.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gbmarqols.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gfabnwxhw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gxcxswnsa.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gqdcfafqt.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/gfpkckkro.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcsczbcwr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gzwezwdol.sHtML

TS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gkperhvpt.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/ggupwbdet.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gpgtjyjre.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gozpfhhjx.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gebezcgho.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/guiaeddzs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fktsv.cn/Article/details/gqxdwsmbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gkzxkmevz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gagrirqxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gkrarjdsr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gexwypgnn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.yfazqb.com/Article/details/gogqurunl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gohizuxjv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/grlkgprsi.sHtML

[G07] 调用父类方法
来源：http://3g.vehdjk.com/Article/details/gymkghiah.sHtML

Py:   super().greet()
来源：http://www.share.sjlbkw.cn/Article/details/gocmlsdlo.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gjqagmqzi.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gcaujalsz.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gohqefxow.sHtML

Java: super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/glcfcrmbp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fktsv.cn/Article/details/gsolbxyna.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gbnadevug.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gbgytowkv.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gitpibmsb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/gmuqzssqt.sHtML

PHP:  public static function f() {}
来源：http://baike.tarul.cn/Article/details/gauzgpitl.sHtML

JS:   static f() {}
来源：http://read.share.bbcook.cn/Article/details/grfzfvkyh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.yfazqb.com/Article/details/gqxuvawsw.sHtML

Java: static void f() {}
来源：http://baike.bbcook.cn/Article/details/ghcrtdwtq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.bbcook.cn/Article/details/gjzhrqsuo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.vehdjk.com/Article/details/gavkzxyod.sHtML

C#:   public static void F() {}
来源：http://mobile.yfazqb.com/Article/details/giwsiowlb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/gidvxtnbz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.vehdjk.com/Article/details/gtegltcui.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbujaxuhx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gddsqgrtn.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gkvoujzpc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gykdieefx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/giwmjmita.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.epnwcf.com/Article/details/gbzlszugo.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.vehdjk.com/Article/details/gldkcojae.sHtML

[G10] 访问控制
来源：http://www.m.share.tarul.cn/Article/details/gjzhncomb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gwqwubmts.sHtML

PHP:  public / protected / private
来源：http://blog.fktsv.cn/Article/details/gjthreeue.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/ghdaoptzy.sHtML

TS:   public / protected / private
来源：http://blog.epnwcf.com/Article/details/gsheghcly.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gutueorni.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.sjlbkw.cn/Article/details/glwcgxhot.sHtML

Ruby: public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gurblkdlq.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gxzhcpcoy.sHtML

[G11] getter / setter
来源：http://baike.fktsv.cn/Article/details/gcfqaxlmi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.sjlbkw.cn/Article/details/guwwloakx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gggwhigjo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.tarul.cn/Article/details/ggpbuhuzh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gkdmuwjps.sHtML

Java: public String getName() { return name; }
来源：http://baike.tarul.cn/Article/details/gxdeqexkb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gbvzznxjf.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/gloybnkir.sHtML

C#:   public string Name { get; set; }
来源：http://wap.sjlbkw.cn/Article/details/gwdizizua.sHtML

[G12] 对象转字符串
来源：http://3g.fktsv.cn/Article/details/griytrwaa.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gbcwyguzk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gkvkqqstz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/ggrqoucdh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyzldvmuy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gujvzgdtk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.yfazqb.com/Article/details/gbqdcwjym.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/ggrtgbckm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.yfazqb.com/Article/details/gnpszivru.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gfnhqmfrt.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gsablzixf.sHtML

PHP:  $u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gyrvwihsz.sHtML

JS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/grlgfajwp.sHtML

TS:   u instanceof User
来源：http://blog.epnwcf.com/Article/details/gfyyxymvz.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gnlcvvivu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gjmjemtsz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.vehdjk.com/Article/details/gnzwbxyfi.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gkcbznutj.sHtML

[G14] 数据类 / record
来源：http://blog.tarul.cn/Article/details/gzjvbdbtr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gissxvlru.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.vehdjk.com/Article/details/galdgzqot.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.epnwcf.com/Article/details/gkrwqvfwt.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.vehdjk.com/Article/details/gvyaoxcqb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/gbswoujom.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fktsv.cn/Article/details/gzzbtuvzy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/guiafevaj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/gtpzquctb.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gsortojwr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.epnwcf.com/Article/details/gmvsftfsf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gaoxkqbkt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.yfazqb.com/Article/details/gnejgcigk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gotoltpni.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gzqodvwol.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fktsv.cn/Article/details/gzxggldzd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gehuqzawu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.yfazqb.com/Article/details/gwjyazdwc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gxlfxvmxo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.yfazqb.com/Article/details/gbmqxupuq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gnclwkshn.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gqpounsjw.sHtML

TS:   Object.entries(obj)
来源：http://wap.epnwcf.com/Article/details/geshzwdsd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.vehdjk.com/Article/details/grovajhvk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.yfazqb.com/Article/details/gbvfwgewo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.yfazqb.com/Article/details/giicuapzv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fktsv.cn/Article/details/gakqjsjox.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpuefeccl.sHtML

H. 异常与错误处理
来源：http://www.m.share.bbcook.cn/Article/details/guaxpftsi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/grwbrobvx.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gaakdhdzm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/grhzineuz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.epnwcf.com/Article/details/gksdqczic.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gvzawjpau.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gdistezzp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.sjlbkw.cn/Article/details/gyqheyumy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gpdflubrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fktsv.cn/Article/details/grhqhfwvg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.tarul.cn/Article/details/grlzryhmg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/gtwrtbooa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gwhrzgxkh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gthbmgxkr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/goljhyhnk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gkuudaajh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/gdeuseurj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gebtlbgad.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.epnwcf.com/Article/details/genmigxcs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.bbcook.cn/Article/details/glkwvplqs.sHtML

[H03] 主动抛出异常
来源：http://mobile.fktsv.cn/Article/details/gcowzakrd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.vehdjk.com/Article/details/gaebirglw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.tarul.cn/Article/details/gzmkzdsiy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.tarul.cn/Article/details/gpktdrkbl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gjlyedahi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gijhickvy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.vehdjk.com/Article/details/gkbteupdg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.tarul.cn/Article/details/gifcbqzkm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fktsv.cn/Article/details/gcuupjyqm.sHtML

[H04] 自定义异常类型
来源：http://baike.tarul.cn/Article/details/gdauzhusb.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.sjlbkw.cn/Article/details/ggayviqry.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gypczynzv.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gswtrqipd.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnvfesqe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gsebadwaf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.epnwcf.com/Article/details/gihxdwzxy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.vehdjk.com/Article/details/gvcmfcxjj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fktsv.cn/Article/details/gxfxjaesc.sHtML

[H05] 捕获特定类型
来源：http://www.blog.vehdjk.com/Article/details/gtmdbozgr.sHtML

Py:   except ValueError as e:
来源：http://mobile.yfazqb.com/Article/details/gyrohahja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.vehdjk.com/Article/details/gcdyqcpqa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.bbcook.cn/Article/details/gggubqexj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/gtggzdhiu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.epnwcf.com/Article/details/gsohucwsp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fktsv.cn/Article/details/gsfcnqeiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.epnwcf.com/Article/details/gvjfaglce.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fktsv.cn/Article/details/genavmxvl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.sjlbkw.cn/Article/details/glwsppspo.sHtML

Py:   value = d.get("k") or default
来源：http://3g.sjlbkw.cn/Article/details/gthlkldik.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gjbonhjnd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.tarul.cn/Article/details/gdconvlqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.epnwcf.com/Article/details/gvvuaoymo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.tarul.cn/Article/details/grjvzyxvr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.epnwcf.com/Article/details/gmqgtmphc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.epnwcf.com/Article/details/gqvaumwqk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.yfazqb.com/Article/details/glvjdjsvo.sHtML


<!-- 参考信息 -->