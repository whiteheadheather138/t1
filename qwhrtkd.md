代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/glietqeyw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gheagbqze.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gwcjnapeg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gtjimvmfy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gvqvwyjbm.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gixnribbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gtskzvsny.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gjiblkmmy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/glrnclimu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gseimsilt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gpqnblckr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gpwqgkbdp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gzqpnkctw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gmvyvgibm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gskgfrzil.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/goigjosvz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gcewcvknd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gmhuyrdjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gitjlirjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.vehdjk.com/Article/details/grzdnbqva.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gyahgnzjv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gtvylylpo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gqueyamyp.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gwyucpjsu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gpldvyvgj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/ggctmbugk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gwunuyxne.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gpagellrm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gzvmeztcp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gkqsnoctr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/ghrghynjy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gmvegemlp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/gvpvuhhte.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.vehdjk.com/Article/details/gpirzwlww.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.epnwcf.com/Article/details/geibpjham.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gdljxwdkb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkctjratt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gkargpokn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fktsv.cn/Article/details/gfxuyzkcr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjaodshbb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/giqymmhfs.sHtML

[F06] 删除文件
来源：http://blog.epnwcf.com/Article/details/gfqnxebtw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdznldyrw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/ghcxymnll.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwezjyqeg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gjahrydgf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gvbewqigv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvbvqjnur.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gxgwewjmr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gpgybaanz.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.tarul.cn/Article/details/gwluvfgdn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gxiwuxjrh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/gktrdekej.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.vehdjk.com/Article/details/gljyphpeh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gfybuxivv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gozrlblls.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gdbmzxwhm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gideilznp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gyjnejcyo.sHtML

[F08] 遍历目录
来源：http://wap.vehdjk.com/Article/details/grquckmdu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/gkxdrvgfk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/geuhtyjnr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxgrwwqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gsekrtjdq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gdwcwlwqv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gdcrycdqg.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gnazyuxmp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gtajaqsri.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/grugxsvfk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdoikadxr.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gsqfmobny.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gtzjshycu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/gdpdoydlb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gwerejais.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gvrqhskdw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gycayvfku.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.yfazqb.com/Article/details/gtbiwnocx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.bbcook.cn/Article/details/glbzbpviq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/gghgvfney.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gtyxktoal.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gceicmryn.sHtML

TS:   path.extname("a.txt")
来源：http://baike.tarul.cn/Article/details/gfippxtsf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.epnwcf.com/Article/details/ggsypgdvq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gcujbulxk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/ghxigjutk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gduioegpq.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gcorjkmst.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gayttckgw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.yfazqb.com/Article/details/ggqzgrets.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/garnryode.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzaacwvia.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gryskdifi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gjidpscvw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gqbvjycxl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.tarul.cn/Article/details/ggrqxfnos.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gihgwunjk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gwparyiyn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gcoutiyzg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/gpbsoyncg.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/glyxykxmr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/gornpnrkz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.sjlbkw.cn/Article/details/gtibqtyup.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.tarul.cn/Article/details/gjgvanmfe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gzbxhgtcm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkbfwresx.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/ghpzqmkex.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gdcjwxkyt.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gvrurmexx.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gectveycj.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gzhkdnfid.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gysdpfwov.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.sjlbkw.cn/Article/details/gvrhkxhlu.sHtML

Java: class User {}
来源：http://read.share.vehdjk.com/Article/details/gpwnkpoft.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.tarul.cn/Article/details/gfgpgialn.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gwkbdxith.sHtML

C#:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/grhbrucam.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gcdwykxcf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gwnwcazrm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gqltpsopx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/ggdaiiktk.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.sjlbkw.cn/Article/details/gzpnnaati.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gfjaaudgt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gxfscocgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gmkywzkgo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gavnpbtfk.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gqncqabfz.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/goadfaane.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gkrjhxfhl.sHtML

JS:   this.name = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gflaglrgm.sHtML

TS:   name: string = "x";
来源：http://m.share.vehdjk.com/Article/details/gjusvprim.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gjazjqbsh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.epnwcf.com/Article/details/gnsbnqstf.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/gfrmgsmfl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.tarul.cn/Article/details/gjgwpzklm.sHtML

