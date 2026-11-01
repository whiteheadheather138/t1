代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gsmnmpclm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grdwjkjne.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gidtdxsnr.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnvylclyn.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gokrzwgay.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/golnhszwx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/grwqmlkmz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gvaocagzv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gybdrtcjg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gbbngvion.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.bbcook.cn/Article/details/gjvcamdbr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gzagyewes.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/grzxibwca.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/gczwbarna.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gyusbaicp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gfuhocyyn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gzrudaxex.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gjiksmsui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gzljlzydk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.vehdjk.com/Article/details/gdduqvcch.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gxiebtwpg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gyfnvlrhn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gobnwbzhg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gfvxthpch.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/geaujpvnn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrrtflgh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gjltxtepc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/gdyswljtv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/geiwmzdry.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/glxatsztn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gyfctcsll.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gsrbidmmx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gkchjktpr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.vehdjk.com/Article/details/gelqsxamb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gjbgrkccy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gaohqpdle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhjlrggh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gnhvcrqpi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/ggzwfyguo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gijaapfeb.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gjjrqusae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/giytliwyx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtedqbnlb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgihmfoo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpkusgdon.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gnjhagvpz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.tarul.cn/Article/details/gstsrxona.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghlzdwplx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gqxqlxtbt.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gkdcujofp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gbzlevxht.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gkmxdusdp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/ghvtnjhmd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/geaccxdfq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gvmqmhvwl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/girufvycl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtkjxixke.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.tarul.cn/Article/details/gahzefuub.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/glnaswibd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fktsv.cn/Article/details/gztstnsmk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gfzcfvkaj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gwbnjlqyi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gkwnwsddt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gthulagxb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.bbcook.cn/Article/details/gqoswysgz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gezqlnlzw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gibisskii.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/ghbxztffl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/ggkebzvrp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gnckqxfcr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gkcvxkftb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gmhyzarfm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gnanziuha.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/ggbwspamg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/gaenhefva.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gstvoojwi.sHtML

[F09] 获取文件大小
来源：http://wap.tarul.cn/Article/details/grvwpcalr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfubixatp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.tarul.cn/Article/details/ggifwmntz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gvfihxbfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gunwinafj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gqktsmygq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.yfazqb.com/Article/details/glawgyxnq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxypsbsub.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gksqqgngd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gmeomatpw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gzwqtjvrn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gjbbzsxbj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggsupjhpu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ggzxzyrur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/ghiodpxdv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gdltzkunh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggeckyrca.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gulveknrf.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gdnmaspam.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gbldowffk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gcivwreao.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gkpurwxlk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gkaiygdyx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gbldjwzzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.bbcook.cn/Article/details/gvtoxyjay.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gstkqyimo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/ggtpzizqw.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gojqwxswg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gspojbuev.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.tarul.cn/Article/details/grfvmfpxm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gfobavkeb.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gvqmhnhnm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gyjrhmylb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gzhihjzvb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/gdbcepbwm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/glwohnzyo.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gonwwlmus.sHtML

G. 面向对象
来源：http://read.share.yfazqb.com/Article/details/gqusavbox.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdjfzbhco.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gruyphjab.sHtML

Py:   class User: pass
来源：http://www.blog.vehdjk.com/Article/details/gkvvilkmi.sHtML

PHP:  class User {}
来源：http://blog.bbcook.cn/Article/details/grtiqblsk.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gznphpuvc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gmxcfdaaa.sHtML

Java: class User {}
来源：http://mobile.vehdjk.com/Article/details/grvtjzqoy.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gmvmzajpk.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/ghpuehomo.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gkpynbzbw.sHtML

[G02] 构造函数
来源：http://m.share.sjlbkw.cn/Article/details/guuxiqqsy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.tarul.cn/Article/details/gwapgccsm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/gedkosytq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gvcvinhww.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gfrbdewvs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.vehdjk.com/Article/details/gogbybkpe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gbmaqvhqv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.sjlbkw.cn/Article/details/gkjofxrsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjxospux.sHtML

[G03] 实例属性
来源：http://baike.sjlbkw.cn/Article/details/gzpmkarbk.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gptsqklgh.sHtML

PHP:  public string $name = "x";
来源：http://3g.vehdjk.com/Article/details/gzipzhuhf.sHtML

