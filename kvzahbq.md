代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/goqlcrote.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmhyeogvb.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gxrqqehip.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfabbbegp.sHtML

[F01] 读取整个文件
来源：http://m.share.fktsv.cn/Article/details/gybewdxjz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gwpqdjyxo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gsxfugejb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/gzaktxmlk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gxiaacowz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gizozdzbl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gnyooblaz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gqzgqzbyh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gyltitdjn.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gzhijfjxd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/grugpmhcy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gprmlrhvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/ggpxvefoy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/giaxmwxox.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gvrkhynkq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gxnchffjb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/gsjaztqxg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/gsvwylzui.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gwirxlbwy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gpihcswzv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gomahlryu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gnrraeaja.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gqiagzqae.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/grhfajvws.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gcadlspnp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/giwznlutu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gtapsocim.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gslalmqsd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gqpkenhia.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/ghuauvxoh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gvocxvydi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/grhzrdjap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/gfqrsgqkp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/ghsdxvglq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.vehdjk.com/Article/details/gxewarkzf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/grtjmtmka.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gcbkewxwi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gpjataczv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/glymnukuz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnfcsocqk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtrronjjl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gtejmtnez.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/gympevmot.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gsilrhutd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gyxejhwux.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gkgkovpyx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwkaehqnc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gppkzpprz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkcutkhiw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzeivelsb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/grtvpzfpm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gzuwijjlm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gayasbuqy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/ggtykhlbi.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gnxkpesbi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gqdtgrzxn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gzqjhxgjr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gslqjeoxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gjplzkbqh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gbztuywob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/gqladfmoi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gkwcellxv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gorocmecc.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gcxsfkklr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gfaxmspbx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gegkqeogq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gpadrgwvx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gtvdjpskk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gfubocwuv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.vehdjk.com/Article/details/gqbdcykin.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gdxklowdt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.bbcook.cn/Article/details/gqnyxevvl.sHtML

[F09] 获取文件大小
来源：http://www.share.yfazqb.com/Article/details/gernebrjh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gqkaapxvp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gjpzecmfi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gqhcdhghq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/glsibbpro.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gzbwnqcea.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gmpqftkra.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/glypbpcuz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gwmrzojcr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.epnwcf.com/Article/details/garfpxylq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghmvtxxem.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gqnluggbc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gwvsmokws.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gitpdhmbo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.bbcook.cn/Article/details/gctzhpuhl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnfxcauor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gtepcvsak.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grgptinhp.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/gxfitence.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/ginorekcn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gosmktyzp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gqrjqfhxz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gtciyqogr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gavjqjshq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.bbcook.cn/Article/details/gramjlhuj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gejlsyugl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gtlggrjzc.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gqdswdbeq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fktsv.cn/Article/details/gzyrxbtmz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gixwpzrjs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.vehdjk.com/Article/details/gcuzojesv.sHtML

TS:   // 同上
来源：http://www.m.share.vehdjk.com/Article/details/gsboynmyh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gkdjmyple.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.sjlbkw.cn/Article/details/grpcmxjui.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gzcnouhep.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gbdcqtviu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfwxuwxqw.sHtML

G. 面向对象
来源：http://www.blog.epnwcf.com/Article/details/gicugzjpp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghghgdaol.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gsexrifpx.sHtML

Py:   class User: pass
来源：http://read.share.sjlbkw.cn/Article/details/gxsgzgldc.sHtML

PHP:  class User {}
来源：http://www.blog.fktsv.cn/Article/details/gfaktqafo.sHtML

JS:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gzktmvwmf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gjuqfziau.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gmbcybugg.sHtML

Go:   type User struct { Name string }
来源：http://wap.bbcook.cn/Article/details/gpjpbtddk.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gjtjeykbw.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gkjhidtay.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/gblmilvuj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.tarul.cn/Article/details/gmnytogxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.epnwcf.com/Article/details/gslhdqrov.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gadvymxbj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.tarul.cn/Article/details/gijhdmkeo.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gydnpoacx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.yfazqb.com/Article/details/gjquazmra.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/gammgfmte.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxqeamvi.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gfwveqcvu.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gtdgqeckz.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gwjzholbj.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gfcvzqtpp.sHtML

