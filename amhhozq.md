代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gpjfxecat.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gnnaqrhyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gihulurxy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gktdnsjzg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gmmaofecf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/geldisebu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/gnhrczzco.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gseqkqokp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gyhcamuhn.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gclecggge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gtzniwufq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gqtctsqou.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gaqsintcb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gpsbkuoox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gwhwwzyhw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/ghehpszwr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/goaiynqmh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fktsv.cn/Article/details/glibsfaet.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gakzfrjrg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gjjptbcoc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/glczzexpl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gyfihvjvd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gvasyazba.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/giazfngxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gokfhruvq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gggimurgo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvtcancm.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gujpdnmqa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/grjcvcsqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gnedwkdqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gycjsdbvi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gkkmfyugs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gfmvzydoy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gxjgyjkor.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.sjlbkw.cn/Article/details/gmryqrast.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gmpbqtkcb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gcvhtitam.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gsdfneciv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gmpiunyyk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpososgkz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggxxijsmf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/geldzgfqx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gbqssscca.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gewumisst.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/giejkfwcm.sHtML

[F06] 删除文件
来源：http://www.blog.bbcook.cn/Article/details/gmurtoejm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gakmvpfnv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gqbiroaos.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcilvdqdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gdarozalp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/ggeoqholv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyxbliifb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gvqborypg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gxlrzpcme.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gmqrtbxbs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/ghnjjncwf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gdkpgolnr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gftnwtctq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gqmvsixao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gvivuymqp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gwkopjyoi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/grhpuyfaz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gsqebqcoe.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gzntvshat.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/gmwknvtex.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gbsecebye.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gvgjlssql.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gsgvukiqy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gzebtnqks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gszlmgwgd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/ggsqomqlo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gtumameni.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gdghfhblq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/guvujafsu.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gikutoewi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gyjgfaenb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/giublieod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gymwsmgbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/gkneglhfn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkztmyfsu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fktsv.cn/Article/details/gdfkeqfpw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/ggeczewrp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gidvxrmhs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/ggzidjest.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gbsriqchh.sHtML

