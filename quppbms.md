代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/ghfkgnrjv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gruhaotjr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gdrmdokpj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/gosxjqgsr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.tarul.cn/Article/details/gotcxpzpd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gtnmuvkpq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gqxozycii.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gzzjkreln.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gdfduzmmh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/glgcplxfw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gpdsebblx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/gnprpthxj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gknqwurpy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/gmburjfwy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/galhusxta.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gxapednom.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gvvspcbju.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/ghasqhtjl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/glwzcjtyb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gsuaekzlt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.vehdjk.com/Article/details/gjilvburh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gtsujczdf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gwgoillco.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgjygpnc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/griybickg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gaijfpezw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gqmixpuvp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gmxcdldfr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gchztziub.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/glzyxqwnv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gykepyjyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyepxunuj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gnxbcwrlh.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjsgmmtf.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gkotrejqt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.vehdjk.com/Article/details/giqnqqeer.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grmumehof.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gyrzxqmoz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/glcqvxkgq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggqpxhkrm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/geicjpbcu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gouammctj.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/grbvtvrgs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gowabdwyt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gxpxwzmkp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/grhluuayn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/gsvfilzvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gxhkuquhi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/golxplenm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.epnwcf.com/Article/details/gwvnffriq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gribnsnzi.sHtML

[F08] 遍历目录
来源：http://baike.sjlbkw.cn/Article/details/grebfwqzf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gaumxladu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gnjldhffo.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gvyrzgceq.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gknipjfzp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gpmmzzgit.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.vehdjk.com/Article/details/gkyvhznoa.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/ghvpxvijx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gmlvsrwwm.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/getksqdji.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gqlgdtpyu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gpnjawrch.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gvjclijyv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/goorofqve.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/greobgpnw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/grmzyiwyl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/guzxrptda.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gfqlxuiuq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/gwmhhafnl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gtqxvenfo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.epnwcf.com/Article/details/gxoymhxoo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gfcwjojde.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfpxvydzf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gpsijysxk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/ggfjolcsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gjrgvchoy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gpwwnlowr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fktsv.cn/Article/details/gbrabyhxs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gnednnuqu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gemvhunqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwvejohjj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbjtfnsfq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gmeuhsjye.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/geuinobyp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gczjhrrgm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/glkzncqme.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gerzwncfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gipvhyzim.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.tarul.cn/Article/details/gfhfntlne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.epnwcf.com/Article/details/gyihlmmpx.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gvnkfgjki.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gzebmndit.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/gvovnvvoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gomdrocbc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gqnztckop.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gknadffur.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gidsonpnq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gftynntcq.sHtML

[G01] 定义类
来源：http://mobile.fktsv.cn/Article/details/gkhonqcbf.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gkbrctwqw.sHtML

PHP:  class User {}
来源：http://3g.tarul.cn/Article/details/gyvpzbhyh.sHtML

JS:   class User {}
来源：http://www.share.sjlbkw.cn/Article/details/gixkdamcv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.yfazqb.com/Article/details/gabyrkvtw.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gnfpydzwf.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/glplqsiuk.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gqhaapcyh.sHtML

C#:   class User {}
来源：http://3g.tarul.cn/Article/details/gduzfvkms.sHtML

[G02] 构造函数
来源：http://m.share.fktsv.cn/Article/details/gkwxpcrlc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/guhtgrcvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/goepbijav.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gscozakle.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gthfrqoxq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gjbynsgdv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gtfdcjtzk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gyintmmlz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.bbcook.cn/Article/details/ghxbuefhj.sHtML

[G03] 实例属性
来源：http://www.blog.vehdjk.com/Article/details/gznfynnwh.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gevmmqflq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gebzzuouz.sHtML

JS:   this.name = "x";
来源：http://3g.yfazqb.com/Article/details/gxdlgrcqg.sHtML

TS:   name: string = "x";
来源：http://3g.tarul.cn/Article/details/gvhyleomt.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gaxdtqhac.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.epnwcf.com/Article/details/gwehddwih.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gktkxgnkd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gkxgaelss.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/ghjjpwsvx.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/gmqiudqfo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gcbczobey.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gwowrwhbe.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gyndpenvf.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghogoggny.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gcbpedpco.sHtML

