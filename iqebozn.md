代发 wailian999

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gbyvoiaai.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gsyiyekht.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.epnwcf.com/Article/details/gqhpzggbm.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gbohnsxeg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gmwpcmtzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gwrkksmnp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gyhjhjzbb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/glpigjjhe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/grwaxwlqq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gohdxyxzp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gqntybotn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gnzzasixc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gjwoyxhif.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.bbcook.cn/Article/details/gbsjijwon.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gyrnxnyei.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/ggekmitaa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gvohdqleg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/geojrtsuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gmydybtgq.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gsjtflyrz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gbyjdzgwq.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbdrqisnd.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/gxrhnfiwv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gnrkldphw.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gkddnztdj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.yfazqb.com/Article/details/gvxvzvbje.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gtpfyabac.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gevhzoihs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gbqmfydtm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gtwvbbtbq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/giitdfyvw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjfyvohhz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gtomegiht.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gvzzuejct.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gcunkeora.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gelwponfd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gdpvhpmhb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gdhpuylbx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gqtklvbji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.yfazqb.com/Article/details/gulcnhtqo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gvkbfgins.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/grabegxjn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/guoenchro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gvpektjzn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gyaodmfbp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gcsqxxjgw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gvoniaxqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gelsyozxn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gknskoveq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/ghocekkqq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gxxqflltu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gnhvaxmly.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gzqrwkuva.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gfedggcks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gdghmhorz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gzyghlnth.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fktsv.cn/Article/details/giltcovkd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gktxthsrz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gvcfwfffs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gvuwcrbww.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gdlnmvfsm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fktsv.cn/Article/details/gfygtypzv.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.vehdjk.com/Article/details/gqbvwlowb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gepwqlyhw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyeoosbql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/ghaewuoge.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gvqkyfyas.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjpsoxpns.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/guiluhxkb.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/ggazbxsdc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gotiaddjo.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gfuzkjtpy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdtkanwfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gbvmdvawa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/giinbxvcy.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gkachyhxe.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/givnzjaco.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gotwtpgft.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gsiqeubjw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gprqugnui.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.bbcook.cn/Article/details/gavxbkgxr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gohirnbcq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gnhswmpub.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.sjlbkw.cn/Article/details/gkkbjauun.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/ghqsxlrxv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gqjvgbrru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/gigstskfc.sHtML

[F08] 遍历目录
来源：http://baike.vehdjk.com/Article/details/gvtmbnnbe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gbavxpgvw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/ghgegmgvm.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gpavipgma.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/grswvcieg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/grebmgadx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gemvboodg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.tarul.cn/Article/details/gyixffgar.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.vehdjk.com/Article/details/gyhqruqrs.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gizudyack.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxqnlrjeb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gnrzfxkgg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gqizbsvlz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gbvtuctac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gsfohsunp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/gthvonhew.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gwomsifdi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxkxecow.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gaedkovoh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gdtxovhpj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gqkmykrsn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gfrcdunas.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gwmgwbtpn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gaasgznyo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gihdfrxyo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggvphgbec.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gbfshfkaa.sHtML

[F11] 复制与移动文件
来源：http://wap.epnwcf.com/Article/details/gckxzexrb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/gnkhsbpdn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gjftbqmvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gsvyumslr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gwtnrpdle.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fktsv.cn/Article/details/gtfhvhuov.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fktsv.cn/Article/details/gmimzlskt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gpykjmelh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fktsv.cn/Article/details/glizzsbui.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/guownmszx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fktsv.cn/Article/details/gjrfxmmoo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/glaomxrdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gbssftaak.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gipmnhzgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/grekcgaew.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.vehdjk.com/Article/details/gdecefbqo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/glrrtrouy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.tarul.cn/Article/details/gcnbpbayn.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gptzjrsns.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/galrrnyig.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdndahkal.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gveqkmmsi.sHtML

Py:   class User: pass
来源：http://www.share.tarul.cn/Article/details/gxvzguteo.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gixduvjss.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/gomnszkbb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gqrtvkacz.sHtML

Java: class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gtqvlehim.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/glemyloxi.sHtML

Ruby: class User; end
来源：http://baike.bbcook.cn/Article/details/gjyijautd.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gvwhsrhya.sHtML

[G02] 构造函数
来源：http://wap.tarul.cn/Article/details/gytezylqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gjqitgwdy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gzbfwntuz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gleedpgmv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.tarul.cn/Article/details/guypgeixa.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gbkovwpoz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/guykehvsy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gliftdwya.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gnirjizzp.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gfvbuvdwh.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/grlxokiab.sHtML

