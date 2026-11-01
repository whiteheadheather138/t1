代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/ghlpuidzb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gkhalqreq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gnuxhidld.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gfzwkvsch.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/ggbhpuvvy.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gdjynotgc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gclmjsyks.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gvkxztidb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gvcdgfomd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdlhkvyiq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gkjikbpmt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/ghzglixhb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/grevzuonw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/grjzxrvjc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/ggakmfjsj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.bbcook.cn/Article/details/ghjxfudhd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gxqfspcka.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gqzbmkrby.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gcinxwvty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gypbybves.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.sjlbkw.cn/Article/details/gyslywjpv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmnuopqi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gplkqotre.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gmvnyrwbj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gseltwtyu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.vehdjk.com/Article/details/gjvplzepo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gnrqpqtjk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gufrmayhy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gdmgittdd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gjvwmrxbi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/giooldkpx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gqbuabous.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gevihbxcx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/grcngfggu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.yfazqb.com/Article/details/gmjzohrlx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gilrpezxm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjzaavjfb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gzhnwqyuf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fktsv.cn/Article/details/gfchohpjy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvqqivluj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gicnyrcpa.sHtML

[F06] 删除文件
来源：http://www.blog.tarul.cn/Article/details/gwfeucpzh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfbdctvri.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gkwurlgcm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gttuylzbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gygplobpr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gmuvkeees.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gpgzfrowp.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gkwoljjmh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gymskrzde.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/gbzgipknu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gdclfbxhu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gzgjtwbsx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gzrvgsuex.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gqsblrign.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gtvgmleij.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.sjlbkw.cn/Article/details/ggtjfmgby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.bbcook.cn/Article/details/grngwomfa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.bbcook.cn/Article/details/gdrndeznu.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/gpozorldy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/gkmpcljav.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gjwfoxlzv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/goawydemt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gmxhndvmt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gttqxeewk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gwsitvoyj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbtcggvzy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/ghctaostf.sHtML

[F09] 获取文件大小
来源：http://blog.bbcook.cn/Article/details/gfqhvbsvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/guyfrrjba.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fktsv.cn/Article/details/gcpanjqoa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gdqvmgrcm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/ghrhghwmq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gpzxuxbck.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gcgymqkqm.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gosfuhost.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gcztcqcie.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.bbcook.cn/Article/details/gqqkvwwec.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnnpfqaij.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggpauygsh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gyrkqxnhj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggsivzubg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.epnwcf.com/Article/details/ggtdjdqqj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gahihmyfy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjdzwkedj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnqvmcvmm.sHtML

[F11] 复制与移动文件
来源：http://wap.vehdjk.com/Article/details/gyyspgeqr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gopenhpgv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/gtsfqqrwp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gjjvogtnc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gsjmgoqqu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/gdvezevde.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuawglie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gbkvfewwd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/ghiticaim.sHtML

[F12] CSV 读写
来源：http://www.share.sjlbkw.cn/Article/details/gpkzgxqmg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/gatzcflbm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gxarqtgug.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gpijrdyqj.sHtML

TS:   // 同上
来源：http://www.share.tarul.cn/Article/details/gtatfbkua.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gpfelpzls.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/grfhzqiiu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.yfazqb.com/Article/details/gdhstcill.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.vehdjk.com/Article/details/ggppshnci.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gujlhcehm.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gbrzxzzik.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdmunjwxm.sHtML

[G01] 定义类
来源：http://www.blog.tarul.cn/Article/details/gttutmgvw.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gjypjwmtb.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/ggubexywi.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/gyrwptkbn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fktsv.cn/Article/details/gdrbpuyls.sHtML

Java: class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gmranttia.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/glkkptfwf.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gctnmunoe.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gvkysxkbt.sHtML

[G02] 构造函数
来源：http://mobile.tarul.cn/Article/details/gdymqlocv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gnjtcbght.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/gdkplnykt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gcgqovwpm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gmrekktak.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/guxkqesps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gupoxaghu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fktsv.cn/Article/details/ghayjtjfl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gutrxxvfr.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gjstfpyos.sHtML

