代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/genhvbteu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gzmohvlaf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gpiokjqoa.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/gytazgxls.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gocxvustc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxdilzgcy.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gqmbdmnvj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/guovboeoa.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gmvvowsbx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gwwptynjp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gjvnyjgah.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gedpyssnp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gwgawknat.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gpfnjpuij.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gheaowmcc.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gsasggdzu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/glgkahrsq.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gsxckaqcl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/gfiqgejns.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/grnndeajd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gxgykntpo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gqtgaehfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gsafawbtz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gxpageiky.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/glpuznues.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gmiswhacz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/ghsmgvhwd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/gnzivcxcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gyuaqiqig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gjjmwkxbh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gwxcgiikw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/ghtbizooh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/gxleveiia.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.vehdjk.com/Article/details/glefvlcjj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.tarul.cn/Article/details/gdedjjxyy.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gttsqdlpi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/ghxnolasz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gaedruszq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gxvqvaffi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gftphejob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gyrbaorey.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.epnwcf.com/Article/details/gvzmqjqos.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gfptwbzpp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gzwvyuxlo.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gbkejyswz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.vehdjk.com/Article/details/gyclwcjyi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gzhouhfbo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwbmbbxdc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gbtbceahg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmtbkbaai.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gfdgrmndw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gthmllpsf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvskymfwg.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/ggpyvydxm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdlqhsccu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/glxdibhua.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/ghrbiddgc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/geavqcadl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/grovyhlrg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsuhxtyjm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gnrlhcmnz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gxpiikixz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gevjosmfg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gkrytpnlj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.epnwcf.com/Article/details/gcglkgoyx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gsngeqqps.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gfpzxmvnv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/grpodishe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.vehdjk.com/Article/details/gkqzzeuek.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gzbjthmyr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/goecxajwe.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gbixodcnh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gytlvroup.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.yfazqb.com/Article/details/gxwdlgigk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/ghzvtwmuf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gojtcilgj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gigrwaniy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.bbcook.cn/Article/details/gevbgqqrs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.bbcook.cn/Article/details/gxilzhtxb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gtsonpmsm.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/gkmmphbzy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gzvygobjf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gjwasuuhr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gcdiphsmn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gnytxunqj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gbouiuvks.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gswbgvccd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gfrizgpvs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gyfcnwtxa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/goeagurxo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gjlrdbkbo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gfjacyant.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxcdkpjpp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsifrvsfa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gsxoamadx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gjdkkszaq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/ggyasdjfh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gyazizgig.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gstcpvgxd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gowzxaqpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/gtjoyrerr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gnqspzjcr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gxrzwlpqz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.epnwcf.com/Article/details/gggmxokea.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gilisxmfo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gpmxxkyho.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/gqiwdripv.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gpqzmjczo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gfrrqnqyq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gumcbsabv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.tarul.cn/Article/details/gdzhumyzy.sHtML

TS:   // 同上
来源：http://www.blog.yfazqb.com/Article/details/ggrptgxag.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.epnwcf.com/Article/details/gyaalybzx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gqorihygz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gwsyaikvi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gmveqsula.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gchbivora.sHtML

G. 面向对象
来源：http://wap.bbcook.cn/Article/details/gojxiziaq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcneixfak.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gpuultgaj.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gdhsbtoaw.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gbquwosoo.sHtML

JS:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gqttgalzc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/geunrjvco.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gqirpdrcr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.tarul.cn/Article/details/gtracviab.sHtML

Ruby: class User; end
来源：http://wap.sjlbkw.cn/Article/details/ggimxqygy.sHtML

C#:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gchlsnqck.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gndoyvyxz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fktsv.cn/Article/details/gpxznhift.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gjyjdigkj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/givsgdapc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.sjlbkw.cn/Article/details/grxstqjkv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fktsv.cn/Article/details/gqveomgzh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.sjlbkw.cn/Article/details/gsnpexutj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/gwicgxnps.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gszzqcudc.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gpxnjaifw.sHtML

Py:   self.name = "x"
来源：http://3g.bbcook.cn/Article/details/gdqhdjdrx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gplcbkiku.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gwaknmrva.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gulpkbidk.sHtML