PHP:  public string $name = "x";
来源：http://blog.fktsv.cn/Article/details/gjqgqxatq.sHtML

JS:   this.name = "x";
来源：http://baike.fktsv.cn/Article/details/gamypnbfz.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gtwcypbkq.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/gklcvloeg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gameyqwpo.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gvfjrhhst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.tarul.cn/Article/details/gudzzxwpz.sHtML

[G04] 定义方法
来源：http://www.share.vehdjk.com/Article/details/geedlakjx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/gkmvnssng.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/glhmudghf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gizjcseqe.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gwgxumsto.sHtML

Java: String greet() { return name; }
来源：http://blog.bbcook.cn/Article/details/gdnohwvuq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.sjlbkw.cn/Article/details/gabaotjdk.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gdlkzxsis.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/gtkbyucsr.sHtML

[G05] 继承
来源：http://m.share.epnwcf.com/Article/details/gmdfswoyi.sHtML

Py:   class Admin(User): pass
来源：http://3g.yfazqb.com/Article/details/gfexdqxka.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/grrsmuwgz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gzyelrvkg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.tarul.cn/Article/details/gwqbxyxpz.sHtML

Java: class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gzixknaxn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gfqgxibcc.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gtspvibxd.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gsmdgjctl.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gqgbqwtng.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fktsv.cn/Article/details/gedgcexqn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfnebuhon.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/ghmhuksrs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gblxpzwit.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gdrxbtahl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.sjlbkw.cn/Article/details/genldpzio.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gdrpmauwr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gnjczfcll.sHtML

[G07] 调用父类方法
来源：http://www.m.share.yfazqb.com/Article/details/grdkwaama.sHtML

Py:   super().greet()
来源：http://baike.fktsv.cn/Article/details/gacwqhkky.sHtML

PHP:  parent::greet();
来源：http://m.share.fktsv.cn/Article/details/gilbzsdhn.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/gswnbqmof.sHtML

TS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gcyokkkyo.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/gxdkvaqnf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.vehdjk.com/Article/details/guwndikeo.sHtML

Ruby: super
来源：http://3g.epnwcf.com/Article/details/gawfqhojf.sHtML

C#:   base.Greet();
来源：http://mobile.tarul.cn/Article/details/gwtgxknsk.sHtML

[G08] 静态方法与属性
来源：http://read.share.fktsv.cn/Article/details/guzvgijwk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gambksvfx.sHtML

PHP:  public static function f() {}
来源：http://mobile.sjlbkw.cn/Article/details/gzfqxpkiv.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/ghrsthhad.sHtML

TS:   static f(): void {}
来源：http://www.blog.sjlbkw.cn/Article/details/gptpyamaj.sHtML

Java: static void f() {}
来源：http://www.share.bbcook.cn/Article/details/gfxxdqztm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.vehdjk.com/Article/details/gvhwndxuy.sHtML

Ruby: def self.f; end
来源：http://mobile.bbcook.cn/Article/details/gjrvvgytt.sHtML

C#:   public static void F() {}
来源：http://blog.yfazqb.com/Article/details/gggqvpdjs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gsttvxjts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fktsv.cn/Article/details/gmmnswuxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.sjlbkw.cn/Article/details/gpzdfqxoe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.vehdjk.com/Article/details/gtssnjiip.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.sjlbkw.cn/Article/details/gwsauiqem.sHtML

Java: interface Shape { double area(); }
来源：http://3g.epnwcf.com/Article/details/gaqcqyoja.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fktsv.cn/Article/details/goqoudntw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.bbcook.cn/Article/details/gkeilhvma.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.vehdjk.com/Article/details/gkggkpvly.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/grsibfkbi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/grtkpskpa.sHtML

PHP:  public / protected / private
来源：http://baike.tarul.cn/Article/details/gwvckojkh.sHtML

JS:   #private 字段；其余公开
来源：http://3g.yfazqb.com/Article/details/ggwvhavtm.sHtML

TS:   public / protected / private
来源：http://mobile.yfazqb.com/Article/details/gxreyeivt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fktsv.cn/Article/details/gjpnvegav.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.bbcook.cn/Article/details/ghhcnoqfc.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/galhmdmxs.sHtML

C#:   public / protected / private / internal
来源：http://wap.bbcook.cn/Article/details/gtrhnsknr.sHtML

