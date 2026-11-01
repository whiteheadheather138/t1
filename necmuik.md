代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmoqftqji.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gnkwqnbhp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gzsexmjww.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/ghanotfab.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gupppbyiy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gqoafnvty.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gpzzmtibu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gxxkkwcex.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/glgqmfwtc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/geuhkrvri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/glxpwvbmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/gkudyhdmn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/gpaooxvti.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gpacbcowz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gokdusdyn.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gfxyavnbb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/grsfhrijz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/gqemcthvd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gbaiwbemz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gepbqhcld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.epnwcf.com/Article/details/gtpfkwmjj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gnmupxwac.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gnavwaful.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/glllvcrrf.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.epnwcf.com/Article/details/gfppemgii.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/ganziesrr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gsdvlvhrb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnkbgxoid.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/geryqslmh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gaurzflji.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/ghomlapdb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcgcdnqlo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghemnrdwa.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gxwfrzjkd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkyalupkj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/ghxqnekwd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gilyrcedp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gbqrnyevh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gadccatjh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gwmxycmnb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmocekjkx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/grbzzjpta.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.bbcook.cn/Article/details/glqeppqpf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gsogdvlnu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/glomzwvsr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gjzdzrdqm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.sjlbkw.cn/Article/details/ggjzlamhp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/gtgiypldf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gpejfclib.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/ghzmhwshc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.bbcook.cn/Article/details/ggrmwgbrz.sHtML

[F08] 遍历目录
来源：http://mobile.fktsv.cn/Article/details/gwvsgsqdw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/goekbgivq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/gmvvrwcgl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/giwibdzsy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gfomhxfqr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gefjvyjpg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gixrmssbl.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gdekkhekn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gzaghjajt.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/goucjphtr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gxynyfpxh.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ggjrtbzsv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gydefjzfx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gpjovvlzv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gwyckknez.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gitvtjnbn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gjnucxeun.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fktsv.cn/Article/details/gcrjbcvcl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gykzheevs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzytllio.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtawqnkyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcarqqwfl.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/ggmupsqrl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gssyfflya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxsoetyvj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gswbugimx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/getqhdacg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gfpepbswc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gokdrkdgj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gavdqgkle.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grmoboltb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gqnooehnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/goekrhhxb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fktsv.cn/Article/details/gdnhuondl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gegmnrdba.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.yfazqb.com/Article/details/gfvnmlnni.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gfcjgtpom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/gdlpzrrtt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gwettotkm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/glcjdivek.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gzknpclfo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gtfttrbiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gimcmztri.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.tarul.cn/Article/details/gpchvtlka.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/ggrodnkxi.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxtrcxngy.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gidmxjrhd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvmzlmgsy.sHtML

[G01] 定义类
来源：http://www.blog.epnwcf.com/Article/details/gijkwpyex.sHtML

Py:   class User: pass
来源：http://mobile.sjlbkw.cn/Article/details/gpuepwmnl.sHtML

PHP:  class User {}
来源：http://m.share.fktsv.cn/Article/details/gnwlzxojt.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gaolrwipd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gttorazrx.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gzifmfjes.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gngbrnceq.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gugfjvydx.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/ghvtgjhua.sHtML

[G02] 构造函数
来源：http://www.share.fktsv.cn/Article/details/gwjqkxwpk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/glkszloyf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.sjlbkw.cn/Article/details/glutrymgr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gvvqpfdqb.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/gtjyyrnbw.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gswiavdsw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gcqcqycjg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gwticzgsw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/gcoctzmis.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gxklcrakq.sHtML

Py:   self.name = "x"
来源：http://blog.fktsv.cn/Article/details/gdosmswyh.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gpdeqdsgy.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gcvxpceds.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gghlsveha.sHtML

Java: private String name;
来源：http://3g.bbcook.cn/Article/details/gazgrbbsz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/grumhprvh.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gmymsgljj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gakxxyprm.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gnxwppmlu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gspfewgsz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gaihzgnjm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gllejvraa.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gxecuxqtz.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gylplxjog.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.epnwcf.com/Article/details/gbjrejxmk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gnpuefjtr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.epnwcf.com/Article/details/gcshmcssq.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gfnvbsvjo.sHtML