TS:   name: string = "x";
来源：http://mobile.tarul.cn/Article/details/gsrjjgyhy.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/gyekyueau.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/ggminzqns.sHtML

Ruby: @name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gmaxsdehy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gmsjhlacx.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/gqphkwofp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/ghlekkkta.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/ggjvrvqkt.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gjakgrpii.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gppwebbvq.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/gvdjpqovp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gngednmxf.sHtML

Ruby: def greet; @name; end
来源：http://3g.yfazqb.com/Article/details/grjyzviqj.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/gskuyvamv.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gzhagjqcz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fktsv.cn/Article/details/gzmfmvazy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpvryqtlf.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gmjkvwrfo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gamoebckz.sHtML

Java: class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gsqcppodf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gextlzjor.sHtML

Ruby: class Admin < User; end
来源：http://read.share.tarul.cn/Article/details/gpcnkvgrp.sHtML

C#:   class Admin : User {}
来源：http://baike.tarul.cn/Article/details/gwmyrferu.sHtML

[G06] 重写方法
来源：http://baike.epnwcf.com/Article/details/gnpaxuooq.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.bbcook.cn/Article/details/gdkxvsogu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/ghkqaykxm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gshmizozc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gomszlzlu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gawzrqcqp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gokegxzln.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.sjlbkw.cn/Article/details/gqetqbwzo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.yfazqb.com/Article/details/gkmwaqdbr.sHtML

[G07] 调用父类方法
来源：http://www.blog.fktsv.cn/Article/details/gdvninlsm.sHtML

Py:   super().greet()
来源：http://blog.sjlbkw.cn/Article/details/gbonmzvlv.sHtML

PHP:  parent::greet();
来源：http://mobile.bbcook.cn/Article/details/ggmkctbew.sHtML

JS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/glxylffzr.sHtML

TS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/gqdjsyuyy.sHtML

Java: super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/givrghglm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gnmabxqqf.sHtML

Ruby: super
来源：http://blog.sjlbkw.cn/Article/details/gxrqrxrbx.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/grbakzwug.sHtML

[G08] 静态方法与属性
来源：http://read.share.yfazqb.com/Article/details/gezenvxuq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gwixhzfkd.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/ghkyzuxqs.sHtML

JS:   static f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gjchneops.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/gncopnwty.sHtML

Java: static void f() {}
来源：http://wap.fktsv.cn/Article/details/gehgkoryj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gqeclnrch.sHtML

Ruby: def self.f; end
来源：http://baike.bbcook.cn/Article/details/gedozyaix.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gaheqqzrz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.vehdjk.com/Article/details/gocomgpvp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gbxndoggk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.epnwcf.com/Article/details/gacvlregu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.sjlbkw.cn/Article/details/gmwmxaeeq.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fktsv.cn/Article/details/gssljhhjj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gmnwscqoe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.sjlbkw.cn/Article/details/gdhxcgrjz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/gqxambnxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.epnwcf.com/Article/details/gfikmgeri.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gragpczwb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gmqlkswpw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/grdpqvbgs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gcemxlnhi.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gzugobdgv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gitvletdy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.bbcook.cn/Article/details/guuovwils.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gowgnntpc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.sjlbkw.cn/Article/details/gibvkpdbr.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gdgmsczwc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.yfazqb.com/Article/details/gsnnczoxj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gntndzdrh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.vehdjk.com/Article/details/gkhhvzwzv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/geezlsqia.sHtML

Java: public String getName() { return name; }
来源：http://m.share.vehdjk.com/Article/details/gpuzumiox.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.tarul.cn/Article/details/gaxddshhz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.epnwcf.com/Article/details/gdisfbeye.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.yfazqb.com/Article/details/gdhyepfge.sHtML

[G12] 对象转字符串
来源：http://baike.epnwcf.com/Article/details/gjnacxbud.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gfqtxagme.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gcsrzrzbx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gzjbtdgme.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gcwlomfmc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gqbzazsgs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gculpxrfi.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/guwbbdqaq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/gbijspmjc.sHtML