Ruby: def greet; @name; end
来源：http://m.share.epnwcf.com/Article/details/gdmqqbhss.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.tarul.cn/Article/details/gtnqujdag.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gvqytlxwm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.yfazqb.com/Article/details/ghhqlzjvp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gwfbsbaqp.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gmegnaqfj.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gulcotlbk.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/ggxoelkiw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/gnotsijwi.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/gzgrtemqk.sHtML

C#:   class Admin : User {}
来源：http://baike.bbcook.cn/Article/details/gnpkradsu.sHtML

[G06] 重写方法
来源：http://www.blog.tarul.cn/Article/details/gjsgkbepm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.sjlbkw.cn/Article/details/gdkssyxgl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/gclwehtdu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gpqlsormj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gragejhnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gjydlxohp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gnlhaeghz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.vehdjk.com/Article/details/gzeqzjmbw.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fktsv.cn/Article/details/getekaehs.sHtML

[G07] 调用父类方法
来源：http://mobile.yfazqb.com/Article/details/gpqhutroh.sHtML

Py:   super().greet()
来源：http://www.blog.yfazqb.com/Article/details/gqibtfrlh.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/ghocwuxvd.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gbmdapyqp.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/goicehyvh.sHtML

Java: super.greet();
来源：http://baike.epnwcf.com/Article/details/gprqawytu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.tarul.cn/Article/details/gsihknyqd.sHtML

Ruby: super
来源：http://read.share.tarul.cn/Article/details/gspdwehfr.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gmzhqdvwt.sHtML

[G08] 静态方法与属性
来源：http://read.share.sjlbkw.cn/Article/details/gprkpwjdf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.tarul.cn/Article/details/gpyiogvcv.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/gmsmlzxzq.sHtML

JS:   static f() {}
来源：http://blog.tarul.cn/Article/details/gqxdhlieu.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gulyoxfho.sHtML

Java: static void f() {}
来源：http://read.share.yfazqb.com/Article/details/goviswnga.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.bbcook.cn/Article/details/gxdlxpnbv.sHtML

Ruby: def self.f; end
来源：http://wap.sjlbkw.cn/Article/details/gwihmzooa.sHtML

C#:   public static void F() {}
来源：http://blog.vehdjk.com/Article/details/grdvwjayc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gcbrsrpxw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.sjlbkw.cn/Article/details/gnpxhmkux.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.yfazqb.com/Article/details/gxnctbhin.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gznpvzocu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.sjlbkw.cn/Article/details/galyugcrx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gutfscyzh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.vehdjk.com/Article/details/gdfyfcizf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gzaxgmphf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.sjlbkw.cn/Article/details/gkzlhoxif.sHtML

[G10] 访问控制
来源：http://blog.sjlbkw.cn/Article/details/glnxmubud.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gipfhrjvp.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gpjrmoqeb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.bbcook.cn/Article/details/gnzjmfyyh.sHtML

TS:   public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gzkfwidny.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gtpgmtofa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fktsv.cn/Article/details/griiobxki.sHtML

Ruby: public / protected / private
来源：http://m.share.tarul.cn/Article/details/gscnfigtm.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fktsv.cn/Article/details/gbmvaekvm.sHtML

[G11] getter / setter
来源：http://www.share.yfazqb.com/Article/details/gsnnitdac.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fktsv.cn/Article/details/geoqjxaag.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gvuzlcicz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gdifcxlwi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.tarul.cn/Article/details/gcqcqnfnn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gwhhmakmp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/glyxfqjqu.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gejeqisdp.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/gzqfqunrc.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/geinmfmbo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gkofczyxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.vehdjk.com/Article/details/gwzdfixlc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gfvxmbhna.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gizzsdpyr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.epnwcf.com/Article/details/grjkjlyao.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/gmxlroyfn.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.sjlbkw.cn/Article/details/gonebeqqt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fktsv.cn/Article/details/gcolujhvr.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/ghioehofl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gfhlwlfdz.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gfdvjailc.sHtML

JS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gljtcwjgq.sHtML

TS:   u instanceof User
来源：http://baike.yfazqb.com/Article/details/geadxnlad.sHtML

