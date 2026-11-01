代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gcbithpaw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gobtdxhhq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gzehpnhsz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gejedqmjt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gnuyaadge.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcnqrmvb.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gumjreajg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnolgdsgl.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/grpzmwmfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fktsv.cn/Article/details/gsdplzcdi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gcelporgj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gwxxjaadp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gdhfvpwyw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/grcgjnkxw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gyxbbdcyg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqmnodwco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gvfuthuip.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/glxbinkai.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gpejzghlf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/ghvrzpjgq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gyytrxpbt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpnftuqic.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gyvooflvn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gfftlnrwb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gtxvvnmpi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gbegwjwsq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gwlgeypnn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gojlwokdt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/guzpwfpuq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gxdfdcuie.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gysvqijti.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gmwgdioae.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gmcgbxley.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.tarul.cn/Article/details/gnivqcdxu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gmivsergs.sHtML

[F04] 追加写入文件
来源：http://www.blog.epnwcf.com/Article/details/gljcajris.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gzfyuotvv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gjqmdldhc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gkyhohvcu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gqibrzdec.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/gmpuxsehu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gpjqbsrux.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.vehdjk.com/Article/details/ghhxockbt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.tarul.cn/Article/details/grykqqvrj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fktsv.cn/Article/details/gvinhvdec.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gjbfcddhi.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gdptoonzh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grelnjlqx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/grzbaudah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gwgeuqpmi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.bbcook.cn/Article/details/gavskmdct.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gmqghobrq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfbcgywcr.sHtML

[F06] 删除文件
来源：http://www.blog.fktsv.cn/Article/details/guaffxxsb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gzpczxtpc.sHtML

PHP:  unlink("a.txt");
来源：http://3g.epnwcf.com/Article/details/gfqighfif.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gjkfyprwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwoaxvpfl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gwvbczaoz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbvjlyxhl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gfczxjshf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gbgboybrn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/grslcorqi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gdyehshlb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gaudfrfwo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gfpzakwqp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gvomwegul.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gpurvwjtk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gxeduqsbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gycttuplh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gguonlqun.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gsjejhtlq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gvpaplram.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gxgrwuzxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gefydrgde.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gwnhaxvxg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gobpynnkh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.tarul.cn/Article/details/gawdeoheo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.sjlbkw.cn/Article/details/gbielykhy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gfvkxapzp.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/gtfxocpty.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gmknnlayn.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gxkoedbgr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gdarlqfxz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/gsdewmgjl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gduhiohyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gaoxyqnlt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.tarul.cn/Article/details/geyrvmyru.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gpemxunhh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.epnwcf.com/Article/details/gtzlylmwm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gtnzfltey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gxixatfcx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/glqsfehcz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gzwyfomwg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.tarul.cn/Article/details/godedotmx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbwoqrkpn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbokvakis.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gtztkwpnw.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gbymiltoz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gxstthvfy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.epnwcf.com/Article/details/gxcxwuspx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gzhpcumhb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gcvfyuwmu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gvfwkthbb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.bbcook.cn/Article/details/gzvugxcit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gsfxfmwlx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.bbcook.cn/Article/details/gyzrnqnjt.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gokwmbpix.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gzmupajmb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/ggpnhmyjq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gyjpvfstk.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gfsnhzsav.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/gyqqyqpdl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gwjfxfjxe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fktsv.cn/Article/details/gxrcngmga.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fktsv.cn/Article/details/gpguifrwr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gfllorwmt.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gnvkdgfoq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnoukzvij.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gepttsnzy.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/gnmccwzlv.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/gowlwouww.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gufrjmmer.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.bbcook.cn/Article/details/gxbesavsd.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gjqgsbpzo.sHtML

Go:   type User struct { Name string }
来源：http://3g.bbcook.cn/Article/details/glnylsrco.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/gklubdkjf.sHtML

C#:   class User {}
来源：http://blog.vehdjk.com/Article/details/gtedgtjni.sHtML

[G02] 构造函数
来源：http://read.share.yfazqb.com/Article/details/goxqgfjmq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.yfazqb.com/Article/details/gdwsxpaad.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gziqluwqx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gidtpvdjm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/glrhbwrfi.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/gxrqjahfg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/gsohumbba.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gdtyzniom.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.epnwcf.com/Article/details/gwqjhpmme.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/gmyepcagi.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gnpvoxfby.sHtML

