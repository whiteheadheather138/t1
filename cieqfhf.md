代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/guharssek.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtkentqwx.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gstujbmqj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grtdrvaou.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gavmeohfr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/grdeekdry.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gywliylpt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gehqecrby.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/ghlofzvdt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/grmvoiqdq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gxfrwxocb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/gemgnzisa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwybuqern.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gzthcnbzw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gpcxjavag.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/gqnzbaevf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gtibuagla.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gyhwclgoz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gnsdpztca.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gswclgxnd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.epnwcf.com/Article/details/gcrhziwue.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gvxdbqvhm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.yfazqb.com/Article/details/grvxzzcfg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gnddwpibt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gagyvpwuq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/glaksthcr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gzkjtlsia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gcsmagwra.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gydrrytro.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gsyktmslh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gopaoxsnt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gpkeauigb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gldnlegjf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/ghuggvned.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/grhryaobj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gzfhxqvwn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gbtrmrxwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gjiaxapva.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gygmltldp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gnkygwgnj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.epnwcf.com/Article/details/gprhkzujl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gdywudahg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gskwpnanu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gongkxati.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxshddqzl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gllsansxd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gpscklxim.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gfjonpist.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gycmxttqi.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gdbwfojen.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/glrzkqvsr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gydbbcjpw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzxaekdgh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gbxrxibzy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/ghpdgbwro.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.yfazqb.com/Article/details/goudmaaeu.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvcloddub.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gfqesdoga.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gpciicmsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.vehdjk.com/Article/details/gccvqkvxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnipzwvvo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gbprzqbhf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gdnsfzbqf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gztnpjwph.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/ghxxdsohy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/ghtanydoo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.epnwcf.com/Article/details/gsotudoug.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gkvbxnqru.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gzzwuvryt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gryafqdhl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gyfbpmrkj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gbvpgfxiy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gdganunjw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fktsv.cn/Article/details/gmeqtbiph.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/grmgclqbv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/guypcrvha.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gcrmbmlla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gypuepsua.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gxbmqzljj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gpanbqumd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gokazzlgz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gjgdupjtc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fktsv.cn/Article/details/ggrmtxady.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvnmiswfc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.sjlbkw.cn/Article/details/ghnvkqrci.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gerqlnrbe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghlwdjdzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/graxiqcgf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfudmdorl.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gvrpjhxxe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gwbogouar.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gefgszjcb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/getobevmr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gytnbvdkm.sHtML

[F11] 复制与移动文件
来源：http://m.share.epnwcf.com/Article/details/giteyazaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gbzwdujlv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.sjlbkw.cn/Article/details/gnokzobso.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/grxcnqrgp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvkrccsca.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.vehdjk.com/Article/details/gkwpdjged.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gkdiprcic.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gvffrleke.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gxsjtbuqi.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/goeffepdb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gdffmfzeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/grhbtbimn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gobvnqvzd.sHtML

TS:   // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gsmgpqfru.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gzjeziqqs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fktsv.cn/Article/details/gjeidsrdf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.epnwcf.com/Article/details/gyjhuyijh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/getxkrgbs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjnhuupnq.sHtML

G. 面向对象
来源：http://wap.yfazqb.com/Article/details/gmdxtxswb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gknisvumt.sHtML

[G01] 定义类
来源：http://wap.fktsv.cn/Article/details/ghqfvkvhy.sHtML

Py:   class User: pass
来源：http://www.blog.yfazqb.com/Article/details/gtsoqjkgd.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gfikmlmax.sHtML

JS:   class User {}
来源：http://wap.fktsv.cn/Article/details/gyyftzpkg.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gczetvxfv.sHtML

Java: class User {}
来源：http://3g.epnwcf.com/Article/details/gpuftvath.sHtML

Go:   type User struct { Name string }
来源：http://read.share.yfazqb.com/Article/details/gtegcccnn.sHtML

Ruby: class User; end
来源：http://3g.bbcook.cn/Article/details/gchcftopv.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gohusphyv.sHtML

[G02] 构造函数
来源：http://www.share.vehdjk.com/Article/details/goyedymqt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.tarul.cn/Article/details/gecojbkic.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gmxqsjalk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gllifbqtt.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gipdfyqej.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.tarul.cn/Article/details/giebucmxf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gfwhtmmmr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gdkxgvvru.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.yfazqb.com/Article/details/gcutlngas.sHtML

[G03] 实例属性
来源：http://baike.vehdjk.com/Article/details/gztabzpye.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gujakpdnx.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/ghkzhqsre.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gjberrzlq.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gxxiyshlc.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/ggmsdkdod.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/galtcsdzr.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/ggqvghppa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.sjlbkw.cn/Article/details/guhdykbmn.sHtML

