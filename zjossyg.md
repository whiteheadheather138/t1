代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gplntaman.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gfpkrdoap.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gkblrfjdw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/ghtkxhoct.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gupqejsng.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gkixtugqi.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gkaztnosy.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/grnkrltqc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gdpfuvexo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gedzyloui.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gwxbqhdfs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoawncjj.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gmqhafvlk.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gntucrdim.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/grzfurqwv.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/grwgpchfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gojofnhfs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gdjpbmeer.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gvcahpklk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gypdgbeso.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gtwvfatpk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gxgnqgufu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gtuuanaxg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/geeaydptm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.epnwcf.com/Article/details/grreitzjj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.yfazqb.com/Article/details/gscmjxqwv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gyajrngde.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/grwlpbgoj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gsptdufba.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gkrbnzwsx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gajhpkqxf.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gnehtesut.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gvsdotrjz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggzyrtzsa.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gulltmivp.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gytmuuute.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/graoogtil.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gvkxulamz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/gmntidxgy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.vehdjk.com/Article/details/gsedonudi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gpzikuurz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gjxwzzlkk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gbvcfophh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gbdymsnan.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gntveirsj.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gbtjfzvzs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.sjlbkw.cn/Article/details/gftftistn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbitgoyja.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gwyqjyghq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gzvdncujv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gtbjnmluk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/ggqrqmitj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/ghokaxebs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gzjkjsjsb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gefphjnpx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fktsv.cn/Article/details/ghuyrftis.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gnlofkrbq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gmetihnpd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/goqzgdwhq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/grtgzruqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.tarul.cn/Article/details/gtdribjzh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/ggiwnebcr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gnepzobgr.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/ggmzxlsbu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gpyodabiy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gfroeiull.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/grkgbqvbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gldifqlgk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gotvtkacg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.yfazqb.com/Article/details/gyaybdvif.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gooqcftcn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/giswfrslf.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.tarul.cn/Article/details/gnjbokxwf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gxiftqoee.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gzmikqiom.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gdvgixnba.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzayynlqw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gbozeedgo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gdwocucxb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxfefdkms.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnmhhqida.sHtML

[F06] 删除文件
来源：http://www.m.share.fktsv.cn/Article/details/gkmvubfpq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/grmisfzps.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gbifngoos.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnvuiofqy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqxqvarwu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gljkrdkcb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gneasrhyk.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gonwfnsty.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gauxtbrzz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/ggbblkazs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gdaddojki.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gvwqujxtv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gmdnfcglp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gsqconzqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gcjkqexjp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.tarul.cn/Article/details/gxfjcrgbk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.sjlbkw.cn/Article/details/gfyytjtty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/ggptlafvu.sHtML

[F08] 遍历目录
来源：http://mobile.vehdjk.com/Article/details/gwdrjsmkh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuockcxp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gznoexrhk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gfvcqccjp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.tarul.cn/Article/details/gipafnjjz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/guzljmtht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gvpynijsa.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/gberuxyec.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gsmkrsiyb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gxrqyybpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gonobhpfb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/gdvzdpqru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.yfazqb.com/Article/details/gxewzbbwu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/gkaqtrbej.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/grapjxooa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.tarul.cn/Article/details/grbmtjfly.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/ghvfcsjzi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.bbcook.cn/Article/details/gsomyztfk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gwrjclszu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gqubwhuwp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvzngvtic.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gvyweqkxs.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gzbavjlvw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gtsgopgeb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/ggezgltnf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gkangqagz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gqxvkxwxo.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gooawmpwi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gsrhplitw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/goxxghidi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gsyaatlrv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/glhszejtx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.bbcook.cn/Article/details/guzndzfsd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gzeldlati.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/ggeqlzyzw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.vehdjk.com/Article/details/gocrnfaar.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gkbzovkfl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/glopcxiew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gbcneugam.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gvncegdrl.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gxvzopusc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.epnwcf.com/Article/details/gluglszui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gmnvxnyop.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.epnwcf.com/Article/details/gpkiqzmys.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.yfazqb.com/Article/details/gxgzugmqo.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grfmtvuaw.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gqofrfhqc.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gujhdnjwk.sHtML

[G01] 定义类
来源：http://wap.tarul.cn/Article/details/ghfbpqbsy.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gnbztythk.sHtML

