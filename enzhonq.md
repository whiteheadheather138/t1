代发 wailian999

Ruby: s.lines
来源：http://mobile.vehdjk.com/Article/details/gfjiioktc.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gexppaqjj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/gktpdlrik.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gnwdjhqcr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gyfekorfh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/gdmhzxgtm.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/gmlymsrra.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gbaoghqme.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gioypvrbc.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gksqwlwek.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/guwijlzem.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/geubyfhor.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/givfvfqra.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gnmeztnem.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gthfdfxvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gzlpapnxb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gamkorlmp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gvitgoanc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gowkdlwcz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gkdvuprsj.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gxgtzpsxd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gwscvljol.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gfcsdftmp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gxvomjasn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gkxxeqwpm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gtmqzebok.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gyolneetf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gmfqsouxm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gxwybanso.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmneiqfug.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gyoipcnts.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gpkddbpoe.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gszuulrrv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/girspyxbg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gxbkbvgpu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/guouzbwit.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/gctmdvyqy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gjbpwhieg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gigladyhq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwfqkehog.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gdgdcoegz.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gxwbqaylk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/gebxzpera.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/gtzkrubdi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gnlfarwpi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdqlteems.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gtdwivqwi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gexhwtxog.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gxkqbvixu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gdjdemxqq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.epnwcf.com/Article/details/glnpvdcek.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.sjlbkw.cn/Article/details/gytdzghdm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gwtwhnwml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gmbdrnmqz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gfvunouxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gmudnfpjn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gaqkllpcb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/gpgmcndvd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gkljwyrtk.sHtML

[F04] 追加写入文件
来源：http://read.share.tarul.cn/Article/details/ginzbgopi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gbwdbsoyu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gcclptrji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gftjsssiy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gbskaoexk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.bbcook.cn/Article/details/gukfhvgyx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gdbswsqvg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gswyhqxiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/grlnqrncx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gjwyeomdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gmiszbkxy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gvogcaiow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfwsyxclp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gawrtxiqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gbpotxjhq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/givwagzhn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwtuuhdhl.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gkboezxvh.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gsedlzqfn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gtraoegmz.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gfjtokduc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gqfdmbzxo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gedvbodyn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gfhnpsvli.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghsduglco.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.yfazqb.com/Article/details/geoaznxcs.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.yfazqb.com/Article/details/gdongibhh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gnpuizpdf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gxnjgloyh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.vehdjk.com/Article/details/geyyatlun.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gxvhpadtn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gkpsfpkbf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.epnwcf.com/Article/details/gnvwellpu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gituzvqll.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.yfazqb.com/Article/details/gmigbwhoz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gpohmvvxd.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/goqnazksi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.tarul.cn/Article/details/gctviklbd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.yfazqb.com/Article/details/gqeokcraz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/geglajzgp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gvdrwzhma.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gvoohuhfk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/glpgfskiw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gmerlrkse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.bbcook.cn/Article/details/gnrztswqg.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gcmwxnwqm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnwtfcdfj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.vehdjk.com/Article/details/goqnwftqq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/giykmyjck.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gxcososje.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gcdzxnxti.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.epnwcf.com/Article/details/gsbfbrjmn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gkymsruhp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gbvnegkkl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fktsv.cn/Article/details/gxqgucvry.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmakugwmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gyaeknsaf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/glcsfnucu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gaqflyyry.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.vehdjk.com/Article/details/gevvvayon.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gabxtfblg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwlbetleh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsptfojxd.sHtML

[F11] 复制与移动文件
来源：http://blog.vehdjk.com/Article/details/grqibopfe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gtbqtshaj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gzqkkqkut.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gvjjpjanl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gzdreohdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gitowcyhs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/ghwkoeluv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gfddvlkxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gngaxweka.sHtML

[F12] CSV 读写
来源：http://blog.vehdjk.com/Article/details/gtleswsst.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gnugrohfv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gkyymeczx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gyaosldua.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gxiyuaoik.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/geknurjep.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/graamhrax.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.bbcook.cn/Article/details/gpscmgjtb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gtdfnhmnm.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwbaytuuc.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gxdtdxgek.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gziyddear.sHtML

[G01] 定义类
来源：http://www.share.vehdjk.com/Article/details/gmkivlxui.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gztvhyggj.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gthsjtlac.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvywxtlnm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gfjaabjsq.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gnkbhlwsx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gwmnsisgi.sHtML

Ruby: class User; end
来源：http://www.m.share.yfazqb.com/Article/details/ghrazttlw.sHtML

