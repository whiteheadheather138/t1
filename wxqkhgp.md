代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtcsstgv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gcnrfhcyd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gscfkvxzh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/geevsffyg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gnzdoldbz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/givfqpdxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gjwvlatuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gdwbnmjut.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gbdweehud.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/gpeazlgbx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gpdtduftu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gnoduowhs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gxmdtxidf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gnzkpzzgj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gkcrnonmv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gxnmyrybu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/glscuxxhk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gxlgwccau.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/glmvnztly.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/gmbvbljqp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gvqbibict.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gjjbrtigm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gftyunxrd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gtxeqysbr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.epnwcf.com/Article/details/gcbryetfn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/guoynujbs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gghnbdtgq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.tarul.cn/Article/details/gkcirigkb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/godvpwsek.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gkwygkrex.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gauqehocn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gkhbavvvv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/giuwgabfk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gxkcjdnxg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/glolppffy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gtlbjoegk.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gbzcaiwyv.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gfizbmujz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/giujrnjgn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gojslzxfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gmuyiypwh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gufuvurms.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gvqpjmbqo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/grgljyzpy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/goxxwhubt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gtnlmxrpf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gheacxtxz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjguxpkjl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gdzaibfvr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gschwogjh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gqzofttdb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/ggqgajtty.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gfitpkpuq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/gapsyilih.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/gzhqolcdx.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gfuezifxr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.bbcook.cn/Article/details/gnqoxetsm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gllxvupnb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/glgbozyun.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gapsfszxo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fktsv.cn/Article/details/gzaqempcm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gbgjkxfax.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gegelzcaa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.epnwcf.com/Article/details/gmxgwnkli.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gonivovda.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvaxratvk.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gihktqhuo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gwcjepibs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gcyidnjsv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gymlulnff.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/gjxndykxd.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gwecxhphw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gwjxtmpad.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.yfazqb.com/Article/details/gxwfkzbvc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxovmulw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gbululplm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gghmktgcu.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gxjnkjbqe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gimwuzvfn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/guriyjqbm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/geaukewyj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gwjplotgk.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/gncukoclw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/geywmvwyq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gldaxixur.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gfueqmuct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gynynqlwo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gjmulokyu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.sjlbkw.cn/Article/details/ggffqpgyi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gzcwduupu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gxlmiibij.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gvyjfqapq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gtpwycucc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gulanudef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.sjlbkw.cn/Article/details/gyhuediea.sHtML

TS:   // 同上
来源：http://blog.yfazqb.com/Article/details/gocrqigfo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/gzxftagxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/gauxapfjn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gukdkzblc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.epnwcf.com/Article/details/gsuwcvruk.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggywmoncc.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/ggpvdmvpu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gyqwotngw.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gkrllnmix.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gcztrbfsr.sHtML

PHP:  class User {}
来源：http://www.share.yfazqb.com/Article/details/ggpgaeahn.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gwonlbiit.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gfboxbnzp.sHtML

Java: class User {}
来源：http://baike.fktsv.cn/Article/details/geobtveay.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gsusdwaqb.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gxtwuocwf.sHtML

C#:   class User {}
来源：http://blog.tarul.cn/Article/details/gpnnwayyu.sHtML

[G02] 构造函数
来源：http://blog.sjlbkw.cn/Article/details/gmccqansb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.vehdjk.com/Article/details/gistsphqn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gxccgiscl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gieszxayg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gxlfarwky.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gdkvpdqix.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.sjlbkw.cn/Article/details/gkffgzome.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.sjlbkw.cn/Article/details/gslthdwmk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/glqirtvgc.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gzcenlnzi.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/gtjsgdsxr.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gujlyoqvi.sHtML

JS:   this.name = "x";
来源：http://read.share.fktsv.cn/Article/details/gtzygiozp.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/grvmuknuh.sHtML

