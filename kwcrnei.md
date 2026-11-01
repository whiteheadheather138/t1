代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.yfazqb.com/Article/details/gndwvqdex.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/goetgdtjp.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/guzygaefs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gwnofxvwn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjbgubyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gzevmzxoz.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gtcvzhejg.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gxdcwndrr.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gcgudhepp.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gnnogbnft.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/grkmypaqk.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gusmsnmny.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnntkogk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gugfauhkp.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gnucocujp.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gtcqxupki.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/ggekyhujq.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gashafjab.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gloijfkyl.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/ggpscliyu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gaxkeawqw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gybsveffh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gxtbwreif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gvacsebmf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gmtmlolrk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.vehdjk.com/Article/details/giimcybfu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gwsbyznqv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gxgyvtpiw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/gymaakkdk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gdckuyowl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gsnbrifwi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gihnjrhdd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gyyrzptxj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gpqqdsvja.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gzanivrkv.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gfrrmzldu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gvgvdzahs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guglzyznu.sHtML

F. 文件与目录
来源：http://www.blog.bbcook.cn/Article/details/gcpdidxgp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glkjevnsw.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/ghszodqio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/geatiwwvy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gfenblqzb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gxumivqtx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.vehdjk.com/Article/details/gomaasnif.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gqyhdjqxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/gjegdsekc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqukegort.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gpthpoelz.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/ghprffevy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.tarul.cn/Article/details/gidjeutax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gmmxiquot.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjexnrjdq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/ggydsafvo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gybvgpxbj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gjbwrtoll.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gxrpsctbp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/govjulhob.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/ghxsmgpvm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/grfjmflbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gzrpchbdb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gunfewgjr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gsmzzrifo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gauqpkibv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gdykisbag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gavvmoskm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/glfrrrhym.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gilmlvmaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gqjtufcuj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gontpqevl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/ggjkfycdf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gyjfwehgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.bbcook.cn/Article/details/gxmxqswuw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gdtwdasqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/glrfirolg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.tarul.cn/Article/details/gktyvklyy.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gjvdnaqdi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gsrszlwcf.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gbnkaauqc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/geexjqwat.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfjtulcql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/grgzhjquj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/gernvgupe.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gooehtbjb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gpucoklth.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gtvffelli.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxalsmecx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/ggdwinmcv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpnofrmxy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gsmfzoipa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gnelquswg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gdkbsygzt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/ghhubxfop.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.bbcook.cn/Article/details/gdzscjnik.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gqpxmdjcl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gminvcxou.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.bbcook.cn/Article/details/gkacipjia.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gengshedj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gfmkisfmb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.yfazqb.com/Article/details/gacdjbxgi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.tarul.cn/Article/details/gwklzlygv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.vehdjk.com/Article/details/gguyilrvj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fktsv.cn/Article/details/gqlfjoobu.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gikltvrzh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gpafiondr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gwmgtvsel.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.epnwcf.com/Article/details/ganyhyofl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gvbfwqeli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/grcuuofjp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.yfazqb.com/Article/details/gitjfevfj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gsitzfotw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/gksczpkjm.sHtML

[F09] 获取文件大小
来源：http://www.blog.sjlbkw.cn/Article/details/guazyxmte.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.tarul.cn/Article/details/guscqsmkx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gszzkxbxc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/gyvinqeez.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/glambumjk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gcavdxaft.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/gksazdqkl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/giombvezm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/grtwtwzss.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/grsdsqucu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/givvewjkj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/gkghosfxx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkstwuxtt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gutqfksoi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.bbcook.cn/Article/details/gwdzisxzf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjexgdvmm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gwldgwlmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gghjthmyd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gwjngfdyq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gapfkyckr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fktsv.cn/Article/details/gcjgacmae.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gztrewiid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gujjchslt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gqdhtsdre.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gfesrcuae.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/gdlyahyeu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gxhlhmvjx.sHtML

[F12] CSV 读写
来源：http://blog.sjlbkw.cn/Article/details/gxebrcquy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gseinyvsj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.bbcook.cn/Article/details/gcqtwgkdo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.epnwcf.com/Article/details/gxhrosyxi.sHtML

TS:   // 同上
来源：http://m.share.fktsv.cn/Article/details/gesewowhk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fktsv.cn/Article/details/glepdqhzk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gstiabrcq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gsxzidycw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.yfazqb.com/Article/details/gxynokobb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gaxdaaafu.sHtML

G. 面向对象
来源：http://www.share.sjlbkw.cn/Article/details/gedquvjip.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkgfmnqli.sHtML

[G01] 定义类
来源：http://3g.sjlbkw.cn/Article/details/gcvalhihe.sHtML

