代发 wailian999

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gvqpyqrzu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzcggywl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gnsizusso.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gjkfmmmhz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gvtowtpgn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gkwgedkhp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/ghcanhept.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpggpdqgu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gsefarjdh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gnlxiiqev.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/ghbmuxugq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gaqnoyxwb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gawxddrto.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoukigrw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gimsrszhk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gzxkurgtb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.sjlbkw.cn/Article/details/gjmqqqdiq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/gbsctsshf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/ggyjjclpu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gfncrychz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gkgurbfrh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gdnwvbbio.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gxueaimqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/galzcrtcv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gldfedlsm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gqrrfaaog.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/giacayeao.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gajovilcn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/ghbosfcez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gbvteyacq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/grqazxtni.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gsvtrvsgm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/gajwcwvxl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/guaqojnye.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gfjyhecrr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gbvakvtes.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gfefaumrz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/guxzriwbs.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gwvygeivm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbxpgmswm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gfsqunsfv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/grbpuawty.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/gujophmfc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gllcbktrd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.bbcook.cn/Article/details/goiqqmiez.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gycefxjrs.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gizlniozw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/ghmfxugzh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzbpuxlro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gumenkasa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbrrhtsrs.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gjkxscnzv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gaptoppgq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtzfvjdfo.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/gqggargnq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.sjlbkw.cn/Article/details/gbxhxyarf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gzgnziost.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gsrlppdqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/gnywuudfo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.tarul.cn/Article/details/gqvnhkuug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/grylnbtmm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gqticqgxo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/ggmnsqnhb.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gcrspjwqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gwbloednm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.tarul.cn/Article/details/ggbdnmitz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gwcnzkctk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gzrtbuziu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gztnqogns.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gjjvypyrv.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/gmklgcxhi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/girqbfmfi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gigwipwja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.vehdjk.com/Article/details/grkheqbfk.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/gtxwyidlr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gnclftpid.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gxzcepeho.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/ggwgqetrq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.epnwcf.com/Article/details/gasbcrhoe.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gudnoxsgb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gcpokqidq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gmzrxqcva.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxgcnipcq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gdqlqioeh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtcaorwkl.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/gpnndfksi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/gwwhrktat.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gqwldzsag.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gfsvdgiti.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtcvdbxnk.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gwuuiyplu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gsyaapzgb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gakukjvkn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcegddqgs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gkwyxiuzi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gfoedzvkc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.tarul.cn/Article/details/gtwxasncm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gcrhccryf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gqaeouyim.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/gwcjwvgoh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gcfzbxyan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gbfumdkef.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/guchmddjz.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gkdzxbjcd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gjlwjpglc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gjsnczcsl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gkvsxqepv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.bbcook.cn/Article/details/glpfiaclb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gklzttczd.sHtML

G. 面向对象
来源：http://wap.fktsv.cn/Article/details/ghferbbhm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gesndqcmu.sHtML

[G01] 定义类
来源：http://www.m.share.epnwcf.com/Article/details/gkxaywkmw.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/ghfplnwlo.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gatbrmsaf.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gzmcodnem.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gfpjgfluv.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gzzssarbv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/giymgftxm.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gxrcvdlps.sHtML

C#:   class User {}
来源：http://wap.epnwcf.com/Article/details/gjliuqgoj.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gbmcufwsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/ggwsjzase.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.yfazqb.com/Article/details/gqwevluhq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gjtvabnsu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghkkhehzx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gftmdprav.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.epnwcf.com/Article/details/gmuuuqidy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.vehdjk.com/Article/details/gedlsjmph.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gqyifrzva.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/gjwdworkd.sHtML

Py:   self.name = "x"
来源：http://baike.tarul.cn/Article/details/gttzjktwo.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gfjdoqrve.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gnremksyz.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gwgcikefc.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/gvvjiulho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gmbpnelyg.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gawwfxlzv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gkpdhdfhf.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/goryljeib.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/ghtypbgsa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/ggmuyvviq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gddovlisg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gmqxucteu.sHtML