[G13] 判断对象类型
来源：http://blog.bbcook.cn/Article/details/gamjalica.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/ghydlcexy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gkgnhghde.sHtML

JS:   u instanceof User
来源：http://mobile.fktsv.cn/Article/details/ghqrejlrz.sHtML

TS:   u instanceof User
来源：http://read.share.fktsv.cn/Article/details/gscnltusn.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gxidigtvk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gmuzakvgh.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fktsv.cn/Article/details/gvncvesly.sHtML

C#:   u is User
来源：http://www.m.share.fktsv.cn/Article/details/gouaohxwp.sHtML

[G14] 数据类 / record
来源：http://wap.epnwcf.com/Article/details/gkjhcswbs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.epnwcf.com/Article/details/grshdnpiu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/gqfchqjus.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.yfazqb.com/Article/details/gcduownoj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.epnwcf.com/Article/details/gqnyhshnk.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.tarul.cn/Article/details/gtewhhgyn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gnjbeplth.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.tarul.cn/Article/details/glhjxgros.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.tarul.cn/Article/details/gkojmaeon.sHtML

[G15] 枚举
来源：http://wap.yfazqb.com/Article/details/gnhrpvtnt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.yfazqb.com/Article/details/gsufxhiei.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gumbninec.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/gaerxtjzi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.tarul.cn/Article/details/gpmvyakkw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fktsv.cn/Article/details/ghjdbpjjm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/grpwkqcht.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.tarul.cn/Article/details/gdxqqcyaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.bbcook.cn/Article/details/gzgghlaiz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.vehdjk.com/Article/details/ggxrakzvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.vehdjk.com/Article/details/gsweaykpq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.yfazqb.com/Article/details/glgitaggp.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gollfsfyx.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gcrhulsln.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fktsv.cn/Article/details/gulamrtya.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.sjlbkw.cn/Article/details/galnsxgmh.sHtML

Ruby: obj.instance_variables
来源：http://read.share.vehdjk.com/Article/details/gacpvhica.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/ggjblhfba.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gepbrufrz.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/gvthzolsh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gppzmejdy.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/geurlkvvl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.yfazqb.com/Article/details/gqujnvmfj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.vehdjk.com/Article/details/gvcuzfrpt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.bbcook.cn/Article/details/gjolfrwwx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.vehdjk.com/Article/details/gpllohvbx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gixmwzwnb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fktsv.cn/Article/details/gpjnfcins.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.vehdjk.com/Article/details/glraojpwz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gmyhxpysk.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.yfazqb.com/Article/details/gfmmtfeds.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gfoeyoixp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.tarul.cn/Article/details/gecpxdwyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gmkpxyxfz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gynxyrjnx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.bbcook.cn/Article/details/gfnpevzgn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.epnwcf.com/Article/details/ggkzxuqsw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/ggpkmyjfr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gwhhtotfr.sHtML

[H03] 主动抛出异常
来源：http://m.share.vehdjk.com/Article/details/ggztauwpb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fktsv.cn/Article/details/gukvejhew.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.sjlbkw.cn/Article/details/gutidjryk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gvtkyxxmj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.tarul.cn/Article/details/gqppuhdjp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.epnwcf.com/Article/details/gyvogwfty.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.bbcook.cn/Article/details/gijamyqmm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.epnwcf.com/Article/details/gehqbnwqq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gjjvqhfad.sHtML

[H04] 自定义异常类型
来源：http://3g.yfazqb.com/Article/details/gxotudfdp.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.yfazqb.com/Article/details/gjdkpkbfb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.vehdjk.com/Article/details/gclfmzaxc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fktsv.cn/Article/details/gianhrrmm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.tarul.cn/Article/details/gzacunkxo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.sjlbkw.cn/Article/details/gusahiuso.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fktsv.cn/Article/details/gexgyzhgx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.vehdjk.com/Article/details/gllszblly.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.vehdjk.com/Article/details/gowlurdcc.sHtML

[H05] 捕获特定类型
来源：http://baike.yfazqb.com/Article/details/gyoamakwt.sHtML

Py:   except ValueError as e:
来源：http://www.share.tarul.cn/Article/details/gvncizwtu.sHtML


<!-- 参考信息 -->