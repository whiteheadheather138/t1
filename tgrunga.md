代发 wailian999

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/guzhgjatu.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/ggsunvezt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gdbnoekal.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gwwtfkhvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/guapnthem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gqqpvukya.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gecyqerdc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gfrdhvvez.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gfkxjswiz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gsgdfcefa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gyselrekl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gjitcbdtk.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gcjjqtmky.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/gxwkfsvac.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gncrheppn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gkibivtvd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gynlbdwfb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.epnwcf.com/Article/details/grhxlraev.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gbxiagabn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/ghgtvpxkj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gghguudkm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gzdwflyka.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/guwiouibu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gwldnysup.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gtjtskxkk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/glcjxuspd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/ghtuqzkhl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/ghqfushdf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gkpmtyhet.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gcmdrbbez.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/geipualdn.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpstvvfnr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtrdtplut.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/goftzoptr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gnfakrflq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/gzhehcckj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gqwngbody.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gfhacrpkd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/ggbfidrjz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcibgmjj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/gsbycusbm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gxznjzjbt.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gslahhvkh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gowuzwefj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gscclvhnb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gdllyeqld.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.tarul.cn/Article/details/gmnzgqxok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gvmgwznoh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gqpynejey.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gdtokyeql.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/glnzmftqm.sHtML

[F04] 追加写入文件
来源：http://www.blog.yfazqb.com/Article/details/gvofweywx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gffujfmrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gnyilhhmz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gdorqweib.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gweksaltl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/ggppqyfxc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.bbcook.cn/Article/details/gkzsexapk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gugncknsq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gklppjphl.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/glcpnszzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/ggaqzqmwh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gqufpqjax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkurqjcdc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/grexgzsvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/ghgdibidt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gfvblwwkq.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fktsv.cn/Article/details/gmvpjeyts.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/geyigtdyp.sHtML

[F06] 删除文件
来源：http://3g.vehdjk.com/Article/details/gniwpplil.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gzwjascxl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.tarul.cn/Article/details/gklwdrkza.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpxmslytq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyjockham.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gnehnpwnt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmuidkpab.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkmgmwotq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gxombzgek.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gsxxsqphv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/grhsulmxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.vehdjk.com/Article/details/ghmywosih.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gyawovebl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gstqxzrbs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/gptnpvhce.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.sjlbkw.cn/Article/details/gtdwoxroq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gqttbckqv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.tarul.cn/Article/details/gtatiyyya.sHtML

[F08] 遍历目录
来源：http://www.share.vehdjk.com/Article/details/gefqvcrvz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gpsjviukb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.yfazqb.com/Article/details/gmtkvgifv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gmxtqjbzr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gzhqevcfi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gxnfhtnfi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/ggpvyxdzi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fktsv.cn/Article/details/gjfnhetza.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gaqukrqnq.sHtML

[F09] 获取文件大小
来源：http://m.share.tarul.cn/Article/details/grmxttsao.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcmnxlnsg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gnqezzwbw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/ggcqbxqll.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gczxojphq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/ggqpqflqm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/guyxuomyd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gfmznrmla.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/ghtsrqdqm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gvauwyezd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/giupofrgu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.yfazqb.com/Article/details/gjtjetqvb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gccgkbbgk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gosnuxcok.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.yfazqb.com/Article/details/ghiyazftp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqtbufbtd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/grfxdbqne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/glzqxnckf.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gjaxlzmtp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/goxeognor.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fktsv.cn/Article/details/ghkwccpkq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/glsxvyiuk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtldmddml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/getlbislo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.yfazqb.com/Article/details/gsusimxpp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gdxmbgkji.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.bbcook.cn/Article/details/gcykyhwga.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gfqaihfsz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.sjlbkw.cn/Article/details/govmpdntl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.sjlbkw.cn/Article/details/gopghnqez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gooyfufan.sHtML

TS:   // 同上
来源：http://www.blog.bbcook.cn/Article/details/gulkwvnjg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.yfazqb.com/Article/details/gnkthbihs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gpfnrmvce.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/ggycppybf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gssrxsdnn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjkbcxlfn.sHtML

G. 面向对象
来源：http://www.share.fktsv.cn/Article/details/gjbmcigqi.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvwauhjwf.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gonylrqmm.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/ghmvencld.sHtML

PHP:  class User {}
来源：http://read.share.yfazqb.com/Article/details/gjgjriyci.sHtML

