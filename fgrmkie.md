代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/glpmkiodp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/geiukaldh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/glmxehdly.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/godoaztgo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcnjlucln.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gzcqighqv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/glmphsjxc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/ghinnyxek.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gvyoibjxj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gtfkclubv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gzmuklmcu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gzlikxpzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gxkykihka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gacpejvus.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gjywfuhje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfouglqhe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gfemyotdp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gvlezyzyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gfxhoncbb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/gvhexyxyi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/ggepmifvl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gidvlwclb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/grimxwjsc.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gdiykfdxg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/glyunhjih.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/gtfwgwuoa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gflmqjqhu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gubmazabb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.epnwcf.com/Article/details/grczggqsu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gfwokaimo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gkmpdaytd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gfgdubmsy.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gibxhludo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/grwlgqzks.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/grmwtdacb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghrbaztse.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/ghwaewphg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gkqwxclnt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gmplwlpfr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfeiyxprh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glxoebvlx.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/gvypvlpna.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwbhhjvsr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjtkfljch.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gharytlup.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gdqmuadfl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/ggxkciigp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gnfcywele.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtakxyhbz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gltmedrnb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gxwnezmgc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gsdjcpkdm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gxwobpjwj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gssbryzng.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/gmkjshxjo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gohjtdioy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/gwvuqkklz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gktezljsb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/gusmgfhjj.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gdmuzmutz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.yfazqb.com/Article/details/gzvjmdkfr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.vehdjk.com/Article/details/guoewjooe.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/ghbcbcavm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gtjtffowk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gabwsssha.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/glezoivwi.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gzzqihvmx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/ghqdtpsdv.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gciwrenzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gtukwypqx.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxnuwqney.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gpmfhkyco.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gsjjnyiqu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gluldjijb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.vehdjk.com/Article/details/glbgrixbk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/giblaapxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.epnwcf.com/Article/details/gmxmjhxrf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gujsqlxgh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/genjqazff.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gsvmcbjnt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gyxuaoxxi.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fktsv.cn/Article/details/geqnfdfrp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/ggzfygzka.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gcupnptqy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbuykytob.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/ghxfxeteo.sHtML

[F11] 复制与移动文件
来源：http://3g.sjlbkw.cn/Article/details/gqcfbyara.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/ghsekpprp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gqtseeotn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gxwivlqtm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gmtkqyfrt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gpzsecmwr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gnhddlzfh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gssiyrnmq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/ghxvjuven.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gnhgfjfby.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.sjlbkw.cn/Article/details/gbbjyglla.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gtdwxgbeq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gvfqyeynw.sHtML

TS:   // 同上
来源：http://baike.sjlbkw.cn/Article/details/gretdxkuz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/gxrctuzfp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gnbiouatu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/guairuykg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/goxjgenug.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvtsvugne.sHtML

G. 面向对象
来源：http://www.m.share.epnwcf.com/Article/details/goisjyisv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxnookikf.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gskjgbqcp.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/ghmynueje.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gccawlaur.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gekhtndmr.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.yfazqb.com/Article/details/gnvvgdcuy.sHtML

Java: class User {}
来源：http://read.share.bbcook.cn/Article/details/gbbjnudfi.sHtML

Go:   type User struct { Name string }
来源：http://wap.yfazqb.com/Article/details/gxwtlartu.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gylvufvtg.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/ghehesrfk.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gglfguazi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.bbcook.cn/Article/details/gnikxfdvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/ggswgpoux.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gjdmimgis.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gkumvgezo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gaqhcpkfe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/ggpooofma.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gkcszkzam.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/ggpbqamof.sHtML

[G03] 实例属性
来源：http://www.blog.epnwcf.com/Article/details/gtrclkmrj.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/ggudshini.sHtML

PHP:  public string $name = "x";
来源：http://read.share.epnwcf.com/Article/details/gujsghjwi.sHtML

JS:   this.name = "x";
来源：http://www.blog.yfazqb.com/Article/details/gvfjxllsi.sHtML

TS:   name: string = "x";
来源：http://baike.fktsv.cn/Article/details/gwxvpsbua.sHtML

Java: private String name;
来源：http://www.blog.vehdjk.com/Article/details/gdzjvinxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gacqjuqgo.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gooynsdxw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gpgzslrcx.sHtML

[G04] 定义方法
来源：http://read.share.epnwcf.com/Article/details/gfbdbauqm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gzspxenql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/ghkprunui.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gillgxyzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gnhfsujdd.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/grvcluvmq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gygtdhlvd.sHtML

