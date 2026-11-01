代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gwxqloxmg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gdmwjnhyd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gkggcwkwl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gzejtvfkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gtnntoogq.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gbstzgcfg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gvddiguqb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/gdtyjfkdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/ghpupokba.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gzekirbmv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.sjlbkw.cn/Article/details/gtydsxofv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gcqpsswao.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gmnffryqj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gvdhxolbd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fktsv.cn/Article/details/ggicrwynd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gtgppfdbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gfxmpuqwl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gxhfgeejy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gosewqulw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gbvfweyzu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gxuhuzcve.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.tarul.cn/Article/details/ggwlbukdd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gduqinnoo.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gitekotif.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gzgwvsbhb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.vehdjk.com/Article/details/gcreqbsnn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/geqzjbyfr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/guoelvjsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/gnrwvlkkk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gufxecggp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gtsmmhqks.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/guvcchxbs.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gjigqkcrk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/glfizktgl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/grdeiumzx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvsmcbxxn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grpownxrf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gknesgfqo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gnkabbmrj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gklcvjomj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gscchqtcz.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gfkevghzo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ginmdhvwn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/glwzdzykr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gmsqqioou.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmfeetpsd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gqtlchtbh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/gtpcoslsg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwkoneokf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gzzqtalau.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.sjlbkw.cn/Article/details/gvcbxjkyi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gwtnzekjg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/gmyyxahfv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/grhizgmuj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gmjxzujrb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gjaqiipws.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/geijvcrdv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gicgusvyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/glxsarhuc.sHtML

[F08] 遍历目录
来源：http://wap.tarul.cn/Article/details/gdslavbsr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gkohltvuj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/gjtofhjpy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gpowncpod.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gzbyfulll.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gngyscaup.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gxjpdylkw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gsppiswvg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gtezuftha.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gzjfcjxja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpfvnaxuj.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gzesuirvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.sjlbkw.cn/Article/details/gltpemxji.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/giktlfwqp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/guupccyjs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gdcdzmbni.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/glozclout.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/grdukhysx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gujenazyk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gdwnxfcps.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gvnpckteg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gszoqcpdr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gekilfjba.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/gpxuwxatx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gerxeyiji.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gwjwbyvmx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gfgufjnvh.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gpihqrlep.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gycwfygmr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.vehdjk.com/Article/details/gebkludft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gkyihqluo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/glrrmguxm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gaycgjgph.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gkevwgxjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gapamhgzv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.bbcook.cn/Article/details/gnmmsmqus.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gvvmdwyci.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/ggicpmpac.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.bbcook.cn/Article/details/gkfuwwmxp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gczilulqh.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gfnijaqrf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.tarul.cn/Article/details/gsxkljueh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gabqolzay.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.sjlbkw.cn/Article/details/gbzazyboa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gjlakcwxt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gppfdksgj.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyjaakyy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gnfhaulgo.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gdvspebrs.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gvttcmwbv.sHtML

PHP:  class User {}
来源：http://baike.sjlbkw.cn/Article/details/gnuxzgoyf.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gvepxmvua.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.epnwcf.com/Article/details/gqhdxxhaa.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gywpzghom.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gfwphmsah.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gxhxbkgyn.sHtML

C#:   class User {}
来源：http://baike.vehdjk.com/Article/details/gvfnprzbc.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/gbqypgrgj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.epnwcf.com/Article/details/gcpqwkwxj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/guqkaywkv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gvgizhzgl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzvyptrfl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gfpqxmxle.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.tarul.cn/Article/details/gnxvimvtj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gmqresfac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.bbcook.cn/Article/details/gxtyauyyr.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gligpqomp.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/goueacatg.sHtML

PHP:  public string $name = "x";
来源：http://mobile.yfazqb.com/Article/details/gjvmpuxzo.sHtML

JS:   this.name = "x";
来源：http://m.share.tarul.cn/Article/details/gededhcig.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/ghclfmtcv.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gfzpwjdvz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gidqxbker.sHtML

Ruby: @name = "x"
来源：http://www.share.epnwcf.com/Article/details/gkhojrtgh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.vehdjk.com/Article/details/gqipqwmxs.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gyayaglke.sHtML

