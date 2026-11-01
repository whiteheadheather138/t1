代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gqqalkyxi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.epnwcf.com/Article/details/ggwxprjjd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gliauggzp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/grxvdipzr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/grbjwiweo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gdbqvlstm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gbokahgbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gteurjlyu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gjncmdigb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwxwkzwlk.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gsiydmaoj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdqixiofb.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gqiyauoxb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gltubftec.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/geecjqxpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gzttdnbna.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gispqksgu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gosnmozot.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/ghqwtzsmq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gmwujlvxq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gqarkqnns.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gvylngrto.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gncstjrie.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gaibzzzky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/guevrawtk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gisblcebc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gcswckgun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gpthtxihz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gkgfglyws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/grqordmwm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/gwkqtklle.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gvmchvdrj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gjaratinb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gkdvhfkns.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gsuziycic.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/grsqxnsbd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/grnfibvms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gjsenfmwu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/ggwnuxunp.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/gjzfzzcck.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/galxaoydt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gswssmucc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gsgmddduf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gdgcoinvk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/glwclhtvj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/gmvqlpgsc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gzzzednlq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.tarul.cn/Article/details/gsziqfdhn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gxuehpyfp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gzoebqgtp.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gdmpgqyyn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/ghwdtvvuq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gchfhtdfb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gckyozlgf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gryydcije.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpvqqslbc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gawvwmrcx.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gzeticxxp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzuukxrzu.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqwjrqsee.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/giquqjufb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gokkvhxlp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/ggvlnejsf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gahtqyknl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqxuoqfrh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gsvltmrxn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gnufudxdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gegjfcwbe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/gyumxoado.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gklrzlozm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gfjhvzyrq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gmedftfja.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/gpywicegc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.sjlbkw.cn/Article/details/gwtbbgtee.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gtxhfspbd.sHtML

[F08] 遍历目录
来源：http://mobile.bbcook.cn/Article/details/giolpgaft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gqkrbfrox.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/gjoqfncaq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/gstzfmbiy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gkpjpdxzf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gkowpuaao.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/goypsrpre.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/govbdgyix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.tarul.cn/Article/details/gptgjqbvu.sHtML

[F09] 获取文件大小
来源：http://wap.epnwcf.com/Article/details/gychqumqy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gfpeamssr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gshkrncqx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/griozprue.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.vehdjk.com/Article/details/gqgsrebxc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gdrpvbynk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gpsndtwwv.sHtML

Ruby: File.size("a.txt")
来源：http://wap.yfazqb.com/Article/details/giyzfnrym.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.sjlbkw.cn/Article/details/gsuebofto.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/gjraqynpr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzwptmqzn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.tarul.cn/Article/details/gustlgiuv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gxxqwoyov.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwcvgmnbn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.sjlbkw.cn/Article/details/gqebkrkgl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtzjqxruu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gpwcepsil.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gllecxnmm.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gikaigjom.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvofvwlpn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gkrssutsa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/giknaagef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gakiueomr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/gkpvojrue.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gnpagxiwb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghdyflpjh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.vehdjk.com/Article/details/gdsflhiqw.sHtML

[F12] CSV 读写
来源：http://www.blog.vehdjk.com/Article/details/gojwrsvkg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.vehdjk.com/Article/details/gynefrggz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.tarul.cn/Article/details/gnnilmiqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gsizcrjuq.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/ghpkrcaat.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/grqfjbhxr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gqmwesoit.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gmaiqvogn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gxgysnflt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcuaiqtwj.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/gqxzuifag.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwvyhonhd.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gnpaoidpr.sHtML

Py:   class User: pass
来源：http://wap.vehdjk.com/Article/details/gkyeqqjfc.sHtML

PHP:  class User {}
来源：http://read.share.vehdjk.com/Article/details/gktspcnww.sHtML

JS:   class User {}
来源：http://3g.tarul.cn/Article/details/gvzbmasek.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gwkfbfnko.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/grgddrwnd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gwfplffjc.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gfaweleim.sHtML

C#:   class User {}
来源：http://baike.tarul.cn/Article/details/gbsmazxqj.sHtML

[G02] 构造函数
来源：http://blog.tarul.cn/Article/details/gbdynuxpo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.yfazqb.com/Article/details/gmpvinnyx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/goxyhjhgv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gehmejrwe.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.yfazqb.com/Article/details/grrqvedjj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gkyhnmtdp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gehadqcrw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fktsv.cn/Article/details/gegfdlkrf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.bbcook.cn/Article/details/gzchgnonm.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/goxeqdjer.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gaxgcxlng.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/ggspmmjzx.sHtML

