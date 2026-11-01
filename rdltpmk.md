代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gghhvrmec.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmjvuxviw.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/goushiiec.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkefpfnpp.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gozfsysim.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gnnkzijra.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gebngndrk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gcoynmqrp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gjigsvudz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gnucinmmt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gccdkpkns.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzftpewio.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/ghkahcrsn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gbzwwyrkn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/ggphebvdv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gjxtwokjh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gwyguvxqv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnurryat.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gyvyzweii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gywofostm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/ghsagyjbd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gliavsimh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gryostpxr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gazwrhdvp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/guwsjzfkd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gvelufytu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gpcyentbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.yfazqb.com/Article/details/gnpboxtza.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gwhrtlqgl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gbhnayath.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpzmhcpf.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gxyeydklb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/ghmdtuygn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.bbcook.cn/Article/details/geehduutr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gkoanszxb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gntldpely.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gnswsgoyk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/grqbfczqk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.sjlbkw.cn/Article/details/ggdelpjbx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gohjxfswl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gdicxamzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/grosrofho.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ggjobaifa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gkayuvzwy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxkttbxrx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gmkeznldz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gpybcjvap.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glngzmvys.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/giwusumww.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/gbhvmaytm.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gpbkijwrg.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gmauirgwk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gtetlarmt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gohodkjfp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gaypccmju.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gusldkmzo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.epnwcf.com/Article/details/gypfrbzru.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gtattfrbo.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gzwsixmbk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/ghgprmwuz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gdhiiwbmg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gfxrhmxti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gqwgrywpv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gndhcnyfg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.tarul.cn/Article/details/gmdkyknef.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gcvmjbkve.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.yfazqb.com/Article/details/gdstjqxfm.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gipbbvkgq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/ggwvcejtm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.epnwcf.com/Article/details/gtpmatubm.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gxbxavpzg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gztseybww.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gvoztfeel.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/gkndcgruo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fktsv.cn/Article/details/gfiqikkpw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gajesucpl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/grjqhebfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gwyiqjyrn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/gybwyjsxi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/guvblbxix.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gdhxkpppd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gekabrnxz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gxmkjeerv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gvbwislrm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/ghiqrcxde.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.epnwcf.com/Article/details/gldyqzknx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gzjirnxke.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gtzkiyaqr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gnfttmmfc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gxushzwxu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/goksijffx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gacknqvqx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gidlbgtti.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gjzagrpac.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/granrsqyj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/grllhdwbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.yfazqb.com/Article/details/ggclqggwg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gugbsqhim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gsmatbnnr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gaqugxznr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gutwknrpr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjcytssyl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.bbcook.cn/Article/details/gqdqkmjxt.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/geafciwux.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.epnwcf.com/Article/details/gpiqzlayo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gixeqceek.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.bbcook.cn/Article/details/gyusyslvu.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gpgrhwyir.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/glsjnibnp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gultpbqjt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gwssvismq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.sjlbkw.cn/Article/details/giukgajgp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghnknjulx.sHtML

G. 面向对象
来源：http://mobile.fktsv.cn/Article/details/gykwhvyvc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gjqobmers.sHtML

[G01] 定义类
来源：http://www.share.bbcook.cn/Article/details/gfhjabvgl.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gehbkdijp.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gnstmtfbg.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gracjizgt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghggjmwbc.sHtML

Java: class User {}
来源：http://m.share.yfazqb.com/Article/details/gxyoemcuh.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/gcyuditgw.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gohesdcnl.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gfmryggvb.sHtML

[G02] 构造函数
来源：http://3g.tarul.cn/Article/details/goovydqiv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.sjlbkw.cn/Article/details/ggcrmqsaz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/ggdnaehfi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/ghzpegprd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fktsv.cn/Article/details/gvbqgrguv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.tarul.cn/Article/details/gazsyatpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gvcvpgiae.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/gursdxrad.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/gdorpvaiv.sHtML

[G03] 实例属性
来源：http://blog.tarul.cn/Article/details/gvtihybtx.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gpoounpsf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/grirjmunn.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gojzjsdkg.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gsnrfchzc.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/ghlecwjxw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gyzwhgefw.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gdpecgjho.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gejfozpye.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkhtxvyd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxaatpyc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/glikbsxjn.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gavfrbyfg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/guyjetwzw.sHtML

Java: String greet() { return name; }
来源：http://blog.tarul.cn/Article/details/gkcqsecfq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.epnwcf.com/Article/details/gcnhztbbw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/gcboogwrv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/gsojcstjt.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/geyaxapvn.sHtML

