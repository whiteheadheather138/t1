代发 wailian999

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gnukqvqzo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gtwqqzafo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gwjgefkso.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gxcnyckdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gggocrkwf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gnlnfskft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/glwdnwpgl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/giyybrggi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gvlotgmvr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gmipnsone.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gkkbhyjik.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gsmvatfxt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/ggmtksorb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gvxcjpxik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gjovesseh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gurpyqors.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/ghzmkkmqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/ggnkefsko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gmrjluqrx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.epnwcf.com/Article/details/gatutizxe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gtfgskmis.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggrwbtikk.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gqgjfnbhn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvacpfuge.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gqdqvzowb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gfchjjvov.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzoendhut.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gucwdffqj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/gykcrvphg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gxwidxobr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gjjtpatrk.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gngucwdns.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gpxprnbbf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gosnwewjs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gqgyersbj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gxpvorcia.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gastgzxjw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gtcmjkdpi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gfahfqxck.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gaqngbffn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.tarul.cn/Article/details/gyfbtuvof.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gpexwmdnx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gugrryesk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gedcnckbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gofowdymx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gozbrnlhr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gsdlhsndp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gdaugjeri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdqiomz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/gbpqoxggd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gfargxzwn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.vehdjk.com/Article/details/gasfvfnxy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gtayniaoj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.sjlbkw.cn/Article/details/gnqknrdou.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gooxkwtbr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gwwwzdyly.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gsuoosdrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gybixubuj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/grpihggxz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gyehgtypx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gtffcbbcc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gbgdqecvs.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gqdcqnjvf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ganvbdnlb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggqihkbny.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/giopajnbc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gilxvfacl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtktxxgfh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfjmatvlp.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gwblyfhjz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gaakircxz.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/grivtsunl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gslccpvoi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/grtxazupv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gqdtujhhv.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtfujkpza.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gdywpozrv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.epnwcf.com/Article/details/gqfhsniey.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gpjiaeysm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gazzhftcn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gljblxmdx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gurmxakgy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fktsv.cn/Article/details/gugwmfwcm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gpdpdarpd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/glomzyvww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gnwgcnhmy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gvligroxq.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/guoddfdmy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gezmktfzw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gvxhmudux.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gazbhwvgx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gutdcaoqa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gmiwryfew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/gqqiexase.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/grbyvqhyn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/gepiqdvsq.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gtqeonlyv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkguytnri.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gpiuwsgvj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/glvuqdrqg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gvztivrpg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gqaxthnku.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.yfazqb.com/Article/details/ghiojecgt.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/gritftelx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fktsv.cn/Article/details/gprpqjqtl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/ggatwakox.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/guaufzdaz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gwzycltew.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gexwpjejn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwohslvhc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gjjwoxkya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gqobnvxuu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gfgfdayug.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gchlvngyn.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/ggcpspglw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/ghmsqgcoj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gklolpijr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gdvtaghwb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gwhtaysox.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gklbnyepm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.vehdjk.com/Article/details/gdnhuttzk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gwabgskkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/gnabphzlk.sHtML

[F12] CSV 读写
来源：http://www.m.share.tarul.cn/Article/details/gqlccrhjx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gdixffhou.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/guliwnfdd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.sjlbkw.cn/Article/details/gdnuvjnvt.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gvnwfspej.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.bbcook.cn/Article/details/gwzipcaew.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.bbcook.cn/Article/details/gzovawczv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gvvywrdfl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gltvypbdq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqtywkhix.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gpdoxhklk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnhwqupbk.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/gqgjfmunj.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gfsalmmiq.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gpxcbwqnm.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gebuxwtcc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gfmrnlxko.sHtML

Java: class User {}
来源：http://m.share.bbcook.cn/Article/details/gxxjbtgsl.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fktsv.cn/Article/details/gecatjepl.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/ghumjgacy.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gyskotplm.sHtML

[G02] 构造函数
来源：http://read.share.fktsv.cn/Article/details/gahhlqrzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.tarul.cn/Article/details/gmcgeypck.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.bbcook.cn/Article/details/gbcmceivu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/gjkcqoaxl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvarkbfox.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/ggyqsumty.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gplnzhmjg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/gdxinklcv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gmhsnejgr.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gzdwknjst.sHtML

Py:   self.name = "x"
来源：http://3g.tarul.cn/Article/details/gsormbssf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.epnwcf.com/Article/details/gxhrcwizv.sHtML

