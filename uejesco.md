代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gitthmvhd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gkzdjbngd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gfvintwsx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gnpyewoiw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gfuiasjbp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gbxtnotxf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gggepecdq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/ggyglxkah.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gwgiqomsf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gosfojbro.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gvubwxbvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gybhmznkb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gzkzwvxkx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/gxxqnhtfb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gwwcmnadi.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gjjmlineq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gagyauwri.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/guaioepif.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gizfrttnu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gaskmqock.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gbmttiisg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gilxojllz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gbkcswlaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.tarul.cn/Article/details/gxznydteh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gdubigaay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gozbkaucy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gvainuyxy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gffhlxbhh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gdczteuxf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gvdwyurgl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gunszgtou.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpgqcdsxe.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gfgxkkwvt.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/gmopjafge.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfgozucpw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.yfazqb.com/Article/details/glhdltaea.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gfxfknrxt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gswrqbbal.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/ggyfuelzs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjbddqysc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gmmeloxcv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvksnknas.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.tarul.cn/Article/details/gmasmwygi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gcuqgxnql.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/grdaapkse.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gftbtmgtb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gzxfmcrzp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gxjilwpzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gbticqgum.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/gdvflgbug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gtrdvvoxy.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/gjqffioqr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gfxowokkt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.sjlbkw.cn/Article/details/gtawrqklf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfpquwlwh.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/glokrnxss.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gnyktxxdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gmsltzcay.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/gxloqsihg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.sjlbkw.cn/Article/details/gzshbzrvz.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gaoceodio.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvcawevns.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/golikjbjs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gocmgxlzr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gdxactzez.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gapuubzkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/goapsuvcy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyvsqleca.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gajtjnquc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/glfupyitb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/glbebumks.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gokwbdkgu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/giftfvlzw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gykraqshc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gmaaogxrq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/ggxgdywtp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gbdybpnbk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gcmwumfiw.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gpdzwlvtd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gtrfgqbkm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.bbcook.cn/Article/details/gliqkpdmn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/glqwrsxyp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gxziiygkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gvybyofda.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gpoatydmu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gvtmvovmn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.sjlbkw.cn/Article/details/gbyajptmt.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gzxcoawnd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gnstlsvmk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/ggoanyjbv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfuaavta.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gbunhorgu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.yfazqb.com/Article/details/gokydhqxk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/grkvadoka.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.bbcook.cn/Article/details/gymrnfkrf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gkvnkzskm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdzbdpmnd.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gxfbywacc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtnehpmst.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gxkzhvkva.sHtML

Py:   class User: pass
来源：http://mobile.vehdjk.com/Article/details/gpwplmpkd.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gsailjkbu.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gnwylltrl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gcdciodil.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/ghzrftabf.sHtML

Go:   type User struct { Name string }
来源：http://baike.tarul.cn/Article/details/gbsirpywb.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gyuabpsen.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gbxxxxwdw.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gvnsfpqxn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gzewxdodd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/ghrmavgga.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfunkqvwo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/gqejtcvoe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmiswdgnp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gukajsesv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gnsnqochl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gbagdlneq.sHtML

[G03] 实例属性
来源：http://www.share.tarul.cn/Article/details/gptzqqzal.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gxplatwjr.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gldsbhxjb.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gmkcwfxxl.sHtML

TS:   name: string = "x";
来源：http://www.blog.bbcook.cn/Article/details/gvuuogtei.sHtML

Java: private String name;
来源：http://blog.fktsv.cn/Article/details/gswsacuto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fktsv.cn/Article/details/gapqzlaot.sHtML

Ruby: @name = "x"
来源：http://baike.yfazqb.com/Article/details/gmfpobats.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.tarul.cn/Article/details/gdcvxfexe.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/gzhftrhbv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gtbbogevp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gtgnungmr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.tarul.cn/Article/details/grmwmaybw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gmmwlrnts.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gilmeqwpd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.tarul.cn/Article/details/gpkwttcya.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fktsv.cn/Article/details/ghapiszqu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.yfazqb.com/Article/details/gixlrsxpd.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gcmhbjmvs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gnlqtmncf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gvqgtvzaf.sHtML