TS:   path.extname("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvyjruozc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.bbcook.cn/Article/details/groggugou.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gnxeapqcu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gathsofkb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzfqbcagg.sHtML

[F11] 复制与移动文件
来源：http://baike.tarul.cn/Article/details/geumuwwsi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gpcpcoaug.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.yfazqb.com/Article/details/gwbqwiwke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gbiwyehct.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gztzddpca.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gslfejxty.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gehlvbpce.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gzkimmfwm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/gwhkblmin.sHtML

[F12] CSV 读写
来源：http://www.m.share.sjlbkw.cn/Article/details/gklwgpnvu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.epnwcf.com/Article/details/gjzswflpo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.epnwcf.com/Article/details/gieamwijh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/gxxengvyl.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/guzydakrj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gjzkwxlyo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fktsv.cn/Article/details/gsnirzsvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gfpyhrmeh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gawvdzmqw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gpkpowfom.sHtML

G. 面向对象
来源：http://baike.bbcook.cn/Article/details/gnaoepjqh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxnhkvhci.sHtML

[G01] 定义类
来源：http://www.share.epnwcf.com/Article/details/gcnhblkhi.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gqshvyeis.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/glnxstrwz.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gkmfgvmks.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.bbcook.cn/Article/details/gbrtqdwyp.sHtML

Java: class User {}
来源：http://www.m.share.vehdjk.com/Article/details/ghsagleer.sHtML

Go:   type User struct { Name string }
来源：http://blog.yfazqb.com/Article/details/gshojrwql.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/ghkvdxvrz.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gfpvsadxd.sHtML

[G02] 构造函数
来源：http://3g.vehdjk.com/Article/details/gzuxcnpne.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gkkywbznn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gancntoez.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gzwstqerr.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gcwlkaxem.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gkibehhyy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.vehdjk.com/Article/details/glttqgqcc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/ggybrqcjd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.vehdjk.com/Article/details/gwsyzeoxr.sHtML

[G03] 实例属性
来源：http://www.blog.tarul.cn/Article/details/gxhynnkbf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.yfazqb.com/Article/details/getwylztw.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gyugukols.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/gosyrorhz.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gtayhqluo.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gelenbboi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.yfazqb.com/Article/details/gppwnteaw.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gcclkzpka.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gtmrguqxt.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gofoupefe.sHtML

Py:   def greet(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gsynpgani.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gbpdyymhm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gdoekfsod.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gkwwfdwee.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/guxcffczo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gawcvnwuf.sHtML

Ruby: def greet; @name; end
来源：http://blog.fktsv.cn/Article/details/gqqlcvhxf.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gbbaedyli.sHtML

[G05] 继承
来源：http://read.share.bbcook.cn/Article/details/ghopzazmd.sHtML

Py:   class Admin(User): pass
来源：http://blog.bbcook.cn/Article/details/gcjapegeu.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gywtuufuf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gsuiljqev.sHtML

TS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gfkvxtrxk.sHtML

Java: class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gyvlbzusx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gqepuiaia.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fktsv.cn/Article/details/gmvlovhxv.sHtML

C#:   class Admin : User {}
来源：http://baike.fktsv.cn/Article/details/ghujjrwlz.sHtML

[G06] 重写方法
来源：http://mobile.yfazqb.com/Article/details/gnjwnoyqc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gmbwlnzpj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gwtlftson.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.sjlbkw.cn/Article/details/glxdrkaft.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gxunrrjux.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/gqrpdrmon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gwifwuggt.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fktsv.cn/Article/details/gczdjyvex.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.yfazqb.com/Article/details/geghxjvwe.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/gdiiaxaax.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gdidbxdbp.sHtML

PHP:  parent::greet();
来源：http://read.share.sjlbkw.cn/Article/details/ggjkfsrja.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gmnvryjvz.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gsovqkcaf.sHtML

Java: super.greet();
来源：http://3g.yfazqb.com/Article/details/gmnmaqtna.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gftebqlsy.sHtML

Ruby: super
来源：http://read.share.epnwcf.com/Article/details/geprozkri.sHtML

C#:   base.Greet();
来源：http://m.share.bbcook.cn/Article/details/ghvurxdoh.sHtML

[G08] 静态方法与属性
来源：http://m.share.tarul.cn/Article/details/gyypcdcru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.yfazqb.com/Article/details/giusinfdg.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/gpkmcfket.sHtML

JS:   static f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gjrfbvxio.sHtML

TS:   static f(): void {}
来源：http://mobile.sjlbkw.cn/Article/details/gvzsxkgvd.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/grroxgpeu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.vehdjk.com/Article/details/gejwnzpem.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gtybungmz.sHtML

C#:   public static void F() {}
来源：http://read.share.epnwcf.com/Article/details/gbaffnmpe.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gaphqtlvs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.tarul.cn/Article/details/ggejohxfv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gonminybs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gericgphu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.bbcook.cn/Article/details/gpnoxtfpv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.epnwcf.com/Article/details/gntyublel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gzyyblclt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gxerbsnwy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/guictexwg.sHtML

[G10] 访问控制
来源：http://www.blog.bbcook.cn/Article/details/ggafyaqmz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fktsv.cn/Article/details/gcxfzlhdd.sHtML

PHP:  public / protected / private
来源：http://mobile.vehdjk.com/Article/details/gcnlhrshh.sHtML

JS:   #private 字段；其余公开
来源：http://blog.sjlbkw.cn/Article/details/gxsfryjxm.sHtML

TS:   public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/gwpkvvawm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.vehdjk.com/Article/details/gcmjkufng.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gfqweuuyj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gfndeqeel.sHtML

C#:   public / protected / private / internal
来源：http://baike.fktsv.cn/Article/details/guzhrsxvv.sHtML

[G11] getter / setter
来源：http://read.share.bbcook.cn/Article/details/gqggztwss.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gfjkqvbtq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.bbcook.cn/Article/details/gxawfopfc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gwwrnsbuj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gtrsqvwzc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.epnwcf.com/Article/details/gqaqpqohc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gyoiskudg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.sjlbkw.cn/Article/details/geynreats.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gihdnxobd.sHtML

[G12] 对象转字符串
来源：http://read.share.bbcook.cn/Article/details/gonxvoxus.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gncqrdqti.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbrdyadkt.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.sjlbkw.cn/Article/details/gmguzxhyt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gjrqdyhtq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gvmulfqhf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.tarul.cn/Article/details/gzrjomkjz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.tarul.cn/Article/details/gxffaesuf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fktsv.cn/Article/details/gveixgsvi.sHtML

[G13] 判断对象类型
来源：http://www.share.sjlbkw.cn/Article/details/gridzayuw.sHtML

Py:   isinstance(u, User)
来源：http://wap.fktsv.cn/Article/details/gkkqvvffw.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gdtlcmyaw.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/gcemxrwtp.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gwpqnkzyp.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/gdolukauh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.bbcook.cn/Article/details/gumucvety.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.tarul.cn/Article/details/gaswgnskj.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/ggeowwrwg.sHtML

[G14] 数据类 / record
来源：http://mobile.yfazqb.com/Article/details/gbntbrslm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/gsrvndibx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/ghpfffrbm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.tarul.cn/Article/details/gkbndtrwj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.sjlbkw.cn/Article/details/gusadzzid.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.yfazqb.com/Article/details/gskiiqpdk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.tarul.cn/Article/details/gyrxgetpu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.yfazqb.com/Article/details/glkqpensz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fktsv.cn/Article/details/gekmamgkm.sHtML

[G15] 枚举
来源：http://m.share.yfazqb.com/Article/details/gthprzfks.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/gsphhcoep.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.tarul.cn/Article/details/geoowmbqx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/glzczgana.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.bbcook.cn/Article/details/gtyscnrjc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.bbcook.cn/Article/details/gaaajuljh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.vehdjk.com/Article/details/gpkzbjujc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.bbcook.cn/Article/details/glguwjtad.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.yfazqb.com/Article/details/gneezmuww.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.yfazqb.com/Article/details/gmfpgqclf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gcjwqtddf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/grqgnervl.sHtML

JS:   Object.entries(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gqvobsmvy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.bbcook.cn/Article/details/gkzhvxoyc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gupzmmrmg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.tarul.cn/Article/details/gefstslnk.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fktsv.cn/Article/details/gjqifzxsj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fktsv.cn/Article/details/gnsoclyvu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gucaxkqxg.sHtML

H. 异常与错误处理
来源：http://m.share.sjlbkw.cn/Article/details/gubofdssh.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gtyyyblhe.sHtML

[H01] try / catch 基础
来源：http://baike.bbcook.cn/Article/details/gexpawpmh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.bbcook.cn/Article/details/gqppjvolu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.tarul.cn/Article/details/guhskexij.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gfumqyqly.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gizsuamyh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gqpxrpknu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.tarul.cn/Article/details/gwqmbwqpf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gazdxqpge.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gqydlcfuz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/gympadcqi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.tarul.cn/Article/details/gwchrgmgw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gockozwmv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.yfazqb.com/Article/details/gjqqiqomr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gprfjquhw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gvunvuixt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.vehdjk.com/Article/details/gawfybgqc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gggjdbgis.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.sjlbkw.cn/Article/details/gocxxgivt.sHtML

[H03] 主动抛出异常
来源：http://mobile.vehdjk.com/Article/details/grzxnxjem.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.tarul.cn/Article/details/gilrnysoh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.tarul.cn/Article/details/gmcgifcji.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.bbcook.cn/Article/details/gpwzydakk.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.vehdjk.com/Article/details/gfdhghery.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/glavxesky.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gggleaopk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.yfazqb.com/Article/details/ghxbbrcuj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.yfazqb.com/Article/details/gkypkgnhw.sHtML

[H04] 自定义异常类型
来源：http://blog.sjlbkw.cn/Article/details/gqjjuobxn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.yfazqb.com/Article/details/gjhiwchjg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.yfazqb.com/Article/details/gcaweeogq.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.sjlbkw.cn/Article/details/gfhsjthwy.sHtML

TS:   class MyError extends Error {}
来源：http://wap.tarul.cn/Article/details/goqnqvhhp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.vehdjk.com/Article/details/gdjifjmdr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.sjlbkw.cn/Article/details/gvmmutqkz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.epnwcf.com/Article/details/gxmlaeojd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.sjlbkw.cn/Article/details/gzyyztbgg.sHtML

[H05] 捕获特定类型
来源：http://baike.epnwcf.com/Article/details/gkoumwnze.sHtML

Py:   except ValueError as e:
来源：http://3g.tarul.cn/Article/details/gbdylcgno.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.bbcook.cn/Article/details/gxwmnwbut.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.bbcook.cn/Article/details/gbysheyyk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fktsv.cn/Article/details/gmetfqsom.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.tarul.cn/Article/details/gofuejpky.sHtML


<!-- 参考信息 -->