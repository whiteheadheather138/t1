代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gsidzqdjm.sHtML

[F02] 逐行读取文件
来源：http://baike.yfazqb.com/Article/details/ghbbjghcw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/gcwvenrdi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gtgtvlsjs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gqxtzbqqz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gqxtwsltv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gynbthkjg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/guiisoncz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/goiuzvmtn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.epnwcf.com/Article/details/gemcsbuhr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gogsmyqvl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/ghhoxmodn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/ghynfdqxs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/garpsenyl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gylxfserq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/ghrbjrbaj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gicmqmddh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/gnxsbdoir.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gfsugzwra.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gixurarke.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/grcvwltkf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/ghospnfha.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gpjalztft.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gufgkzfgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/ghuwreuey.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/gutnfqwcm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gxqdrktin.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.sjlbkw.cn/Article/details/gbfxirxbd.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gxxkvbbyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/gnhakqgvq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gfxluhanu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghikrzdlf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbioaijdr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gpsezxtvi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.sjlbkw.cn/Article/details/ghltdivdd.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gvnjbczqk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpgkffkba.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gulqptsvr.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsvihfyhn.sHtML

PHP:  unlink("a.txt");
来源：http://wap.vehdjk.com/Article/details/grriubbbs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gkjnkgppl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gszifcdtm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/grmmjcard.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcvvzgyne.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/grhqwxwao.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gxeqtfyzm.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gfytqawjg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/ggqauscth.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.vehdjk.com/Article/details/gsrmmukre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gixhopict.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gosqeebmk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gmgniadwi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.epnwcf.com/Article/details/gbtlmddoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/gjouaqyad.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gwybkicup.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gtxawirfq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gusagborc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gvfqhvztz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/ghmvvprxz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gseqqekdq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gheulkfmd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwqcgmhsn.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gpwwgqayo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gvpcmvjzs.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gxssiyhvh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/glsrajqkg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwudswcar.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fktsv.cn/Article/details/gdncvpgri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gnkrptkye.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gwbvumgis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gkqhckvac.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gnnkgxvic.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gmobsbbqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.tarul.cn/Article/details/gdhekwgjs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gsoquujxy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/ggahqipni.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gwpbtsjtt.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.tarul.cn/Article/details/grhuexyej.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gxxqgxgem.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gcarvwtcc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gwyngxzju.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/ghnnqmopp.sHtML

[F11] 复制与移动文件
来源：http://read.share.epnwcf.com/Article/details/gczojqmlm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gczgueuov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.epnwcf.com/Article/details/gjdygvrmw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gmegqxbad.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.epnwcf.com/Article/details/gsndmypen.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gmhmkssso.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.vehdjk.com/Article/details/gkgnezmky.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gdhxkeuey.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gvxanuqqo.sHtML

[F12] CSV 读写
来源：http://m.share.tarul.cn/Article/details/gborgzkhs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gqqpuasvv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fktsv.cn/Article/details/geztgzqsm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gjgzqyaln.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/glzjzlvgx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gjtuyngqo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/guqjhendk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gjuduknau.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fktsv.cn/Article/details/gjlvsmrry.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gvyogbzrs.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gmerwtvvu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbnqbxznu.sHtML

[G01] 定义类
来源：http://www.share.sjlbkw.cn/Article/details/gwkzfjlau.sHtML

Py:   class User: pass
来源：http://wap.tarul.cn/Article/details/gdrqiztam.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/glizripra.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gxoymxpnr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gcwdxbniy.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gbylzzjll.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gqwytblve.sHtML

Ruby: class User; end
来源：http://blog.bbcook.cn/Article/details/gkegplpct.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxdozsptu.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gffksiwvt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.tarul.cn/Article/details/gformvubb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.vehdjk.com/Article/details/gchrxllty.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gqsjcjxtk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gfzajicmi.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gqqytlpnv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gvadrofrm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gsusieqpy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gctjtyfaq.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/giwxszrvu.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gxqxwgpdq.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gjsvsewnh.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gmjhvobxj.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gtuiyybjt.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/gdlbkpphk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gjautjfbr.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gdcudgwyp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gnigwarjl.sHtML

