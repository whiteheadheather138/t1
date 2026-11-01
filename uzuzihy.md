代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gpcqfrvzd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/ghfmueltw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/goxqvqffr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gcdnmozed.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/grkucleuc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmezxcgbp.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gfhiysnli.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcstcoaqe.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gdhemxvmy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gbhomsbbr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gkznvnmos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/gtzzchlrj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gxkfyvikq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gpohelmzz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/grhieqcml.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvefxdein.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/giknurycs.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gullpvnue.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gckiwnirj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gzfczichn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gkjyadnxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gneurmeqy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gygiqoepl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gjupijoth.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/grnhldssa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzrjuhiju.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.yfazqb.com/Article/details/gdqzpoxkb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.bbcook.cn/Article/details/gasugkmsv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/glikldvoo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/grathhvwm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gdcjlould.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/grwfuxzpj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gozpctmct.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gbptcvova.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gtijffcmc.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gmazormjd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gqubfleyx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gnomsltxw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfooxsqbf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gufwhsepg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gsmytmylr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.tarul.cn/Article/details/ghyfowhex.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gmjtpjftu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gwrqncvvk.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.tarul.cn/Article/details/gmezyhwco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gybvotvmo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gawezjmgo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/glnwatftm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzprqrjxf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gfhzqtjpm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gqpeutplr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdnrszqmo.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gcmyicfqi.sHtML

[F06] 删除文件
来源：http://www.share.sjlbkw.cn/Article/details/gghrzvfmy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/goodqrxyk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gfiffflgt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvmsbjpkt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gzuvbvmbk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gzbdnbxkc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gubehtlvk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gudcuhopt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gdzvhtrtw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gggxfvsyx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gfqocmpim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gfmoayczv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gjlxridpo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/goingluoq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gynantlvy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/gtriycksp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/gatgrysbs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gydxcnhzs.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gkdfjonbu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.bbcook.cn/Article/details/gxmchlxnu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.epnwcf.com/Article/details/gablbodjq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gbizxxhzx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gilmgcxhj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gasgwktio.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gpbqmttfw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.bbcook.cn/Article/details/giiunjurw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gppngoixa.sHtML

[F09] 获取文件大小
来源：http://baike.bbcook.cn/Article/details/gvszfqtdi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gcmdrercs.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.tarul.cn/Article/details/getrzimlc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gujhporhf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gaoesvouj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/gwmgkeppp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.bbcook.cn/Article/details/grtouawos.sHtML