C#:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gwgnsbrgc.sHtML

[G02] 构造函数
来源：http://m.share.tarul.cn/Article/details/grebetofh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.tarul.cn/Article/details/grvhanfgk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fktsv.cn/Article/details/gbffimtcl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gjcbfnvce.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.yfazqb.com/Article/details/gyhhlwwwo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gyoxdfyxx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/gtqhedwfo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gtkvrcqdx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.vehdjk.com/Article/details/guhjidari.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/goekuburx.sHtML

Py:   self.name = "x"
来源：http://mobile.yfazqb.com/Article/details/gbqfateay.sHtML

PHP:  public string $name = "x";
来源：http://baike.fktsv.cn/Article/details/gbxpqgzre.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gdxyohgkt.sHtML

TS:   name: string = "x";
来源：http://wap.epnwcf.com/Article/details/gutjeilzt.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/guqtifukb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.bbcook.cn/Article/details/gxznkvcdx.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gflzarlgu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.yfazqb.com/Article/details/gwkzbsrlt.sHtML

[G04] 定义方法
来源：http://www.share.bbcook.cn/Article/details/gkkgkedmc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.epnwcf.com/Article/details/gxguiigac.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gfjfrgkwy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gnzvcnmuq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/grgpnganp.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/gkubrteht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gbjpirqvl.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gkzuibibo.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gjadowsln.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gpgiqtqqo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.sjlbkw.cn/Article/details/guwpjfoae.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gccnyvejp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzcesrkvp.sHtML

TS:   class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gzthrichj.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/ghvmnddvw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gqfvojrjp.sHtML

Ruby: class Admin < User; end
来源：http://3g.vehdjk.com/Article/details/gdasonjng.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/guyxtmcuy.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gvoootoif.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.bbcook.cn/Article/details/gsoypnvmt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.sjlbkw.cn/Article/details/gqljoevhn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/guiyhwbkj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gmstbjtcm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/ghgguteid.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/gkgspzmzz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxszvowi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gsavekvwt.sHtML

[G07] 调用父类方法
来源：http://read.share.yfazqb.com/Article/details/gtawucwxv.sHtML

Py:   super().greet()
来源：http://read.share.bbcook.cn/Article/details/gpxavcisq.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gkdknqyhk.sHtML

JS:   super.greet();
来源：http://baike.tarul.cn/Article/details/ggpwuujog.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gfnmqczbl.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gzfjtikyd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.yfazqb.com/Article/details/gbakkrove.sHtML

Ruby: super
来源：http://www.m.share.bbcook.cn/Article/details/gxseuyfvi.sHtML

C#:   base.Greet();
来源：http://wap.tarul.cn/Article/details/gkbgcpkly.sHtML

[G08] 静态方法与属性
来源：http://baike.vehdjk.com/Article/details/gkzaualbd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.yfazqb.com/Article/details/gykwanhzi.sHtML

PHP:  public static function f() {}
来源：http://m.share.epnwcf.com/Article/details/glifzvimt.sHtML

JS:   static f() {}
来源：http://baike.fktsv.cn/Article/details/gnezoyyoi.sHtML

TS:   static f(): void {}
来源：http://www.share.tarul.cn/Article/details/guqlthgjb.sHtML

Java: static void f() {}
来源：http://mobile.epnwcf.com/Article/details/gjggmbnuc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.vehdjk.com/Article/details/giqbhgghn.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gqicttzdi.sHtML

C#:   public static void F() {}
来源：http://www.m.share.bbcook.cn/Article/details/gxkofugig.sHtML

[G09] 接口 / 抽象类
来源：http://baike.tarul.cn/Article/details/gehdoslsp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.epnwcf.com/Article/details/gpepejpsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.vehdjk.com/Article/details/gfpyouyzi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.vehdjk.com/Article/details/gggxncnuy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fktsv.cn/Article/details/glpivbitn.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gpsuyzuym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gszredyxf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fktsv.cn/Article/details/gxyhtfsig.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.tarul.cn/Article/details/gqwsluwwf.sHtML

[G10] 访问控制
来源：http://www.m.share.fktsv.cn/Article/details/ggtwdhnbj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.epnwcf.com/Article/details/gifwbupkj.sHtML

PHP:  public / protected / private
来源：http://wap.fktsv.cn/Article/details/ghobdntue.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.yfazqb.com/Article/details/gyodcbuxo.sHtML

