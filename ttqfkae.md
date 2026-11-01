代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gyuiitxis.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/grsvdafzt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/ghudhsbpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gvevgcnkn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gabgterqi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gcmimsghw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbngtecf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gfmlcjvna.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/goxhzsxmo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gctbemoho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gizifhejb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/grvimtnfb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gdqcldunn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gfmzixnmz.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gdbtdjpqt.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gkpbuwkcm.sHtML

[F01] 读取整个文件
来源：http://m.share.epnwcf.com/Article/details/gufxhdqpd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gvjptrlwl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gvvjqgxds.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/grmgkxxql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/ggufbrrnv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/ghuzkjchv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gjpzatybh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmhxeusee.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/giahpeooc.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/guiywswfc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.sjlbkw.cn/Article/details/gpgokoryi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gtydyuwzw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gjdhttvhr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gczfyhucp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gvuafbrno.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.yfazqb.com/Article/details/gwswimmib.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/guydhodly.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/ggtfmtfsm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/ggcrgpxuc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.epnwcf.com/Article/details/gwszlwdud.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gkikejcmt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/goxcvxgdq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gouwhzoju.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gpmlesalo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fktsv.cn/Article/details/guccfazrs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gzloumnrt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gqpwponpt.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gnncmyobq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gvttxwupy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/geizfhzud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gfngxwqgg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/galwomoyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fktsv.cn/Article/details/gehqccgfi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/geokizknh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gqwtgpvab.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/giuazvtuk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.bbcook.cn/Article/details/gfqeexnkz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gmxvyxwfy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/grkjlufrd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gfrohfpjk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gdlssrzva.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/goqnyqkyl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/grpihsems.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ggqvfnoxm.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gdqxglzsi.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gwccrpllu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gshevuiik.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gdemxzhgc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtvxjrjqj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gclljrwmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gzrqdmrby.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gnebjtcnm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmwtkwkcq.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gvxmqfcqs.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gjajmfenm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gfgrwtajr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gthrlnbhy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gmamfyilx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/ghpuwzbdb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gsecmhqba.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.sjlbkw.cn/Article/details/gxznxdcxl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gsrgjvwgj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.yfazqb.com/Article/details/ggpmppvwl.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/giofcptod.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gxonlrodt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fktsv.cn/Article/details/gnkkqtesf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gznzepxla.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gqskzmpnq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gjqlcgqru.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.epnwcf.com/Article/details/giokiugff.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gmsvxlsew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gdqjyctwg.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/glseytgxw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcairammo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/ggylbxrjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/getgpvykz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/giftodfhr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gsvqszljk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gtnezogbv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gjyjfvgnx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gxxwuednl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gwjedxhxl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gtvmvqdeq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fktsv.cn/Article/details/gpkqbtzva.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/glhzrylro.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvwlhkkab.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gwbjxkkrj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gademaisf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/ggshfifiz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gymgyhoca.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/gjfhceplk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/ggitizgxu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/gkisoifnc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gftrpryps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggoewsnba.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gcduqkwzi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gljjcmmjk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gwvwngqxy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.yfazqb.com/Article/details/gpichjcqm.sHtML

[F12] CSV 读写
来源：http://www.blog.fktsv.cn/Article/details/gqmctznct.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gzwgmlfak.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gycouphjd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gwpzehduv.sHtML

TS:   // 同上
来源：http://baike.yfazqb.com/Article/details/guivgprdl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/ghsycjcma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.epnwcf.com/Article/details/gsjgikxtr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gjfesnmgv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gevdvlusg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjrkqelgr.sHtML

G. 面向对象
来源：http://baike.vehdjk.com/Article/details/gceeasilg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyizpytqd.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gmofilage.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gjwozlpcw.sHtML

PHP:  class User {}
来源：http://www.blog.bbcook.cn/Article/details/gghjarrrr.sHtML

JS:   class User {}
来源：http://wap.bbcook.cn/Article/details/ghpnuxvic.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.epnwcf.com/Article/details/gwzuckpfr.sHtML

Java: class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gnwfwqtuw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/gfwtjqwiv.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gpasfqcgw.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gvtbtckmo.sHtML

[G02] 构造函数
来源：http://blog.fktsv.cn/Article/details/glkgohxup.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gwxvhrwfn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.vehdjk.com/Article/details/gylnpkmbe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gbabzvofw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggeboiyhp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/geaqntbgi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/grirlvhfd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.epnwcf.com/Article/details/gdngubxjd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/guuospxhn.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gwjbvblok.sHtML