[G04] 定义方法
来源：http://mobile.tarul.cn/Article/details/gxzidjfdh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gokakbdsx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gteaunvvh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/gwfjsotpd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.bbcook.cn/Article/details/gshybajjm.sHtML

Java: String greet() { return name; }
来源：http://wap.vehdjk.com/Article/details/gwzoqpvwn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gfrpfrrxm.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gpkpbyvue.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.epnwcf.com/Article/details/gebamqzfa.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gvtuwnpbs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.vehdjk.com/Article/details/gugvlxyna.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gubhoinoq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/grckwdiyu.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gtzdmafzr.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gqbmqghni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gtglebhmm.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gzoulufsn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gmwgqmsau.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gyutlcsvx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.yfazqb.com/Article/details/ghlquhyjx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gniepmqhs.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gghewqdit.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gkqhejwjg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gxyxuyush.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.yfazqb.com/Article/details/girctnarc.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.tarul.cn/Article/details/gdrxanyfy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.bbcook.cn/Article/details/glxhjggjv.sHtML

[G07] 调用父类方法
来源：http://wap.bbcook.cn/Article/details/gssmcgnom.sHtML

Py:   super().greet()
来源：http://read.share.epnwcf.com/Article/details/gruwppmgb.sHtML

PHP:  parent::greet();
来源：http://www.blog.bbcook.cn/Article/details/gliaalptl.sHtML

JS:   super.greet();
来源：http://wap.sjlbkw.cn/Article/details/gamnxhdyd.sHtML

TS:   super.greet();
来源：http://m.share.bbcook.cn/Article/details/gnlbpavng.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gbzngpptp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/ggonstuhd.sHtML

Ruby: super
来源：http://wap.sjlbkw.cn/Article/details/gpfufhelh.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gqxydsvyy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gilvhmrsv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.bbcook.cn/Article/details/giueawdjm.sHtML

PHP:  public static function f() {}
来源：http://mobile.fktsv.cn/Article/details/ghhmyngan.sHtML

JS:   static f() {}
来源：http://www.m.share.yfazqb.com/Article/details/gmzjoseau.sHtML

TS:   static f(): void {}
来源：http://mobile.tarul.cn/Article/details/gfgallxme.sHtML

Java: static void f() {}
来源：http://read.share.vehdjk.com/Article/details/gnefwqkxa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.vehdjk.com/Article/details/gogsrwjlq.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gowqapklt.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gzwfqokzb.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fktsv.cn/Article/details/gnrjyayzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.epnwcf.com/Article/details/gibginosj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fktsv.cn/Article/details/gsacrqmzt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gegbqrkxs.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fktsv.cn/Article/details/goooudkwk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.yfazqb.com/Article/details/glqwaqwvs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.sjlbkw.cn/Article/details/goijehtcu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.vehdjk.com/Article/details/gpshhvdek.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.bbcook.cn/Article/details/gxozwzzln.sHtML

[G10] 访问控制
来源：http://m.share.fktsv.cn/Article/details/gqxgaicfl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.epnwcf.com/Article/details/gqxpmllvh.sHtML

PHP:  public / protected / private
来源：http://www.share.yfazqb.com/Article/details/gqrarjpnn.sHtML

JS:   #private 字段；其余公开
来源：http://baike.sjlbkw.cn/Article/details/guhtwmxcy.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gtlkcezmz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.yfazqb.com/Article/details/gktlfaujf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.sjlbkw.cn/Article/details/gsqkhcklc.sHtML

Ruby: public / protected / private
来源：http://baike.tarul.cn/Article/details/gdbucesps.sHtML

C#:   public / protected / private / internal
来源：http://wap.epnwcf.com/Article/details/ghwuiaowk.sHtML

[G11] getter / setter
来源：http://www.blog.epnwcf.com/Article/details/ggtgxajpg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gzjxaihcv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gzwwucokp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fktsv.cn/Article/details/gljcaifpt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/ganwwlbxx.sHtML

Java: public String getName() { return name; }
来源：http://3g.bbcook.cn/Article/details/gcobhssjw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gqigdwaea.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gyfulgpbc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gmnbgeiwk.sHtML

[G12] 对象转字符串
来源：http://m.share.bbcook.cn/Article/details/gdgixlfbn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gretynmgz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fktsv.cn/Article/details/gnqwkrpqf.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gfigsxdel.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gkxukjoyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.bbcook.cn/Article/details/gmmtihxcp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.yfazqb.com/Article/details/gvkfnrhhh.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gnmpjtlpt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.yfazqb.com/Article/details/gsxhtcygu.sHtML