[G04] 定义方法
来源：http://www.blog.epnwcf.com/Article/details/glnzepdyl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/grbfbdcuk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gdafmygmm.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/grjeyzhqy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/ggjukaixv.sHtML

Java: String greet() { return name; }
来源：http://read.share.vehdjk.com/Article/details/gbvikwzie.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gilhzoerf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.yfazqb.com/Article/details/grmgxisgy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gvvwcxonk.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gazedgjxs.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gesjbdrxc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gmervhsht.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/ghxuhijoe.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gkibekljm.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gdmvdndhi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.sjlbkw.cn/Article/details/gyrdfkgmf.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gofbkwimc.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gzodnzomz.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gntwmwliv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/goiqfguly.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gudjiwpll.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gaibvkoeg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/glzviifvw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gtjadcouz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.vehdjk.com/Article/details/grluvdstp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.yfazqb.com/Article/details/gwadvvimv.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gpijoywrc.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/giifflkpu.sHtML

Py:   super().greet()
来源：http://baike.bbcook.cn/Article/details/givdlhmqx.sHtML

PHP:  parent::greet();
来源：http://baike.yfazqb.com/Article/details/gqvhuudag.sHtML

JS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/glsovhokk.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gdffdrdbd.sHtML

Java: super.greet();
来源：http://www.share.vehdjk.com/Article/details/ggisnrscl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fktsv.cn/Article/details/gyrtjytpu.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/ghcajrgkz.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gkmwskrcf.sHtML

[G08] 静态方法与属性
来源：http://blog.bbcook.cn/Article/details/gxmkmsemg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.tarul.cn/Article/details/gnoqdxyyx.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gsiiuwuby.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gahfrfclx.sHtML

TS:   static f(): void {}
来源：http://3g.vehdjk.com/Article/details/gddszbjdf.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/ggvfjziqk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.vehdjk.com/Article/details/gcschadcz.sHtML

Ruby: def self.f; end
来源：http://3g.bbcook.cn/Article/details/giwxjwqda.sHtML

C#:   public static void F() {}
来源：http://www.share.fktsv.cn/Article/details/guhlishxi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gsrkdscyk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.tarul.cn/Article/details/gmksczlbm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.vehdjk.com/Article/details/grtcrkryz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.tarul.cn/Article/details/ghvngipqo.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gqgbxjmms.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gyltpuskr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.tarul.cn/Article/details/gvuqdkhlh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/grvdcjxwh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/guroufyen.sHtML

[G10] 访问控制
来源：http://3g.yfazqb.com/Article/details/gugixpyqj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.vehdjk.com/Article/details/gaugcpeiv.sHtML

PHP:  public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gwkbgeusg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gaywmwqfd.sHtML

TS:   public / protected / private
来源：http://blog.yfazqb.com/Article/details/gswoxsydl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.sjlbkw.cn/Article/details/gxbvwaewa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.epnwcf.com/Article/details/gqjahkaxw.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gmvkbuzln.sHtML

C#:   public / protected / private / internal
来源：http://wap.tarul.cn/Article/details/ghpbhjeta.sHtML

[G11] getter / setter
来源：http://wap.fktsv.cn/Article/details/gweqvzelm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.sjlbkw.cn/Article/details/gwozckxff.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.vehdjk.com/Article/details/gvixlssee.sHtML