JS:   this.name = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gxfmsojci.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gaomlpwnr.sHtML

Java: private String name;
来源：http://baike.vehdjk.com/Article/details/giuhwsnzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/goymyyfcg.sHtML

Ruby: @name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gsjkkfayu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/grmzdobsz.sHtML

[G04] 定义方法
来源：http://wap.tarul.cn/Article/details/gbnpekrkz.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gsdyiqehy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/gjrwmdozo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gulbssitl.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gyfuxlvbw.sHtML

Java: String greet() { return name; }
来源：http://m.share.epnwcf.com/Article/details/gdahfnolu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gceogauqa.sHtML

Ruby: def greet; @name; end
来源：http://m.share.bbcook.cn/Article/details/ghxszxpmk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/gmqnnmghr.sHtML

[G05] 继承
来源：http://wap.sjlbkw.cn/Article/details/gwpnfpufs.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/govlhztgf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gzpikjaya.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gozdopgxt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.bbcook.cn/Article/details/grxkuaviw.sHtML

Java: class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gwwgbpcel.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gfraeombo.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gkxhmatde.sHtML

C#:   class Admin : User {}
来源：http://www.share.fktsv.cn/Article/details/gcpjvslia.sHtML

[G06] 重写方法
来源：http://wap.tarul.cn/Article/details/gzsjbfnht.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.yfazqb.com/Article/details/gjlfslffs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gjngnntnr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gugczfulj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fktsv.cn/Article/details/gaujsbwqr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/gojujnpza.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/ghvjnvuak.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/ghsnbzqxv.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.epnwcf.com/Article/details/ggaronsyu.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gvkxycezi.sHtML

Py:   super().greet()
来源：http://www.share.fktsv.cn/Article/details/ghyzjjtev.sHtML

PHP:  parent::greet();
来源：http://www.m.share.bbcook.cn/Article/details/gkjripssd.sHtML

JS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gbwpesuqe.sHtML

TS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gankyyigy.sHtML

Java: super.greet();
来源：http://m.share.fktsv.cn/Article/details/grjihcssu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.bbcook.cn/Article/details/gfjkksfhh.sHtML

Ruby: super
来源：http://mobile.sjlbkw.cn/Article/details/guqkkihfy.sHtML

C#:   base.Greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gdxpflhfa.sHtML

[G08] 静态方法与属性
来源：http://wap.vehdjk.com/Article/details/gmuwepccj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/gaaigcpqo.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gafnwrwdw.sHtML

JS:   static f() {}
来源：http://read.share.epnwcf.com/Article/details/gcrhutewv.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gmklfodhz.sHtML

Java: static void f() {}
来源：http://www.blog.vehdjk.com/Article/details/gxtlzmejx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/gveiftaki.sHtML

Ruby: def self.f; end
来源：http://wap.epnwcf.com/Article/details/gullamsel.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gnrgvjcsf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.vehdjk.com/Article/details/gomnlhxfa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/ghcxmgfwu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fktsv.cn/Article/details/grbpdryda.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fktsv.cn/Article/details/gcbqtbuql.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gctfqitrp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.yfazqb.com/Article/details/goxwyzzvz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fktsv.cn/Article/details/gsojeufwk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fktsv.cn/Article/details/gzsizqsxm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.yfazqb.com/Article/details/gwpugchkh.sHtML

[G10] 访问控制
来源：http://baike.epnwcf.com/Article/details/gfilwtxad.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.vehdjk.com/Article/details/gaqhhsgvh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/ghujezstz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.vehdjk.com/Article/details/gwqfzjpmf.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gitviyqfb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlxpmuel.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.tarul.cn/Article/details/gpfnvghpi.sHtML

Ruby: public / protected / private
来源：http://3g.tarul.cn/Article/details/gfibzuowy.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gmrncqbry.sHtML

[G11] getter / setter
来源：http://3g.fktsv.cn/Article/details/gthfjwxkx.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gfelgecwi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gwpojfmtc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fktsv.cn/Article/details/grhqxmata.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.tarul.cn/Article/details/gljxlincd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmusmomh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/gjdbsbjxj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.sjlbkw.cn/Article/details/gsqdvwmya.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.tarul.cn/Article/details/gycfjywbj.sHtML

