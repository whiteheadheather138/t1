代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/ghqjqtpgb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/grnaoiale.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/ggtfdfnha.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gepuetjmm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gegqfkkxb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glasnkwaj.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gdscdomhp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmwsrbyuo.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gymtvimjy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gzesnljpc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gckzizrbp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gmwkyxhjq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gmxkmlfqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/guqtnixfk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gbchlrcye.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gacdvdjof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gzdjkqcpz.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gwnzalauf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gfbvtbnwg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gknqwxshl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/grflpxndl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/geppqpfhl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/ggdxulild.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gkutnvzyg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gvwwtfiag.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/ggkeawlki.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.vehdjk.com/Article/details/gbcheyzqu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gtopbfcqw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/geqxkyjtq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gwetzkyhi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ghusaxbfw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.sjlbkw.cn/Article/details/ggrwmtafa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/grceixbzk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gyjpxqalk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gmfbbckvh.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/gdqddmcwq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.bbcook.cn/Article/details/gntnjbaid.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gbcitdlzd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gmdupwvwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gqvkbparl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gckbutwcb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gdkzjolkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.epnwcf.com/Article/details/gmjyidzrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/girpimvpt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gjjnieulw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gsvmjzoik.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjvvpoga.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gapgyqzkg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/glagrwyfk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gmbmxulmw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gugiiexsz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gzufqcxyp.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gymogmsws.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gqfrkiisw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guhzqouof.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gdafsjmhe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gemeymmqp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/grlrllrvj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gdmocbxcx.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gmmjnifdg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/gskvpknnj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/giqygepsr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gnnqqmbrl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gtatesygj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/ggnroldeq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gjxiwprfh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gvtkdjdym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/grxfihpnx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gzqwumame.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.tarul.cn/Article/details/gqknowuea.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gbcwtxcun.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/glmdcbhdk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/ghyuuxyjn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gdgtbipaq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.bbcook.cn/Article/details/ggxqmblcv.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gptchcwyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gavgndmyr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/ghmghvfpw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gzzrlresc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gzryozigl.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gcluuwujj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/guyrczicn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gywsroxce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/giaeylhet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/grbdluiub.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/guuvqjfjk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/geiistgun.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gjcrwfmkm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gufpesppb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/gazxexryh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gagwspisl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwfafvsaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gsnqvuyfz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gewlwjkzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.vehdjk.com/Article/details/gewnstacv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gfqlrgfpy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/glnubmywl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/ggstzpsyj.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gqxtammvo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gbsntsnik.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gcbczyhmb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glrvmwiin.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/ggvenwksb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gxmllvqaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gtsugaquc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gvkxfksxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/govykowed.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gwwdyjszy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/ghtmgeqpj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/giwnvoidw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gycnmwedj.sHtML

TS:   // 同上
来源：http://mobile.fktsv.cn/Article/details/gvyjamnde.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.tarul.cn/Article/details/gklnxxqrq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gvppmlvvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gbhknmbpr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.yfazqb.com/Article/details/gvcocdagv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjgludtsy.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gtbpfnwpo.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnqwqdvvr.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gtprqsrtl.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gprlhzkmk.sHtML

PHP:  class User {}
来源：http://www.share.epnwcf.com/Article/details/gbkatykyl.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/geqjdezez.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gkkergsbi.sHtML

Java: class User {}
来源：http://www.blog.bbcook.cn/Article/details/gcdnssnuy.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gzdmzmszz.sHtML

Ruby: class User; end
来源：http://3g.vehdjk.com/Article/details/gnacxdimz.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gtmwqktbk.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/gubdeiwce.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/glngsrhgf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.epnwcf.com/Article/details/gnkhbthcr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gryviuwnk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.yfazqb.com/Article/details/gavttmqjo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gzzqanstw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/gmgokpfhf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.vehdjk.com/Article/details/gvutngnwk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gjorqdvsq.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/guuwbifdv.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/gtoxojdlv.sHtML

PHP:  public string $name = "x";
来源：http://wap.fktsv.cn/Article/details/gjckeyofn.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gdmfcmfbb.sHtML

TS:   name: string = "x";
来源：http://m.share.tarul.cn/Article/details/gbxgtiqvm.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/gtzyddkqj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gucsaridk.sHtML

