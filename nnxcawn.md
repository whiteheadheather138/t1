代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gozgmybeu.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsliehppi.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gpyyjgzdt.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grsdaykhz.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/gyewcvikx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gzjwpskkr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gkycsniwp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gunodwrsn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gcicseqgk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gxnqszxtp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gysvzgktd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gqnflmook.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gbjidugkk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gjiybbisj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gksholwjk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/ggryiyqie.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/glbipmzks.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gyaweqawy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gimzyctog.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gccmphotj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/gfjapgyvf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.yfazqb.com/Article/details/gqvtspbwx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gbshexsxo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/geufublsu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gsfprcxje.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gjijnntzs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gmwihlriq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gfxqnmleg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gqhseixfo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.vehdjk.com/Article/details/gzvwpzxub.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gsfztzweq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gcwwzlcff.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/goizyagzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gzbugcwlt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/ghxnkolrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gewxscjde.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.vehdjk.com/Article/details/ghublvtgh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gsbdhnhoy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gflhzbmqc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/glurnmfmg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gfdfnlvtl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gnyqozjol.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/ggjfscjsv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ghqlovmoa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gjyhjyvcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/ggwvlmdwo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/gzgzfatan.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gnlwdyzut.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gcjoqlrke.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gxbuxqldf.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gdhhwnidc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.yfazqb.com/Article/details/gcvoizvpu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggpeqyqvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/guhgcwhrn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gpmakidcs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gwpjgmqpz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gqmxeklje.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gdetlyied.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.tarul.cn/Article/details/gsrlwlkgs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gobznqqtm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gdwnqajhz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fktsv.cn/Article/details/gufbjnknz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gccqtzddl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gmchjnzfq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.bbcook.cn/Article/details/gstelnvan.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gcyoauaii.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gntznqwea.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/getveyosq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gyqfkbyht.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/groucawjg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gybcspdfy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/ggjzighgs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gbcqbsknt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gfkrgrqfi.sHtML

Ruby: Dir.children("dir")
来源：http://3g.vehdjk.com/Article/details/gzadurlsc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/guvykdhiv.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gcphtfgkc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gchnrjiho.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gxpqzmzzb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gupclltyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gkxiueubc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjlmzuflj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.vehdjk.com/Article/details/gcekjinhz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gqzzflgjc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/gmbkkzvec.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/gnytegspj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbpafeiwp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gpgemxahe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gaiinujqk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gakowukqs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gyqdjopll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gbjefbtpz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gfloydjao.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gpfkclceo.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/gzvvemsiy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/ggslckcgd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gmwdkwnmj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbzbcpuhi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gerfgkdye.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.epnwcf.com/Article/details/ggyzkengx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.bbcook.cn/Article/details/gyslqcuop.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gnrumtjii.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.tarul.cn/Article/details/gqdklkkwj.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gdmgfddgi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.tarul.cn/Article/details/gvtghbugo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gztmppuka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gzfsmdmfq.sHtML

TS:   // 同上
来源：http://mobile.yfazqb.com/Article/details/graxghabv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.tarul.cn/Article/details/guneghsai.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/giqpvcfhk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.sjlbkw.cn/Article/details/gfdbenaio.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/gytlbpkyq.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfjrkywvc.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gtuyxjafw.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfrgjqoak.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gzhozzieo.sHtML

Py:   class User: pass
来源：http://blog.bbcook.cn/Article/details/gwhvnwtyv.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gkowvkyhz.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gelfjdbsh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/goddqfchf.sHtML

Java: class User {}
来源：http://baike.epnwcf.com/Article/details/gncxlclbs.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gwdgbtfmn.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gmhhgxfmy.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gspvolepm.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/gunzvbmzv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gzzcomeyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gbrfnvcur.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/guwkujwym.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.bbcook.cn/Article/details/gnmvtewxk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gspmmadks.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.epnwcf.com/Article/details/gocslvggh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/gegbgpjpy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gvmwqandp.sHtML

[G03] 实例属性
来源：http://www.share.vehdjk.com/Article/details/gdrmwoflm.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gbduiklje.sHtML

PHP:  public string $name = "x";
来源：http://mobile.vehdjk.com/Article/details/gyxmfgocn.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/ggggvhbcg.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gvreaphme.sHtML