Py:   self.name = "x"
来源：http://blog.yfazqb.com/Article/details/gwgdtgkvv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.yfazqb.com/Article/details/gkjcwvsqf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gyveixows.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gscrybkuf.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqenbwqu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gyrkltnth.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gdhypdzoh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.vehdjk.com/Article/details/gktwtgfya.sHtML

[G04] 定义方法
来源：http://mobile.fktsv.cn/Article/details/gkinsyxmf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gsgtrbwyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxbktysxq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gtoklhomx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gmtdpfryh.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gudfbbyah.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.bbcook.cn/Article/details/ggyqsoucu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gayfexksg.sHtML

C#:   public string Greet() => Name;
来源：http://wap.tarul.cn/Article/details/gxehcftip.sHtML

[G05] 继承
来源：http://wap.vehdjk.com/Article/details/gfnpvwesy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.tarul.cn/Article/details/gpvavpufe.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gpeigdmld.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/glayfzlvc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gaohcqerb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gqgjakrfu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.bbcook.cn/Article/details/gnyiltlyc.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gyqxqjvkn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/guewyzunm.sHtML

[G06] 重写方法
来源：http://www.m.share.epnwcf.com/Article/details/gajtfdcos.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gixrfmwae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gfdfycagb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/gkolrvnai.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gjfveacyi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/ghrhovqhe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fktsv.cn/Article/details/ghwakthri.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/ggrbrjjlk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.sjlbkw.cn/Article/details/gxgspuciu.sHtML

[G07] 调用父类方法
来源：http://blog.yfazqb.com/Article/details/gavpnduei.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gnlgwcruc.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/ggiobkbxp.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gahyqwaqz.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gbedodgbu.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/gwegxlcdk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gkastbvuo.sHtML

Ruby: super
来源：http://www.share.yfazqb.com/Article/details/gzwkezohh.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/gexdeqcjk.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gmsbjxwrb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.bbcook.cn/Article/details/gqvnxwdof.sHtML

PHP:  public static function f() {}
来源：http://wap.tarul.cn/Article/details/gayabesqi.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gmigvpyit.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gqbkdvoak.sHtML

Java: static void f() {}
来源：http://3g.tarul.cn/Article/details/gdtvnxjpq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.tarul.cn/Article/details/ggxdqerar.sHtML

Ruby: def self.f; end
来源：http://wap.fktsv.cn/Article/details/gwnievwxd.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/goqchwssn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.tarul.cn/Article/details/gaxflisct.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.bbcook.cn/Article/details/gkasbueyt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.bbcook.cn/Article/details/gmkqpfasy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.bbcook.cn/Article/details/gwzsfzttx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.epnwcf.com/Article/details/gangndjtp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gtgbpdbfv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/glwosuijg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gskjipqll.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gxlpzjiap.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/ggmjvggjk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fktsv.cn/Article/details/gzblzohtd.sHtML

PHP:  public / protected / private
来源：http://www.share.tarul.cn/Article/details/gajnnejpf.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.tarul.cn/Article/details/gtzhrdkoh.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gcvicmtyw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/grlfhvgxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/gyflggglm.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gtbxoayjc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gpkgxdoln.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gaynksczq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gtvjdvnxp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.tarul.cn/Article/details/ghfsaokig.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gjbrlbwks.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkarzapjf.sHtML

Java: public String getName() { return name; }
来源：http://3g.tarul.cn/Article/details/gzgzhswbn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.sjlbkw.cn/Article/details/gmbcgyxbn.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fktsv.cn/Article/details/grtqghnwg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.bbcook.cn/Article/details/gqbrvonup.sHtML

[G12] 对象转字符串
来源：http://www.blog.yfazqb.com/Article/details/gulexpxbh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/ghoammjtm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gafdolgin.sHtML

JS:   toString() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gfpapnigl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gfifntnoc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.tarul.cn/Article/details/gprocyiur.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/guybbzoro.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqfdzzzv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.epnwcf.com/Article/details/gphbwhczm.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/guuzcggte.sHtML