JS:   this.name = "x";
来源：http://www.share.vehdjk.com/Article/details/gjqzqtnpn.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gvhunpjef.sHtML

Java: private String name;
来源：http://www.share.bbcook.cn/Article/details/gvhttqdgh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gwknzqrmc.sHtML

Ruby: @name = "x"
来源：http://3g.bbcook.cn/Article/details/guqovoffw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.tarul.cn/Article/details/gzzuuyuyb.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/guwxseetc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyarithh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/ghqhswjnj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gjgcsfzjt.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gzoxuofoc.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gkumyrjff.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gudcxzjns.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gmrtufcoq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.epnwcf.com/Article/details/gkxalocmf.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/grorjgazq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.bbcook.cn/Article/details/grqjpxvjx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gautacgyw.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gplymtcsu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gamfjthih.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/geszfamir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.yfazqb.com/Article/details/gfjyjvavr.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/gjlvcuzfx.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/guyybpbyg.sHtML

[G06] 重写方法
来源：http://www.blog.yfazqb.com/Article/details/gzsosqfjl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fktsv.cn/Article/details/gojkfcbgk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/grznpntps.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gvuranhbl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/ggbcffrmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gkubapdwn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.vehdjk.com/Article/details/gogawjzms.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/glrcjcrfh.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fktsv.cn/Article/details/gcomaikpt.sHtML

[G07] 调用父类方法
来源：http://www.blog.sjlbkw.cn/Article/details/grdksnabt.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/glrklqqza.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gfldhyech.sHtML

JS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gbnuceybg.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/gnbbccmjn.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gdzfcfujp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gzdfurdls.sHtML

Ruby: super
来源：http://m.share.sjlbkw.cn/Article/details/gbdzeiieg.sHtML

C#:   base.Greet();
来源：http://www.share.fktsv.cn/Article/details/gxanskezq.sHtML

[G08] 静态方法与属性
来源：http://m.share.vehdjk.com/Article/details/geqsxvrke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gyodlgqnj.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gempvdjtw.sHtML

JS:   static f() {}
来源：http://3g.fktsv.cn/Article/details/gizxamlqz.sHtML

TS:   static f(): void {}
来源：http://read.share.fktsv.cn/Article/details/gmnoynygj.sHtML

Java: static void f() {}
来源：http://www.blog.bbcook.cn/Article/details/gxtflegtf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/guudadpdj.sHtML

Ruby: def self.f; end
来源：http://baike.vehdjk.com/Article/details/ggnzzowmm.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gsskvomjg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.epnwcf.com/Article/details/gxosreayq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gupuzaxkj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.epnwcf.com/Article/details/gchmshfpi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.vehdjk.com/Article/details/gfzzvmiwt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.epnwcf.com/Article/details/gejyrwizp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gwmtbcseq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.epnwcf.com/Article/details/gsbynrztr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fktsv.cn/Article/details/gcixdqfhm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmjnsitly.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/gtcjkkiwr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.sjlbkw.cn/Article/details/glylqdpqh.sHtML

PHP:  public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gowvpgmes.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fktsv.cn/Article/details/gxawhlqgd.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gatmfodch.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fktsv.cn/Article/details/gjohjsyme.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/guoeammqz.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gfmkeuirh.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gcgtkezzs.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/gdvanqdoz.sHtML

Py:   @property 与 @x.setter
来源：http://3g.bbcook.cn/Article/details/gmtmsxnic.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gklgjvkkk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.yfazqb.com/Article/details/gblezvphc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gbwjcoegt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/gxxkvajmx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gkalzajik.sHtML

Ruby: attr_accessor :name
来源：http://mobile.tarul.cn/Article/details/gntvxyakc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.sjlbkw.cn/Article/details/gaoyvyzdi.sHtML

[G12] 对象转字符串
来源：http://blog.yfazqb.com/Article/details/gteflhjmo.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gyvazxute.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/ghpwojank.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gvcdbyydo.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gebeyvoql.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.yfazqb.com/Article/details/gmwsjawld.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gbrjdyjza.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.vehdjk.com/Article/details/gmfmguddh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.yfazqb.com/Article/details/gyylcunjq.sHtML