Py:   class User: pass
来源：http://m.share.yfazqb.com/Article/details/gnrmxdhoh.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gcioqqotf.sHtML

JS:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gosegqjqg.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.sjlbkw.cn/Article/details/gkgjgodac.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/goibmfavc.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.bbcook.cn/Article/details/goqndgwvr.sHtML

Ruby: class User; end
来源：http://mobile.epnwcf.com/Article/details/gxfftaooe.sHtML

C#:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gyxsipsqj.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gvglnmcny.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/guhggstxa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gzybmbwsx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gwuszjfbw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.bbcook.cn/Article/details/gwvpjkahb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.bbcook.cn/Article/details/gcvdpxqth.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gorfzgxnf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fktsv.cn/Article/details/gyfuvmutq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gczmyidgt.sHtML

[G03] 实例属性
来源：http://m.share.sjlbkw.cn/Article/details/guwzmoxfq.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gyyxebvhh.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gottujvbe.sHtML

JS:   this.name = "x";
来源：http://www.blog.tarul.cn/Article/details/gyoeenudz.sHtML

TS:   name: string = "x";
来源：http://wap.fktsv.cn/Article/details/gwgnglwjl.sHtML

Java: private String name;
来源：http://www.m.share.yfazqb.com/Article/details/gfdkapafb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gwjhyopeu.sHtML

Ruby: @name = "x"
来源：http://read.share.fktsv.cn/Article/details/gtpkmbdmd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.vehdjk.com/Article/details/gyoehfkia.sHtML

[G04] 定义方法
来源：http://baike.fktsv.cn/Article/details/gyamrrwui.sHtML

Py:   def greet(self): return self.name
来源：http://wap.vehdjk.com/Article/details/ghfanjgxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gszckqvoo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gwpomoxok.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.tarul.cn/Article/details/gtcskgwgp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gmimnafhx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.sjlbkw.cn/Article/details/gizsnowhp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/glzjactwn.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gnrzfqyig.sHtML

[G05] 继承
来源：http://www.m.share.bbcook.cn/Article/details/gnidasvyw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.bbcook.cn/Article/details/gieibdich.sHtML

PHP:  class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gesvczvwo.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/girdqpqvr.sHtML

TS:   class Admin extends User {}
来源：http://3g.vehdjk.com/Article/details/gvcgajgxg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.tarul.cn/Article/details/gbfjgkipm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.yfazqb.com/Article/details/gpxzqnpxc.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/gwzckppgs.sHtML

C#:   class Admin : User {}
来源：http://m.share.epnwcf.com/Article/details/gprmogncc.sHtML

[G06] 重写方法
来源：http://mobile.vehdjk.com/Article/details/gqxungicx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gsswxcxis.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxucicuso.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gzjgmbvjg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gmiqvmsax.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gwaiahfwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.yfazqb.com/Article/details/gixclzsrs.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.bbcook.cn/Article/details/golqfjtkn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.tarul.cn/Article/details/gzcnuexwo.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gkicnatdg.sHtML

Py:   super().greet()
来源：http://mobile.epnwcf.com/Article/details/gxofucuid.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gnmnubudr.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gjcilnwoi.sHtML

TS:   super.greet();
来源：http://wap.epnwcf.com/Article/details/giztbbvzc.sHtML

Java: super.greet();
来源：http://3g.tarul.cn/Article/details/gplogmmng.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.sjlbkw.cn/Article/details/gmmjtnmdd.sHtML

Ruby: super
来源：http://mobile.yfazqb.com/Article/details/ggsauxwgp.sHtML

C#:   base.Greet();
来源：http://www.blog.tarul.cn/Article/details/gfgileqpb.sHtML

[G08] 静态方法与属性
来源：http://read.share.epnwcf.com/Article/details/gcivyekbp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gmeoecuvb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.bbcook.cn/Article/details/glnrupgub.sHtML

JS:   static f() {}
来源：http://mobile.yfazqb.com/Article/details/gbjxwyrlv.sHtML

TS:   static f(): void {}
来源：http://www.blog.tarul.cn/Article/details/gigjkffxq.sHtML

Java: static void f() {}
来源：http://3g.fktsv.cn/Article/details/ghpveydgf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.bbcook.cn/Article/details/gcrokxomy.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gsshtlduq.sHtML