JS:   this.name = "x";
来源：http://blog.fktsv.cn/Article/details/glysimbpz.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gxwmnxcog.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gqbsyxunz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gkhbidqbf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.epnwcf.com/Article/details/ggtfdmfbi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/ghnyramkl.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gbmaixmvx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.tarul.cn/Article/details/grmqbumrc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.tarul.cn/Article/details/gqenjlhwh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gsltjtjvf.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gqqnobpgn.sHtML

Java: String greet() { return name; }
来源：http://www.share.fktsv.cn/Article/details/gkcvcxhmd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/grbdxsqim.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gbwxiuveu.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/ghbsxgifj.sHtML

[G05] 继承
来源：http://blog.yfazqb.com/Article/details/gfhfylsum.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/gtgdjusti.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gwfgmcycm.sHtML

JS:   class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gqjzplagq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gqbyecnuh.sHtML

Java: class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gnevdqekw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.sjlbkw.cn/Article/details/gdyparovy.sHtML

Ruby: class Admin < User; end
来源：http://mobile.epnwcf.com/Article/details/getltnvla.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/gxxeibsbk.sHtML

[G06] 重写方法
来源：http://www.m.share.vehdjk.com/Article/details/gxfpmrcpl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/gecmsxdnw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gcksjojiy.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.tarul.cn/Article/details/gyfmexkqs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gkmwzctby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.bbcook.cn/Article/details/govchxwkd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fktsv.cn/Article/details/gjfsebeqv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gldxlngot.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.sjlbkw.cn/Article/details/grnkblzfq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.tarul.cn/Article/details/gruvfiyyd.sHtML

Py:   super().greet()
来源：http://read.share.vehdjk.com/Article/details/gjnfcbymu.sHtML

PHP:  parent::greet();
来源：http://blog.tarul.cn/Article/details/gdiqupvlp.sHtML

JS:   super.greet();
来源：http://www.share.fktsv.cn/Article/details/gvoaocmwd.sHtML

TS:   super.greet();
来源：http://blog.vehdjk.com/Article/details/gqzhvtskp.sHtML

Java: super.greet();
来源：http://wap.bbcook.cn/Article/details/gurkbifvs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.tarul.cn/Article/details/gmectoark.sHtML

Ruby: super
来源：http://mobile.vehdjk.com/Article/details/gcnzfyhmn.sHtML

C#:   base.Greet();
来源：http://read.share.fktsv.cn/Article/details/gcmcnpmcj.sHtML

[G08] 静态方法与属性
来源：http://m.share.fktsv.cn/Article/details/gzdscjktp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.tarul.cn/Article/details/gcoobikzc.sHtML

PHP:  public static function f() {}
来源：http://3g.tarul.cn/Article/details/gkymgnmem.sHtML

JS:   static f() {}
来源：http://www.blog.bbcook.cn/Article/details/gdjdnykvb.sHtML

TS:   static f(): void {}
来源：http://wap.tarul.cn/Article/details/gtnrtukpq.sHtML

Java: static void f() {}
来源：http://baike.tarul.cn/Article/details/gbimzoxhv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.sjlbkw.cn/Article/details/gkqljbaip.sHtML

Ruby: def self.f; end
来源：http://mobile.sjlbkw.cn/Article/details/gbjpnxljf.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/ghhtusgiu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.yfazqb.com/Article/details/gmxdzttjd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.vehdjk.com/Article/details/guktxuyzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gagxqymnq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzpvqyod.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.epnwcf.com/Article/details/gscgqcfio.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.vehdjk.com/Article/details/glsdwadew.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.bbcook.cn/Article/details/gdrxzmdvh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.vehdjk.com/Article/details/gytrnlhwh.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gblwndube.sHtML

[G10] 访问控制
来源：http://read.share.epnwcf.com/Article/details/gvmesoplm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.tarul.cn/Article/details/grvhqvkog.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gmcptitki.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fktsv.cn/Article/details/gixuwwjdi.sHtML

TS:   public / protected / private
来源：http://read.share.tarul.cn/Article/details/gwtddtbhs.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.epnwcf.com/Article/details/gekxmvkaf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.epnwcf.com/Article/details/gnlrrzllj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gxjdfsoal.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.tarul.cn/Article/details/gtuwpztlb.sHtML