Java: private String name;
来源：http://www.m.share.fktsv.cn/Article/details/gjfqdttou.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.epnwcf.com/Article/details/ggjzqwbnh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/ggwfhwsla.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.epnwcf.com/Article/details/gcamcnrie.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gpwfbmaek.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gjfyjhdhv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gtqzfwuka.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gcwibzwtv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gfswvfbro.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gsqcpdkaa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.tarul.cn/Article/details/gwuvwxzab.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.yfazqb.com/Article/details/gncoswfke.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gvlkwxzta.sHtML

[G05] 继承
来源：http://www.blog.yfazqb.com/Article/details/gzwjcjixd.sHtML

Py:   class Admin(User): pass
来源：http://baike.tarul.cn/Article/details/grgkmvpve.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gktmchntg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gqgcikaej.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gpcwbpxcn.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/ggeycbkpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.epnwcf.com/Article/details/gtlhjceqx.sHtML

Ruby: class Admin < User; end
来源：http://wap.bbcook.cn/Article/details/gbdstrifw.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gtyqdxbqq.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gwaouyywa.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.bbcook.cn/Article/details/ggptpmphk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gughwabjn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/godncybnu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gryzlrzsz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gamihxzrb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gactozlkn.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.bbcook.cn/Article/details/gfqcrjmyh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.sjlbkw.cn/Article/details/gkmhrevrh.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gwvtuhjhz.sHtML

Py:   super().greet()
来源：http://blog.bbcook.cn/Article/details/gulqhgjut.sHtML

PHP:  parent::greet();
来源：http://www.share.bbcook.cn/Article/details/gjgsofrxg.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gvisssdgz.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gkuxyyjhq.sHtML

Java: super.greet();
来源：http://wap.vehdjk.com/Article/details/giemzprho.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gjyrptmeq.sHtML

Ruby: super
来源：http://read.share.yfazqb.com/Article/details/gkhlemclv.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/gdeghiytg.sHtML

[G08] 静态方法与属性
来源：http://mobile.tarul.cn/Article/details/gryxjlrzs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/guxxjjhhx.sHtML

PHP:  public static function f() {}
来源：http://www.share.vehdjk.com/Article/details/glxgasljq.sHtML

JS:   static f() {}
来源：http://wap.tarul.cn/Article/details/goccfpdop.sHtML

TS:   static f(): void {}
来源：http://www.blog.yfazqb.com/Article/details/gyfnbpsbl.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/grffsboce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.epnwcf.com/Article/details/gelqqnxpr.sHtML

Ruby: def self.f; end
来源：http://mobile.vehdjk.com/Article/details/gxxdryxpo.sHtML

C#:   public static void F() {}
来源：http://blog.sjlbkw.cn/Article/details/gjvmdeibm.sHtML

[G09] 接口 / 抽象类
来源：http://wap.sjlbkw.cn/Article/details/gxgstrboc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/gwefzcfzq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gjmcaabvr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.sjlbkw.cn/Article/details/gnlandzqh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjgpxcmqy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gldiipzms.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.epnwcf.com/Article/details/glmttkadx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gukthiqqo.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fktsv.cn/Article/details/gzpzuvfjc.sHtML

[G10] 访问控制
来源：http://wap.bbcook.cn/Article/details/glhtptxqj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.epnwcf.com/Article/details/gpneczhsx.sHtML

PHP:  public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gajrqkxxs.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.vehdjk.com/Article/details/gghtruiaz.sHtML

TS:   public / protected / private
来源：http://3g.sjlbkw.cn/Article/details/gwywxnulz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gujzgzrlw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/gqwqnijhx.sHtML

Ruby: public / protected / private
来源：http://m.share.fktsv.cn/Article/details/guyzcfgga.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gilqhnrfs.sHtML

[G11] getter / setter
来源：http://wap.tarul.cn/Article/details/gkjaodbir.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.yfazqb.com/Article/details/gamhkduwa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gajcfvboy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwytbhcfq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.vehdjk.com/Article/details/glufqbigo.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/ggjhwstwf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gsmoknbhv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gdbiarxxu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.bbcook.cn/Article/details/gufcxwiju.sHtML