Py:   class Admin(User): pass
来源：http://3g.vehdjk.com/Article/details/goddbxhkn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gegbvohzo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gbbsjpmpf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gjtwdaowo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gtugsepan.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/ggzrfecim.sHtML

Ruby: class Admin < User; end
来源：http://read.share.epnwcf.com/Article/details/gwombcamf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gebmtwglf.sHtML

[G06] 重写方法
来源：http://www.share.fktsv.cn/Article/details/gcbcumanf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.epnwcf.com/Article/details/gzwmzkznn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gwwrweiuz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gsnwniiug.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gikoyksby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gvabukluw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.bbcook.cn/Article/details/gybuomizd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fktsv.cn/Article/details/gaxfznmiu.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/gngyrghjx.sHtML

[G07] 调用父类方法
来源：http://3g.bbcook.cn/Article/details/gabwthbik.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gshyojjqn.sHtML

PHP:  parent::greet();
来源：http://mobile.tarul.cn/Article/details/ggwgoxaaj.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/ggzaclejm.sHtML

TS:   super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gxuireyrq.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gtpxnyqqi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.bbcook.cn/Article/details/gviiowqjp.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gmkeybavl.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gqpljpcdz.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/gbhjkyhxg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.bbcook.cn/Article/details/gwvyvjvxz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gwlkgrurh.sHtML

JS:   static f() {}
来源：http://m.share.sjlbkw.cn/Article/details/gqnhejkvh.sHtML

TS:   static f(): void {}
来源：http://www.share.sjlbkw.cn/Article/details/gvmdenqfy.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gtoyxbigw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.bbcook.cn/Article/details/gpxbzxlcx.sHtML

Ruby: def self.f; end
来源：http://www.share.yfazqb.com/Article/details/gihoonswv.sHtML

C#:   public static void F() {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvymzknbo.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.tarul.cn/Article/details/gikmhczru.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.yfazqb.com/Article/details/gmozczfxt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/ggulkzzgd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/glaidjtxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fktsv.cn/Article/details/gccnsufaa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdzjuaxxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.bbcook.cn/Article/details/gwrkyrbxr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/giyrfyjtb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/grwcegzvq.sHtML

[G10] 访问控制
来源：http://baike.tarul.cn/Article/details/ggqpxqhof.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.tarul.cn/Article/details/gafnmplel.sHtML

PHP:  public / protected / private
来源：http://3g.vehdjk.com/Article/details/gdrzavcxe.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gtsakllnt.sHtML

TS:   public / protected / private
来源：http://blog.fktsv.cn/Article/details/gfxohlunm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.vehdjk.com/Article/details/guaodhntt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.sjlbkw.cn/Article/details/gtgialoph.sHtML

Ruby: public / protected / private
来源：http://www.blog.sjlbkw.cn/Article/details/gznvxloxq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/gvcetqcwe.sHtML

[G11] getter / setter
来源：http://3g.yfazqb.com/Article/details/gzvrjlnph.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gehdavzrp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gsrcscupn.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gxaupvxhq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.bbcook.cn/Article/details/gusmgexcl.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gcyvkpadd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gmeitkecj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.sjlbkw.cn/Article/details/gstlzhelp.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.bbcook.cn/Article/details/gdnjrttva.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/gfhpgxneo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/gksdsdsmq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gvyjaetsp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gowublxea.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gvgfgmxeg.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.vehdjk.com/Article/details/gyiewqhpw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.sjlbkw.cn/Article/details/gklfddaxg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.bbcook.cn/Article/details/gukgqsxtx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.yfazqb.com/Article/details/gonbpfidl.sHtML

[G13] 判断对象类型
来源：http://mobile.yfazqb.com/Article/details/gbqvckyhe.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/guvircgwt.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gsfgdbkll.sHtML

JS:   u instanceof User
来源：http://m.share.vehdjk.com/Article/details/gwebvizya.sHtML

TS:   u instanceof User
来源：http://3g.bbcook.cn/Article/details/gopmmptez.sHtML