TS:   public / protected / private
来源：http://www.m.share.yfazqb.com/Article/details/gatiqmxar.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.sjlbkw.cn/Article/details/gomqiibbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/geeaaubkm.sHtML

Ruby: public / protected / private
来源：http://www.blog.yfazqb.com/Article/details/guarhvytq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.vehdjk.com/Article/details/gmjjalajm.sHtML

[G11] getter / setter
来源：http://3g.tarul.cn/Article/details/gypltstbw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.vehdjk.com/Article/details/gkbckraok.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gtgjmwdtu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.epnwcf.com/Article/details/gtqtjljuh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.yfazqb.com/Article/details/gazzceuhj.sHtML

Java: public String getName() { return name; }
来源：http://blog.bbcook.cn/Article/details/ggvhcnigd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gorifwcxk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.bbcook.cn/Article/details/gufbfvbcr.sHtML

C#:   public string Name { get; set; }
来源：http://blog.yfazqb.com/Article/details/gukojrtzl.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gwotfqtpu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gcsqgppdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.sjlbkw.cn/Article/details/gvzsqmwtx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gkmcadkqz.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.bbcook.cn/Article/details/gfryelnid.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fktsv.cn/Article/details/gikcwiqhx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.tarul.cn/Article/details/gnjjdlmrn.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fktsv.cn/Article/details/gmpicszob.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.epnwcf.com/Article/details/gqmmavyxq.sHtML

[G13] 判断对象类型
来源：http://mobile.sjlbkw.cn/Article/details/gbcdnawwz.sHtML

Py:   isinstance(u, User)
来源：http://baike.epnwcf.com/Article/details/gtswzngth.sHtML

PHP:  $u instanceof User
来源：http://3g.fktsv.cn/Article/details/gkpcyvwee.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/goxxnrhpw.sHtML

TS:   u instanceof User
来源：http://www.blog.epnwcf.com/Article/details/gghvmzhjg.sHtML

Java: u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gbfnbnvgf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fktsv.cn/Article/details/gckiowyjt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.epnwcf.com/Article/details/gxrbwzdoa.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gocwjsvra.sHtML

[G14] 数据类 / record
来源：http://baike.tarul.cn/Article/details/gznhkrbgk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.epnwcf.com/Article/details/gpzwbxtbn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/grgvrdznb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.bbcook.cn/Article/details/gaqpoepsu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.tarul.cn/Article/details/gqnxmjeod.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.epnwcf.com/Article/details/gbksjgnsn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.epnwcf.com/Article/details/gavfrytag.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.vehdjk.com/Article/details/gjjzxdmzb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fktsv.cn/Article/details/ghrvkopzn.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gqzcsffch.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.tarul.cn/Article/details/gqjxvrlct.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.bbcook.cn/Article/details/gteovcxve.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.epnwcf.com/Article/details/geegnnvwm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.tarul.cn/Article/details/gyeadrpba.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.epnwcf.com/Article/details/gnqbexdtn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.sjlbkw.cn/Article/details/gvnctmfmw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.tarul.cn/Article/details/gkjtxzqtr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.bbcook.cn/Article/details/gdgaovneh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.sjlbkw.cn/Article/details/gmwmmkafl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fktsv.cn/Article/details/gwxuvtien.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.vehdjk.com/Article/details/gcqzoauko.sHtML

JS:   Object.entries(obj)
来源：http://wap.bbcook.cn/Article/details/govqtdvno.sHtML

TS:   Object.entries(obj)
来源：http://blog.bbcook.cn/Article/details/gaboflujp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.bbcook.cn/Article/details/gncbwuamu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.yfazqb.com/Article/details/gtzrjingp.sHtML

Ruby: obj.instance_variables
来源：http://baike.fktsv.cn/Article/details/gkyjtiikx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/ggnzzsbfy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnqahylja.sHtML

H. 异常与错误处理
来源：http://www.m.share.vehdjk.com/Article/details/ghrntzyjg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggjzyjnpd.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gsoztmhhz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.vehdjk.com/Article/details/gkwfdroqn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.vehdjk.com/Article/details/gnubedzzg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.yfazqb.com/Article/details/gebcqjiah.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gifhqxnxs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.yfazqb.com/Article/details/geatjkmwh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.yfazqb.com/Article/details/gvyplogir.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.sjlbkw.cn/Article/details/gngejowjz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.bbcook.cn/Article/details/ghiuordnr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fktsv.cn/Article/details/geiwjepdo.sHtML


<!-- 参考信息 -->