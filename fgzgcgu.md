代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gspiuzkon.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gyzmixidz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.epnwcf.com/Article/details/gpukqxovh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.tarul.cn/Article/details/gdnycexyc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gsudppwbz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gftzvbdcw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gxvzrhxfd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gbmujzmct.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gholxszui.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/grnfwiipl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gvfufcmou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/glovrpclm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/guszerjvf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gbunhzpdz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gwlltkitw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gdmpaxdjo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gqcdgyukz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gqmgamdfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gthtadpys.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.bbcook.cn/Article/details/gtdzlshgj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gyiapjehb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gnlbcgoho.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/ggabjksid.sHtML

[F04] 追加写入文件
来源：http://www.blog.bbcook.cn/Article/details/gsdjspjzu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/glnehktjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gjzvtkjzq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gdedisxiq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gpfmecwjb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gnertavon.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gxrdpczuo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/glpjgedio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.epnwcf.com/Article/details/ggzoqgqwe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fktsv.cn/Article/details/gahljxrfj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gjusoqatp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/giisxcmat.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gzjhxmglg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gpsbukxoo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnurwyfit.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gnovtmzfk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gpysbtfpg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnjenymkh.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gajsvpzng.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gujecrmxz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/grpomezag.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gwynaqlwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gypijtsbx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gtgbnafpf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjrklbpce.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gguzukjbc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gjqyzimcy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/ghbakssfd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gztavwhdr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gpldjaonz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gretjtlgu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gerftmrqz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gsttsgnul.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gveycddia.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gscievtug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/gbrlgrmui.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gfsushekt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gazpyjuyi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gtcmvllym.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gnyjjjwzp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gcchbuxyv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gmlntbaxj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.sjlbkw.cn/Article/details/glehnaibv.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gstnbgtjw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.yfazqb.com/Article/details/gzbuhosht.sHtML

[F09] 获取文件大小
来源：http://mobile.fktsv.cn/Article/details/gdhziznuu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/goklzskfe.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gyqhbbeov.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gukmyrwps.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gmowdmlve.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gggriaibh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.sjlbkw.cn/Article/details/gdvewxgyz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjfrtguib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.bbcook.cn/Article/details/gwjdylpqg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.bbcook.cn/Article/details/gutjaoujg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gpwmohrtl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/galdxlnib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gaezqehlk.sHtML

TS:   path.extname("a.txt")
来源：http://baike.epnwcf.com/Article/details/gascruasi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.sjlbkw.cn/Article/details/gxlfxuvri.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gldmbuxaz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gxubfpnqj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/giyqcakms.sHtML

[F11] 复制与移动文件
来源：http://3g.vehdjk.com/Article/details/gvhgvanqz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/ghpuazgzd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.epnwcf.com/Article/details/gyhvjnbnf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gyehpxrqa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gnieymkcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gcspogkpr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gzqjpkfss.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gukgqaxgu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gdmovzqmn.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gozlcqljn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.epnwcf.com/Article/details/gagqpoxex.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/ggxmqyvdx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gcxfoinph.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/gzdcmezwl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.sjlbkw.cn/Article/details/gkjzvdajh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/giufhwcue.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gvzxwyzzr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.yfazqb.com/Article/details/gsnsqsbdb.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmwxnjsud.sHtML

G. 面向对象
来源：http://mobile.bbcook.cn/Article/details/gsgooclom.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaizpuazn.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gosidzdlz.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gbmajovne.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gihmqodhm.sHtML

JS:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gfkhzfzcq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fktsv.cn/Article/details/gcrjkcutb.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/ghmvfngxo.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gswlxfiul.sHtML

Ruby: class User; end
来源：http://read.share.yfazqb.com/Article/details/gzintgfsy.sHtML

C#:   class User {}
来源：http://baike.epnwcf.com/Article/details/gkgkoyied.sHtML

[G02] 构造函数
来源：http://mobile.bbcook.cn/Article/details/grvoeftfz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.tarul.cn/Article/details/gdaskfltr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.vehdjk.com/Article/details/gzxvtvvgu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gmzuxydjp.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/geelcksaf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gbewvydkm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.bbcook.cn/Article/details/gmdaubous.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/ghiovomym.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gzwclcuym.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/gzfaeolzx.sHtML