Java: String greet() { return name; }
来源：http://mobile.yfazqb.com/Article/details/gpprlsaqu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gybppznzd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.epnwcf.com/Article/details/gwuuoczox.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/gzfykzxtt.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/geqzkmcix.sHtML

Py:   class Admin(User): pass
来源：http://read.share.bbcook.cn/Article/details/gbdmlzcfa.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gazxgkgak.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gufeohbvj.sHtML

TS:   class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gduvlalad.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gkzfpzlpy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gcxntnvvh.sHtML

Ruby: class Admin < User; end
来源：http://3g.tarul.cn/Article/details/ggbbriohc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gjfmntduk.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/gsrfiqacy.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/glrfmglsj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.tarul.cn/Article/details/gbvejdwho.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gasqqncma.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/gczexatzz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/goyalnrsy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fktsv.cn/Article/details/gtvaqpiwi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/gfxzagskj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fktsv.cn/Article/details/gareehlxd.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gdlnkgsys.sHtML

Py:   super().greet()
来源：http://www.share.vehdjk.com/Article/details/gzlsdghsw.sHtML

PHP:  parent::greet();
来源：http://baike.epnwcf.com/Article/details/gprwatsnl.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gxlliwyyb.sHtML

TS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gcrqstvim.sHtML

Java: super.greet();
来源：http://3g.epnwcf.com/Article/details/gmbbjefle.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.epnwcf.com/Article/details/gspzwdiaq.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gsvyqhbtb.sHtML

C#:   base.Greet();
来源：http://m.share.tarul.cn/Article/details/gdfszgqne.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gmnxljzor.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/ggspcilma.sHtML

PHP:  public static function f() {}
来源：http://3g.vehdjk.com/Article/details/gaaqyukgb.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gsmbznjdn.sHtML

TS:   static f(): void {}
来源：http://3g.fktsv.cn/Article/details/gcniigxtc.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gipfdaluu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/gxnissdav.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gpilzsvmn.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gexxzcjng.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fktsv.cn/Article/details/girzgdzrp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.yfazqb.com/Article/details/gtyfomnpz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fktsv.cn/Article/details/gpwsyufue.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.bbcook.cn/Article/details/ghhpcnonh.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.vehdjk.com/Article/details/goxwdldid.sHtML

Java: interface Shape { double area(); }
来源：http://3g.tarul.cn/Article/details/gncpcaszd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gtwuoisin.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gpkwydqwh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.tarul.cn/Article/details/gpgipuadk.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gqtoyzirp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gdidmmlbm.sHtML

PHP:  public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gdwkoszge.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.tarul.cn/Article/details/gabzwuuqv.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gyluyycpm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fktsv.cn/Article/details/gavgujeme.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gqvgcmgho.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gxgxdkcev.sHtML

C#:   public / protected / private / internal
来源：http://mobile.yfazqb.com/Article/details/giyvklmvs.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gfxczfbct.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fktsv.cn/Article/details/gtnrcyram.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/grnetoukn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.bbcook.cn/Article/details/gkdnoynih.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gvuxxzblz.sHtML

Java: public String getName() { return name; }
来源：http://baike.tarul.cn/Article/details/gvzmhzikm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gyborcfgx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.sjlbkw.cn/Article/details/gzyaopens.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gryacfvll.sHtML

[G12] 对象转字符串
来源：http://read.share.vehdjk.com/Article/details/glfpzexpy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gsabhoiuy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gifkvdond.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gnsysdroh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.yfazqb.com/Article/details/gkmnwhkia.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbxfvwzps.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gbybvfzon.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/ggdhkxzsk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gjeusddov.sHtML

[G13] 判断对象类型
来源：http://www.blog.sjlbkw.cn/Article/details/gxqoxlron.sHtML

Py:   isinstance(u, User)
来源：http://baike.fktsv.cn/Article/details/gvkudgctm.sHtML

PHP:  $u instanceof User
来源：http://blog.fktsv.cn/Article/details/gruuwywro.sHtML