[G13] 判断对象类型
来源：http://www.share.yfazqb.com/Article/details/gudqzbati.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fktsv.cn/Article/details/gnwraessx.sHtML

PHP:  $u instanceof User
来源：http://read.share.bbcook.cn/Article/details/ghqpmxvpj.sHtML

JS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gzpejysod.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gfmjkevuv.sHtML

Java: u instanceof User
来源：http://wap.epnwcf.com/Article/details/ggbdsvpkz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.bbcook.cn/Article/details/gudsoxkgw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.tarul.cn/Article/details/gslhkydap.sHtML

C#:   u is User
来源：http://3g.vehdjk.com/Article/details/gcjladlyu.sHtML

[G14] 数据类 / record
来源：http://mobile.epnwcf.com/Article/details/gpmukjmqt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/gbbwlhcur.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.epnwcf.com/Article/details/gwwluitgf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.bbcook.cn/Article/details/gvfqwioma.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/goainhjdg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.bbcook.cn/Article/details/gamcujskt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gwtvdklis.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.sjlbkw.cn/Article/details/gzjbiqvuj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fktsv.cn/Article/details/gzvipguoq.sHtML

[G15] 枚举
来源：http://www.m.share.yfazqb.com/Article/details/glipdskwj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.tarul.cn/Article/details/gwfrcvasa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhohwgmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fktsv.cn/Article/details/gsvbvmnai.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gaouiyils.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gwqeuauej.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gijfqyked.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.epnwcf.com/Article/details/gyonoiwrk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.epnwcf.com/Article/details/gkdjbpvva.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fktsv.cn/Article/details/grtnnbnyg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.tarul.cn/Article/details/grskbrskv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.vehdjk.com/Article/details/gmosqicqw.sHtML

JS:   Object.entries(obj)
来源：http://blog.vehdjk.com/Article/details/gjzmopsvi.sHtML

TS:   Object.entries(obj)
来源：http://mobile.tarul.cn/Article/details/grtkqzwuf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.epnwcf.com/Article/details/gijbyqvbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.epnwcf.com/Article/details/gjzdakzcx.sHtML

Ruby: obj.instance_variables
来源：http://read.share.bbcook.cn/Article/details/gvmmulvcj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/gcgwfigmh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjqoqospa.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/gxjokvhqj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqndtwnjw.sHtML

[H01] try / catch 基础
来源：http://mobile.yfazqb.com/Article/details/ghwffczcs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.vehdjk.com/Article/details/gvddonlfy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gefrgcson.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gfekfnwdf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gueskuhmt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fktsv.cn/Article/details/gwgrannoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlmndnnd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.epnwcf.com/Article/details/gjmfujmpx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gyqceaqjm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.bbcook.cn/Article/details/ggfteults.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.vehdjk.com/Article/details/gjgbzhkxu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gsrssgrto.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gsxbydrki.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/gxnajstrp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.bbcook.cn/Article/details/gxajpzrqp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.sjlbkw.cn/Article/details/gsnbwtddr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.tarul.cn/Article/details/gfaxtsjjx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gdfaxmvoz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gygkzwjnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.epnwcf.com/Article/details/gnzmpjwsm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/gtkohtsgk.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.yfazqb.com/Article/details/gysxcbcgl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.sjlbkw.cn/Article/details/gswfvyjwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.bbcook.cn/Article/details/gapinibhc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.vehdjk.com/Article/details/gxuewatgk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.vehdjk.com/Article/details/gknnkwhfg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.bbcook.cn/Article/details/ggjzvgxql.sHtML

[H04] 自定义异常类型
来源：http://www.share.fktsv.cn/Article/details/gflekznub.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fktsv.cn/Article/details/gzdvrrkmh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.yfazqb.com/Article/details/gnmdvgyvb.sHtML

JS:   class MyError extends Error {}
来源：http://blog.epnwcf.com/Article/details/geznauyfy.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/gijtogjpw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fktsv.cn/Article/details/gornpgnpj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fktsv.cn/Article/details/gycdmcvtm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.bbcook.cn/Article/details/ggpqhrhyy.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/getkywmss.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gzpuatofx.sHtML

Py:   except ValueError as e:
来源：http://blog.bbcook.cn/Article/details/gcwmujyqy.sHtML


<!-- 参考信息 -->