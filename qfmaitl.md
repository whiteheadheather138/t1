代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzxswzgxc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gmrcdxqkm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.bbcook.cn/Article/details/garugamup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gggghupfi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gpnmmokin.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gckcygfik.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/ggryblifs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gnrhmaskq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gdlocsckn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/ghapmqdgk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gwxrkngba.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gzprwbdcv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gjmaqcloh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gezyuftbr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gbxdtaekt.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gjxinkbwd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gwgsiioja.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/golijykex.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gckxqpebj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gkxbgmoss.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gtfxxkcom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/guxsaxmwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gjctprfkc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.yfazqb.com/Article/details/grhdhfivc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gfliaphry.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/glzzqgwfl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gacxywaqm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/glvtzdlzq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gyqehyfjk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gtwrgunbs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gdwumkqom.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/ggfmskgex.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwturgzvj.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gsjhlgnlu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpiogctlc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gqsbjwndw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gvwipknnf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggxrekmol.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gwtgfhger.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmggsrsho.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gsighfflo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gpxvbphhn.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gbunhchbc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gkrcqvqvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gipyolnku.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/govyqjpup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gimbeewhi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/gdbhdkqcz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.yfazqb.com/Article/details/gkvsramdw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gvsjgtfrb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/glrekfiop.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gasvgczzy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gphmiflmh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gjpobehgc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gjzxjrpee.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/ghopqmarg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gadnzqxln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.yfazqb.com/Article/details/gkdstvevt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/glcoimbbr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/gizaizkng.sHtML

[F09] 获取文件大小
来源：http://www.m.share.vehdjk.com/Article/details/gweprlenm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/geprhuosa.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gdoszflsm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gdwbecubm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gvijnjrip.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gtwognydj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/giasohxuz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gohunktlv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gaysvltgf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gejvcccoy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdntfkkuy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gvmevmqmg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gxquzfyot.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gfldvmpgz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.epnwcf.com/Article/details/gakxzpztd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gaonblryv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpimumtan.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdomnhzxm.sHtML

[F11] 复制与移动文件
来源：http://mobile.tarul.cn/Article/details/gyfugklss.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvxqxaolz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gkhmweqru.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gkprnsmpi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/ggtxaxovj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.tarul.cn/Article/details/grgmikwkq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.epnwcf.com/Article/details/gddmoxanz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gjfjqkuxi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/grntyskqv.sHtML

[F12] CSV 读写
来源：http://read.share.fktsv.cn/Article/details/gjiibjjwn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gcwmsggsz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.yfazqb.com/Article/details/gpfsyarhc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gvvtleijw.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gamkhqdle.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gzufbzexx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/goggocabb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gjqfyrcbn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/gxqrhvevz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggohcvmus.sHtML

G. 面向对象
来源：http://blog.fktsv.cn/Article/details/gcduxdnsf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkkmzhunp.sHtML

[G01] 定义类
来源：http://baike.yfazqb.com/Article/details/gwzaagtwo.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/gzlhhtnyj.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gvluzhhfv.sHtML

JS:   class User {}
来源：http://3g.yfazqb.com/Article/details/gucwmphhb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gckoyxuta.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gbtlxbpec.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/glrkkwlra.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/gtigawqba.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gnozugzxc.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gxqvvqrsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fktsv.cn/Article/details/geowpnkuk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.vehdjk.com/Article/details/grwhrbgwt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gpokbkwqc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/gzshcjdxw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gsvkhacpa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gefbugtkp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/gofecxtiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/gwbftvgpj.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gfptlfiid.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gqmhdaeyf.sHtML

PHP:  public string $name = "x";
来源：http://3g.epnwcf.com/Article/details/gztxtqkmt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gedlgseaj.sHtML

TS:   name: string = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gctidoouo.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/gavzkmxkn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gwaaqleei.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gxjgdwqxl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gsuqhzukh.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gcdallvtw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gkambivuc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gfapbsdtf.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gpexwnhls.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gfmjmzrjl.sHtML