[G11] getter / setter
来源：http://www.m.share.tarul.cn/Article/details/gopuplugl.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.vehdjk.com/Article/details/gxzmswdwn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.yfazqb.com/Article/details/ghymxxxnr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.tarul.cn/Article/details/gegxuopih.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gfwqjeaav.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/gjgrqcfny.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.vehdjk.com/Article/details/getvbbtgu.sHtML

Ruby: attr_accessor :name
来源：http://baike.tarul.cn/Article/details/grpufkmub.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/gkgfejbek.sHtML

[G12] 对象转字符串
来源：http://wap.fktsv.cn/Article/details/gkzkktsfe.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.yfazqb.com/Article/details/ggzywshyo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gsngzqtpm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.yfazqb.com/Article/details/gmvknmibx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.vehdjk.com/Article/details/gtmmhothb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/ghxpwubqq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.yfazqb.com/Article/details/gavcfttab.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fktsv.cn/Article/details/gpcxeubmw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.bbcook.cn/Article/details/gclrrklvm.sHtML

[G13] 判断对象类型
来源：http://read.share.sjlbkw.cn/Article/details/gczzhmniz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.tarul.cn/Article/details/gdhwhksbi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.tarul.cn/Article/details/gqwilgvvx.sHtML

JS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/ggcvwtwia.sHtML

TS:   u instanceof User
来源：http://blog.yfazqb.com/Article/details/gpavrjxog.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/ggmhweoru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.vehdjk.com/Article/details/gzzcjnqel.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.epnwcf.com/Article/details/gocpigwre.sHtML

C#:   u is User
来源：http://www.share.vehdjk.com/Article/details/ggydhlkzc.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gkrscacyh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.bbcook.cn/Article/details/gxqntwzap.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gennqmgka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/giehdcxtf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.yfazqb.com/Article/details/gpwyuxeqf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/gegiombli.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.sjlbkw.cn/Article/details/gxulvuuca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.sjlbkw.cn/Article/details/gbmfjlnom.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.epnwcf.com/Article/details/gzabdqrng.sHtML

[G15] 枚举
来源：http://m.share.vehdjk.com/Article/details/gpyznmbov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.yfazqb.com/Article/details/gnhhbqzje.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.bbcook.cn/Article/details/gdvwjkwre.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.epnwcf.com/Article/details/grfoouwto.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.epnwcf.com/Article/details/gosqrxjcu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.vehdjk.com/Article/details/gkrqlella.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.bbcook.cn/Article/details/gbqnyvyge.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.sjlbkw.cn/Article/details/gjxsoiiwp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.bbcook.cn/Article/details/gxrvambij.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.bbcook.cn/Article/details/ggbyxcooo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.tarul.cn/Article/details/gwuaqhpwy.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.bbcook.cn/Article/details/gyupeabui.sHtML

JS:   Object.entries(obj)
来源：http://mobile.vehdjk.com/Article/details/gsexpwpmp.sHtML

TS:   Object.entries(obj)
来源：http://read.share.bbcook.cn/Article/details/gojvbmefo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.tarul.cn/Article/details/gpbmcphed.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.vehdjk.com/Article/details/gjuhffols.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gqriimpfl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gnqwliasq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcnbdaqpi.sHtML

H. 异常与错误处理
来源：http://www.blog.tarul.cn/Article/details/gaddggtyl.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gomfhcmvu.sHtML

[H01] try / catch 基础
来源：http://wap.sjlbkw.cn/Article/details/gadhzdfgy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.epnwcf.com/Article/details/gkmiigbql.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fktsv.cn/Article/details/goltpmmnp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/grwgyuhsf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.sjlbkw.cn/Article/details/gdfkeudns.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.bbcook.cn/Article/details/gvulazlod.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.sjlbkw.cn/Article/details/gmodkzuvd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fktsv.cn/Article/details/gpmaixehy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.sjlbkw.cn/Article/details/gfykzvcyj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gkdriffff.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.vehdjk.com/Article/details/gyshsinln.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.bbcook.cn/Article/details/gpsqcdbky.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fktsv.cn/Article/details/gcxvuhcqu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.yfazqb.com/Article/details/ghvynthtq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.bbcook.cn/Article/details/gidtbglwk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gdjodigrl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fktsv.cn/Article/details/gxfpcnymr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.yfazqb.com/Article/details/gmzipcjfe.sHtML


<!-- 参考信息 -->