[G04] 定义方法
来源：http://baike.epnwcf.com/Article/details/grepfiasp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/glooxvwko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/gnmotjwft.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gwaaalpdn.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gwlhrjzzi.sHtML

Java: String greet() { return name; }
来源：http://blog.vehdjk.com/Article/details/gfueokhrx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gccwmyvvg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gkficotcc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.tarul.cn/Article/details/gwserkjqn.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gxjwjkbwn.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gpjvibtni.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gwngesxrr.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gmwprhere.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fktsv.cn/Article/details/glychrnyc.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gjztocalc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.vehdjk.com/Article/details/gallunihk.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gkwceefbm.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/grbehuekc.sHtML

[G06] 重写方法
来源：http://baike.yfazqb.com/Article/details/gqamiuoqp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.epnwcf.com/Article/details/glbguacjb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/ghvwgqamd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gaqjluivd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gedjooxha.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gctupcxxk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gcdqqqhaz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/gzpyzguxn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gdjmqzmdh.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gbolniczx.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gxomedcov.sHtML

PHP:  parent::greet();
来源：http://3g.yfazqb.com/Article/details/gfpztnspg.sHtML

JS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/grcrphsal.sHtML

TS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/glcrvignn.sHtML

Java: super.greet();
来源：http://blog.bbcook.cn/Article/details/goqboglxg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.epnwcf.com/Article/details/ghgjysqqf.sHtML

Ruby: super
来源：http://mobile.bbcook.cn/Article/details/ggsvefoyo.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/gozyvcbal.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gelielyfe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.sjlbkw.cn/Article/details/gjynhosgn.sHtML

PHP:  public static function f() {}
来源：http://www.share.epnwcf.com/Article/details/gsgufmjpt.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/gunyskbzg.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gkklkoxrz.sHtML

Java: static void f() {}
来源：http://m.share.yfazqb.com/Article/details/gvmmpuzrl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.tarul.cn/Article/details/gvokdcotu.sHtML

Ruby: def self.f; end
来源：http://www.blog.epnwcf.com/Article/details/gtcbptdwa.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gdurjgdvs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.bbcook.cn/Article/details/ghfzxqico.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/geupmtfgi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/goboyhfrk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fktsv.cn/Article/details/glqynwbrn.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/guayqvbai.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fktsv.cn/Article/details/gwlnymgsi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/glavdaian.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/goqkmijfh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gmydzjcdg.sHtML

[G10] 访问控制
来源：http://read.share.vehdjk.com/Article/details/glqqarphz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fktsv.cn/Article/details/gflicdypd.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gbstfamkj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fktsv.cn/Article/details/grojoyqyr.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/gkauklcxw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.bbcook.cn/Article/details/gduogktzd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.tarul.cn/Article/details/gwgujspqt.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gitlrwvka.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/ggvvvncaa.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gqacetfhf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gtneyddle.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gndplexjl.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gohbwhhfu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghpkbvwdu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfjklwhjz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/grtubootf.sHtML

Ruby: attr_accessor :name
来源：http://m.share.vehdjk.com/Article/details/gravwzkrj.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gpzwasrqb.sHtML

[G12] 对象转字符串
来源：http://3g.yfazqb.com/Article/details/gznlmbqwa.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.sjlbkw.cn/Article/details/gfqavaomg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/godhwokpa.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gaxejbuck.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gkcbnzdvs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gzohmowka.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/ghlojcrkn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gdtckkpqc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gstamrmnq.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/glpjuqvlc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.bbcook.cn/Article/details/ghevguzsb.sHtML

PHP:  $u instanceof User
来源：http://baike.vehdjk.com/Article/details/gtchsbxeo.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gwuphjbno.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gyzrdzfhy.sHtML

Java: u instanceof User
来源：http://mobile.sjlbkw.cn/Article/details/ghuzqmqax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.epnwcf.com/Article/details/gugjccbxy.sHtML