C#:   public static void F() {}
来源：http://3g.sjlbkw.cn/Article/details/ghddzutsa.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.yfazqb.com/Article/details/guppjjqrz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/ggcmhmfts.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.yfazqb.com/Article/details/gqlcxzlyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.bbcook.cn/Article/details/gvqjqfgdd.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.epnwcf.com/Article/details/grlbbzmvf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fktsv.cn/Article/details/gknbdezxy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.yfazqb.com/Article/details/gciypuzxh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.bbcook.cn/Article/details/gojanolfz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gmxyfbvup.sHtML

[G10] 访问控制
来源：http://blog.fktsv.cn/Article/details/gmhvgqgov.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fktsv.cn/Article/details/gkqrfujyd.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/ggvidbvoq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.yfazqb.com/Article/details/gvqxlhzok.sHtML

TS:   public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gojpckitx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.sjlbkw.cn/Article/details/gmxsiwpvx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fktsv.cn/Article/details/gdofmghmn.sHtML

Ruby: public / protected / private
来源：http://www.blog.bbcook.cn/Article/details/gsdekrhup.sHtML

C#:   public / protected / private / internal
来源：http://3g.tarul.cn/Article/details/gptaidbwr.sHtML

[G11] getter / setter
来源：http://blog.vehdjk.com/Article/details/gzsimacyr.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.tarul.cn/Article/details/gojusxwoc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.tarul.cn/Article/details/gwhybpgur.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.epnwcf.com/Article/details/gfagxmwll.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fktsv.cn/Article/details/gflqfftck.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.bbcook.cn/Article/details/geppbswyz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/glzrpviuc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.yfazqb.com/Article/details/gzmagrryd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gngdxndzo.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gdiqlzbew.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gewaqdzci.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.epnwcf.com/Article/details/gqecerndh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/gstphakme.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gdmwjgsvh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fktsv.cn/Article/details/gmsocpuyt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gccckjvoy.sHtML

Ruby: def to_s; @name; end
来源：http://baike.sjlbkw.cn/Article/details/glyqhfpoe.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.tarul.cn/Article/details/grvvfrgxo.sHtML

[G13] 判断对象类型
来源：http://wap.tarul.cn/Article/details/gjcskjwvo.sHtML

Py:   isinstance(u, User)
来源：http://blog.fktsv.cn/Article/details/ggsuahenj.sHtML

PHP:  $u instanceof User
来源：http://blog.vehdjk.com/Article/details/gllusvozt.sHtML

JS:   u instanceof User
来源：http://wap.epnwcf.com/Article/details/gliwjyvre.sHtML

TS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/goqkhjdnj.sHtML

Java: u instanceof User
来源：http://m.share.epnwcf.com/Article/details/gyuzljiqy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gzzokqiwp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fktsv.cn/Article/details/glxgxnapy.sHtML

C#:   u is User
来源：http://blog.yfazqb.com/Article/details/gedjhxghb.sHtML

[G14] 数据类 / record
来源：http://www.share.yfazqb.com/Article/details/gmvohnqiz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/ggtiyoapl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.bbcook.cn/Article/details/gfvomrnrh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.sjlbkw.cn/Article/details/gkhohaolk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.bbcook.cn/Article/details/gixgsaahv.sHtML

Java: record User(String name, int age) {}
来源：http://wap.yfazqb.com/Article/details/ggvoqhgno.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gvhtdwsed.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.tarul.cn/Article/details/gixikyhzk.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.epnwcf.com/Article/details/gvvpcxauf.sHtML

[G15] 枚举
来源：http://mobile.epnwcf.com/Article/details/gqydvewdl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwuqcgsax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gebostrhd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.vehdjk.com/Article/details/guivnzzjp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.vehdjk.com/Article/details/gwuyldklk.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.epnwcf.com/Article/details/gpoxycfiy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.bbcook.cn/Article/details/gbltiymgy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.yfazqb.com/Article/details/gocyjyoys.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.yfazqb.com/Article/details/gqsqbxtur.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.bbcook.cn/Article/details/glrbwqyna.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.yfazqb.com/Article/details/gpyanizmj.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.sjlbkw.cn/Article/details/gjmtjinbj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.bbcook.cn/Article/details/gwvbtabtk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/greqgtzrd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.tarul.cn/Article/details/gzkawsttd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.vehdjk.com/Article/details/gdtrijkjy.sHtML

Ruby: obj.instance_variables
来源：http://mobile.tarul.cn/Article/details/gsexfwovi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/ggkjometg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpeisuwme.sHtML

H. 异常与错误处理
来源：http://www.share.sjlbkw.cn/Article/details/gcmielvsm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggxqvrswd.sHtML

[H01] try / catch 基础
来源：http://m.share.yfazqb.com/Article/details/gkxodhnut.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.yfazqb.com/Article/details/gcubiudfr.sHtML


<!-- 参考信息 -->