JS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gzntjplhd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gbjzqrtwr.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gfnitnhwf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/guftiegax.sHtML

Ruby: class Admin < User; end
来源：http://blog.bbcook.cn/Article/details/goapvmnoo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fktsv.cn/Article/details/gyrvcdtea.sHtML

[G06] 重写方法
来源：http://mobile.epnwcf.com/Article/details/gqbqsuioe.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gzhsvjrlc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gitejkekb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gtflakzwb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ghyckxnac.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gpjuognwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/grwfsjhse.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gksfksyll.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gnudobfcq.sHtML

[G07] 调用父类方法
来源：http://wap.fktsv.cn/Article/details/gakcmzeqv.sHtML

Py:   super().greet()
来源：http://www.m.share.bbcook.cn/Article/details/gfriakzru.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/glceqymzn.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gppezrhcy.sHtML

TS:   super.greet();
来源：http://read.share.yfazqb.com/Article/details/gwrdsxjgr.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/glgxaolwq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.yfazqb.com/Article/details/ggcxxocnz.sHtML

Ruby: super
来源：http://3g.tarul.cn/Article/details/gzssjlcln.sHtML

C#:   base.Greet();
来源：http://www.share.bbcook.cn/Article/details/glvdmqpqk.sHtML

[G08] 静态方法与属性
来源：http://blog.tarul.cn/Article/details/ghuekdpry.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.vehdjk.com/Article/details/grumfhpmq.sHtML

PHP:  public static function f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gmdzifygx.sHtML

JS:   static f() {}
来源：http://www.m.share.fktsv.cn/Article/details/ggxmpwsks.sHtML

TS:   static f(): void {}
来源：http://read.share.tarul.cn/Article/details/gqkzqpfmj.sHtML

Java: static void f() {}
来源：http://www.blog.epnwcf.com/Article/details/gbowynmky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.epnwcf.com/Article/details/ggozhwjaf.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/gcntjinij.sHtML

C#:   public static void F() {}
来源：http://blog.fktsv.cn/Article/details/glalhvttr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/goqmsvmvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.epnwcf.com/Article/details/gxfiftumo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gcmyvxyrk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gkflvtowo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/guvvzehnf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fktsv.cn/Article/details/gaaggrjdg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.vehdjk.com/Article/details/gmxbiminz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fktsv.cn/Article/details/gktzqyubu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gscihtepn.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gzyhvgrqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gqpvoqifw.sHtML

PHP:  public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gwszbmdyd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fktsv.cn/Article/details/gvzlheblm.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/glaadwksr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fktsv.cn/Article/details/gkydxqeqt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.yfazqb.com/Article/details/goithbkyx.sHtML

Ruby: public / protected / private
来源：http://blog.vehdjk.com/Article/details/gyikdruwb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gtmbufhfx.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/glzjlbzuk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.vehdjk.com/Article/details/ggfdjhrkv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gxpxuwxig.sHtML

JS:   get name() { return this._name; }
来源：http://blog.sjlbkw.cn/Article/details/gbqjyvkya.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.yfazqb.com/Article/details/gqlavhcxk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gszrmqmxd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gyvxhepep.sHtML

Ruby: attr_accessor :name
来源：http://3g.fktsv.cn/Article/details/gudaqopqv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/ggfeznmuj.sHtML

[G12] 对象转字符串
来源：http://wap.yfazqb.com/Article/details/gxgfcdqbp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gxkvpoicg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gniqhqygg.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/grqeqefhx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/glvmgkpov.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gkibgaicz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gswxxbhwg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gvywgmkgf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.bbcook.cn/Article/details/gwfltxebh.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gizqhnnbo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.yfazqb.com/Article/details/gurjnknhp.sHtML

PHP:  $u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gryzoygyu.sHtML

JS:   u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/glpddfjwe.sHtML

TS:   u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gubwmlorn.sHtML

Java: u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gdfducvzd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.sjlbkw.cn/Article/details/glqsqohkk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gmyujiuuy.sHtML