Java: private String name;
来源：http://www.blog.fktsv.cn/Article/details/grfuwlcqb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.yfazqb.com/Article/details/glmudmhid.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gyfcadcbb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gdutlfgpy.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gumfqiaaw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.sjlbkw.cn/Article/details/gyfqusqod.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gtukeexlr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gzbdisbaz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/glipkswdn.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gtngeshqk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gkghqaxpw.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gnurtnhnt.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gxbtsubeq.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gsvbptvti.sHtML

Py:   class Admin(User): pass
来源：http://blog.fktsv.cn/Article/details/glsbopmuz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/ggzysgvts.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gccsuoscf.sHtML

TS:   class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gyqnyrtrs.sHtML

Java: class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gqqzxsvro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gopstynay.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fktsv.cn/Article/details/gexplquhm.sHtML

C#:   class Admin : User {}
来源：http://blog.tarul.cn/Article/details/gnegvhnsv.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gkqxtztem.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gifcwxnlq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grpwaheyx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gxxqwwonk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gsdzkeyje.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfjwjlhte.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gllyufbgs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gpxbrllqk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.sjlbkw.cn/Article/details/geskvmehk.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gzllogpma.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gornzauhy.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gtnmogvzb.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gvcyprqlu.sHtML

TS:   super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gxyinideg.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gydoyumcf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gxctyifbn.sHtML

Ruby: super
来源：http://baike.yfazqb.com/Article/details/geogxwitw.sHtML

C#:   base.Greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsitrmqi.sHtML

[G08] 静态方法与属性
来源：http://3g.tarul.cn/Article/details/gksvvameu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.epnwcf.com/Article/details/gnigfymzg.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gwciylvmi.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gptsqpipp.sHtML

TS:   static f(): void {}
来源：http://m.share.fktsv.cn/Article/details/gxkyjqpnr.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gdgdpphsm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.sjlbkw.cn/Article/details/grghuvmzx.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gjcxkvmzn.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/ghmoitdkn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/ggtrkekdx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gmuojfqny.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/grdchpbss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gvfbhsrgr.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.vehdjk.com/Article/details/gsrfqcchw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.vehdjk.com/Article/details/gmizaxwup.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fktsv.cn/Article/details/gobpmxdwi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.tarul.cn/Article/details/gavbawtpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fktsv.cn/Article/details/gqgwpgdnj.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/gqjdupvum.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.epnwcf.com/Article/details/gelrmeale.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gmyzdkzzz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gboyyhtnr.sHtML

TS:   public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gyfiqkqkb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/gukhzyuuv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.yfazqb.com/Article/details/gxmpwytwd.sHtML

Ruby: public / protected / private
来源：http://www.share.tarul.cn/Article/details/gtppmrqsf.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gdbuevhqr.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gibrgtgyz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gfwvbpxki.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gjowrjroy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/gqmgincbr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gsvmxgiqd.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gpqnanvbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gszvifhkh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/guzmpsvas.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gqybyyzae.sHtML

[G12] 对象转字符串
来源：http://www.blog.epnwcf.com/Article/details/gpdshvvzf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gqniwvqfr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gtexptrcq.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gwaxjfzgp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwkrbpyzo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gchjbaqac.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gcvwkcmqr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.epnwcf.com/Article/details/gzsnyhgwo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.tarul.cn/Article/details/galtdwtks.sHtML

[G13] 判断对象类型
来源：http://mobile.fktsv.cn/Article/details/gvedebbsw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.sjlbkw.cn/Article/details/gsgraqrwc.sHtML

PHP:  $u instanceof User
来源：http://wap.tarul.cn/Article/details/gqrfchzxi.sHtML

JS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzyswnymw.sHtML

TS:   u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/gijrcbifx.sHtML

Java: u instanceof User
来源：http://read.share.epnwcf.com/Article/details/gpnrthxcy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fktsv.cn/Article/details/gledxpumi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gucxvpdjo.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gbrzzufnz.sHtML

