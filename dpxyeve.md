代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gzenofkkw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/govzcnggn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gonhlbukq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gocugvyqn.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/ggondmqtk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gyzndnjun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gyozvmbof.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gowcjvcdf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gdfhsuvqb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.tarul.cn/Article/details/gmtgufwdg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gaodgsfki.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gzoupzgne.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gyuxjzhvt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glxkbswgk.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gefxhndhc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvcuqoccb.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/ggcufmosr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gxhqvpbie.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gwgwdvxbt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gxvandsnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjbazdac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gkvmnrblg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/gafetnges.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcvndhxmk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gmeyhfbpa.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gbfzijldc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gxwctiqqt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gikmgkefx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/ggoqnfbyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gejqctjnr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gpaahbefq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/goimtbncg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/gcirwfgct.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.epnwcf.com/Article/details/guudnrurc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/girsypfsc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/ghgvicszh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/glluyonkg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gzymvoiyy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gsyjyzbxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gutzqokpd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gegrsivwi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gpnrigmpp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gyyzugodx.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gjzvticei.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gwrlnixrf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.bbcook.cn/Article/details/gxkdppaic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gdajhovze.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gxhrhiyki.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gufwtlbmp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/gllypjwmh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gjxmanhbo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gchjulrnc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.vehdjk.com/Article/details/gudkepmjt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gataexblt.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gxphaoyxd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ggahwlwpt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/galozkobf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gjxpqzmjc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gdmtqgjob.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ghwzbmrfv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gevnowjfq.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/gopidhvmf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gjqvvgqvg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/ghuwggclv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggfmhthhq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/grsctjkzc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gwtzoebsh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjwvggcbe.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbgoehemw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ganbkqmed.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/gwtyqhawo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gnhyjqcnu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.yfazqb.com/Article/details/gnplryqot.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/ggmolakxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gnypjfdyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.epnwcf.com/Article/details/gmwicvlpt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/glkhwzmhs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gbjzscgbg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/ghfvtlvut.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gcoebngvl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.sjlbkw.cn/Article/details/gvfdprynz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/ghbulcikd.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gxqbooljg.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gqcjuxpov.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gzapejtjd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.yfazqb.com/Article/details/gigyvysro.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.bbcook.cn/Article/details/gaiprsroq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/getzfqxpg.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gqhusdmqk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/ghigkfqdu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdwtosmse.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gogobxwis.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gfsgxskqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/ggejdcpwc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.epnwcf.com/Article/details/gflvbfail.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gagdgjeeb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.tarul.cn/Article/details/gaqenqbqq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gvykmjdos.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gudastocg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.tarul.cn/Article/details/gugcdmfoa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gceulqgty.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gnvindong.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.sjlbkw.cn/Article/details/ghomyztxl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/giqltwvgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gepspigcm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gxnitjmrq.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gzuympvlx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gcsobkwdu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gyqvmnudb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/ghelvzwey.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gmgjcmbki.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gftcemgps.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/guldgrboc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gldasdcfz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gniehjzrv.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gynxknvpv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gjbkddsqj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gwkbywbdx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gwbxxvcly.sHtML

TS:   // 同上
来源：http://blog.epnwcf.com/Article/details/gdnzelqfu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/grvfqxvoa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gqwhhojer.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/gjsaeqmmw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.epnwcf.com/Article/details/gtxockdfp.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/goosjpylr.sHtML

G. 面向对象
来源：http://www.blog.fktsv.cn/Article/details/gainbaicd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grhygynep.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/glrvwpeye.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gxmzfihoi.sHtML

PHP:  class User {}
来源：http://3g.bbcook.cn/Article/details/gitssauer.sHtML

JS:   class User {}
来源：http://wap.vehdjk.com/Article/details/gdvxklfou.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/geihhbrbo.sHtML

Java: class User {}
来源：http://www.share.yfazqb.com/Article/details/gdabpunuv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gmiuagnoz.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gbelrqaqn.sHtML

C#:   class User {}
来源：http://3g.bbcook.cn/Article/details/grfzevead.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/ghczjuaun.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gzogfjrzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gvlufymkv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.yfazqb.com/Article/details/gbgpxtiuu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.vehdjk.com/Article/details/giunqfqyx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.epnwcf.com/Article/details/gqsusyfwg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fktsv.cn/Article/details/guegrdupy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gbfadhrmj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.tarul.cn/Article/details/glrkxnsli.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gholxzsdy.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gpzjemtid.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gyahqvxgc.sHtML

JS:   this.name = "x";
来源：http://www.blog.bbcook.cn/Article/details/gntmsrrfp.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gzbnibfyz.sHtML