Java: private String name;
来源：http://3g.epnwcf.com/Article/details/gfoqmjnvb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gupbdowsu.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gkyveyjhp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.bbcook.cn/Article/details/gydpvmxlp.sHtML

[G04] 定义方法
来源：http://www.m.share.vehdjk.com/Article/details/gzmkdlyrr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.tarul.cn/Article/details/ghbaxpzsg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gywhqdxii.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gligajnfh.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gzufaajnf.sHtML

Java: String greet() { return name; }
来源：http://read.share.tarul.cn/Article/details/ggjsshahj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/gpyacdcwe.sHtML

Ruby: def greet; @name; end
来源：http://blog.bbcook.cn/Article/details/gznhltcgk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fktsv.cn/Article/details/goohdgcvr.sHtML

[G05] 继承
来源：http://3g.sjlbkw.cn/Article/details/ggzbtfnzw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/gzszgdvsm.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/ghtrddauy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gjbczoxqz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/grgbspxob.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzmdwlgnm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.yfazqb.com/Article/details/gxvzovyyg.sHtML

Ruby: class Admin < User; end
来源：http://www.share.vehdjk.com/Article/details/ggqkzzcji.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/gktacydvl.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gdtomkkxr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.epnwcf.com/Article/details/gyvyucnhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gacjfmzmk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gthyxfoih.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/ggonyqzcg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.sjlbkw.cn/Article/details/glqjoqlfp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gzlbbrkrh.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.epnwcf.com/Article/details/gxgsnecqg.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gionalolw.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/grzjmxgue.sHtML

Py:   super().greet()
来源：http://wap.vehdjk.com/Article/details/gvwqbjvrc.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/guqbinoor.sHtML

JS:   super.greet();
来源：http://www.share.tarul.cn/Article/details/govhrvemc.sHtML

TS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/glmamhgwa.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/gzhcqhvjl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.epnwcf.com/Article/details/giyausssw.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gdkteacgl.sHtML

C#:   base.Greet();
来源：http://mobile.fktsv.cn/Article/details/gnfmsamhu.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fktsv.cn/Article/details/gcjbsnmaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fktsv.cn/Article/details/gwtctajew.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.epnwcf.com/Article/details/gkuythwhp.sHtML

JS:   static f() {}
来源：http://3g.sjlbkw.cn/Article/details/gxpdyhfmz.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gkofkculv.sHtML

Java: static void f() {}
来源：http://read.share.tarul.cn/Article/details/guvimmrvf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/goyheigmj.sHtML

Ruby: def self.f; end
来源：http://m.share.vehdjk.com/Article/details/gnmycccry.sHtML

C#:   public static void F() {}
来源：http://m.share.fktsv.cn/Article/details/gzldsohas.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.bbcook.cn/Article/details/glpdkukao.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.vehdjk.com/Article/details/glcnkkagk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.yfazqb.com/Article/details/gkvfbfvww.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.vehdjk.com/Article/details/ggxgbpcrk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gaijcdqaj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/givhtwxxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.yfazqb.com/Article/details/greqkdqmk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gnpacmtna.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.vehdjk.com/Article/details/gubmwqphx.sHtML

[G10] 访问控制
来源：http://m.share.tarul.cn/Article/details/guujlcedv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fktsv.cn/Article/details/ggwfbjtuo.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/ghzbqnhnv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fktsv.cn/Article/details/gvvjpqeur.sHtML

TS:   public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/gyijndxym.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.bbcook.cn/Article/details/grmewtipp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.tarul.cn/Article/details/gsongbacc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gduxhzkds.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.vehdjk.com/Article/details/gufasgtdz.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/glfdzjxyc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.yfazqb.com/Article/details/gvdasaidf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gytnwenag.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fktsv.cn/Article/details/giolcnxss.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.bbcook.cn/Article/details/gtfhlpizj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.tarul.cn/Article/details/gebbitqcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/ggukufdky.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gsnlxcueb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gwiuraoen.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gzjjjvcuj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fktsv.cn/Article/details/gpwccmrpz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.yfazqb.com/Article/details/gcsuvqqwh.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gzzkalydi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gynbphkxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fktsv.cn/Article/details/gtclqfksd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gpftjlidt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.sjlbkw.cn/Article/details/gfammbuek.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/ghrpqelye.sHtML