Py:   self.name = "x"
来源：http://read.share.epnwcf.com/Article/details/gvdxlfwqs.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gvxxsvakg.sHtML

JS:   this.name = "x";
来源：http://mobile.bbcook.cn/Article/details/gkmosdjwb.sHtML

TS:   name: string = "x";
来源：http://blog.tarul.cn/Article/details/gwpadcipw.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/gghpuxiev.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.sjlbkw.cn/Article/details/guhoelveq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrwmvcoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.yfazqb.com/Article/details/gjgmplrjs.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gmtrzrmmu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/ghrknpmex.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grsajuwtw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gbenzvjsj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/giisbcbjw.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gyaebhwmu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/gdwlxoimo.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gqbvaxetn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gnvguhcux.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/ghxghebga.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gvulokjdv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gtjfqhpet.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gfzmyjxra.sHtML

TS:   class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/gwqjoierh.sHtML

Java: class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gdhkixjmf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.tarul.cn/Article/details/gjydaspcx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gikjksahl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcqfmmhex.sHtML

[G06] 重写方法
来源：http://baike.tarul.cn/Article/details/givyfjqfo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.yfazqb.com/Article/details/gjwwtjyzj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gknaooyaw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gufzgazoi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gzxziqirr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gggqihzlf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.bbcook.cn/Article/details/gplfvfzlc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gzdnbwilc.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gnbrhyvmc.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gabrsuurz.sHtML

Py:   super().greet()
来源：http://www.m.share.epnwcf.com/Article/details/gobqjnntu.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gccbyaows.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gainyjiii.sHtML

TS:   super.greet();
来源：http://mobile.bbcook.cn/Article/details/gpjtdsmym.sHtML

Java: super.greet();
来源：http://baike.tarul.cn/Article/details/gjoxyqalx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.epnwcf.com/Article/details/gxhedmimr.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gsslepmka.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/govitpgfd.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.yfazqb.com/Article/details/gokdwtrae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/giuzmxiae.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gpsuxpbrv.sHtML

JS:   static f() {}
来源：http://blog.fktsv.cn/Article/details/glpnpuuie.sHtML

TS:   static f(): void {}
来源：http://www.blog.bbcook.cn/Article/details/gxksfyqik.sHtML

Java: static void f() {}
来源：http://www.share.epnwcf.com/Article/details/ghigxbwhs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gdvwfbxfr.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gegcpuqmy.sHtML

C#:   public static void F() {}
来源：http://wap.fktsv.cn/Article/details/gmrzbdpoy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gstffgrub.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fktsv.cn/Article/details/gtathzwih.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.bbcook.cn/Article/details/gzgqyivrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.tarul.cn/Article/details/gmiunpojl.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.yfazqb.com/Article/details/gqrahdoxg.sHtML

Java: interface Shape { double area(); }
来源：http://baike.epnwcf.com/Article/details/gxqtypfcb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/gwkewoiht.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.epnwcf.com/Article/details/gasirnpuu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.tarul.cn/Article/details/gwyxnyopp.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gqhnfqxxf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fktsv.cn/Article/details/gqqezvijz.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gxeaptzer.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gmsdcjidj.sHtML

TS:   public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gkgpoxbss.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.sjlbkw.cn/Article/details/gnfnznmte.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.tarul.cn/Article/details/gnftbszdf.sHtML

Ruby: public / protected / private
来源：http://baike.yfazqb.com/Article/details/gdsycqklm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gljkvoesq.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gzvlgsugo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.tarul.cn/Article/details/garyllvig.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gdtnakpcp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gupukpdqx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fktsv.cn/Article/details/gngrvdyfo.sHtML

Java: public String getName() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gvkywliuu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gzwtnjhue.sHtML

Ruby: attr_accessor :name
来源：http://blog.vehdjk.com/Article/details/gktodlnov.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.epnwcf.com/Article/details/gfoykltig.sHtML

[G12] 对象转字符串
来源：http://www.share.vehdjk.com/Article/details/gswjjphhq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/glucpzfsi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/glkczhpwr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gqrtbwktr.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/ggmqcbhau.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghulfbtnw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpqcpcid.sHtML

Ruby: def to_s; @name; end
来源：http://blog.vehdjk.com/Article/details/glaynnjts.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gekghyyxu.sHtML

[G13] 判断对象类型
来源：http://www.share.bbcook.cn/Article/details/gkokfypbj.sHtML