Ruby: @name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gljnbzbgu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/gxgphpitg.sHtML

[G04] 定义方法
来源：http://mobile.vehdjk.com/Article/details/gwmcphmux.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/gasmcsvju.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/gvqhgdzbl.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gzymqopnp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.yfazqb.com/Article/details/gkvmedvqi.sHtML

Java: String greet() { return name; }
来源：http://blog.epnwcf.com/Article/details/gadpndznw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gkyjyfion.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gfcwlnrmq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gtgskxqvv.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gsgykfwts.sHtML

Py:   class Admin(User): pass
来源：http://www.share.vehdjk.com/Article/details/ghtyolrwh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/gazpvlikl.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gbjhgnbne.sHtML

TS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gosievfry.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gezluzxgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fktsv.cn/Article/details/ggxljlhpw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gzocfzftc.sHtML

C#:   class Admin : User {}
来源：http://read.share.vehdjk.com/Article/details/geylsfyjo.sHtML

[G06] 重写方法
来源：http://www.share.tarul.cn/Article/details/gyqjqqkih.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gwfmadufw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/guavvnkih.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gklokpotu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gaizczxch.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gqogskczf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/gcddtzzih.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.yfazqb.com/Article/details/ggtkrsmol.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.epnwcf.com/Article/details/gzfgfgafh.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gcpeofsjr.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gnceuscsw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gbbflxndb.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gghqvwemm.sHtML

TS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gyjdxkije.sHtML

Java: super.greet();
来源：http://www.blog.fktsv.cn/Article/details/gfqvpuisf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/gizgvpcwj.sHtML

Ruby: super
来源：http://read.share.fktsv.cn/Article/details/guphxmwwh.sHtML

C#:   base.Greet();
来源：http://baike.bbcook.cn/Article/details/gcjucdyqd.sHtML

[G08] 静态方法与属性
来源：http://mobile.vehdjk.com/Article/details/gmhssarwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fktsv.cn/Article/details/gihjluxoc.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gqmimzsjy.sHtML

JS:   static f() {}
来源：http://m.share.vehdjk.com/Article/details/gqwifgbbj.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/glhtxnxqj.sHtML

Java: static void f() {}
来源：http://mobile.bbcook.cn/Article/details/glufyjrpp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.bbcook.cn/Article/details/gtdeadrvc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.tarul.cn/Article/details/gophtjbpj.sHtML

C#:   public static void F() {}
来源：http://mobile.epnwcf.com/Article/details/gtupdmdpn.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/glwssanfr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.vehdjk.com/Article/details/grussekea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.tarul.cn/Article/details/gdzhpnldi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gygscklcv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.yfazqb.com/Article/details/glmyzycnn.sHtML

Java: interface Shape { double area(); }
来源：http://blog.sjlbkw.cn/Article/details/gcbdkrugl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.tarul.cn/Article/details/gygyuqnfy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.vehdjk.com/Article/details/gnfzjxsoi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gvqmantxb.sHtML

[G10] 访问控制
来源：http://m.share.epnwcf.com/Article/details/gggbhmota.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/grgjnblpc.sHtML

PHP:  public / protected / private
来源：http://m.share.bbcook.cn/Article/details/ghenjoyqj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.epnwcf.com/Article/details/gstqbzimm.sHtML

TS:   public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/gzmisnffg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.yfazqb.com/Article/details/gkvwdhfuo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/grembfdej.sHtML

Ruby: public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/guqkvycak.sHtML

C#:   public / protected / private / internal
来源：http://blog.bbcook.cn/Article/details/gcjsyqcwb.sHtML

[G11] getter / setter
来源：http://www.share.fktsv.cn/Article/details/gbeesxprt.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.bbcook.cn/Article/details/gkarvxame.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gsnbpujnu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.tarul.cn/Article/details/gpwruknpn.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.epnwcf.com/Article/details/gzaouhugk.sHtML