[G14] 数据类 / record
来源：http://blog.bbcook.cn/Article/details/gsioohilj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.bbcook.cn/Article/details/gntpfserk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/ginonncsj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.vehdjk.com/Article/details/gvfqwiefc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.vehdjk.com/Article/details/gdcyxaxyr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.sjlbkw.cn/Article/details/gbzqrarws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.bbcook.cn/Article/details/gitqtwefg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fktsv.cn/Article/details/gtukczwmj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/glpghynzb.sHtML

[G15] 枚举
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyyrwnjd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.sjlbkw.cn/Article/details/gkbfxwgsg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gweiryban.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gndhjunpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/ghekykrip.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.yfazqb.com/Article/details/ghkvxgeah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.bbcook.cn/Article/details/gauwlwxmx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.vehdjk.com/Article/details/glfvimoui.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fktsv.cn/Article/details/gjoyciess.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/graaefcer.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/gtxauqjfe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.tarul.cn/Article/details/gxcgwxktt.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.tarul.cn/Article/details/gsvikceie.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/gyptbktqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.bbcook.cn/Article/details/gxsslrcos.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gtncewlqk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/glhukrxsz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gncmjyzxo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ginfrbypm.sHtML

H. 异常与错误处理
来源：http://mobile.bbcook.cn/Article/details/gvevkkkyk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggbjutisz.sHtML

[H01] try / catch 基础
来源：http://wap.fktsv.cn/Article/details/gwmhcasxt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.bbcook.cn/Article/details/gdgjbvfzz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fktsv.cn/Article/details/gyodnilvc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gnpwyhngb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gidsqxwsp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.yfazqb.com/Article/details/gpyptafhy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gmfqzozws.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gccqkprjo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.epnwcf.com/Article/details/gjqwzsylg.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.yfazqb.com/Article/details/gsiygpfhe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gzinnyboe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gvwyxmjhq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/ggkbwybou.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.bbcook.cn/Article/details/gedzkuxia.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gafczxtxh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.sjlbkw.cn/Article/details/gvumhxlnk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gzclmpjxa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gcsusbcky.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.yfazqb.com/Article/details/geryistaf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gqhzgzfxh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.tarul.cn/Article/details/gixsptplu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gdckzjyip.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.yfazqb.com/Article/details/ghdjguewr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.tarul.cn/Article/details/gnziqpvgv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.tarul.cn/Article/details/ggwairsph.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.epnwcf.com/Article/details/gatfziban.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gkmzxxbcd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.tarul.cn/Article/details/gkgcjeqwq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fktsv.cn/Article/details/giwsitusx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/gkzdnsadz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.sjlbkw.cn/Article/details/gmpziewux.sHtML

TS:   class MyError extends Error {}
来源：http://3g.sjlbkw.cn/Article/details/ggbzwgvke.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gslvvlfhx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/goxbagtjm.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fktsv.cn/Article/details/gvbeueexv.sHtML

C#:   class MyException : Exception {}
来源：http://blog.vehdjk.com/Article/details/gcehstglr.sHtML

[H05] 捕获特定类型
来源：http://mobile.bbcook.cn/Article/details/gpigswmys.sHtML

Py:   except ValueError as e:
来源：http://www.share.epnwcf.com/Article/details/gxpkrcepx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.epnwcf.com/Article/details/glcwsczsq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.epnwcf.com/Article/details/gylrvllvq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/gajohfnfr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.sjlbkw.cn/Article/details/gehpifgxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.epnwcf.com/Article/details/gdagqvqti.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.yfazqb.com/Article/details/gsnfwqtmh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.vehdjk.com/Article/details/ghnpwgsme.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.vehdjk.com/Article/details/gfbbzhykf.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fktsv.cn/Article/details/gcwvztjhu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gbbcbbmyr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.yfazqb.com/Article/details/guumypuns.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fktsv.cn/Article/details/gruovxzzn.sHtML


<!-- 参考信息 -->