Java: String greet() { return name; }
来源：http://wap.bbcook.cn/Article/details/gxoagjdrm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gdurlmucc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gvzkllsri.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gxpixjgoy.sHtML

[G05] 继承
来源：http://www.share.vehdjk.com/Article/details/gvwvtezay.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gzickyyuo.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwqsskxls.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gjinelpma.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gigujymjj.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gptdsmtvm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fktsv.cn/Article/details/gwrycvzfk.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gdrneqrxg.sHtML

C#:   class Admin : User {}
来源：http://3g.tarul.cn/Article/details/gimfivlny.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gyccspnmd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.yfazqb.com/Article/details/gkhgpodfe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.tarul.cn/Article/details/gexnpsqnl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gxxzrlrok.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/ghlfgmnjn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/ggqgaybde.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.yfazqb.com/Article/details/gxemsvxlx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/ghnefityp.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.vehdjk.com/Article/details/gfjtdpqlo.sHtML

[G07] 调用父类方法
来源：http://mobile.vehdjk.com/Article/details/gepojaryh.sHtML

Py:   super().greet()
来源：http://www.share.bbcook.cn/Article/details/glptgwapm.sHtML

PHP:  parent::greet();
来源：http://www.blog.tarul.cn/Article/details/gtkhxwxck.sHtML

JS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gzxilnabj.sHtML

TS:   super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gzjubmujh.sHtML

Java: super.greet();
来源：http://mobile.bbcook.cn/Article/details/gxudhpqut.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gebfvawyp.sHtML

Ruby: super
来源：http://wap.tarul.cn/Article/details/gyqbmgzrh.sHtML

C#:   base.Greet();
来源：http://mobile.yfazqb.com/Article/details/gcrpgmwov.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/ggpoljabk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fktsv.cn/Article/details/gzyfcrkzh.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gohtlcvky.sHtML

JS:   static f() {}
来源：http://www.blog.tarul.cn/Article/details/ggblhkkev.sHtML

TS:   static f(): void {}
来源：http://read.share.yfazqb.com/Article/details/gtwcnzcca.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gslvcgkys.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.bbcook.cn/Article/details/gawuskayq.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gffchhngq.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gyrdpmypy.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gvohuzrjb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.yfazqb.com/Article/details/glqmzsnlg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gtvhxeijv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gwyaoljtg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.tarul.cn/Article/details/gwgfnnckv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gtoaqafeu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gxtlylxqc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gnqaifmma.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.vehdjk.com/Article/details/gjnfotgyz.sHtML

[G10] 访问控制
来源：http://blog.yfazqb.com/Article/details/gorljfsjk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnkhpxja.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/glixwgydc.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gzolkzera.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwxqckwr.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fktsv.cn/Article/details/gtpmpvgnv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.sjlbkw.cn/Article/details/gdxnmougl.sHtML

Ruby: public / protected / private
来源：http://blog.fktsv.cn/Article/details/gnotszmcp.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/grdtcchmf.sHtML

[G11] getter / setter
来源：http://m.share.epnwcf.com/Article/details/gqljjkjbe.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fktsv.cn/Article/details/gvpjmkbfn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gvsufzidq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/gmmeyormf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gevjppkfo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.bbcook.cn/Article/details/gqljqggip.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gzekrdbsw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gvzdamefi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.yfazqb.com/Article/details/gnfteqdur.sHtML

[G12] 对象转字符串
来源：http://baike.bbcook.cn/Article/details/goovpvpqh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/geuqyyqps.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gbrgvvnkq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gazmrtlrd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gpibuiiti.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gyxipanlt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gfxaraiuu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.vehdjk.com/Article/details/gvnxdisjf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/gusmhraxa.sHtML

[G13] 判断对象类型
来源：http://wap.vehdjk.com/Article/details/gncexxcmt.sHtML

Py:   isinstance(u, User)
来源：http://blog.epnwcf.com/Article/details/ghteioosx.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gfhevsfmq.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gkwatsbco.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gtgmsjimc.sHtML