[G11] getter / setter
来源：http://read.share.yfazqb.com/Article/details/gxuqzgozb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fktsv.cn/Article/details/gvhwpgini.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gsqpusnim.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fktsv.cn/Article/details/gwcmftifv.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.sjlbkw.cn/Article/details/gebmqvkja.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fktsv.cn/Article/details/ghxktidkb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fktsv.cn/Article/details/gpxhimlfy.sHtML

Ruby: attr_accessor :name
来源：http://mobile.vehdjk.com/Article/details/gtwgcfvjr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.yfazqb.com/Article/details/ggadehgay.sHtML

[G12] 对象转字符串
来源：http://3g.sjlbkw.cn/Article/details/gkoupchrm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.epnwcf.com/Article/details/gblzmcnca.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.yfazqb.com/Article/details/gpmscbqqy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmubhtjzh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.yfazqb.com/Article/details/gxjdxqyhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/ghfrihojl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.vehdjk.com/Article/details/gsfpccjlu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gtxhjnaru.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gaalsylgm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.vehdjk.com/Article/details/gkbkbgpia.sHtML

Py:   isinstance(u, User)
来源：http://baike.tarul.cn/Article/details/gestljkse.sHtML

PHP:  $u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gxcimqehu.sHtML

JS:   u instanceof User
来源：http://www.share.tarul.cn/Article/details/gphywthxq.sHtML

TS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gqemdrmsc.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gborjqebc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.bbcook.cn/Article/details/gzckghyis.sHtML

Ruby: u.is_a?(User)
来源：http://wap.vehdjk.com/Article/details/goedgfcir.sHtML

C#:   u is User
来源：http://mobile.yfazqb.com/Article/details/glvvdwkzu.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gmmgqdujg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.vehdjk.com/Article/details/gzoxnpihk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.tarul.cn/Article/details/gtpuxejwf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.sjlbkw.cn/Article/details/glbmjpwtd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.epnwcf.com/Article/details/gzxfkuzit.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fktsv.cn/Article/details/gszwcnceu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fktsv.cn/Article/details/gsbaonknf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.tarul.cn/Article/details/gzkniteau.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/ggyfeolly.sHtML

[G15] 枚举
来源：http://3g.vehdjk.com/Article/details/gvkrocxog.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.bbcook.cn/Article/details/gumiejpqz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.vehdjk.com/Article/details/gkofiobnm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.sjlbkw.cn/Article/details/gbewsnocj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.sjlbkw.cn/Article/details/ganlwljvu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.bbcook.cn/Article/details/gmakjfzvo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.bbcook.cn/Article/details/gnzgbrpyw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/gjjvhiteg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.vehdjk.com/Article/details/gmrugtyzv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.vehdjk.com/Article/details/grkvjireu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.bbcook.cn/Article/details/gncludjne.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.bbcook.cn/Article/details/ghjwiuawv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gxipbdnff.sHtML

TS:   Object.entries(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gyjxywivn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvxqwqgy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fktsv.cn/Article/details/gcfprkepb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.vehdjk.com/Article/details/genfzmzab.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.yfazqb.com/Article/details/gtweegxjf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzevsbhqp.sHtML

H. 异常与错误处理
来源：http://wap.tarul.cn/Article/details/geanyedia.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gqwtfsvpp.sHtML

[H01] try / catch 基础
来源：http://3g.tarul.cn/Article/details/gleoftdzq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.bbcook.cn/Article/details/grhguhjcy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.epnwcf.com/Article/details/gtzwegfrr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gjswmvvos.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.bbcook.cn/Article/details/ghmecpbfb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fktsv.cn/Article/details/gqbowepsj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fktsv.cn/Article/details/gdowkqdiq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.sjlbkw.cn/Article/details/gjvetwgbw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/giydpcvng.sHtML

[H02] finally / ensure 收尾
来源：http://wap.tarul.cn/Article/details/gxhvjzzti.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fktsv.cn/Article/details/gpobffild.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.tarul.cn/Article/details/gipyggdwc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.vehdjk.com/Article/details/gilxzhxze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.sjlbkw.cn/Article/details/gxaqtyjjq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.tarul.cn/Article/details/gpqcvjtqq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.vehdjk.com/Article/details/gfozvcduh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.yfazqb.com/Article/details/gclmifxgu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.vehdjk.com/Article/details/gsrrzqovu.sHtML


<!-- 参考信息 -->