[G12] 对象转字符串
来源：http://mobile.epnwcf.com/Article/details/ggmxkrkao.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gokprniiw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fktsv.cn/Article/details/gvdgkayna.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/gojftvpun.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/galnrtbmv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/gwvjfkzor.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.bbcook.cn/Article/details/gcxvcvjgk.sHtML

Ruby: def to_s; @name; end
来源：http://baike.tarul.cn/Article/details/gtwhyjbxa.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/guzzfdtnj.sHtML

[G13] 判断对象类型
来源：http://www.blog.bbcook.cn/Article/details/gdkcxaebe.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fktsv.cn/Article/details/gzdogsusl.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fktsv.cn/Article/details/gjpybiyat.sHtML

JS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gdntsguun.sHtML

TS:   u instanceof User
来源：http://mobile.epnwcf.com/Article/details/gagovumjs.sHtML

Java: u instanceof User
来源：http://wap.fktsv.cn/Article/details/ggclerafo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/gyolcpuqh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.tarul.cn/Article/details/gdmseuqgh.sHtML

C#:   u is User
来源：http://wap.fktsv.cn/Article/details/gjrqumyad.sHtML

[G14] 数据类 / record
来源：http://www.share.tarul.cn/Article/details/gwkunzlog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.tarul.cn/Article/details/gqiaaneim.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gjszfyrni.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.bbcook.cn/Article/details/gsqvuwqvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.yfazqb.com/Article/details/gnnmcuhai.sHtML

Java: record User(String name, int age) {}
来源：http://3g.tarul.cn/Article/details/gvlmmbahu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.sjlbkw.cn/Article/details/gamtnvhmq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.vehdjk.com/Article/details/guldlvxka.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.tarul.cn/Article/details/gwcxlupfn.sHtML

[G15] 枚举
来源：http://read.share.bbcook.cn/Article/details/gtdaclncq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.sjlbkw.cn/Article/details/gobblhazg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gptfpctji.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.vehdjk.com/Article/details/gnnzqqjem.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.sjlbkw.cn/Article/details/gxcsxqqkm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.epnwcf.com/Article/details/gsvymwvbl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.bbcook.cn/Article/details/gmqxwbtic.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gokcdqvmd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/godzedgxj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.yfazqb.com/Article/details/gwwvyvewy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.epnwcf.com/Article/details/ghtfrajoh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gmmiztejf.sHtML

JS:   Object.entries(obj)
来源：http://3g.vehdjk.com/Article/details/gokaxhxpf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fktsv.cn/Article/details/gyzzsuvnk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.yfazqb.com/Article/details/gbagbopep.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.yfazqb.com/Article/details/gtfcjwbsk.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gurjosovg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gtspfgyfd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdgutfbvl.sHtML

H. 异常与错误处理
来源：http://baike.sjlbkw.cn/Article/details/gxnkkrzzv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gauldbimt.sHtML

[H01] try / catch 基础
来源：http://3g.vehdjk.com/Article/details/gwmcvwxzj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.yfazqb.com/Article/details/ghlfwatjp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fktsv.cn/Article/details/grqtoxtpg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmshgfhf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gojwxtjdc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.vehdjk.com/Article/details/glylvdnlw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fktsv.cn/Article/details/gvibvxijm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gsegkjgox.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.sjlbkw.cn/Article/details/gjviojxlw.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.tarul.cn/Article/details/geffnayah.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.bbcook.cn/Article/details/gpivxvbfw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.epnwcf.com/Article/details/gavestwyi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdnzidlzw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.tarul.cn/Article/details/gtrpyhcup.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.bbcook.cn/Article/details/gxvcvpxax.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.epnwcf.com/Article/details/gmbdadomz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.yfazqb.com/Article/details/gbjdejkgk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gwxavmdbi.sHtML

[H03] 主动抛出异常
来源：http://mobile.bbcook.cn/Article/details/gnepcfsvx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.bbcook.cn/Article/details/grcwufbxs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.tarul.cn/Article/details/gyevwuvam.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fktsv.cn/Article/details/ghczzmsxv.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.vehdjk.com/Article/details/gmplmmidn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/ghryizdly.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.yfazqb.com/Article/details/gsnlazzjt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.sjlbkw.cn/Article/details/gjxvctgum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gmqedxjfm.sHtML

[H04] 自定义异常类型
来源：http://3g.fktsv.cn/Article/details/gnabrjxdo.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.epnwcf.com/Article/details/gemfvrshf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.tarul.cn/Article/details/gfusavlpy.sHtML


<!-- 参考信息 -->