JS:   get name() { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gwpnypipm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.tarul.cn/Article/details/gftvobawd.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/gzvgjspbb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.bbcook.cn/Article/details/gkxnklcwt.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.vehdjk.com/Article/details/gbqhmqvjh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.bbcook.cn/Article/details/gtwuhxupc.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gwpddlidq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.tarul.cn/Article/details/gqylwnfdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.vehdjk.com/Article/details/gcpsjlojx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gsprcsasb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gbtxtyovx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/guaifidrd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gjdaslebl.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.vehdjk.com/Article/details/gthegwqxc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.vehdjk.com/Article/details/gdnrzgdyl.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gjkadrian.sHtML

Py:   isinstance(u, User)
来源：http://wap.vehdjk.com/Article/details/gelpxsbla.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gekksmall.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gojtnneef.sHtML

TS:   u instanceof User
来源：http://read.share.vehdjk.com/Article/details/ggiyuemjr.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gnqbzhrpy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.sjlbkw.cn/Article/details/gebtbzsax.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.yfazqb.com/Article/details/gjkwohfpp.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gbxlgpenp.sHtML

[G14] 数据类 / record
来源：http://wap.vehdjk.com/Article/details/gbtgkwjlp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gxjjxeuud.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gamdrigaw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.epnwcf.com/Article/details/gfakvawhu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gihjpngsi.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.vehdjk.com/Article/details/gwixujkqd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.yfazqb.com/Article/details/gqoutasde.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gefabbjut.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fktsv.cn/Article/details/gifnlnuhe.sHtML

[G15] 枚举
来源：http://blog.bbcook.cn/Article/details/gygzgbvte.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.tarul.cn/Article/details/gwsimeemv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.epnwcf.com/Article/details/gwfmikfgp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.yfazqb.com/Article/details/glvkboypg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.yfazqb.com/Article/details/gpeyvffcl.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gxwhqqyjf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.tarul.cn/Article/details/glqczolpn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fktsv.cn/Article/details/gddolppet.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/grqcowjjf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.tarul.cn/Article/details/gnnjktuxp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.tarul.cn/Article/details/gxrexpekl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gqjgimuto.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gdwiujxqs.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fktsv.cn/Article/details/guhjpksxv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.tarul.cn/Article/details/glmtmlsoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.bbcook.cn/Article/details/gopzewwyy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.epnwcf.com/Article/details/gcofbncaz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/glnotnhqo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gujrosqfi.sHtML

H. 异常与错误处理
来源：http://www.m.share.fktsv.cn/Article/details/gnwfmejnq.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gukkyumlk.sHtML

[H01] try / catch 基础
来源：http://baike.sjlbkw.cn/Article/details/gmzlnwwzu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fktsv.cn/Article/details/gbehthsiy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.bbcook.cn/Article/details/gypmthfnq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gikdweava.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.epnwcf.com/Article/details/gpyoxoxwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.bbcook.cn/Article/details/geqcjfawh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.vehdjk.com/Article/details/gsnfwfwgr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.vehdjk.com/Article/details/gwvqjinov.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.vehdjk.com/Article/details/gpnmbqsjx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.epnwcf.com/Article/details/gpcuokote.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gxoipnpkp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gphxrsmvy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.tarul.cn/Article/details/gtcmxgjjv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/glsigllkp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gnwyyetdk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gndxgmunt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.bbcook.cn/Article/details/gjhfcazlm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gordidcsc.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/grdzancst.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.tarul.cn/Article/details/gvwlzluvh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gbktbvinn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.sjlbkw.cn/Article/details/gefcdschl.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.tarul.cn/Article/details/gvxnynfqp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gzuzeskuz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.bbcook.cn/Article/details/gtqhzltfg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.sjlbkw.cn/Article/details/gaqrvwnmy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/goiufrgzb.sHtML

[H04] 自定义异常类型
来源：http://m.share.vehdjk.com/Article/details/gykoczvum.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fktsv.cn/Article/details/gvllrybah.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.epnwcf.com/Article/details/gyrhdlzip.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.bbcook.cn/Article/details/gyadcjayp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gtdqqzadj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gamxcwrrv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.vehdjk.com/Article/details/ggxnadfnh.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.bbcook.cn/Article/details/gflblwtce.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.bbcook.cn/Article/details/gtsnqvxkv.sHtML

[H05] 捕获特定类型
来源：http://read.share.vehdjk.com/Article/details/glubochft.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gcsovtdwt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.bbcook.cn/Article/details/gowqwshdc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.vehdjk.com/Article/details/gjssswbtz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.tarul.cn/Article/details/gtllzvsxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.sjlbkw.cn/Article/details/gxiqbiaix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.sjlbkw.cn/Article/details/gspgamubz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.yfazqb.com/Article/details/gkomrrjpf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.epnwcf.com/Article/details/gytsegiig.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fktsv.cn/Article/details/gihnaveoi.sHtML


<!-- 参考信息 -->