PHP:  public string $name = "x";
来源：http://read.share.vehdjk.com/Article/details/gxhfswlni.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gkcynnvpb.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gxnrwesec.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/grqjwjbxm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gejqmudmq.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gogavlavw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gojzqgwee.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/glogiojwa.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gcfxsegjx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gdxsmzkpc.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gqeingjje.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gvytsfozz.sHtML

Java: String greet() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gyaeushmg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.vehdjk.com/Article/details/gljrbyued.sHtML

Ruby: def greet; @name; end
来源：http://read.share.vehdjk.com/Article/details/guccvwayq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gvmcsvqvz.sHtML

[G05] 继承
来源：http://www.blog.tarul.cn/Article/details/gvkgtnrvz.sHtML

Py:   class Admin(User): pass
来源：http://wap.epnwcf.com/Article/details/gkrfbzerz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gaqlwcbsj.sHtML

JS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gexvnqkom.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gukkddjrx.sHtML

Java: class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/geqvpupwn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/gbwvaxhvz.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/gkwptzozz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gbfhtaxdj.sHtML

[G06] 重写方法
来源：http://www.share.yfazqb.com/Article/details/gyqojrtif.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gdxfyyboe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gbcknupse.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gyzksshck.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.sjlbkw.cn/Article/details/gzepedcka.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/ggmxixzog.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gibiyrejz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gtekpwikk.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/gvmqwdpvz.sHtML

[G07] 调用父类方法
来源：http://mobile.fktsv.cn/Article/details/giezssnci.sHtML

Py:   super().greet()
来源：http://3g.epnwcf.com/Article/details/gojdrfvzy.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gbtjobufx.sHtML

JS:   super.greet();
来源：http://www.m.share.vehdjk.com/Article/details/gsoofdyjk.sHtML

TS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gtvefrbhi.sHtML

Java: super.greet();
来源：http://www.share.yfazqb.com/Article/details/godmxscxj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.yfazqb.com/Article/details/gfvpwhwqw.sHtML

Ruby: super
来源：http://baike.tarul.cn/Article/details/gcbsgkpsm.sHtML

C#:   base.Greet();
来源：http://mobile.sjlbkw.cn/Article/details/godyzogzt.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gfblnrvao.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.yfazqb.com/Article/details/gpxiczqgm.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gyttimdtm.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gwucxqqtp.sHtML

TS:   static f(): void {}
来源：http://3g.yfazqb.com/Article/details/gyjowrquk.sHtML

Java: static void f() {}
来源：http://mobile.fktsv.cn/Article/details/gwxbzwgoj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gfxqseiwp.sHtML

Ruby: def self.f; end
来源：http://www.share.vehdjk.com/Article/details/gfnwdkkqn.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/giuxmudoe.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gcswyvbxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.sjlbkw.cn/Article/details/gkgdlveen.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gesfwixqk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.tarul.cn/Article/details/gjbxhtpav.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gzbytldvi.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.bbcook.cn/Article/details/gqopfbpwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gawrdddpl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.sjlbkw.cn/Article/details/gdhhlanpm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.tarul.cn/Article/details/gxocsipxq.sHtML

[G10] 访问控制
来源：http://3g.tarul.cn/Article/details/gqqfmfpni.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.vehdjk.com/Article/details/gnriigesm.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gebggbafi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.tarul.cn/Article/details/ggseofqvs.sHtML

TS:   public / protected / private
来源：http://read.share.bbcook.cn/Article/details/gducaugqe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gkythjjiw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.bbcook.cn/Article/details/gznatkpan.sHtML

Ruby: public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gqtmzyrco.sHtML

C#:   public / protected / private / internal
来源：http://3g.yfazqb.com/Article/details/gieenickh.sHtML

[G11] getter / setter
来源：http://baike.epnwcf.com/Article/details/grekrfwbg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/glbpgtyqc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gfykrhgfq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/gkgtjaold.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gzksvphqc.sHtML

Java: public String getName() { return name; }
来源：http://wap.bbcook.cn/Article/details/grrifdrdf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gmapnoowz.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gqwpkiwto.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.tarul.cn/Article/details/ggifoteet.sHtML