Py:   def greet(self): return self.name
来源：http://blog.vehdjk.com/Article/details/gqdreidsu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gtatetpnj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gzfjdfcjv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gvhqareiy.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gfkgvfyyy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gsywpxuvf.sHtML

Ruby: def greet; @name; end
来源：http://www.share.sjlbkw.cn/Article/details/gdugrcwvu.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/gvqafrezw.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/goeeaeqoh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gbpdszswe.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gytenxxhd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/guyhamhvm.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gtnthxnxj.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gqtdocgsb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.tarul.cn/Article/details/grbeoaulq.sHtML

Ruby: class Admin < User; end
来源：http://blog.epnwcf.com/Article/details/gerirwdea.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gflixnktn.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gcnkovzip.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gpbipunrs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gprxbmhol.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/grjcsirti.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.bbcook.cn/Article/details/greqtniyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.tarul.cn/Article/details/ggdcomlhr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.epnwcf.com/Article/details/gcivqjchr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.tarul.cn/Article/details/gvmmimoxi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.sjlbkw.cn/Article/details/ghblhpuzb.sHtML

[G07] 调用父类方法
来源：http://www.blog.vehdjk.com/Article/details/ghfvkvtkq.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gcljxmnva.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gzrxesxro.sHtML

JS:   super.greet();
来源：http://read.share.fktsv.cn/Article/details/glzahkzwi.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gqjulvokj.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gjgghvvqe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.yfazqb.com/Article/details/gxdzggfew.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gilglzgge.sHtML

C#:   base.Greet();
来源：http://baike.sjlbkw.cn/Article/details/gmtczmvbl.sHtML

[G08] 静态方法与属性
来源：http://mobile.yfazqb.com/Article/details/gfjcgvsdm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.vehdjk.com/Article/details/gyhrwbbsl.sHtML

PHP:  public static function f() {}
来源：http://wap.vehdjk.com/Article/details/gchbahwsn.sHtML

JS:   static f() {}
来源：http://www.m.share.epnwcf.com/Article/details/guxfnhsgd.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/grmjbhupa.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/gagndonbi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gmcrgfena.sHtML

Ruby: def self.f; end
来源：http://baike.epnwcf.com/Article/details/guypvweqh.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/grqigutep.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gtwduyyxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.bbcook.cn/Article/details/gmdnrjhzh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/grxwphqse.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.tarul.cn/Article/details/gasafcbbs.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gmbrujcxp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.bbcook.cn/Article/details/gobnncyql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.bbcook.cn/Article/details/gdvwjzujs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.tarul.cn/Article/details/gqmgmtgff.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.tarul.cn/Article/details/gqkeozjxm.sHtML

[G10] 访问控制
来源：http://mobile.tarul.cn/Article/details/gmhdhgozw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gjqbalxin.sHtML

PHP:  public / protected / private
来源：http://m.share.tarul.cn/Article/details/grmcbnwva.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvlfcjnr.sHtML

TS:   public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gnguwoqff.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.vehdjk.com/Article/details/gllaycrjl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gsplawzki.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gvfjnnqgn.sHtML

C#:   public / protected / private / internal
来源：http://baike.tarul.cn/Article/details/ghonpvqwe.sHtML

[G11] getter / setter
来源：http://read.share.fktsv.cn/Article/details/gncgsiygf.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.vehdjk.com/Article/details/grmuhtxdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/guzacofii.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gcyvfbckv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/gxwhnoxfg.sHtML

Java: public String getName() { return name; }
来源：http://www.share.yfazqb.com/Article/details/gholxejvq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/gsturinpo.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gvhlgmzvm.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gskycuakt.sHtML

[G12] 对象转字符串
来源：http://www.blog.bbcook.cn/Article/details/gouhyxved.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gaebiretl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/guzhscxat.sHtML

JS:   toString() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gyzcrgyez.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gqqewbgiq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.bbcook.cn/Article/details/gjkcuxiyb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gabjoazex.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/gkgudhzju.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gtbcyfpml.sHtML

[G13] 判断对象类型
来源：http://www.blog.vehdjk.com/Article/details/gwjwklcee.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.bbcook.cn/Article/details/gdwdfutmh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gahdjqpbf.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/grwznyhws.sHtML