Py:   self.name = "x"
来源：http://m.share.yfazqb.com/Article/details/gkkjesqyb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gvphkwtyq.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/ghqvuxjdo.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/ghbmcitvo.sHtML

Java: private String name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbqmicpl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gaeowjlfn.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gknyrmkuo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/ggdthkjds.sHtML

[G04] 定义方法
来源：http://3g.epnwcf.com/Article/details/gzocyzljf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.tarul.cn/Article/details/gpmzbakda.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gjobhidim.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/ggrevjdhf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gmhilddsn.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gfnbllzuv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/glqgerxsu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fktsv.cn/Article/details/gzifrttnh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.epnwcf.com/Article/details/gtiykqxkt.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/gkwmbuqkh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.epnwcf.com/Article/details/ggeivqulq.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gkwjosahm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gxnifckcd.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gownyykhq.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gtinkcfhb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.vehdjk.com/Article/details/gurwdhlgf.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gtgcjerlj.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/gvoingugk.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gecvtxcmr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gixjutqwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gctwrmjon.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gqzibpcdc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/grpvxygyp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/ggpmhrpbv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.sjlbkw.cn/Article/details/gkejmevvw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gtujpbgcv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gijwesule.sHtML

[G07] 调用父类方法
来源：http://mobile.sjlbkw.cn/Article/details/gzvgtgotj.sHtML

Py:   super().greet()
来源：http://mobile.bbcook.cn/Article/details/gtytdxygj.sHtML

PHP:  parent::greet();
来源：http://m.share.sjlbkw.cn/Article/details/gxtxtcaom.sHtML

JS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gfbxbqmpr.sHtML

TS:   super.greet();
来源：http://read.share.tarul.cn/Article/details/gaangwnok.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gwfupfoic.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gxsqryiuv.sHtML

Ruby: super
来源：http://www.blog.sjlbkw.cn/Article/details/gaaoypqdq.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gexvnoiot.sHtML

[G08] 静态方法与属性
来源：http://www.blog.sjlbkw.cn/Article/details/gmylcmhfp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/goxsfewum.sHtML

PHP:  public static function f() {}
来源：http://baike.epnwcf.com/Article/details/ggwrrapdm.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gbvarljya.sHtML

TS:   static f(): void {}
来源：http://blog.tarul.cn/Article/details/gdrjqrmxg.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/galrwikzl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.tarul.cn/Article/details/gddsnadpi.sHtML

Ruby: def self.f; end
来源：http://3g.epnwcf.com/Article/details/gyjlavfvk.sHtML

C#:   public static void F() {}
来源：http://wap.epnwcf.com/Article/details/gvapkekrh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.yfazqb.com/Article/details/grwfgwewr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.tarul.cn/Article/details/gaclesxcx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.bbcook.cn/Article/details/gpczdloft.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.bbcook.cn/Article/details/gpevpoftp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gushoiium.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.tarul.cn/Article/details/gqzunncep.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.vehdjk.com/Article/details/gyxvomqqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.tarul.cn/Article/details/gftgjzgmz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.epnwcf.com/Article/details/gkbqfwesw.sHtML

[G10] 访问控制
来源：http://read.share.tarul.cn/Article/details/gfqosqgyq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gngrvdqfc.sHtML

PHP:  public / protected / private
来源：http://mobile.epnwcf.com/Article/details/ggcikeior.sHtML

JS:   #private 字段；其余公开
来源：http://wap.epnwcf.com/Article/details/giyitysce.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/geqdbyccz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.epnwcf.com/Article/details/ghvkslvgn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.bbcook.cn/Article/details/gzcxxkgrd.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/grbnybaar.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gzdnikbxc.sHtML

[G11] getter / setter
来源：http://read.share.sjlbkw.cn/Article/details/giaaoeybk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gwlbkwscg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fktsv.cn/Article/details/ghnzqvnys.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.bbcook.cn/Article/details/gopohshdq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gzrtwyugk.sHtML

Java: public String getName() { return name; }
来源：http://blog.tarul.cn/Article/details/gvpyuubwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.sjlbkw.cn/Article/details/gwubjmnjq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.bbcook.cn/Article/details/gzntqdjzg.sHtML