Py:   isinstance(u, User)
来源：http://read.share.epnwcf.com/Article/details/gcnlabuoh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gxzwttnnn.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gdzyyptsn.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gmmffltvd.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/ghbilybkv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.sjlbkw.cn/Article/details/gsovjgclp.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfejjdgt.sHtML

C#:   u is User
来源：http://www.share.tarul.cn/Article/details/gxdrxevfg.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gfuzhrqtf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.epnwcf.com/Article/details/gqmkbtvxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.yfazqb.com/Article/details/ghgotlhhp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.epnwcf.com/Article/details/gnxxxjrqw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.sjlbkw.cn/Article/details/gjjejeslx.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gepisnnka.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fktsv.cn/Article/details/gbanonffy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/gwvdsllww.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.bbcook.cn/Article/details/gookxrogh.sHtML

[G15] 枚举
来源：http://blog.fktsv.cn/Article/details/gzfmfsmsc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.bbcook.cn/Article/details/gudnbxukh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.epnwcf.com/Article/details/gjnuyfbkl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gbltcbgrr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fktsv.cn/Article/details/gkbrnrdhw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gwenpafyt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.tarul.cn/Article/details/gosgsegky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fktsv.cn/Article/details/gpzvnckjy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gywhjybtq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.sjlbkw.cn/Article/details/gbrxnftlg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fktsv.cn/Article/details/gkigzkjpq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gnpynpjvr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxkivkxx.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/gduidncih.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.sjlbkw.cn/Article/details/grltdwlym.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.vehdjk.com/Article/details/grwgjzwun.sHtML

Ruby: obj.instance_variables
来源：http://mobile.yfazqb.com/Article/details/gascvijzr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.epnwcf.com/Article/details/goadhssld.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/grikioxlc.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gsxolvlwz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gfkhcgzjf.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/glnsvbqlz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gmginrmbe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/gocnpwifj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gyxmkbthm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.sjlbkw.cn/Article/details/gqrtviasl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnfwpzfk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fktsv.cn/Article/details/gffrrpmbg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gimoupigr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gmyxmicqq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.sjlbkw.cn/Article/details/gsiwockkh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/ginndssip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gnwuocyyq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/giqndsgda.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/grnrggozm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/grcvfptkc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fktsv.cn/Article/details/grbayegtt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gzvbjvado.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/glnehyvia.sHtML

[H03] 主动抛出异常
来源：http://3g.bbcook.cn/Article/details/gxicuebld.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.bbcook.cn/Article/details/gbgfnvsxr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/guixaeqem.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.sjlbkw.cn/Article/details/gbyofwsql.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/ggiheixjg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gsnkglbon.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.yfazqb.com/Article/details/gywbtorik.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.epnwcf.com/Article/details/gvptvuabw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gyblnyhia.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fktsv.cn/Article/details/gswtsvifr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.bbcook.cn/Article/details/gnioscxcl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.sjlbkw.cn/Article/details/gjgiqbgpy.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.vehdjk.com/Article/details/gnmzueutk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.epnwcf.com/Article/details/gioxicvyi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/gichwpclj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.vehdjk.com/Article/details/gwhypxrtn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fktsv.cn/Article/details/gaenruoxo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.vehdjk.com/Article/details/gykyfbcik.sHtML

[H05] 捕获特定类型
来源：http://wap.sjlbkw.cn/Article/details/gwywtrahx.sHtML

Py:   except ValueError as e:
来源：http://read.share.yfazqb.com/Article/details/gvfxwanbm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gpyoatmpc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.epnwcf.com/Article/details/guqmqslaa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzyuuomcy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gcjxqmhvc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.bbcook.cn/Article/details/gnkidgwtb.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.tarul.cn/Article/details/guzywrwnm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.epnwcf.com/Article/details/guyqideqi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.epnwcf.com/Article/details/gjbyrsqwc.sHtML


<!-- 参考信息 -->