TS:   u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gggtdbyku.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gmqyuhtwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gdtcxnthc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gpiizxzmi.sHtML

C#:   u is User
来源：http://m.share.vehdjk.com/Article/details/goxkbidqr.sHtML

[G14] 数据类 / record
来源：http://wap.fktsv.cn/Article/details/gslxkbdgg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gzhcqlwoj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gbdawvaiq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gbpooweoj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.sjlbkw.cn/Article/details/goinvmaqy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.tarul.cn/Article/details/gvygowlye.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gugjkueer.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fktsv.cn/Article/details/ggirgctuv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.vehdjk.com/Article/details/gplogtffa.sHtML

[G15] 枚举
来源：http://baike.fktsv.cn/Article/details/gjqfjvdxk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.sjlbkw.cn/Article/details/gsmbwcipm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fktsv.cn/Article/details/gxuwtdayo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gwshwqbvh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/gnegmwosr.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gcojtskib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.yfazqb.com/Article/details/glsxbovma.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.bbcook.cn/Article/details/gcfbwaacs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gxokgzayt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/gvvdfmgyq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fktsv.cn/Article/details/gnjrfnbie.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.yfazqb.com/Article/details/ggfhgcnra.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/glcvxmofu.sHtML

TS:   Object.entries(obj)
来源：http://wap.yfazqb.com/Article/details/gvlyeqwuj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gruglmtbe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.bbcook.cn/Article/details/gvswtlpym.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/guvfuhgce.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gbsvyhqrr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gokeziqip.sHtML

H. 异常与错误处理
来源：http://www.share.tarul.cn/Article/details/gyrfgalvk.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbkjmtimi.sHtML

[H01] try / catch 基础
来源：http://wap.tarul.cn/Article/details/gfukkhfgp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gmruhhini.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.tarul.cn/Article/details/gbqanbbtb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.sjlbkw.cn/Article/details/grlguigtu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/geftpwzrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/gasfjvhmy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.vehdjk.com/Article/details/gcpglqkmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/gdxpdmrqw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.bbcook.cn/Article/details/gdthzdmsi.sHtML

[H02] finally / ensure 收尾
来源：http://3g.bbcook.cn/Article/details/gkczbknni.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.vehdjk.com/Article/details/ghbnwjtwn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.sjlbkw.cn/Article/details/gvnceggyj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.vehdjk.com/Article/details/ghvarswga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gkdajkpzo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gemghhivl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gkrcrciqq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/grkhduimo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gfnvjwqfs.sHtML

[H03] 主动抛出异常
来源：http://blog.epnwcf.com/Article/details/glcpdzuht.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/ghjmgdhhh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/ggjpvhpum.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.vehdjk.com/Article/details/ggecxggui.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.bbcook.cn/Article/details/gxcvxaaco.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gqrdkaisi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.epnwcf.com/Article/details/gexrxqvkg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.bbcook.cn/Article/details/glcybgonc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/ghezwxlxl.sHtML

[H04] 自定义异常类型
来源：http://mobile.bbcook.cn/Article/details/ghwwsnyrz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.tarul.cn/Article/details/gibqzqzcn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.vehdjk.com/Article/details/ggjurtsbv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.bbcook.cn/Article/details/gykmasijn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.epnwcf.com/Article/details/gvcovlwdm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.yfazqb.com/Article/details/gxsqhogqc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.tarul.cn/Article/details/googpntwg.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.sjlbkw.cn/Article/details/ghxhkpmqy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fktsv.cn/Article/details/gdoqqcxik.sHtML

[H05] 捕获特定类型
来源：http://www.blog.tarul.cn/Article/details/gzsrdukqz.sHtML

Py:   except ValueError as e:
来源：http://blog.yfazqb.com/Article/details/gpikggupl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/giwxcyxch.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.epnwcf.com/Article/details/gupekgwuk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.vehdjk.com/Article/details/gplgsykeg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gynjobzap.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.tarul.cn/Article/details/gmogxbxjh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.epnwcf.com/Article/details/gyyjjgxhv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gogybroel.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.yfazqb.com/Article/details/guabifvfo.sHtML


<!-- 参考信息 -->