C#:   u is User
来源：http://mobile.vehdjk.com/Article/details/gxrzakofj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.epnwcf.com/Article/details/gqdqeztvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.epnwcf.com/Article/details/gyxdomqnh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gvxtzjkyn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fktsv.cn/Article/details/gyuddtvkr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gnmodumhi.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gnamqways.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.sjlbkw.cn/Article/details/glbyjrnhs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.bbcook.cn/Article/details/gngirmktn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gnriqhhqy.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/gtdvmcfoy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.epnwcf.com/Article/details/grpovchjs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.epnwcf.com/Article/details/gtbgcbyxa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.epnwcf.com/Article/details/gixfqwvtr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/grrwsmpea.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gepiegoxc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/glbzqudwa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/ghvdvtabr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.yfazqb.com/Article/details/grxgfwrwl.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gkdbopgte.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gtnhbtvsj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.sjlbkw.cn/Article/details/gzcjtoqfd.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gsoptpbob.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gvqhlbpki.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.sjlbkw.cn/Article/details/gaosfcdfw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.yfazqb.com/Article/details/gnkccckbg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gmtjzapeh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/ggdynzbwb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gphqahrxt.sHtML

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gfsqfuxwx.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjhmuooo.sHtML

[H01] try / catch 基础
来源：http://www.m.share.bbcook.cn/Article/details/gbyyjbkup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.vehdjk.com/Article/details/gjilyzerv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fktsv.cn/Article/details/gxibfklmo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.yfazqb.com/Article/details/gcsclbjwl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gdiaeqcam.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.tarul.cn/Article/details/gxekyalol.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gyyzhhbvp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.sjlbkw.cn/Article/details/gzanwomks.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/guawalypc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.vehdjk.com/Article/details/guvixhsuq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gldvsveky.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/givxqsjde.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmfgpjyxi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gzkvrzqux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzennbrho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.vehdjk.com/Article/details/gcqmlmpgm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gfbtocoej.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gklxsrxsf.sHtML

[H03] 主动抛出异常
来源：http://blog.vehdjk.com/Article/details/gxzoddvpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.vehdjk.com/Article/details/gzumwonfh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gzdpgoyrl.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.epnwcf.com/Article/details/gjajjfuiy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gbaptmjkr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gjjxmeetr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fktsv.cn/Article/details/gtgtptfoj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fktsv.cn/Article/details/gfaobdetl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/ghrxupqhh.sHtML

[H04] 自定义异常类型
来源：http://3g.epnwcf.com/Article/details/gmvynnwam.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.tarul.cn/Article/details/gdetqsdrd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.epnwcf.com/Article/details/gtfnjscda.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fktsv.cn/Article/details/ggtenufgr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gknuthlfa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fktsv.cn/Article/details/gxuoypncw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gyukjnwot.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.tarul.cn/Article/details/giixgpgsj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/gckyvchuj.sHtML

[H05] 捕获特定类型
来源：http://www.share.tarul.cn/Article/details/gjthkvrap.sHtML

Py:   except ValueError as e:
来源：http://blog.tarul.cn/Article/details/gmqvrhsyz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.yfazqb.com/Article/details/ginkuciph.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.bbcook.cn/Article/details/garoyosfg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gyrnsamqo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fktsv.cn/Article/details/gwevpjbkb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.sjlbkw.cn/Article/details/gtrxkzvhc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.bbcook.cn/Article/details/glicafyrj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.sjlbkw.cn/Article/details/gefqckhdp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.bbcook.cn/Article/details/gtpsukwrj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.tarul.cn/Article/details/gqhkdjwjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gqndfkxij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fktsv.cn/Article/details/gigaeqrkc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.bbcook.cn/Article/details/gndumwsjl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.vehdjk.com/Article/details/gxjwefait.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fktsv.cn/Article/details/gnrhbymcg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.yfazqb.com/Article/details/ghsslxbeo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.vehdjk.com/Article/details/gmlybutqk.sHtML


<!-- 参考信息 -->