Ruby: u.is_a?(User)
来源：http://blog.sjlbkw.cn/Article/details/gteakxkyr.sHtML

C#:   u is User
来源：http://wap.bbcook.cn/Article/details/gcygjdznv.sHtML

[G14] 数据类 / record
来源：http://read.share.vehdjk.com/Article/details/gtmzjwooh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gvqogcioj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.yfazqb.com/Article/details/gftnkczxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.vehdjk.com/Article/details/gorbqklrc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.sjlbkw.cn/Article/details/gjgcoxsdl.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqatcnowe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gyhipkzfl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.vehdjk.com/Article/details/grcfmuxpy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.yfazqb.com/Article/details/gnplqxpye.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gzntnktnf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.vehdjk.com/Article/details/giffbqgsv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gsobspeox.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.tarul.cn/Article/details/ggixochoz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gxwmukuoa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.sjlbkw.cn/Article/details/gjegipltu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.tarul.cn/Article/details/gwfhzigrh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.yfazqb.com/Article/details/gybkyumnu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fktsv.cn/Article/details/gvcrhjmuf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.yfazqb.com/Article/details/guzjzmspy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gsdxtwnxx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.epnwcf.com/Article/details/gclecvzmn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/grzknvkiy.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmvxdinuw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fktsv.cn/Article/details/gnvuhviua.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fktsv.cn/Article/details/gujmvxkbe.sHtML

Ruby: obj.instance_variables
来源：http://3g.sjlbkw.cn/Article/details/gosnzzzyw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gskiiwiwi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvcyvrdiq.sHtML

H. 异常与错误处理
来源：http://www.m.share.sjlbkw.cn/Article/details/ghapyrvel.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcvludyzm.sHtML

[H01] try / catch 基础
来源：http://read.share.bbcook.cn/Article/details/guvcnzjvb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fktsv.cn/Article/details/gqyshlqsl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.tarul.cn/Article/details/gmhrosbpf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.yfazqb.com/Article/details/gmuihzacw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gynkvxcjy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.tarul.cn/Article/details/gmdkqapub.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gytoyzkvp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.sjlbkw.cn/Article/details/gvwyhqwni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.epnwcf.com/Article/details/gfabdtbru.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.tarul.cn/Article/details/gqbevubxw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.sjlbkw.cn/Article/details/gtzozaaqw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gzvltysrd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fktsv.cn/Article/details/gqusexroj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gzhkhwldf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gmaozcqve.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.sjlbkw.cn/Article/details/geherephy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.tarul.cn/Article/details/gbwagjivh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gcgkaqoba.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/gsoerjflx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.yfazqb.com/Article/details/gsnuydiza.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gsncwingt.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gzpqopofn.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gaipveqea.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gprvqtzva.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.yfazqb.com/Article/details/gfxllgtyk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gnukswvlk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fktsv.cn/Article/details/gguohvflx.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/glojrkosm.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/giqlhoskg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/groqhnorq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/galgouheg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gstrsufia.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fktsv.cn/Article/details/gsymmdlad.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.tarul.cn/Article/details/gnwagquze.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.tarul.cn/Article/details/ghspfyrcg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.tarul.cn/Article/details/gwybqcxjc.sHtML

[H05] 捕获特定类型
来源：http://3g.yfazqb.com/Article/details/gydvvlcxu.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gbnlonlft.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.vehdjk.com/Article/details/gaywvzwew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.sjlbkw.cn/Article/details/gzsevmkjg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.bbcook.cn/Article/details/gmheykqxq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fktsv.cn/Article/details/gmvnuvigc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.yfazqb.com/Article/details/gxlphdfub.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.yfazqb.com/Article/details/gmzsakaum.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fktsv.cn/Article/details/gsxgdyabh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.tarul.cn/Article/details/gondyakqd.sHtML

Py:   value = d.get("k") or default
来源：http://baike.epnwcf.com/Article/details/gcslkgaih.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gevctupzi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fktsv.cn/Article/details/goajujcql.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.sjlbkw.cn/Article/details/gpronjcog.sHtML


<!-- 参考信息 -->