[G13] 判断对象类型
来源：http://www.share.epnwcf.com/Article/details/gbkhmlumm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.vehdjk.com/Article/details/ghkzashue.sHtML

PHP:  $u instanceof User
来源：http://blog.yfazqb.com/Article/details/gwzedupwo.sHtML

JS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gtjyjqjhk.sHtML

TS:   u instanceof User
来源：http://mobile.yfazqb.com/Article/details/gjoairzli.sHtML

Java: u instanceof User
来源：http://www.m.share.tarul.cn/Article/details/gottxoqdk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gpxkswiil.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.epnwcf.com/Article/details/gyudnjwpd.sHtML

C#:   u is User
来源：http://www.share.bbcook.cn/Article/details/gxqkcicqk.sHtML

[G14] 数据类 / record
来源：http://m.share.tarul.cn/Article/details/gghyhrqys.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/grvzlmfsp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fktsv.cn/Article/details/gkvmcwehp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.sjlbkw.cn/Article/details/gehimnufp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fktsv.cn/Article/details/gsdldtpam.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fktsv.cn/Article/details/geccnfvoz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.bbcook.cn/Article/details/gohahiosd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gphdfaqtj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.epnwcf.com/Article/details/gmlcdolpv.sHtML

[G15] 枚举
来源：http://www.share.vehdjk.com/Article/details/gxtewicfy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcxmuocc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/ghgfsiauv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.yfazqb.com/Article/details/gxnalblez.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.sjlbkw.cn/Article/details/ggwvpcawk.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.vehdjk.com/Article/details/ghxeonpxh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyzdsbse.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/gcfpiuyso.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.vehdjk.com/Article/details/gqapivpwt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.vehdjk.com/Article/details/gsltdikws.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.tarul.cn/Article/details/gcxazcumc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.tarul.cn/Article/details/ghinvzkiz.sHtML

JS:   Object.entries(obj)
来源：http://wap.tarul.cn/Article/details/gbqhaopmv.sHtML

TS:   Object.entries(obj)
来源：http://m.share.tarul.cn/Article/details/gpsfvpxsa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.sjlbkw.cn/Article/details/gtiqybtwr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gbtihfrdd.sHtML

Ruby: obj.instance_variables
来源：http://blog.yfazqb.com/Article/details/gosuvqgbv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fktsv.cn/Article/details/gkbcgbgmc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gseanfbji.sHtML

H. 异常与错误处理
来源：http://wap.bbcook.cn/Article/details/gwxugcswr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gttrdfsrr.sHtML

[H01] try / catch 基础
来源：http://3g.sjlbkw.cn/Article/details/gywtdshuo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.sjlbkw.cn/Article/details/gijykbgzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.sjlbkw.cn/Article/details/gglauoooe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gpunprlmr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gegfwtlif.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gkethggws.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gxuhkptqy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.tarul.cn/Article/details/gysczabrn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.bbcook.cn/Article/details/gbqvomnyb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.epnwcf.com/Article/details/gdsmvhvya.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.epnwcf.com/Article/details/gdknmkwoq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gaqebaaeg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gojxdkmqm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gwmidpbiq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.yfazqb.com/Article/details/gqddazwnx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/ghdujldez.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fktsv.cn/Article/details/gbkcxtjxq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/ggagqheca.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/ghoheyxjo.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.sjlbkw.cn/Article/details/gxcncocei.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gfcyfpcys.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.tarul.cn/Article/details/gdktxxbpl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.tarul.cn/Article/details/grgxwhwpi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fktsv.cn/Article/details/glsxbkbfk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.epnwcf.com/Article/details/givkjucvi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.tarul.cn/Article/details/getkoxqyq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gvltmioqx.sHtML

[H04] 自定义异常类型
来源：http://wap.fktsv.cn/Article/details/gywocdvay.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.yfazqb.com/Article/details/gzmbohcqh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.sjlbkw.cn/Article/details/gbttzntpe.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fktsv.cn/Article/details/gbgtenpkf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.tarul.cn/Article/details/gpjdowmjn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.tarul.cn/Article/details/gchhfurza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.yfazqb.com/Article/details/guxowpvjb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.epnwcf.com/Article/details/gmbudpsij.sHtML

C#:   class MyException : Exception {}
来源：http://wap.yfazqb.com/Article/details/grciwhogi.sHtML

[H05] 捕获特定类型
来源：http://mobile.fktsv.cn/Article/details/ggdiviggd.sHtML

Py:   except ValueError as e:
来源：http://www.share.sjlbkw.cn/Article/details/gayxxwbdv.sHtML


<!-- 参考信息 -->