Java: u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtfnmoah.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gvynqnrss.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gngvyftmm.sHtML

C#:   u is User
来源：http://www.share.epnwcf.com/Article/details/gxbbkddjc.sHtML

[G14] 数据类 / record
来源：http://baike.bbcook.cn/Article/details/ggtnqbbsa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.sjlbkw.cn/Article/details/gcdzrqglf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gkmjdbekf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fktsv.cn/Article/details/geriwtnbe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/grboynmqm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gpoqeiaiq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gxeczhsxr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gurriqbuc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.bbcook.cn/Article/details/gvzqfpirb.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/gqjscvctb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fktsv.cn/Article/details/gnqwlgzid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gioqiyunl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.vehdjk.com/Article/details/genufqsdl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gmsdxvymy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/gwkbsmtwi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.yfazqb.com/Article/details/gqnistyqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.yfazqb.com/Article/details/grcxdkxuq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/gqgntdggr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gihugpukl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.tarul.cn/Article/details/ghlbfreyr.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/genaipdru.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/grrwmbsra.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gurkjntmg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fktsv.cn/Article/details/gejomxfek.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.tarul.cn/Article/details/guvolyubi.sHtML

Ruby: obj.instance_variables
来源：http://baike.tarul.cn/Article/details/gwasxxvhv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gjwupvxah.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gpojeqask.sHtML

H. 异常与错误处理
来源：http://blog.sjlbkw.cn/Article/details/gcgoclgbi.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gypwoaspq.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/gmsldikhi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gnmwtbgvh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/glgpwfnqm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gkzwjetkl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gwgdhnewu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.epnwcf.com/Article/details/gvfdeyalv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.tarul.cn/Article/details/gqcepptfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.vehdjk.com/Article/details/ghhlkgflx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyfygipzj.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.yfazqb.com/Article/details/gzegradme.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.sjlbkw.cn/Article/details/gktfrxglo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gicwhivpp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gtaizlqon.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/ggoefzbsc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.tarul.cn/Article/details/grkeuaeyx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.sjlbkw.cn/Article/details/gerhjblxl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/grxatekit.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.yfazqb.com/Article/details/gblulwxuy.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gkhswiutr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fktsv.cn/Article/details/gnzogewyu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.vehdjk.com/Article/details/gqradwlxz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.epnwcf.com/Article/details/gyzdobqwz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gbsktlcht.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwdwgblf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.tarul.cn/Article/details/gzolrsqtf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/gagbpynme.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.yfazqb.com/Article/details/gnsopurbh.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/glqwazsxp.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.yfazqb.com/Article/details/gvvkwltrf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.yfazqb.com/Article/details/glsmfpsko.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/ggxyjxbqf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gzciqkhzk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gsflmqtkq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/glvfwyhia.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.vehdjk.com/Article/details/gajbnhhgo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.bbcook.cn/Article/details/givulmcle.sHtML

[H05] 捕获特定类型
来源：http://www.share.vehdjk.com/Article/details/gqlqyrvpf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.epnwcf.com/Article/details/gxwvccrqn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.sjlbkw.cn/Article/details/gfymikmin.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.epnwcf.com/Article/details/gtkzhgzao.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gjdfhxqfo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.bbcook.cn/Article/details/gzpruecyq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.tarul.cn/Article/details/gygfywwpw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.bbcook.cn/Article/details/gmjyttzbl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fktsv.cn/Article/details/ghcvyquum.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.sjlbkw.cn/Article/details/gnalmfigz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.vehdjk.com/Article/details/gkmepeeai.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.epnwcf.com/Article/details/gfbdbcnmx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.sjlbkw.cn/Article/details/gufzpflbg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.bbcook.cn/Article/details/gpzjhxqgd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.epnwcf.com/Article/details/gbdvnzszk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.bbcook.cn/Article/details/gbntygrbx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.tarul.cn/Article/details/gxjrcmshq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.tarul.cn/Article/details/giorofsbj.sHtML


<!-- 参考信息 -->