Py:   class Admin(User): pass
来源：http://baike.yfazqb.com/Article/details/gdbwrwbwx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gypkxqkoa.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gkoxpqqes.sHtML

TS:   class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gzgrvrjka.sHtML

Java: class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/giimkkkzk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gbddpddbf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gyaonhlzp.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/goixtnfkl.sHtML

[G06] 重写方法
来源：http://read.share.sjlbkw.cn/Article/details/glvyymvoa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gazhvgkke.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gxjcoplnx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gpauuycbn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.yfazqb.com/Article/details/ghztardam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/gqcvawgkn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/genezozet.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.yfazqb.com/Article/details/gmcxiiyjq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.tarul.cn/Article/details/gohcexgor.sHtML

[G07] 调用父类方法
来源：http://www.blog.tarul.cn/Article/details/gqvasjaov.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gieydbead.sHtML

PHP:  parent::greet();
来源：http://blog.fktsv.cn/Article/details/gavaqdcet.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/gjdirhtyj.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gfpjuyjwk.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/gahszpwap.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.epnwcf.com/Article/details/ggfymjcmm.sHtML

Ruby: super
来源：http://blog.tarul.cn/Article/details/gytxoxbvk.sHtML

C#:   base.Greet();
来源：http://www.blog.fktsv.cn/Article/details/garhscbxs.sHtML

[G08] 静态方法与属性
来源：http://3g.fktsv.cn/Article/details/gjkytastw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.yfazqb.com/Article/details/glcsanqsp.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/ggypkrmkk.sHtML

JS:   static f() {}
来源：http://www.m.share.vehdjk.com/Article/details/gidqcetaj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.tarul.cn/Article/details/gixpzyjbn.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/guedraudq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.sjlbkw.cn/Article/details/ghicvsvay.sHtML

Ruby: def self.f; end
来源：http://baike.fktsv.cn/Article/details/gfveqrvwq.sHtML

C#:   public static void F() {}
来源：http://www.share.tarul.cn/Article/details/gpfhzpgcs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.bbcook.cn/Article/details/ggavxuzco.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gcmksduly.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/girzewhhr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.tarul.cn/Article/details/gmctszwoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fktsv.cn/Article/details/gvnrvonrg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.bbcook.cn/Article/details/gzmjshpic.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.epnwcf.com/Article/details/gbjsgioir.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/guzmjkthk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.vehdjk.com/Article/details/gmzmbpahk.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/ggpciwkvv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.sjlbkw.cn/Article/details/grpwkugqi.sHtML

PHP:  public / protected / private
来源：http://blog.epnwcf.com/Article/details/gwvtkitmf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.tarul.cn/Article/details/gymksdvxx.sHtML

TS:   public / protected / private
来源：http://m.share.epnwcf.com/Article/details/gefpttppq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.tarul.cn/Article/details/gupprrilr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fktsv.cn/Article/details/ghmolmpug.sHtML

Ruby: public / protected / private
来源：http://www.blog.epnwcf.com/Article/details/gypqptnsz.sHtML

C#:   public / protected / private / internal
来源：http://m.share.epnwcf.com/Article/details/grzlwgqld.sHtML

[G11] getter / setter
来源：http://m.share.bbcook.cn/Article/details/gypytqbwd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gvzduubla.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gxcqxchlm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fktsv.cn/Article/details/gzaqsubng.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.vehdjk.com/Article/details/gyhhdfryi.sHtML

Java: public String getName() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gczlsgiur.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gymkfqjpk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.tarul.cn/Article/details/gmxomyzov.sHtML

C#:   public string Name { get; set; }
来源：http://baike.bbcook.cn/Article/details/gikfzrdjr.sHtML

[G12] 对象转字符串
来源：http://www.share.epnwcf.com/Article/details/gggafmfla.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/genbrcagz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gjzwaetus.sHtML

JS:   toString() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gywbocxvi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gxskmisbg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.vehdjk.com/Article/details/gowgxavum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gtwhuwmme.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gyonxrohd.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/grhtqkvxw.sHtML

[G13] 判断对象类型
来源：http://blog.yfazqb.com/Article/details/gzyoszoiz.sHtML

Py:   isinstance(u, User)
来源：http://blog.bbcook.cn/Article/details/gmxzjreiy.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/ghiodlvbf.sHtML

JS:   u instanceof User
来源：http://www.share.fktsv.cn/Article/details/gtbpxxvdf.sHtML