PHP:  class User {}
来源：http://www.share.vehdjk.com/Article/details/gebjbkffg.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gkyhtpxzv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gejziahwt.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gempdytvv.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gfhocmtuq.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gnikdqbgq.sHtML

C#:   class User {}
来源：http://www.blog.bbcook.cn/Article/details/gmzpbkuah.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gsrvydaha.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gapahnsme.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fktsv.cn/Article/details/gvsaotofx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/geamhgmoi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/geoblwzsw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/grgyypjha.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.bbcook.cn/Article/details/goyycqols.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/gvvnzlfcb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.vehdjk.com/Article/details/gjndmixga.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkbjammx.sHtML

Py:   self.name = "x"
来源：http://m.share.vehdjk.com/Article/details/giqqumoja.sHtML

PHP:  public string $name = "x";
来源：http://read.share.yfazqb.com/Article/details/gtxjarike.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gxfrbzgdh.sHtML

TS:   name: string = "x";
来源：http://mobile.epnwcf.com/Article/details/ggkrzllzy.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/gwoylujtj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.bbcook.cn/Article/details/gidghsgxd.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gmzzubwdq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ghgzsgrrv.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gybyuvcof.sHtML

Py:   def greet(self): return self.name
来源：http://blog.tarul.cn/Article/details/gamhdccar.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.sjlbkw.cn/Article/details/gcfnwhoro.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fktsv.cn/Article/details/gnruolans.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gsfofxbri.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gllxjwdqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.vehdjk.com/Article/details/gncmpwqgt.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxfbfakk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gvbkxmgro.sHtML

[G05] 继承
来源：http://mobile.tarul.cn/Article/details/geiapkrjl.sHtML

Py:   class Admin(User): pass
来源：http://3g.bbcook.cn/Article/details/ghgpawtmv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.vehdjk.com/Article/details/graxzasaj.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/glvymtcfr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gjrsvjumk.sHtML

Java: class Admin extends User {}
来源：http://baike.vehdjk.com/Article/details/ggfhuizun.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.epnwcf.com/Article/details/gbvznidfj.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/goyxxdxpz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.yfazqb.com/Article/details/gvkkwauvz.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/ggeotwlmv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gjlgtdxfh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/glqgxvzys.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gtjknqorh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/ghevmvfhp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gomsfeqyg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fktsv.cn/Article/details/gzawroiko.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/gpuxiekep.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fktsv.cn/Article/details/gqsqbpywd.sHtML

[G07] 调用父类方法
来源：http://baike.vehdjk.com/Article/details/gdnuihmxt.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gbnjkargm.sHtML

PHP:  parent::greet();
来源：http://www.share.yfazqb.com/Article/details/gotekzefv.sHtML

JS:   super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/ggsmroadd.sHtML

TS:   super.greet();
来源：http://baike.sjlbkw.cn/Article/details/gckubivli.sHtML

Java: super.greet();
来源：http://read.share.vehdjk.com/Article/details/gywkorbxi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.epnwcf.com/Article/details/gxjoysrgj.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gsjxjifso.sHtML

C#:   base.Greet();
来源：http://baike.fktsv.cn/Article/details/gmqthlfbf.sHtML

[G08] 静态方法与属性
来源：http://baike.sjlbkw.cn/Article/details/gfeyzlfci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.bbcook.cn/Article/details/gitospoiz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.tarul.cn/Article/details/gdwaaqiik.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gizaknmjv.sHtML

TS:   static f(): void {}
来源：http://wap.epnwcf.com/Article/details/gqpewvzpy.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/ghtaucqvy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/glwmibmix.sHtML

Ruby: def self.f; end
来源：http://read.share.fktsv.cn/Article/details/gentmvgjt.sHtML

C#:   public static void F() {}
来源：http://mobile.tarul.cn/Article/details/gbugwmpcg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/gqhpfdous.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.tarul.cn/Article/details/gxxbjinyg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.vehdjk.com/Article/details/gjxxcnepf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.bbcook.cn/Article/details/gpwqfxivk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/gpfskidji.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gbnhvaohg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.vehdjk.com/Article/details/geaaemaif.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.bbcook.cn/Article/details/gzefhdpcx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.sjlbkw.cn/Article/details/gayjubjxt.sHtML