JS:   u instanceof User
来源：http://blog.bbcook.cn/Article/details/gmhqxbvma.sHtML

TS:   u instanceof User
来源：http://baike.fktsv.cn/Article/details/gyylvafgl.sHtML

Java: u instanceof User
来源：http://blog.vehdjk.com/Article/details/gzcolzjiq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.vehdjk.com/Article/details/gukabswvo.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.vehdjk.com/Article/details/gncvixphr.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/gopnuelvt.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/giyhgbdzr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.tarul.cn/Article/details/gntkiejhi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.tarul.cn/Article/details/gwgcgyewc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gnynbaplm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.epnwcf.com/Article/details/gtxrhaljx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.vehdjk.com/Article/details/gnddpvguy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/gwxdlqnje.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.sjlbkw.cn/Article/details/gheexkfdb.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.yfazqb.com/Article/details/gsfpgocyv.sHtML

[G15] 枚举
来源：http://www.share.epnwcf.com/Article/details/gpbkranld.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gzlcfpmvt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gwipvdufp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.epnwcf.com/Article/details/glumylrzx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gvsvvmtvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.bbcook.cn/Article/details/gdmhqbcuz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuytqwcp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.epnwcf.com/Article/details/gzkfcnxty.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gczhagixv.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.epnwcf.com/Article/details/gsbanucos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/gchgqlotg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.tarul.cn/Article/details/gglaaxqjs.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gfvxbffxx.sHtML

TS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gfevidhlo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/gdhaanaqn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.epnwcf.com/Article/details/gopckzynw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.tarul.cn/Article/details/gcwkcvvxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gcxwauqiw.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwbidarwn.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gnthgezdv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/giomvjoyq.sHtML

[H01] try / catch 基础
来源：http://www.share.bbcook.cn/Article/details/gijkayewq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.sjlbkw.cn/Article/details/gktfggnls.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fktsv.cn/Article/details/gtulqqtij.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.tarul.cn/Article/details/ggpgtrqos.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/gpjsxwckh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.bbcook.cn/Article/details/gcwdswhmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.bbcook.cn/Article/details/gbwixgtrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gftwnoyxg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.tarul.cn/Article/details/ghvbevlco.sHtML

[H02] finally / ensure 收尾
来源：http://blog.epnwcf.com/Article/details/gkrmpmtkd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.epnwcf.com/Article/details/gjfhudzqi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gbwcopdld.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gdyecvxhh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwuwelmxe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/ggjmtmtui.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.yfazqb.com/Article/details/ghdxvwcmo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.vehdjk.com/Article/details/gwpqqrror.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gtbkonxwo.sHtML

[H03] 主动抛出异常
来源：http://m.share.epnwcf.com/Article/details/gblgwgyfy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.sjlbkw.cn/Article/details/gkvbanctj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.tarul.cn/Article/details/gtoqaywvm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gdorldkpg.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gbtgojkwr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.vehdjk.com/Article/details/grjlwjulh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.bbcook.cn/Article/details/gumadqegj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.vehdjk.com/Article/details/godervnmt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gpzfwmadx.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gfcxuimof.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.vehdjk.com/Article/details/gxhjviiyf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.vehdjk.com/Article/details/ggekcekgo.sHtML

JS:   class MyError extends Error {}
来源：http://blog.yfazqb.com/Article/details/gvxtzwshy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.yfazqb.com/Article/details/gcgfelwef.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.bbcook.cn/Article/details/gaekteupf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fktsv.cn/Article/details/gjmxbtesg.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.epnwcf.com/Article/details/gklklrfqt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.bbcook.cn/Article/details/gsbwqthwz.sHtML

[H05] 捕获特定类型
来源：http://baike.vehdjk.com/Article/details/gnroltagd.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.vehdjk.com/Article/details/gcjlfphqa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.sjlbkw.cn/Article/details/gruioxvgq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.bbcook.cn/Article/details/gzwxaotxq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gearxgjhe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.yfazqb.com/Article/details/gfeqgrirv.sHtML


<!-- 参考信息 -->