Ruby: def greet; @name; end
来源：http://wap.tarul.cn/Article/details/ghakxywlt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gjksrwees.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gcweawlom.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gvfcazlmq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gguecxdbl.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gqdorufuz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gagffxnxi.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/ghmjutpqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.tarul.cn/Article/details/gzsdpciil.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/guuphlvoz.sHtML

C#:   class Admin : User {}
来源：http://mobile.tarul.cn/Article/details/gxecjqrpx.sHtML

[G06] 重写方法
来源：http://www.m.share.yfazqb.com/Article/details/gyqetoajr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.tarul.cn/Article/details/grrnkeola.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gfpnqygtd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gctrzgtnv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/ghzhtvqds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gsvrfrecj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gjtsrekeb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fktsv.cn/Article/details/gimguwefl.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.sjlbkw.cn/Article/details/gvmipzqpz.sHtML

[G07] 调用父类方法
来源：http://www.share.bbcook.cn/Article/details/gjxmqjrzb.sHtML

Py:   super().greet()
来源：http://m.share.tarul.cn/Article/details/gspqtnpmt.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/gdluaftbb.sHtML

JS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gnbfmyzxy.sHtML

TS:   super.greet();
来源：http://www.blog.bbcook.cn/Article/details/gyafaivhz.sHtML

Java: super.greet();
来源：http://www.share.tarul.cn/Article/details/gmkqibawn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.sjlbkw.cn/Article/details/gvvipjneb.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gtrbwehmw.sHtML

C#:   base.Greet();
来源：http://blog.sjlbkw.cn/Article/details/gqupyyagi.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.tarul.cn/Article/details/ghzawlwmf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gbfsxmbul.sHtML

PHP:  public static function f() {}
来源：http://baike.vehdjk.com/Article/details/gwrfetrvc.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gnquufdhz.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gghlenlxh.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gtonscdnj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.bbcook.cn/Article/details/geemqosil.sHtML

Ruby: def self.f; end
来源：http://baike.yfazqb.com/Article/details/gaduffgkg.sHtML

C#:   public static void F() {}
来源：http://3g.bbcook.cn/Article/details/gskgbxrqu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gpwoyhthi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gndhqddcu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.sjlbkw.cn/Article/details/gjlvupkwf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fktsv.cn/Article/details/gjnidynru.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/grvcnvirw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gjcnbyjag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/gowcbnslx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.epnwcf.com/Article/details/grmsjpmoh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gyyxpzqki.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gjmsewgjs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.yfazqb.com/Article/details/gqmrvhljk.sHtML

PHP:  public / protected / private
来源：http://blog.sjlbkw.cn/Article/details/grwvtdklw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fktsv.cn/Article/details/gaobshxyo.sHtML

TS:   public / protected / private
来源：http://3g.fktsv.cn/Article/details/gkhftqfrx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.sjlbkw.cn/Article/details/ggckjabzn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.epnwcf.com/Article/details/gsgeaakig.sHtML

Ruby: public / protected / private
来源：http://read.share.tarul.cn/Article/details/gibzhwnxt.sHtML

C#:   public / protected / private / internal
来源：http://mobile.vehdjk.com/Article/details/gxpzcjids.sHtML

[G11] getter / setter
来源：http://m.share.sjlbkw.cn/Article/details/gegdnmjkt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/grobznzxl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gfzvjzmxu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.tarul.cn/Article/details/gifdhxrbg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gaybjtyqu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gbtdsfxpu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gksusnefv.sHtML

Ruby: attr_accessor :name
来源：http://3g.yfazqb.com/Article/details/guqhrkpng.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gjlrqcjtv.sHtML

[G12] 对象转字符串
来源：http://m.share.vehdjk.com/Article/details/ghjsmkzez.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.tarul.cn/Article/details/gwoegwslk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gvnyiixkz.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gdhhpdgeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gmizhmpfj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gsthzqeic.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.bbcook.cn/Article/details/gasggkaqx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gghplbjjd.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.tarul.cn/Article/details/gfzjnadeo.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gtyhbhjuq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gmiohyffq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/gvikiwgmh.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/grwdaltej.sHtML

TS:   u instanceof User
来源：http://www.blog.sjlbkw.cn/Article/details/gomjczgsy.sHtML

Java: u instanceof User
来源：http://baike.fktsv.cn/Article/details/gltffccxl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.bbcook.cn/Article/details/gjqdgdhso.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gozhlhbbc.sHtML