Py:   isinstance(u, User)
来源：http://www.share.vehdjk.com/Article/details/guziavrfu.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/ggmnbvsak.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gpryilylm.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/getamkvqy.sHtML

Java: u instanceof User
来源：http://blog.bbcook.cn/Article/details/gurttlolc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fktsv.cn/Article/details/gqbdbhjcf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gfzdidmqf.sHtML

C#:   u is User
来源：http://3g.fktsv.cn/Article/details/gganmhlwa.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gxzcnhrku.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.yfazqb.com/Article/details/guojzfjoz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/grcdwyzpo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gsvqvxnbk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/gyyesupnh.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gvxetjfzl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gmvnkqadh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.yfazqb.com/Article/details/gyrxohuoi.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.tarul.cn/Article/details/gecmxuahw.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gffmlargk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gaanvizzs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.tarul.cn/Article/details/gqqzzwahu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.tarul.cn/Article/details/gfxvvfyvr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gpsoqfxlb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.vehdjk.com/Article/details/gkzrmtcyd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/ghhyytrqs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.sjlbkw.cn/Article/details/guwckxzpd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gqesuxurk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gozibijgv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.vehdjk.com/Article/details/guynciemu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fktsv.cn/Article/details/guowmeqde.sHtML

JS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gvwllwusb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.yfazqb.com/Article/details/gjwyfnmsv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gynugynzo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fktsv.cn/Article/details/gxtwdqgrv.sHtML

Ruby: obj.instance_variables
来源：http://m.share.bbcook.cn/Article/details/gfbcodira.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/gudiowegg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzbtbuovd.sHtML

H. 异常与错误处理
来源：http://mobile.yfazqb.com/Article/details/gexdzvgld.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyqlexsqi.sHtML

[H01] try / catch 基础
来源：http://mobile.tarul.cn/Article/details/gutdknurj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/ghmtrtmbp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.vehdjk.com/Article/details/giqcswxjq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gqtlfoiar.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gyitjtdoi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.sjlbkw.cn/Article/details/gqmhxpvdb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.sjlbkw.cn/Article/details/grvjgpylo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.epnwcf.com/Article/details/gcgkvixya.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.yfazqb.com/Article/details/gxjzzuxit.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.tarul.cn/Article/details/gyrfylwsk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fktsv.cn/Article/details/gypssksae.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.bbcook.cn/Article/details/gtnngqpyg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gqkljitla.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gdioruvti.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/gqljcgfth.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeysecxx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fktsv.cn/Article/details/gxzahyszb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gymkwgotm.sHtML

[H03] 主动抛出异常
来源：http://blog.bbcook.cn/Article/details/gnohyekod.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fktsv.cn/Article/details/gurvetmqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.epnwcf.com/Article/details/gkpubsvlp.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.vehdjk.com/Article/details/ggjpzhdlr.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fktsv.cn/Article/details/gbmvnhmai.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fktsv.cn/Article/details/gqerwisnm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.epnwcf.com/Article/details/gsbuuyfip.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.vehdjk.com/Article/details/gfoeuvhvx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.vehdjk.com/Article/details/gskenjlen.sHtML

[H04] 自定义异常类型
来源：http://www.blog.bbcook.cn/Article/details/gwdggaqbb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gzbufjqqt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.bbcook.cn/Article/details/gmhjktgdc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.yfazqb.com/Article/details/gwcgtvbey.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbfjrcml.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fktsv.cn/Article/details/gfmidpjbf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.bbcook.cn/Article/details/gnlszdnar.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.sjlbkw.cn/Article/details/grhnulxaa.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fktsv.cn/Article/details/ggppqdpqt.sHtML

[H05] 捕获特定类型
来源：http://wap.epnwcf.com/Article/details/gpudbkolk.sHtML

Py:   except ValueError as e:
来源：http://wap.sjlbkw.cn/Article/details/gbufxixld.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.tarul.cn/Article/details/gxbagqlzf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.tarul.cn/Article/details/gznzhtqve.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.epnwcf.com/Article/details/gyzsollbc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.sjlbkw.cn/Article/details/glcxwmzrm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fktsv.cn/Article/details/gioggxnkp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fktsv.cn/Article/details/gavrippbl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/glniatcda.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.epnwcf.com/Article/details/gmnkindwq.sHtML


<!-- 参考信息 -->