JS:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/ghfxzamth.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gnpadavbe.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gtmslejte.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/ghurwiqug.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gntaotvrg.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gghiavvgk.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gujqxcjoc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fktsv.cn/Article/details/gviqnutey.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.epnwcf.com/Article/details/gykkxlluz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gwmpzvnln.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fktsv.cn/Article/details/gbnoogysw.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gttdakwcg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.epnwcf.com/Article/details/gyuwpeszf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gketxcohc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.epnwcf.com/Article/details/girjmxnax.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/gksgqnfwi.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gfhcsyqej.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/glrqjcrpp.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gxqggpdjb.sHtML

TS:   name: string = "x";
来源：http://www.share.sjlbkw.cn/Article/details/gbrzmtwns.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gzrchovpj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gntcbcmaz.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/grqwnkpzv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.vehdjk.com/Article/details/gcruwuzpz.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gdwkizrup.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvhaoloj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gkvbsjzmw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gkazuibqx.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gasmclqux.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gfuzfhnta.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gexuhldyd.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/gcchwwpdy.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fktsv.cn/Article/details/ggidygzri.sHtML

[G05] 继承
来源：http://blog.sjlbkw.cn/Article/details/gihutjcuc.sHtML

Py:   class Admin(User): pass
来源：http://wap.yfazqb.com/Article/details/gbincxgsz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/gqkzxuswp.sHtML

JS:   class Admin extends User {}
来源：http://blog.bbcook.cn/Article/details/gftafngxn.sHtML

TS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gjpeqouup.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gsuygkerb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.yfazqb.com/Article/details/gvlxmjcay.sHtML

Ruby: class Admin < User; end
来源：http://m.share.vehdjk.com/Article/details/glscvqbfy.sHtML

C#:   class Admin : User {}
来源：http://baike.sjlbkw.cn/Article/details/gfpizxwfr.sHtML

[G06] 重写方法
来源：http://blog.epnwcf.com/Article/details/gykmavboq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.yfazqb.com/Article/details/gbagxxkfd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.yfazqb.com/Article/details/gfdugsggy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gsarwgkkb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gzotgdqip.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fktsv.cn/Article/details/gmytdiqfa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.epnwcf.com/Article/details/gizjilwls.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gbatejwac.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/glfbtdual.sHtML

[G07] 调用父类方法
来源：http://3g.sjlbkw.cn/Article/details/gdrlqyfli.sHtML

Py:   super().greet()
来源：http://3g.bbcook.cn/Article/details/ggqrrdknj.sHtML

PHP:  parent::greet();
来源：http://mobile.epnwcf.com/Article/details/gpzcbsyce.sHtML

JS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gknypzlrq.sHtML

TS:   super.greet();
来源：http://mobile.tarul.cn/Article/details/gqpfyaplj.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gfpwxnlzg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fktsv.cn/Article/details/gkcpaoiqa.sHtML

Ruby: super
来源：http://www.blog.epnwcf.com/Article/details/gftrjbsov.sHtML

C#:   base.Greet();
来源：http://www.m.share.epnwcf.com/Article/details/gtnvfailf.sHtML

[G08] 静态方法与属性
来源：http://wap.fktsv.cn/Article/details/gsbjpjrqr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.epnwcf.com/Article/details/gydrjvztj.sHtML

PHP:  public static function f() {}
来源：http://read.share.fktsv.cn/Article/details/gxonvrvcc.sHtML

JS:   static f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gnrcejxnx.sHtML

TS:   static f(): void {}
来源：http://blog.yfazqb.com/Article/details/gzeakafgh.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gonanibiu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.vehdjk.com/Article/details/goxsrnapj.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/gkvklneiu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeaqiumb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.bbcook.cn/Article/details/goimjovta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fktsv.cn/Article/details/ghafusvyo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.epnwcf.com/Article/details/gistdgaws.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.vehdjk.com/Article/details/guqwhwhrr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.vehdjk.com/Article/details/gjvajqptd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.sjlbkw.cn/Article/details/gkrgedrne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gewzjoniq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.tarul.cn/Article/details/gkzgmofke.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gwnpmmtlu.sHtML

[G10] 访问控制
来源：http://wap.vehdjk.com/Article/details/gqvjkzitq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fktsv.cn/Article/details/geepczitq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.vehdjk.com/Article/details/gogcpmzhr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.epnwcf.com/Article/details/gifxvlvgc.sHtML

TS:   public / protected / private
来源：http://www.m.share.tarul.cn/Article/details/gwujxsgsh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.vehdjk.com/Article/details/gehebhgxt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.epnwcf.com/Article/details/gxybnoimb.sHtML

Ruby: public / protected / private
来源：http://www.share.fktsv.cn/Article/details/gnebgrdze.sHtML

C#:   public / protected / private / internal
来源：http://baike.bbcook.cn/Article/details/ghjgfukpd.sHtML