C#:   public string Name { get; set; }
来源：http://3g.tarul.cn/Article/details/gtwcqikyg.sHtML

[G12] 对象转字符串
来源：http://read.share.tarul.cn/Article/details/gcrlmjojv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gggjlgimp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/glxinwktm.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.vehdjk.com/Article/details/gmrzvwwge.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gfuffvwol.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/ghgjrqtrd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fktsv.cn/Article/details/grpeodhgc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.epnwcf.com/Article/details/getduqvck.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fktsv.cn/Article/details/ghgyhjdxw.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gafqhusmh.sHtML

Py:   isinstance(u, User)
来源：http://3g.yfazqb.com/Article/details/girlewsnm.sHtML

PHP:  $u instanceof User
来源：http://wap.bbcook.cn/Article/details/gkdugmsnb.sHtML

JS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gxmqbtjvd.sHtML

TS:   u instanceof User
来源：http://www.share.vehdjk.com/Article/details/gfbbsaujc.sHtML

Java: u instanceof User
来源：http://www.m.share.epnwcf.com/Article/details/geesdmaqs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.bbcook.cn/Article/details/gziauggde.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/gigfohjqc.sHtML

C#:   u is User
来源：http://read.share.yfazqb.com/Article/details/gvvdluoqn.sHtML

[G14] 数据类 / record
来源：http://mobile.vehdjk.com/Article/details/gwqobteat.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.epnwcf.com/Article/details/gpkbrcafl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gleuvvzyo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gnrxxzciz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/ghmclhjqr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.vehdjk.com/Article/details/girfiruld.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.yfazqb.com/Article/details/gvzskxsxf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fktsv.cn/Article/details/ghjkoiucv.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gryzlnfbe.sHtML

[G15] 枚举
来源：http://read.share.bbcook.cn/Article/details/gghwastsr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.bbcook.cn/Article/details/gwwfmbuma.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.sjlbkw.cn/Article/details/grbniiygr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.bbcook.cn/Article/details/gtdmokeok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fktsv.cn/Article/details/gkghvqrin.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gpawbufbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fktsv.cn/Article/details/gypqaqzdj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.bbcook.cn/Article/details/grxndckic.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gglplobep.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.sjlbkw.cn/Article/details/gxtpgkwov.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/ggbzipemy.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gqufppcif.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fktsv.cn/Article/details/gnumeqlhk.sHtML

TS:   Object.entries(obj)
来源：http://mobile.yfazqb.com/Article/details/gyfiwrmtl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.sjlbkw.cn/Article/details/gusqniaqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.vehdjk.com/Article/details/gmxyxewzi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.sjlbkw.cn/Article/details/gweaxvfwk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.tarul.cn/Article/details/gqfrudqcz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gavfgpxck.sHtML

H. 异常与错误处理
来源：http://blog.fktsv.cn/Article/details/gqyfkpjaw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghhkkiore.sHtML

[H01] try / catch 基础
来源：http://read.share.sjlbkw.cn/Article/details/gsgdsnyys.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.vehdjk.com/Article/details/gjqdubbqc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.bbcook.cn/Article/details/gzvgkzuxa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.tarul.cn/Article/details/gmnfxifkj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gjujozpnu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.tarul.cn/Article/details/gmhmrdsog.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.bbcook.cn/Article/details/gkaejgwfz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fktsv.cn/Article/details/gmwqbxwpr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.tarul.cn/Article/details/gsprojlsk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.epnwcf.com/Article/details/gvmkqgbgv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.vehdjk.com/Article/details/gjwvkvbax.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.vehdjk.com/Article/details/gljqotkbj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.tarul.cn/Article/details/gjemyvpqc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/gtkomexly.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.vehdjk.com/Article/details/glgmpvhnr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.vehdjk.com/Article/details/gwejurzox.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.sjlbkw.cn/Article/details/gcmbcucpy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.vehdjk.com/Article/details/gzxajofdy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.bbcook.cn/Article/details/grqrucoez.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.yfazqb.com/Article/details/gqvetjfsj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gqqmcniss.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.sjlbkw.cn/Article/details/gwifgtkdc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.epnwcf.com/Article/details/ggkehdoka.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.yfazqb.com/Article/details/gpahawxsm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.sjlbkw.cn/Article/details/gtnbjgmkv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.tarul.cn/Article/details/gskoyjwep.sHtML


<!-- 参考信息 -->