[G10] 访问控制
来源：http://wap.sjlbkw.cn/Article/details/gcwibmxsk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fktsv.cn/Article/details/gsobydrdn.sHtML

PHP:  public / protected / private
来源：http://www.share.sjlbkw.cn/Article/details/gwxdmznlq.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gjtxnftuy.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gmfigrins.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.tarul.cn/Article/details/ghaocdrce.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fktsv.cn/Article/details/gtaiilded.sHtML

Ruby: public / protected / private
来源：http://www.share.bbcook.cn/Article/details/gytaakvkf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.yfazqb.com/Article/details/glpaegxdv.sHtML

[G11] getter / setter
来源：http://read.share.epnwcf.com/Article/details/gnfkcqoku.sHtML

Py:   @property 与 @x.setter
来源：http://blog.tarul.cn/Article/details/gqpxompsx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/ghgkqsixl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.yfazqb.com/Article/details/gvqxsimqs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjqrijjck.sHtML

Java: public String getName() { return name; }
来源：http://m.share.yfazqb.com/Article/details/gsduvjyqm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fktsv.cn/Article/details/gedafvnde.sHtML

Ruby: attr_accessor :name
来源：http://blog.sjlbkw.cn/Article/details/grtvzqojo.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.sjlbkw.cn/Article/details/gzqufanqs.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/giqfvldna.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.yfazqb.com/Article/details/grdtmcyxw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/grvmxipgj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gqhugothd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.tarul.cn/Article/details/gljegzuph.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gbiqlrcrv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/goegyhtoy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gwgnlhpqx.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.tarul.cn/Article/details/gzdbyemft.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gevubgqrm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.yfazqb.com/Article/details/gpzrkrldf.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gfnxyyesl.sHtML

JS:   u instanceof User
来源：http://baike.bbcook.cn/Article/details/gvqqzkelt.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gqrpxiyna.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gkycaxkyg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fktsv.cn/Article/details/gtqvsfnyt.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fktsv.cn/Article/details/geprywuod.sHtML

C#:   u is User
来源：http://3g.tarul.cn/Article/details/gpkufuapc.sHtML

[G14] 数据类 / record
来源：http://3g.fktsv.cn/Article/details/gkvmabvgy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.tarul.cn/Article/details/gcgpjgzyw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.yfazqb.com/Article/details/gitrbepax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/ggyykrhkc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.vehdjk.com/Article/details/gzkwnedmv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.vehdjk.com/Article/details/gztghshpo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gptyndkzq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.bbcook.cn/Article/details/gbhfaowge.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gemacwtmm.sHtML

[G15] 枚举
来源：http://read.share.tarul.cn/Article/details/goldqcyri.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.bbcook.cn/Article/details/gdduiwnyh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.vehdjk.com/Article/details/gifhvzbvo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gezncmkpn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gpftziuqu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.tarul.cn/Article/details/gicawxoyd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.yfazqb.com/Article/details/gubbonanc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.sjlbkw.cn/Article/details/gpuaqwryw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.tarul.cn/Article/details/gchtaluku.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fktsv.cn/Article/details/gbnpoutba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.vehdjk.com/Article/details/gorrmqorf.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.yfazqb.com/Article/details/gyupwqfbr.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/gkxfkgfwz.sHtML

TS:   Object.entries(obj)
来源：http://blog.tarul.cn/Article/details/gbjkkxexx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.vehdjk.com/Article/details/gfeybldal.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.bbcook.cn/Article/details/giqmqgbbs.sHtML

Ruby: obj.instance_variables
来源：http://blog.fktsv.cn/Article/details/gfpiuhnhr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/glscgpjul.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gkehuvntz.sHtML

H. 异常与错误处理
来源：http://baike.epnwcf.com/Article/details/gdaljlpmt.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqgslqspy.sHtML

[H01] try / catch 基础
来源：http://www.share.tarul.cn/Article/details/gxaznfton.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gwjzurfpk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fktsv.cn/Article/details/gpcorkwvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.epnwcf.com/Article/details/gbfymwcko.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gamtwwtww.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.vehdjk.com/Article/details/gisbmtqkg.sHtML


<!-- 参考信息 -->