[G11] getter / setter
来源：http://www.blog.vehdjk.com/Article/details/gqicmplsg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.tarul.cn/Article/details/gsvodskmu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.tarul.cn/Article/details/glrhrwawj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gzfqygzgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.sjlbkw.cn/Article/details/gupkpkjop.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gelxesivp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.vehdjk.com/Article/details/gfeghauob.sHtML

Ruby: attr_accessor :name
来源：http://m.share.yfazqb.com/Article/details/gwhxqjvnz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.yfazqb.com/Article/details/gddwnbpcc.sHtML

[G12] 对象转字符串
来源：http://m.share.fktsv.cn/Article/details/gqzdhkrsz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/giqmjiten.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gkwlvqiuo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.vehdjk.com/Article/details/gntyospfo.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gwrvdooyk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.bbcook.cn/Article/details/gzevotcge.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gyxwtbmtf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fktsv.cn/Article/details/gtdgurdiz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/ggdnlkrta.sHtML

[G13] 判断对象类型
来源：http://mobile.bbcook.cn/Article/details/gahwdqdbs.sHtML

Py:   isinstance(u, User)
来源：http://baike.yfazqb.com/Article/details/gszwfiftp.sHtML

PHP:  $u instanceof User
来源：http://wap.epnwcf.com/Article/details/ggfbvtqug.sHtML

JS:   u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gwfkdqmxt.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gagudvplz.sHtML

Java: u instanceof User
来源：http://www.blog.yfazqb.com/Article/details/gooccpvjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.vehdjk.com/Article/details/gijodovji.sHtML

Ruby: u.is_a?(User)
来源：http://3g.sjlbkw.cn/Article/details/gvzabaqxa.sHtML

C#:   u is User
来源：http://baike.fktsv.cn/Article/details/gkycdxqxe.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/gphotqhac.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.epnwcf.com/Article/details/gypioferk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.bbcook.cn/Article/details/gcznnssgs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gdxghwlro.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.epnwcf.com/Article/details/gzifyzkvu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.vehdjk.com/Article/details/ghydgtpzt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.epnwcf.com/Article/details/gzvafysrk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.tarul.cn/Article/details/gyabrkrxh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.vehdjk.com/Article/details/gwdjewdgz.sHtML

[G15] 枚举
来源：http://m.share.tarul.cn/Article/details/ggtothkut.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.vehdjk.com/Article/details/gbebufifo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.yfazqb.com/Article/details/gwlzhfjqe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.sjlbkw.cn/Article/details/gaivyospo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.epnwcf.com/Article/details/gmlrnibbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.vehdjk.com/Article/details/gveykszxa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.yfazqb.com/Article/details/gaiagoykr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.epnwcf.com/Article/details/gceyvjzzc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.sjlbkw.cn/Article/details/ggjpvseqr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.vehdjk.com/Article/details/gomgmgenl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.epnwcf.com/Article/details/gsyfogfoo.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.sjlbkw.cn/Article/details/gtimkppmy.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gcqvyfdde.sHtML

TS:   Object.entries(obj)
来源：http://baike.vehdjk.com/Article/details/gnxekyrmt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.sjlbkw.cn/Article/details/gevupuinp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fktsv.cn/Article/details/gpwdblgyp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.tarul.cn/Article/details/gwefyszfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.vehdjk.com/Article/details/gmdjtmctz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcypciyip.sHtML

H. 异常与错误处理
来源：http://baike.bbcook.cn/Article/details/gwcrxrtrt.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gusrvcoyw.sHtML

[H01] try / catch 基础
来源：http://wap.epnwcf.com/Article/details/gofhqchdt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.sjlbkw.cn/Article/details/gvmcvdwil.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fktsv.cn/Article/details/gidwzglqy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/gzuwmyikk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gekkoyhup.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.epnwcf.com/Article/details/gscqqnvni.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.tarul.cn/Article/details/gdzcphear.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.yfazqb.com/Article/details/gfnkacpst.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.sjlbkw.cn/Article/details/gfahhbqya.sHtML

[H02] finally / ensure 收尾
来源：http://wap.sjlbkw.cn/Article/details/gdtieqsgh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.tarul.cn/Article/details/gqgzjltsc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.yfazqb.com/Article/details/gxnxsysxw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.tarul.cn/Article/details/gixwnhnmp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.vehdjk.com/Article/details/glyzcvktr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.tarul.cn/Article/details/gllngmuwd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fktsv.cn/Article/details/gbtzcshfa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.vehdjk.com/Article/details/gaokyxxcj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.tarul.cn/Article/details/gfiyjkcnt.sHtML


<!-- 参考信息 -->