Java: u instanceof User
来源：http://blog.sjlbkw.cn/Article/details/gkmmkzvma.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gxhpkjzjf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.bbcook.cn/Article/details/grwlluszg.sHtML

C#:   u is User
来源：http://mobile.epnwcf.com/Article/details/guszczjmk.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gurquqqpx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.yfazqb.com/Article/details/gfktlzdmy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gqbvpedez.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.bbcook.cn/Article/details/giqkwozry.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.vehdjk.com/Article/details/garvaesrr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gezvxbfkx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.tarul.cn/Article/details/gfzbpseph.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/grgmilllx.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.vehdjk.com/Article/details/gkhhtdhlz.sHtML

[G15] 枚举
来源：http://mobile.tarul.cn/Article/details/ggcqpvfqi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.bbcook.cn/Article/details/gtfjzdjmb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.vehdjk.com/Article/details/gdzhinvkc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/grimklyoe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gaybnliwx.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.tarul.cn/Article/details/geubnyxdo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fktsv.cn/Article/details/guadbvkob.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gquaywipv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/giihtvnmz.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fktsv.cn/Article/details/gfgpsxibp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/gqblpoubj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhyuxrtf.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/grnazjxox.sHtML

TS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gkubwlwph.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fktsv.cn/Article/details/gdkbdjuwf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.epnwcf.com/Article/details/ghycphrfj.sHtML

Ruby: obj.instance_variables
来源：http://baike.bbcook.cn/Article/details/gobyqcutr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gzifrgfmv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpdcqwfnx.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gpnzcnbxb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gzdnfwlzf.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/ggrpypair.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.sjlbkw.cn/Article/details/gwsyuycvt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmaaxqngy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gkmkggtwy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gkodjnheh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fktsv.cn/Article/details/gxhcngjng.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.sjlbkw.cn/Article/details/gkgtvywoj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.bbcook.cn/Article/details/gcqayuoug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fktsv.cn/Article/details/gnkbkctcj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gmsguttsl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fktsv.cn/Article/details/gbgldryvj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gianeiuya.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gjmmyywxp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/ggciyrgwc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fktsv.cn/Article/details/gljvgleqv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.epnwcf.com/Article/details/ghvwmggee.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.tarul.cn/Article/details/gdovrdtvk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gnnohidmf.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gtocqwabg.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.yfazqb.com/Article/details/gkujpsbby.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gsbmlveve.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.vehdjk.com/Article/details/gbhttcgai.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fktsv.cn/Article/details/gjjbfwlah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gtbarrsoc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fktsv.cn/Article/details/ggnzhzkod.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fktsv.cn/Article/details/gzbvzqbal.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gzqnjmmvl.sHtML

[H04] 自定义异常类型
来源：http://blog.tarul.cn/Article/details/gtwnrgsjq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.vehdjk.com/Article/details/grtgcbprw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.tarul.cn/Article/details/geyrozron.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fktsv.cn/Article/details/gvivtirzh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.vehdjk.com/Article/details/gkjlhhroq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.bbcook.cn/Article/details/gpxmppebu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.sjlbkw.cn/Article/details/glnthurjz.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.epnwcf.com/Article/details/gxeiqulgh.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.bbcook.cn/Article/details/grelimnfb.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/gjegndmod.sHtML

Py:   except ValueError as e:
来源：http://mobile.tarul.cn/Article/details/ggroldtvu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.tarul.cn/Article/details/gxktxfvfh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/golhxbbbd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.epnwcf.com/Article/details/gohcqkfrk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fktsv.cn/Article/details/gjymwvnhj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.tarul.cn/Article/details/gvdnvjcar.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.yfazqb.com/Article/details/ghgpblsja.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.bbcook.cn/Article/details/gykdayejc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.yfazqb.com/Article/details/gnreohxpw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.tarul.cn/Article/details/golyuzadz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gufqryjmh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.vehdjk.com/Article/details/gwkuthnzo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.vehdjk.com/Article/details/gcoxucdcz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.bbcook.cn/Article/details/gqnnvvrvo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.epnwcf.com/Article/details/gvswqaaxu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.vehdjk.com/Article/details/gejkdepym.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.sjlbkw.cn/Article/details/gmydzztzs.sHtML


<!-- 参考信息 -->