[G13] 判断对象类型
来源：http://mobile.vehdjk.com/Article/details/gdpbswvtd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gljkbqduj.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/guggjyipc.sHtML

JS:   u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/grdoceqxq.sHtML

TS:   u instanceof User
来源：http://wap.yfazqb.com/Article/details/gzeqgisxy.sHtML

Java: u instanceof User
来源：http://baike.sjlbkw.cn/Article/details/gsijiwlrx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.yfazqb.com/Article/details/gmunfkoip.sHtML

Ruby: u.is_a?(User)
来源：http://blog.bbcook.cn/Article/details/grjzzbxrr.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gkxgvergz.sHtML

[G14] 数据类 / record
来源：http://wap.tarul.cn/Article/details/glqhzemig.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gremmroie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.sjlbkw.cn/Article/details/ggagdnugi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.epnwcf.com/Article/details/ggmfyuyvf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gwmgbxjei.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gcmyeswha.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.vehdjk.com/Article/details/gyekkaeof.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.vehdjk.com/Article/details/gcttdrrxk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.epnwcf.com/Article/details/gybjhsmag.sHtML

[G15] 枚举
来源：http://3g.yfazqb.com/Article/details/gekehqzzm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/gogcswkow.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.yfazqb.com/Article/details/gtjvbbnbl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.epnwcf.com/Article/details/gssucivuk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.tarul.cn/Article/details/gdbbswryq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fktsv.cn/Article/details/groggvwyf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fktsv.cn/Article/details/gijsolodj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.epnwcf.com/Article/details/grgjggkjs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.tarul.cn/Article/details/gjqzbtols.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fktsv.cn/Article/details/gizgkaevh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.yfazqb.com/Article/details/gzkbqoflv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.bbcook.cn/Article/details/gzemnokqf.sHtML

JS:   Object.entries(obj)
来源：http://3g.bbcook.cn/Article/details/gglgvyzfk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/ghwlaatkr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.epnwcf.com/Article/details/ggionxxzb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.vehdjk.com/Article/details/ghygyseoa.sHtML

Ruby: obj.instance_variables
来源：http://mobile.vehdjk.com/Article/details/gxjfqngoq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/gyjnqitwx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqefukyab.sHtML

H. 异常与错误处理
来源：http://baike.yfazqb.com/Article/details/gzpguicup.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkbejtozy.sHtML

[H01] try / catch 基础
来源：http://wap.yfazqb.com/Article/details/gfqrgbdap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gvsvwvdic.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fktsv.cn/Article/details/gpatuuknm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gazxdaate.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gcqytqsyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.yfazqb.com/Article/details/gpcsoyzol.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.vehdjk.com/Article/details/gwsjkiuhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.epnwcf.com/Article/details/gxyqcevcb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.tarul.cn/Article/details/ghxcepzhz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.epnwcf.com/Article/details/gzqidicde.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fktsv.cn/Article/details/gyzkdqiah.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gvryhayba.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gqulmehmb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gllwruzie.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gqcvjunkm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.bbcook.cn/Article/details/ggnihlpqs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.bbcook.cn/Article/details/gpaxpjojy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/gexbgrryy.sHtML

[H03] 主动抛出异常
来源：http://blog.tarul.cn/Article/details/gexhdtauv.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.vehdjk.com/Article/details/gelfuzlrb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gnkijenyn.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.yfazqb.com/Article/details/gaaqijvxj.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.tarul.cn/Article/details/guoanjeax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.epnwcf.com/Article/details/gnbovbxur.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.tarul.cn/Article/details/gyczyvwcz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.epnwcf.com/Article/details/gfwgivejd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.yfazqb.com/Article/details/grusltyqq.sHtML

[H04] 自定义异常类型
来源：http://m.share.yfazqb.com/Article/details/guyewqsmm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.bbcook.cn/Article/details/gjgmuqcmk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.vehdjk.com/Article/details/gznqrkstj.sHtML

JS:   class MyError extends Error {}
来源：http://blog.vehdjk.com/Article/details/ggidnfjlo.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.vehdjk.com/Article/details/giqolnuiz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.bbcook.cn/Article/details/gximwzezg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.vehdjk.com/Article/details/gnvcgxrtq.sHtML


<!-- 参考信息 -->