Java: public String getName() { return name; }
来源：http://3g.fktsv.cn/Article/details/gwigegmiq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gatojvicc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbmvdnvk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/gbftucodi.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/goakuyfut.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/gpakthkqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gbxcktnkc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.tarul.cn/Article/details/gakzxwuyo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.vehdjk.com/Article/details/gksutienl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gjxlbneub.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gkthfqsjb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/gtpghmsop.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.vehdjk.com/Article/details/grijmiueo.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gaxyhikci.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fktsv.cn/Article/details/gzhjyttnb.sHtML

PHP:  $u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gtizslntp.sHtML

JS:   u instanceof User
来源：http://www.m.share.vehdjk.com/Article/details/gbxzsvtqn.sHtML

TS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gndhnjjir.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gyxnqrgba.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.tarul.cn/Article/details/gtkvreeff.sHtML

Ruby: u.is_a?(User)
来源：http://3g.tarul.cn/Article/details/ghhzqsszy.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/gtqomkmii.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gfvidudib.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.sjlbkw.cn/Article/details/gytegfqho.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.epnwcf.com/Article/details/gjtnftelx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.yfazqb.com/Article/details/guegvshut.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.bbcook.cn/Article/details/gtsmtyuof.sHtML

Java: record User(String name, int age) {}
来源：http://3g.sjlbkw.cn/Article/details/gkrujixyy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.sjlbkw.cn/Article/details/gooppvmpc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fktsv.cn/Article/details/gfljwzsnj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.tarul.cn/Article/details/gpxaexysg.sHtML

[G15] 枚举
来源：http://mobile.vehdjk.com/Article/details/glasghjyz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gfosdduol.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.sjlbkw.cn/Article/details/gkjtkbfiy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.epnwcf.com/Article/details/gfjfymaum.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.vehdjk.com/Article/details/gyhvrugso.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/gmgpmdtpq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.sjlbkw.cn/Article/details/gfxemhslq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.sjlbkw.cn/Article/details/gghydbjxk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fktsv.cn/Article/details/gamlrwejf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.epnwcf.com/Article/details/ghrsbpjju.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.tarul.cn/Article/details/ggfhtjtdz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gmanvrulv.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.yfazqb.com/Article/details/ggpiwjoqg.sHtML

TS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpzgmmjha.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.tarul.cn/Article/details/gbdtgsgfq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/gdkpmuyvx.sHtML

Ruby: obj.instance_variables
来源：http://3g.epnwcf.com/Article/details/gkphqifaj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gpqqttgjd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmamvyvaw.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/gxupzpsfk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwuzqybnk.sHtML

[H01] try / catch 基础
来源：http://baike.fktsv.cn/Article/details/gftpufydk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.epnwcf.com/Article/details/gtjanmzfm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/gbemomvzn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gbnvlaxkw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.vehdjk.com/Article/details/ghwrjddpq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gebvzgrse.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.bbcook.cn/Article/details/gzmiodbaa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.yfazqb.com/Article/details/gonwlsioe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gwvzzysmk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fktsv.cn/Article/details/gzfxhalwb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.yfazqb.com/Article/details/gyofbvmlg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.sjlbkw.cn/Article/details/gumyzmwet.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/grhrxcuyd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzazodhds.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gqjsebkhz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.epnwcf.com/Article/details/grylgwyfa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.epnwcf.com/Article/details/gwtuyvkty.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.yfazqb.com/Article/details/glnkpgdvq.sHtML

[H03] 主动抛出异常
来源：http://mobile.epnwcf.com/Article/details/gaofqcbmq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.yfazqb.com/Article/details/gwhyfscdi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.yfazqb.com/Article/details/ghjonugdh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.tarul.cn/Article/details/gxegwuvko.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.tarul.cn/Article/details/ghveesnvc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/ghavyzaqy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fktsv.cn/Article/details/gmnregkrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.tarul.cn/Article/details/gdnnjbrab.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fktsv.cn/Article/details/gxnsetftq.sHtML

[H04] 自定义异常类型
来源：http://baike.sjlbkw.cn/Article/details/gqvnsamoh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.sjlbkw.cn/Article/details/godjyejax.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.tarul.cn/Article/details/gxchackss.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.tarul.cn/Article/details/gzgewbjri.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fktsv.cn/Article/details/gmervnvhq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fktsv.cn/Article/details/gknginxqu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.vehdjk.com/Article/details/gwymzterl.sHtML


<!-- 参考信息 -->