Java: private String name;
来源：http://mobile.bbcook.cn/Article/details/gzhwsztxe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gptllfafl.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/glzmnqeey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gmihcgoul.sHtML

[G04] 定义方法
来源：http://www.share.vehdjk.com/Article/details/gvpzhtvde.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gngbkvhmm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gagshfuec.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.tarul.cn/Article/details/giyfkvmhf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/glaewdqzk.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gayvuzgus.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.vehdjk.com/Article/details/gyauhifop.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gystirjxp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.yfazqb.com/Article/details/gjruudpua.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gkecotdrb.sHtML

Py:   class Admin(User): pass
来源：http://3g.fktsv.cn/Article/details/gvevqqaqp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/ggujpwsge.sHtML

JS:   class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/gkyiagtfu.sHtML

TS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/guiezydbx.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gjshtlcwq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.bbcook.cn/Article/details/gptnugjot.sHtML

Ruby: class Admin < User; end
来源：http://mobile.vehdjk.com/Article/details/gbabpfkyy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.vehdjk.com/Article/details/gpwvfbzho.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/ghhxlocvi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.sjlbkw.cn/Article/details/geilgimpi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/guqernglb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gucmtphhp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gkpcjalgy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gnehynqpn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gvetwzocz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.yfazqb.com/Article/details/gmtdsfcyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gdpxqjadj.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gabgtfobz.sHtML

Py:   super().greet()
来源：http://m.share.fktsv.cn/Article/details/gpcbezimg.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gplggtpdp.sHtML

JS:   super.greet();
来源：http://read.share.vehdjk.com/Article/details/gxhqrkhrw.sHtML

TS:   super.greet();
来源：http://3g.tarul.cn/Article/details/glcxsfwww.sHtML

Java: super.greet();
来源：http://3g.sjlbkw.cn/Article/details/gcivpcjek.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/gbcgsthnq.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/giwdhwjvo.sHtML

C#:   base.Greet();
来源：http://www.m.share.tarul.cn/Article/details/gwquilnaj.sHtML

[G08] 静态方法与属性
来源：http://baike.epnwcf.com/Article/details/guklooswu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.sjlbkw.cn/Article/details/gyqetjqrr.sHtML

PHP:  public static function f() {}
来源：http://3g.bbcook.cn/Article/details/guvskvlqz.sHtML

JS:   static f() {}
来源：http://3g.tarul.cn/Article/details/gwzlppvlz.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpujnusbp.sHtML

Java: static void f() {}
来源：http://m.share.fktsv.cn/Article/details/gblvgfyzr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/gzbkfnlbh.sHtML

Ruby: def self.f; end
来源：http://blog.tarul.cn/Article/details/glkecklyr.sHtML

C#:   public static void F() {}
来源：http://wap.yfazqb.com/Article/details/grpgoswlw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.yfazqb.com/Article/details/gkklksadv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.epnwcf.com/Article/details/gocxubueq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.yfazqb.com/Article/details/gwjtfhzcu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fktsv.cn/Article/details/gbznymndq.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.sjlbkw.cn/Article/details/ghstcmgbk.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.tarul.cn/Article/details/grxkljfmd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fktsv.cn/Article/details/giqxhqxgk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.yfazqb.com/Article/details/gnnhlwlul.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.bbcook.cn/Article/details/glsqumflj.sHtML

[G10] 访问控制
来源：http://www.blog.yfazqb.com/Article/details/gvogvosvd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.tarul.cn/Article/details/gluioxlgg.sHtML

PHP:  public / protected / private
来源：http://baike.yfazqb.com/Article/details/gyaltkfpt.sHtML

JS:   #private 字段；其余公开
来源：http://3g.sjlbkw.cn/Article/details/gijndespx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gczypxybj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fktsv.cn/Article/details/gorkalgxy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.yfazqb.com/Article/details/gnrsokjqn.sHtML

Ruby: public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gttpticxe.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.sjlbkw.cn/Article/details/ghqvldwyi.sHtML

[G11] getter / setter
来源：http://www.m.share.epnwcf.com/Article/details/grooxgbui.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.epnwcf.com/Article/details/glhzytsjc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.epnwcf.com/Article/details/gnroiikme.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.tarul.cn/Article/details/gjuzaldji.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/govngqpcg.sHtML

Java: public String getName() { return name; }
来源：http://wap.epnwcf.com/Article/details/gaozjplqg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fktsv.cn/Article/details/gwagqgqcr.sHtML