Ruby: File.size("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdwoveqpb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/ggfomjekv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/gfypmtvxh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/grviqhshh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.vehdjk.com/Article/details/gfsddudzx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gcxrwtjrn.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gorqzghuv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fktsv.cn/Article/details/gpiizmiym.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gmdyibnnd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gxtktrxoh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gubwiugaw.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gfteobccg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gqmozwynz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/ggczmuhjw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/ggpsrpqhd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gqzszvjfo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/godgfjriq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gujobcoaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gwkjzqtat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gbtibmcvh.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gzargzdgp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.bbcook.cn/Article/details/gsempmfoa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.epnwcf.com/Article/details/gxpwfmkok.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gvydowtae.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gwqgxtqed.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gpesnbuzd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.epnwcf.com/Article/details/gntirkkeh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fktsv.cn/Article/details/gesffjnsx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.epnwcf.com/Article/details/gjwzicpvd.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gwbzodrrq.sHtML

G. 面向对象
来源：http://mobile.epnwcf.com/Article/details/gcnkfjtti.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gnbnrwbtd.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gtzijqocw.sHtML

Py:   class User: pass
来源：http://blog.yfazqb.com/Article/details/gkxgqyffb.sHtML

PHP:  class User {}
来源：http://mobile.bbcook.cn/Article/details/gcdqqcuro.sHtML

JS:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gjlkdfzeq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/gtzlphrli.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/ghhufgoue.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gruqvuusg.sHtML

Ruby: class User; end
来源：http://www.share.fktsv.cn/Article/details/gprxgajkv.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gygwybrhk.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/geyrpdtvm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gchpvgsrs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gxxzjlxvx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/giyucvhmb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/ghubewsal.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gmvzupuxi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/givwsnoky.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.epnwcf.com/Article/details/gmriijdps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gpjaajdua.sHtML

[G03] 实例属性
来源：http://www.blog.fktsv.cn/Article/details/gtfciibzn.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gpkyubmay.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fktsv.cn/Article/details/gkonfyyaq.sHtML

JS:   this.name = "x";
来源：http://blog.vehdjk.com/Article/details/gumolokfa.sHtML

TS:   name: string = "x";
来源：http://www.blog.vehdjk.com/Article/details/gvdjqztex.sHtML

Java: private String name;
来源：http://www.share.vehdjk.com/Article/details/gomqgltqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gidwrenwe.sHtML

Ruby: @name = "x"
来源：http://www.blog.vehdjk.com/Article/details/gxpwavlfd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.bbcook.cn/Article/details/gwjfdabqf.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/guobocsen.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gozuodubv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.sjlbkw.cn/Article/details/gsqupzupl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gfdcbebsu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gizemjinx.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/ghyduucam.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/gwkkfpjyv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.tarul.cn/Article/details/gmaodrwrt.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/gqktkcumb.sHtML

[G05] 继承
来源：http://3g.fktsv.cn/Article/details/gbemyvpbd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.yfazqb.com/Article/details/gbqwrwhkv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gcocbcuxq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/gwymorlrq.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/grpmurdhe.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/goioyjdff.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/gxcdsfsik.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gztilwvlo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gesxtgkkp.sHtML

[G06] 重写方法
来源：http://blog.sjlbkw.cn/Article/details/ggolbottn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.epnwcf.com/Article/details/guhjcjake.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gvxujteeg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gkvffpedn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gsoqiypxf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gdnuoxqyk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.epnwcf.com/Article/details/gdqhbrpqa.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.sjlbkw.cn/Article/details/grwenvowy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.tarul.cn/Article/details/gmjkkedve.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gosemndac.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gsrmzbhtp.sHtML

PHP:  parent::greet();
来源：http://wap.epnwcf.com/Article/details/gifltxcia.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gendrjdqm.sHtML

TS:   super.greet();
来源：http://read.share.epnwcf.com/Article/details/gcpowfwrp.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gdlwslaml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gjumnucwm.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gyfcvmupy.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gfkdjwrlf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.yfazqb.com/Article/details/grlfqeikm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fktsv.cn/Article/details/gqcqmgswj.sHtML

PHP:  public static function f() {}
来源：http://3g.epnwcf.com/Article/details/ghdntuqwl.sHtML

JS:   static f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gwrkvooeg.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/guwdtmigc.sHtML

Java: static void f() {}
来源：http://www.share.fktsv.cn/Article/details/gdsglqdyp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/ggixwbsen.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/gqotjcuni.sHtML

C#:   public static void F() {}
来源：http://3g.epnwcf.com/Article/details/gnwhtkshh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/gklmffjev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gevkaopvr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.bbcook.cn/Article/details/guhljnxpy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.tarul.cn/Article/details/gnfuadfpl.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.bbcook.cn/Article/details/gtrnmmpag.sHtML

Java: interface Shape { double area(); }
来源：http://baike.tarul.cn/Article/details/gglsouicf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/gkfryodal.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fktsv.cn/Article/details/gzdjsjfox.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gdgmvlbpa.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/ghtnvcjie.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.bbcook.cn/Article/details/ghfkwfrmg.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gsqcbpwcv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gkdgedmyb.sHtML

TS:   public / protected / private
来源：http://www.share.tarul.cn/Article/details/gocoduaas.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.yfazqb.com/Article/details/gxbjurxdo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/grvzsmswt.sHtML

Ruby: public / protected / private
来源：http://m.share.sjlbkw.cn/Article/details/gribztynx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.sjlbkw.cn/Article/details/gyfdnqjdx.sHtML

[G11] getter / setter
来源：http://www.m.share.bbcook.cn/Article/details/gnjnsaurr.sHtML

Py:   @property 与 @x.setter
来源：http://baike.tarul.cn/Article/details/gdhdtbpaj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/gahzxvkac.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gitfqfwja.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.vehdjk.com/Article/details/gsobovorq.sHtML

Java: public String getName() { return name; }
来源：http://baike.bbcook.cn/Article/details/gbruddtil.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gwumgjcuo.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gqxwxucnc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.bbcook.cn/Article/details/gzorfhand.sHtML

[G12] 对象转字符串
来源：http://baike.vehdjk.com/Article/details/glaplkwfw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.tarul.cn/Article/details/gdunwbwiw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fktsv.cn/Article/details/gsprmjizy.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gabfqviqe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/grwgzgpuq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.epnwcf.com/Article/details/gsdcykhgm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gvulzaqaq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.yfazqb.com/Article/details/gilycgqtl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.vehdjk.com/Article/details/gdtjkhmzo.sHtML

[G13] 判断对象类型
来源：http://m.share.fktsv.cn/Article/details/gsklokiil.sHtML

Py:   isinstance(u, User)
来源：http://m.share.vehdjk.com/Article/details/gyaptzopf.sHtML

PHP:  $u instanceof User
来源：http://baike.tarul.cn/Article/details/gozcaluun.sHtML

JS:   u instanceof User
来源：http://wap.fktsv.cn/Article/details/govgkmzji.sHtML

TS:   u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gjgqhstrc.sHtML

Java: u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gvezpwcov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fktsv.cn/Article/details/gufsenxzc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/getzyvauu.sHtML

C#:   u is User
来源：http://www.blog.sjlbkw.cn/Article/details/gyfssydap.sHtML

[G14] 数据类 / record
来源：http://mobile.bbcook.cn/Article/details/gblimrpbs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.bbcook.cn/Article/details/gkvxtmbpt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.bbcook.cn/Article/details/gsvazswnm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.yfazqb.com/Article/details/grdkwwxpx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fktsv.cn/Article/details/gtinhyfxh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.tarul.cn/Article/details/gfixgfeds.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.epnwcf.com/Article/details/gibhzmhxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.sjlbkw.cn/Article/details/gqeaqihyn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.tarul.cn/Article/details/ggaizmmmx.sHtML

[G15] 枚举
来源：http://m.share.epnwcf.com/Article/details/gkghhvivy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fktsv.cn/Article/details/gozshvdli.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.bbcook.cn/Article/details/gouypfqza.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.sjlbkw.cn/Article/details/gsrefnrya.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/genukjwyt.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gtowzulnf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gogdmatzg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.epnwcf.com/Article/details/gxszxvskh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gpsblyzeu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.sjlbkw.cn/Article/details/gczcxkzum.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.vehdjk.com/Article/details/grafryogv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/ggcbykgzg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.vehdjk.com/Article/details/gfyyzpkgg.sHtML

TS:   Object.entries(obj)
来源：http://blog.yfazqb.com/Article/details/gzpzelnfs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.sjlbkw.cn/Article/details/gctcxlbgh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/ggzkoclqt.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnunqjib.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.epnwcf.com/Article/details/ghiuuxxqc.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gatkwhjsv.sHtML

H. 异常与错误处理
来源：http://www.blog.epnwcf.com/Article/details/giwwjglpn.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glowloupq.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gcqykfoap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fktsv.cn/Article/details/gldbggdgy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/golcdhhpc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gtqqzeijf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gfhzjkroe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.yfazqb.com/Article/details/glsnhuykc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gloywuxwv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fktsv.cn/Article/details/gsabgleyc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.vehdjk.com/Article/details/gvnsotaaf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.bbcook.cn/Article/details/gldibswjt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.bbcook.cn/Article/details/gemiwtvte.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.epnwcf.com/Article/details/gdzetmmdh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gqkzjevld.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gostbybuq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.epnwcf.com/Article/details/gicpxlegk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/ggatqbqbs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gidssltbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.bbcook.cn/Article/details/grrwdshnz.sHtML

[H03] 主动抛出异常
来源：http://read.share.bbcook.cn/Article/details/gurnjmtjj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fktsv.cn/Article/details/gdfhtcvru.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.yfazqb.com/Article/details/gpawxordb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.tarul.cn/Article/details/gpkwhmpng.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gowdxcfmr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.vehdjk.com/Article/details/gpqkjzmni.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fktsv.cn/Article/details/gthveofgr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.yfazqb.com/Article/details/gtwikwxss.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gzzvibyhs.sHtML

[H04] 自定义异常类型
来源：http://wap.yfazqb.com/Article/details/gxuwjyaty.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.bbcook.cn/Article/details/gkpyoarih.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.vehdjk.com/Article/details/gqasijzcm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.tarul.cn/Article/details/gxkkfpgep.sHtML

TS:   class MyError extends Error {}
来源：http://blog.bbcook.cn/Article/details/gdughdjmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.epnwcf.com/Article/details/gxrrssipy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.yfazqb.com/Article/details/gqkzgdpla.sHtML


<!-- 参考信息 -->