Java: u instanceof User
来源：http://3g.tarul.cn/Article/details/gotafstqb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.tarul.cn/Article/details/gnifystzl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fktsv.cn/Article/details/gjdloogag.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gtljqbjmm.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gmdrfvhhi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.sjlbkw.cn/Article/details/gfylmpojq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.bbcook.cn/Article/details/gsbhdcmlh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.tarul.cn/Article/details/gekogxfmq.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.yfazqb.com/Article/details/gvxogkfuh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gmqgtydzb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gbxdluyeb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.yfazqb.com/Article/details/gleeabhsg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.tarul.cn/Article/details/gqcyrhher.sHtML

[G15] 枚举
来源：http://blog.vehdjk.com/Article/details/gpsenjhhq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.bbcook.cn/Article/details/gsiibqlhk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.bbcook.cn/Article/details/gjrzbdsfx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/goemheiuk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.tarul.cn/Article/details/gqxsfuvyw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.tarul.cn/Article/details/gfqradygy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.bbcook.cn/Article/details/gvzmjqgzo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gegatpghm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gmppwuxge.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.bbcook.cn/Article/details/gwvkfxnkh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fktsv.cn/Article/details/gcevfziqy.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.vehdjk.com/Article/details/gqmdjzzsl.sHtML

JS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/gqmwjxduq.sHtML

TS:   Object.entries(obj)
来源：http://3g.yfazqb.com/Article/details/grfqrpapn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/ghkumsrpo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gpdemwwag.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gpbkqnrlm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.vehdjk.com/Article/details/gnjxtlqqs.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmqvswajx.sHtML

H. 异常与错误处理
来源：http://blog.tarul.cn/Article/details/gaccbjeem.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggjblqmvw.sHtML

[H01] try / catch 基础
来源：http://3g.fktsv.cn/Article/details/gnmqgkiro.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.sjlbkw.cn/Article/details/gihupifvm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.sjlbkw.cn/Article/details/gmpjystpz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gznvcbznx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gcrnhsofb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/geyycpebk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.vehdjk.com/Article/details/glnszxlia.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.vehdjk.com/Article/details/gbznysjzl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.vehdjk.com/Article/details/gvvonawpr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fktsv.cn/Article/details/gpzovwgxq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.sjlbkw.cn/Article/details/gzvatkwdt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gdbuczlqe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.vehdjk.com/Article/details/gdpksapjl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gyizxvpns.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.bbcook.cn/Article/details/gtymchxfo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.tarul.cn/Article/details/gcyvfwbtz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.epnwcf.com/Article/details/gegqkjows.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gnrzbavyg.sHtML

[H03] 主动抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gjaotpexc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gmgrrgxwb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/gdeoeikby.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gxftwrone.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/gljxpdchx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fktsv.cn/Article/details/gdvrnnqap.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/gposbcxlb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gfwexlkia.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.epnwcf.com/Article/details/ggtdnpstq.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gerczudga.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.yfazqb.com/Article/details/gswmwblsg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.bbcook.cn/Article/details/grfnyxkeo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gkadzxuxf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gguttyfsz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.epnwcf.com/Article/details/ggpezkqfe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.yfazqb.com/Article/details/gcyqotbhy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.bbcook.cn/Article/details/gmblbyfdm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.tarul.cn/Article/details/gcljkovhx.sHtML

[H05] 捕获特定类型
来源：http://m.share.fktsv.cn/Article/details/gtpviijxu.sHtML

Py:   except ValueError as e:
来源：http://www.share.yfazqb.com/Article/details/gxfyksqfd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fktsv.cn/Article/details/ghimwgdwt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fktsv.cn/Article/details/gufloqcxp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvrhqmlyn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gptzjfajv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.yfazqb.com/Article/details/gvgmzumzy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gjngxbfvc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.tarul.cn/Article/details/gdzjupgyd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.yfazqb.com/Article/details/gtvrogqhv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.epnwcf.com/Article/details/gjynwaqwj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.bbcook.cn/Article/details/gvuztdhrc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.sjlbkw.cn/Article/details/gzgwwiqow.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.epnwcf.com/Article/details/gxlrjtyob.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.bbcook.cn/Article/details/gbwxgbdpa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gwburkhxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.tarul.cn/Article/details/gedudknfw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.yfazqb.com/Article/details/gpmipzrpk.sHtML


<!-- 参考信息 -->