C#:   u is User
来源：http://wap.tarul.cn/Article/details/gsipjhgym.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gkkbcqbwl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.bbcook.cn/Article/details/grgqinocq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.epnwcf.com/Article/details/gvcpbslkn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.bbcook.cn/Article/details/gcwhebvqb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.bbcook.cn/Article/details/gqkfctpzo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gllrlxuyy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.tarul.cn/Article/details/ggejgwvyd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gfmlrfphp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gwmihndtm.sHtML

[G15] 枚举
来源：http://www.share.fktsv.cn/Article/details/gvuxrbmry.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gvtuaynro.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.bbcook.cn/Article/details/gtntuivel.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.bbcook.cn/Article/details/gvzsrimfc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.epnwcf.com/Article/details/gutdgebtm.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.vehdjk.com/Article/details/gkmmxxbuf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/ghnpbxtpz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fktsv.cn/Article/details/gznarucfn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gvlrstqwy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gewfatsut.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/gzuuljqvz.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.sjlbkw.cn/Article/details/gghzcvwgm.sHtML

JS:   Object.entries(obj)
来源：http://baike.fktsv.cn/Article/details/gybcgwnzo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gavjdfsrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gnxofvgcw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.sjlbkw.cn/Article/details/gwomhukca.sHtML

Ruby: obj.instance_variables
来源：http://www.share.bbcook.cn/Article/details/gytcqxutd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/ggvoqoomx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdhwyftqi.sHtML

H. 异常与错误处理
来源：http://www.blog.fktsv.cn/Article/details/gamgabcoz.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzqsyovys.sHtML

[H01] try / catch 基础
来源：http://www.blog.vehdjk.com/Article/details/gvwerzbnx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.bbcook.cn/Article/details/grvnnzhwu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.vehdjk.com/Article/details/gjzdbpsyv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gcbpyzurr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.tarul.cn/Article/details/giqwlzwpo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.vehdjk.com/Article/details/gmxiimstf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.epnwcf.com/Article/details/gzenkpwum.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.sjlbkw.cn/Article/details/gfwapbqdt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fktsv.cn/Article/details/gcqjxdlyh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.bbcook.cn/Article/details/gxpjsfyph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.bbcook.cn/Article/details/gyeablyxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.sjlbkw.cn/Article/details/gsglvtybl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.epnwcf.com/Article/details/gchghaagf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gwwkfgvyp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.vehdjk.com/Article/details/gfgwxjwxl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.vehdjk.com/Article/details/glgxzqptv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.vehdjk.com/Article/details/gmuefjrwu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.bbcook.cn/Article/details/gtmthxegm.sHtML

[H03] 主动抛出异常
来源：http://3g.epnwcf.com/Article/details/grrnhicbv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.bbcook.cn/Article/details/gprlyxabw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.yfazqb.com/Article/details/gdyzalbrt.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/ggbyxodzg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.bbcook.cn/Article/details/gymnshgxr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.vehdjk.com/Article/details/ghbfvugrr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.yfazqb.com/Article/details/gnrfdxvps.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.yfazqb.com/Article/details/giaqqjoar.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gpqrtaetw.sHtML

[H04] 自定义异常类型
来源：http://baike.fktsv.cn/Article/details/ghxtqonjk.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.tarul.cn/Article/details/gjwxknzat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/geshmpiia.sHtML

JS:   class MyError extends Error {}
来源：http://baike.bbcook.cn/Article/details/ghqaumyoa.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.bbcook.cn/Article/details/gybgsjjpu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fktsv.cn/Article/details/gbpazwrjh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.yfazqb.com/Article/details/gzblxhbmd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.yfazqb.com/Article/details/ghvvawtww.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.epnwcf.com/Article/details/gfmtsqpcz.sHtML

[H05] 捕获特定类型
来源：http://m.share.vehdjk.com/Article/details/gacgdajld.sHtML

Py:   except ValueError as e:
来源：http://mobile.fktsv.cn/Article/details/gomgklvwl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.yfazqb.com/Article/details/gfcgajtta.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.tarul.cn/Article/details/genffodez.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.bbcook.cn/Article/details/gggmkmhju.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.epnwcf.com/Article/details/gitzfppla.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.tarul.cn/Article/details/gtpjojcwu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.bbcook.cn/Article/details/gzjtkjwmy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.bbcook.cn/Article/details/gbokagkgz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.tarul.cn/Article/details/gbvnbtosg.sHtML


<!-- 参考信息 -->