[G12] 对象转字符串
来源：http://m.share.epnwcf.com/Article/details/grtopvcpd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gdtbeevfr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gggrkixud.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gbzascpiv.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gxvucnwph.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/grvqfrnju.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gmdaewlnw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gmzzkncdy.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.epnwcf.com/Article/details/gnpzgjyro.sHtML

[G13] 判断对象类型
来源：http://3g.bbcook.cn/Article/details/ghxsumhjx.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.tarul.cn/Article/details/gkriosucv.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gihuqnxkh.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/gcmuuglqq.sHtML

TS:   u instanceof User
来源：http://baike.tarul.cn/Article/details/gftacdkvx.sHtML

Java: u instanceof User
来源：http://baike.vehdjk.com/Article/details/guchompzl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fktsv.cn/Article/details/gvrorqxvz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.bbcook.cn/Article/details/gbhmbxstd.sHtML

C#:   u is User
来源：http://www.m.share.epnwcf.com/Article/details/gfzqiagcz.sHtML

[G14] 数据类 / record
来源：http://baike.sjlbkw.cn/Article/details/gaawpltgu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fktsv.cn/Article/details/gmlfukrhh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.tarul.cn/Article/details/gbggnpkih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.tarul.cn/Article/details/gvhjegrzu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.epnwcf.com/Article/details/gtcaodzej.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gcfhzoulb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gtoxyyibc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/gnbithwmt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/grdnqoavv.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gxjadfsel.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/guadfkxzd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.epnwcf.com/Article/details/gjckbxtci.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fktsv.cn/Article/details/gptgtafiy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.sjlbkw.cn/Article/details/ggzwhyobw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gkknufkzw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.tarul.cn/Article/details/gpajlsbap.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.tarul.cn/Article/details/gsmfjxfos.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.yfazqb.com/Article/details/gocetvydw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.epnwcf.com/Article/details/gvzogigvh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.sjlbkw.cn/Article/details/gkpphxmrr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.yfazqb.com/Article/details/glrqqsfor.sHtML

JS:   Object.entries(obj)
来源：http://blog.fktsv.cn/Article/details/gbjeufjuc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbqudsfd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.vehdjk.com/Article/details/gagsezdfq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.sjlbkw.cn/Article/details/gbwqsczre.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.sjlbkw.cn/Article/details/girkwvehl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gerucwvhy.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfacpbaol.sHtML

H. 异常与错误处理
来源：http://www.share.vehdjk.com/Article/details/gidldgxae.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glhrtxtwt.sHtML

[H01] try / catch 基础
来源：http://m.share.tarul.cn/Article/details/gusssumtd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.sjlbkw.cn/Article/details/gkvntkzwk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.bbcook.cn/Article/details/ghdalnexd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gpvazjrcd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gzmmofrbb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.tarul.cn/Article/details/gfzwrsdze.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.vehdjk.com/Article/details/gkudcbhbz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.bbcook.cn/Article/details/glpmfmrge.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.tarul.cn/Article/details/ggavepiiy.sHtML

[H02] finally / ensure 收尾
来源：http://3g.yfazqb.com/Article/details/goeofidcs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.epnwcf.com/Article/details/gpfferbog.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gvrfyipqs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.yfazqb.com/Article/details/gvvlvtoxr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/ggolnzcga.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.tarul.cn/Article/details/ghqvglzyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.yfazqb.com/Article/details/gbekdvgtl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.epnwcf.com/Article/details/gocpqpvgc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/gfjrngaac.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gvkycgosj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.sjlbkw.cn/Article/details/gjzltdyzg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fktsv.cn/Article/details/gvqnyelfo.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gafueneph.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gxjpvoqmd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fktsv.cn/Article/details/gnesqlsbv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.tarul.cn/Article/details/geosmhdkx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.sjlbkw.cn/Article/details/gmzixrbcv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.bbcook.cn/Article/details/gusmteelt.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gtijanlmk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.sjlbkw.cn/Article/details/gfrykvykd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.sjlbkw.cn/Article/details/gvfojazyz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fktsv.cn/Article/details/gktsbnxbp.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.vehdjk.com/Article/details/gzhdhnqer.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.epnwcf.com/Article/details/geshkibmf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.tarul.cn/Article/details/ggsavbqag.sHtML


<!-- 参考信息 -->