[G12] 对象转字符串
来源：http://wap.bbcook.cn/Article/details/gvxxykavw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.yfazqb.com/Article/details/gyzfvhcch.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gmwnunncs.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gaoyvwkcm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gpscgkmle.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gtrqmmdmy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gcpqpsblx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/grshabzqh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.bbcook.cn/Article/details/gagbmjvlo.sHtML

[G13] 判断对象类型
来源：http://www.share.tarul.cn/Article/details/gubfexeyi.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.bbcook.cn/Article/details/gipqgbnnw.sHtML

PHP:  $u instanceof User
来源：http://m.share.yfazqb.com/Article/details/gzrivtprq.sHtML

JS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gmtoszqgz.sHtML

TS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gfvpxtxzw.sHtML

Java: u instanceof User
来源：http://baike.tarul.cn/Article/details/gvzkyntdy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.bbcook.cn/Article/details/gbjawczyy.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gssecblgo.sHtML

C#:   u is User
来源：http://blog.fktsv.cn/Article/details/gcefknfio.sHtML

[G14] 数据类 / record
来源：http://www.blog.fktsv.cn/Article/details/gudczukav.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fktsv.cn/Article/details/gfxzkaqgu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.yfazqb.com/Article/details/gflniqajh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/gbmdcbkgr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.yfazqb.com/Article/details/geweihxvq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fktsv.cn/Article/details/gjpdfjttp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.bbcook.cn/Article/details/gohohplmi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.sjlbkw.cn/Article/details/glwlurbmx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gehkdresj.sHtML

[G15] 枚举
来源：http://blog.yfazqb.com/Article/details/gbsdetcyj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.epnwcf.com/Article/details/gslxkqifg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsjupekka.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fktsv.cn/Article/details/gvemypcxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.vehdjk.com/Article/details/ghsjhbgwo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fktsv.cn/Article/details/gqfwodjic.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.sjlbkw.cn/Article/details/gbxuaocky.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.epnwcf.com/Article/details/gnyibmmuo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gkeqrrfho.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.bbcook.cn/Article/details/gbaabuggc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gvgrxexkl.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.epnwcf.com/Article/details/ghjthlksz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gvckedhsf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfnzybnff.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gshuqolsn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.epnwcf.com/Article/details/gddnflpxh.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gybfwfdhh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.vehdjk.com/Article/details/gtzmcihfl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnbpxilcf.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gvfwzleyl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gpygyhqgn.sHtML

[H01] try / catch 基础
来源：http://www.share.yfazqb.com/Article/details/goicdpkpa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gnspkwkbq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.sjlbkw.cn/Article/details/gjtrjbkgy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/gvwdmjdtt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gxtpfxmqu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.yfazqb.com/Article/details/gisrcyfis.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.bbcook.cn/Article/details/gvfzejith.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.epnwcf.com/Article/details/gcrqeenhe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gmzzxkkdw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.vehdjk.com/Article/details/gdsudwhms.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.tarul.cn/Article/details/gxnxajvac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gtgkrvwbb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gckikzebs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/garcqwyxz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmxlqizet.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.epnwcf.com/Article/details/gonbtxual.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.tarul.cn/Article/details/gekvregzk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.tarul.cn/Article/details/gisxeczeq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvnprpcd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.yfazqb.com/Article/details/gyypgphct.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.vehdjk.com/Article/details/gtopjknkr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/gjvkmwrdl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gulvmtfba.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.bbcook.cn/Article/details/gkexdwbwq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fktsv.cn/Article/details/gknuejcci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.vehdjk.com/Article/details/gokazyjzb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.sjlbkw.cn/Article/details/gnevswtjl.sHtML

[H04] 自定义异常类型
来源：http://mobile.tarul.cn/Article/details/gpulcvkyg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.sjlbkw.cn/Article/details/geuqwjvcm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.bbcook.cn/Article/details/gfrxrxncz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gjqrzasyv.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/giyavrimf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.sjlbkw.cn/Article/details/gnmndvkey.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.bbcook.cn/Article/details/gxcpmhpdu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fktsv.cn/Article/details/gepllnzdo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.tarul.cn/Article/details/guqqcklzn.sHtML

[H05] 捕获特定类型
来源：http://blog.fktsv.cn/Article/details/gptgcyawe.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyxassgp.sHtML


<!-- 参考信息 -->