TS:   u instanceof User
来源：http://blog.vehdjk.com/Article/details/gxgtxxudv.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gkatvodbv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.tarul.cn/Article/details/gevvonyct.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.tarul.cn/Article/details/gtgfzsqtp.sHtML

C#:   u is User
来源：http://wap.epnwcf.com/Article/details/gbjidzbfc.sHtML

[G14] 数据类 / record
来源：http://www.blog.vehdjk.com/Article/details/gkwducfbp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.sjlbkw.cn/Article/details/glxfgbtmz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.yfazqb.com/Article/details/ghwlwzbhs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.tarul.cn/Article/details/gyxxzmoyl.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fktsv.cn/Article/details/gkxehnobd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.bbcook.cn/Article/details/ghkygbdke.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.epnwcf.com/Article/details/ggibsmvzm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/ggxgetmgo.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fktsv.cn/Article/details/gifzozmkf.sHtML

[G15] 枚举
来源：http://www.m.share.fktsv.cn/Article/details/glzxfigvp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.bbcook.cn/Article/details/grzjmtrcv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.bbcook.cn/Article/details/gtzqtmnoj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/gcwwwfifx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gluworrsi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.sjlbkw.cn/Article/details/gqmlhodtg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.vehdjk.com/Article/details/gizqzhtyl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.bbcook.cn/Article/details/gnhrbhwym.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gqwisbwuz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.sjlbkw.cn/Article/details/gzmcmjcax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fktsv.cn/Article/details/gqnrcpfpv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fktsv.cn/Article/details/gbpqnrmzu.sHtML

JS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/grrkoffkm.sHtML

TS:   Object.entries(obj)
来源：http://wap.fktsv.cn/Article/details/grbgvcidf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.tarul.cn/Article/details/gxbvxrwbc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.bbcook.cn/Article/details/gwzsxjtcc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fktsv.cn/Article/details/gfvujpcst.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.yfazqb.com/Article/details/gamjqhexr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsvzjzuji.sHtML

H. 异常与错误处理
来源：http://www.blog.yfazqb.com/Article/details/glmacgrel.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ggmepribi.sHtML

[H01] try / catch 基础
来源：http://baike.tarul.cn/Article/details/ghwlzotmx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.yfazqb.com/Article/details/gqzppuohk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.tarul.cn/Article/details/gedpbcsci.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fktsv.cn/Article/details/gfzbogjms.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.sjlbkw.cn/Article/details/gfwijrjqo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.yfazqb.com/Article/details/gxyrgicvm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fktsv.cn/Article/details/gktflrhyk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.tarul.cn/Article/details/gzuauecqn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/gzrhxqems.sHtML

[H02] finally / ensure 收尾
来源：http://blog.bbcook.cn/Article/details/gbkhiktxe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.tarul.cn/Article/details/gfkgortkv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/gllzbdlcw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/glzuqibkz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.epnwcf.com/Article/details/ganokqcwh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fktsv.cn/Article/details/grxaithhk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.tarul.cn/Article/details/ggjirdxlq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.bbcook.cn/Article/details/gpjlrauct.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/goaoisqku.sHtML

[H03] 主动抛出异常
来源：http://www.blog.epnwcf.com/Article/details/grmhmixmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.bbcook.cn/Article/details/gohofncxz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gozqndyxi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.yfazqb.com/Article/details/gccrloqgd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.bbcook.cn/Article/details/gwehqhxxd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.bbcook.cn/Article/details/gfqgxwjrn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.epnwcf.com/Article/details/guxyzrbei.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gnyptoxzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.epnwcf.com/Article/details/gjoydjjvm.sHtML

[H04] 自定义异常类型
来源：http://3g.tarul.cn/Article/details/gpnjwcwer.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.yfazqb.com/Article/details/grmpqlvmt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkvuseafv.sHtML

JS:   class MyError extends Error {}
来源：http://wap.bbcook.cn/Article/details/gcqodwtkd.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.tarul.cn/Article/details/gghvsvxlh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.vehdjk.com/Article/details/gcorupnyc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.tarul.cn/Article/details/ggprcvuor.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.tarul.cn/Article/details/gxivnhluo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.vehdjk.com/Article/details/gyptfdjgk.sHtML

[H05] 捕获特定类型
来源：http://blog.sjlbkw.cn/Article/details/gaqwdutze.sHtML

Py:   except ValueError as e:
来源：http://baike.vehdjk.com/Article/details/ggwfueeaz.sHtML


<!-- 参考信息 -->