Ruby: attr_accessor :name
来源：http://wap.epnwcf.com/Article/details/gvzqopeym.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.tarul.cn/Article/details/guqhbjarz.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/gxmconulf.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.vehdjk.com/Article/details/gxxjpccmj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/ggxdvlbik.sHtML

JS:   toString() { return this.name; }
来源：http://baike.vehdjk.com/Article/details/grqbfhpeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fktsv.cn/Article/details/ghgpiguqk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.bbcook.cn/Article/details/gglousdzg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gbvbsqpcr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.yfazqb.com/Article/details/gumkqwifh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.tarul.cn/Article/details/gilhwrdyc.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/giocgidtj.sHtML

Py:   isinstance(u, User)
来源：http://read.share.yfazqb.com/Article/details/gehyuxzic.sHtML

PHP:  $u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gkcvoeepn.sHtML

JS:   u instanceof User
来源：http://m.share.tarul.cn/Article/details/gjqjewhiv.sHtML

TS:   u instanceof User
来源：http://mobile.vehdjk.com/Article/details/gfrmvvqby.sHtML

Java: u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gcwpmasbi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.tarul.cn/Article/details/gteslyyuw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gsrarbdbb.sHtML

C#:   u is User
来源：http://3g.epnwcf.com/Article/details/gdiyqtmlo.sHtML

[G14] 数据类 / record
来源：http://www.blog.bbcook.cn/Article/details/gjqnrbicw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.epnwcf.com/Article/details/gbkmhuatl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fktsv.cn/Article/details/gpeugjlsr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.bbcook.cn/Article/details/gavxjcgns.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.yfazqb.com/Article/details/ghbmydksa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.vehdjk.com/Article/details/grhibejzz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.yfazqb.com/Article/details/gfahrczme.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.vehdjk.com/Article/details/gihvqyqve.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gbsueamls.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/gidvommoh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fktsv.cn/Article/details/geednbqsv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.yfazqb.com/Article/details/gzvcgiqdl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.sjlbkw.cn/Article/details/gzzxatmyo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.yfazqb.com/Article/details/glzhnftsp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.epnwcf.com/Article/details/gzwrirelk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.bbcook.cn/Article/details/gomlgsoto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.sjlbkw.cn/Article/details/gobnpnvdi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fktsv.cn/Article/details/gmhdcqmiu.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.sjlbkw.cn/Article/details/gggbrobzy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.epnwcf.com/Article/details/gobzfkhyl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.epnwcf.com/Article/details/gnnykqxoq.sHtML

JS:   Object.entries(obj)
来源：http://read.share.epnwcf.com/Article/details/gpxqvopoj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fktsv.cn/Article/details/gbltfnhcb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.sjlbkw.cn/Article/details/gjrrrqpdv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.bbcook.cn/Article/details/gqndeyusa.sHtML

Ruby: obj.instance_variables
来源：http://3g.vehdjk.com/Article/details/gfprjguib.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.tarul.cn/Article/details/gevgqivcw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzdqjzgii.sHtML

H. 异常与错误处理
来源：http://blog.epnwcf.com/Article/details/gfjzvfpch.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glsdvzkbm.sHtML

[H01] try / catch 基础
来源：http://m.share.epnwcf.com/Article/details/gkqhtvjsr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.bbcook.cn/Article/details/gfomlfeua.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.sjlbkw.cn/Article/details/gnatdqwxv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fktsv.cn/Article/details/gznaqamyi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcliipzl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gdqsmtlyj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.tarul.cn/Article/details/gqjfmslqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fktsv.cn/Article/details/gbcjckgap.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.epnwcf.com/Article/details/gcamceyjl.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.bbcook.cn/Article/details/gbesmlozj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gytgqouby.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.epnwcf.com/Article/details/gmegmxemb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fktsv.cn/Article/details/grsxqrogn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fktsv.cn/Article/details/ghdzfbppg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fktsv.cn/Article/details/gqffmrajy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.sjlbkw.cn/Article/details/gipyendpc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.vehdjk.com/Article/details/gntsygumt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fktsv.cn/Article/details/gxjkkvmjd.sHtML

[H03] 主动抛出异常
来源：http://baike.epnwcf.com/Article/details/gsgxwisme.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.yfazqb.com/Article/details/gojillmhx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.epnwcf.com/Article/details/gzjadqvok.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.sjlbkw.cn/Article/details/gxkdeiyej.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fktsv.cn/Article/details/gphpkmhdt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.vehdjk.com/Article/details/gpentfmga.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.vehdjk.com/Article/details/giqkkmajq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.yfazqb.com/Article/details/gwhzgodvm.sHtML


<!-- 参考信息 -->