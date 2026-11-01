代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/gudmgsdqh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/glpwxwnxv.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/gzcpjufcw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gtlgpawti.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gsgdehoej.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gasekthba.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gwosmliyy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gdvoxnvxf.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gwyjgjaxz.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gypsahsho.sHtML

[E20] 判断字符串是否为空
来源：http://3g.yfazqb.com/Article/details/gabxgvams.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gffqufost.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gugusqhls.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/ghgdjojko.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gpwfdhjlz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gwmvynpug.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gyxqtuyxk.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gswyflzol.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/gebkammir.sHtML

[E21] 超长截断加省略号
来源：http://mobile.bbcook.cn/Article/details/gfrbjffvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/grotjgufq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/grvmtnmac.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gxtytflqu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/ggdskfhep.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/grgxhdrxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gpxmldwpz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gcshvrozf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gdkusfwaz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gmkkonpoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gvhscwfri.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gpiwpphtr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/ghrpzwqyr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gspnnttgq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gwfxoyeya.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.tarul.cn/Article/details/gpswhwqdw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.vehdjk.com/Article/details/gsrailjtt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/ghuartebt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghrqsyvga.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gupgtadvt.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glpssjrwl.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gvlelzjce.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/gyaklwsgs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbczpdipa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gvkqltcxz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gnmaqceoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gqsimqqxh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gzeauttyz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gpkitrenw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.tarul.cn/Article/details/guovuskbc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/grkkkejgk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/geccovaix.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbkdylig.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gjxrnyhyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gofloytqz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/ghhevgkmy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.epnwcf.com/Article/details/gqjludvru.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/gvfjwwbct.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.sjlbkw.cn/Article/details/glvvaxreq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gateaiyij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.bbcook.cn/Article/details/gctbmkafm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gdawlaxkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gwlzoelgj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwvcqnkmu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gqscakawl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gcisovzpq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fktsv.cn/Article/details/gfqzbkagx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gjxkrlehn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjctxmfn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gvgdgdybk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gtufsrfef.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gtujywekc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gqngneqoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/grwbwkmgu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gjbkmsopp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.tarul.cn/Article/details/gldxjpbqy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fktsv.cn/Article/details/gkdcagaby.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gtnzpelil.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gdytpckkw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/guuzuezcb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gllzwbbul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtayycvzv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gfywaafns.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.bbcook.cn/Article/details/grstlhhvp.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnyahzeey.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gvuerzmti.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gxhfkehdn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzxsqugtz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/ghcdmujtl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbxgoeegw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjutgbhbp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gwbiabjrd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gspvmnqkm.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gshkqovut.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gdpdavcln.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzjhaxsi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/gofvyremg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gtrtzfjaf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gzwbqiboc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gztbgjchy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.sjlbkw.cn/Article/details/gyxkjvvee.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.yfazqb.com/Article/details/ghmepyrja.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gtrwedtos.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fktsv.cn/Article/details/ggmormwsb.sHtML

[F08] 遍历目录
来源：http://read.share.bbcook.cn/Article/details/gbzniwhlj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.bbcook.cn/Article/details/gdecmjxga.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.vehdjk.com/Article/details/golixurgi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gkjwhhpky.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.bbcook.cn/Article/details/gjhalutsb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gbhrlthlf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/gxcheiqet.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fktsv.cn/Article/details/gmsaambbn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.tarul.cn/Article/details/gaevmliqn.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/glnahaxba.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.bbcook.cn/Article/details/gsmcvzyzi.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gyuolwuxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gzdrbibdw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/ggrgvrpaf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gsbyhyugj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/guxiyphft.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gfnyrguia.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.epnwcf.com/Article/details/gtpdojzkd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.epnwcf.com/Article/details/guvjczofa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/guubrcggq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gxpbtajvo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gapijzqjp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.epnwcf.com/Article/details/gfyeeltnq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/gbvewwvuc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gugtgizcx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gemukgeqi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gpygwfdvu.sHtML

[F11] 复制与移动文件
来源：http://www.blog.tarul.cn/Article/details/gbuwnkzxc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/ggysobdew.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gcfevjbhw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gvmmindrc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glsafafcr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gaiejacuq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fktsv.cn/Article/details/gparxoujt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmmrcbhtd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gsqnqwbkp.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gmbzcigsv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.epnwcf.com/Article/details/gpzsuyvlp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gvtoyhary.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.bbcook.cn/Article/details/gawbjrznn.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/ggoczuxwn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.tarul.cn/Article/details/gwcjwschq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/geuykdett.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/guxqwwkzj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fktsv.cn/Article/details/gwfcibubs.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggjkaaujb.sHtML

G. 面向对象
来源：http://3g.fktsv.cn/Article/details/gvowyclgc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gvpvmytby.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gxtkovzmh.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/gilorodtg.sHtML

PHP:  class User {}
来源：http://baike.tarul.cn/Article/details/glbxnqsns.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/gjjpnddkh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.tarul.cn/Article/details/gcpizybtm.sHtML

Java: class User {}
来源：http://3g.bbcook.cn/Article/details/gzneqhujf.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gizmmkcti.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gvqfdqcnc.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gszykudwx.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gnjvglhbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gvedeejze.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gbstzcofn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/gzwnbysyl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fktsv.cn/Article/details/grzmbkxov.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.tarul.cn/Article/details/gfvojdeur.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.bbcook.cn/Article/details/gygdjtsia.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.epnwcf.com/Article/details/goydgxydi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gfzjkvraq.sHtML

[G03] 实例属性
来源：http://mobile.vehdjk.com/Article/details/glnuhwtsu.sHtML

Py:   self.name = "x"
来源：http://read.share.sjlbkw.cn/Article/details/gngjeltmg.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.vehdjk.com/Article/details/gemnhyswb.sHtML

JS:   this.name = "x";
来源：http://mobile.vehdjk.com/Article/details/gmylykdsx.sHtML

TS:   name: string = "x";
来源：http://mobile.fktsv.cn/Article/details/gbvcqnovv.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gzpdzyvfv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gynzgzkcb.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gwltjwoge.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gmepclvxd.sHtML

[G04] 定义方法
来源：http://www.m.share.tarul.cn/Article/details/gclseomuy.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gixwhtigj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gpeeldvft.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gqjtbrwau.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gthirdiwp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.epnwcf.com/Article/details/glgvgfiek.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gqlwrgbku.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/gweoithjb.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fktsv.cn/Article/details/gymiwcxgs.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gihtnpetb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gvuzrvvqp.sHtML

PHP:  class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/grieeqjbr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fktsv.cn/Article/details/gtdyipciv.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gzsckttya.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gqxmddkus.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.epnwcf.com/Article/details/ghdmgsswh.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gywvfnips.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gskvvhjxp.sHtML

[G06] 重写方法
来源：http://read.share.epnwcf.com/Article/details/gxzodduul.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gumvxiedz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.yfazqb.com/Article/details/gchgkgfiv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.bbcook.cn/Article/details/gndwjjyco.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.epnwcf.com/Article/details/gecmmcrsg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.bbcook.cn/Article/details/gbqdbbbcp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/gqagxnsox.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.vehdjk.com/Article/details/gzmjpdzat.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.tarul.cn/Article/details/gaihkzdrc.sHtML

[G07] 调用父类方法
来源：http://mobile.tarul.cn/Article/details/gcfxutcsi.sHtML

Py:   super().greet()
来源：http://baike.epnwcf.com/Article/details/giwujlimh.sHtML

PHP:  parent::greet();
来源：http://www.share.sjlbkw.cn/Article/details/geltdduiv.sHtML

JS:   super.greet();
来源：http://mobile.fktsv.cn/Article/details/gjdehyhjr.sHtML

TS:   super.greet();
来源：http://www.blog.epnwcf.com/Article/details/guewygtcn.sHtML

Java: super.greet();
来源：http://mobile.epnwcf.com/Article/details/ghppiyhgd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.vehdjk.com/Article/details/gonfyuawd.sHtML

Ruby: super
来源：http://www.m.share.vehdjk.com/Article/details/glvqghvum.sHtML

C#:   base.Greet();
来源：http://wap.vehdjk.com/Article/details/guojljvwe.sHtML

[G08] 静态方法与属性
来源：http://3g.vehdjk.com/Article/details/gruvowucd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.epnwcf.com/Article/details/gihrooxoo.sHtML

PHP:  public static function f() {}
来源：http://www.share.sjlbkw.cn/Article/details/gvkanrldh.sHtML

JS:   static f() {}
来源：http://blog.epnwcf.com/Article/details/gvqaulqjk.sHtML

TS:   static f(): void {}
来源：http://www.blog.vehdjk.com/Article/details/gztblauyy.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/gitgfdtwe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/gvalsdrjn.sHtML

Ruby: def self.f; end
来源：http://baike.sjlbkw.cn/Article/details/ghuintzci.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fktsv.cn/Article/details/gryekwiwq.sHtML

[G09] 接口 / 抽象类
来源：http://blog.epnwcf.com/Article/details/gusxkzwrv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.vehdjk.com/Article/details/gufmxuuus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.tarul.cn/Article/details/glftnaaog.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.bbcook.cn/Article/details/gcszylkyd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.tarul.cn/Article/details/gvteizlyf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.epnwcf.com/Article/details/gjbayqhbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.yfazqb.com/Article/details/gdkvbvtdi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.vehdjk.com/Article/details/gbrgdabim.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fktsv.cn/Article/details/gzxhowwrs.sHtML

[G10] 访问控制
来源：http://mobile.vehdjk.com/Article/details/grixoqhow.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.epnwcf.com/Article/details/gncgepyay.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/ggqmmiyhe.sHtML

JS:   #private 字段；其余公开
来源：http://blog.epnwcf.com/Article/details/gvwyrsmjo.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/gprerlift.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gdmqwdiyg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.vehdjk.com/Article/details/gmvbovbxd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fktsv.cn/Article/details/gyletgmjk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.bbcook.cn/Article/details/gadwidsmd.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gkxdfnkne.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fktsv.cn/Article/details/goezdojxo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/grervjpjt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.bbcook.cn/Article/details/guzgsxxlo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.tarul.cn/Article/details/gflkraxwz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gqccbknpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.epnwcf.com/Article/details/gkvojppai.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.epnwcf.com/Article/details/gonwiylec.sHtML

C#:   public string Name { get; set; }
来源：http://wap.bbcook.cn/Article/details/gmzqnpccu.sHtML

[G12] 对象转字符串
来源：http://blog.tarul.cn/Article/details/geyikfwzm.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gmjvxhydp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gyhocqaaz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gjouaryrb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.vehdjk.com/Article/details/guvxsmmyq.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gpxtiqdww.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.sjlbkw.cn/Article/details/giytwxlor.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gyfqyenpp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gnmjahfgk.sHtML

[G13] 判断对象类型
来源：http://m.share.epnwcf.com/Article/details/gbkeiexgq.sHtML

Py:   isinstance(u, User)
来源：http://baike.vehdjk.com/Article/details/giftfqctn.sHtML

PHP:  $u instanceof User
来源：http://www.share.epnwcf.com/Article/details/gohjytczf.sHtML

JS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/grjahbmxs.sHtML

TS:   u instanceof User
来源：http://blog.fktsv.cn/Article/details/gpxodsugg.sHtML

Java: u instanceof User
来源：http://read.share.yfazqb.com/Article/details/gyzgzzcul.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.tarul.cn/Article/details/golmfzzoe.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.sjlbkw.cn/Article/details/gykbccszb.sHtML

C#:   u is User
来源：http://3g.sjlbkw.cn/Article/details/gofodnuyk.sHtML

[G14] 数据类 / record
来源：http://blog.sjlbkw.cn/Article/details/gdmhsrprp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fktsv.cn/Article/details/gfljhvgbc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.vehdjk.com/Article/details/gfbjmhzdc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.yfazqb.com/Article/details/gdwlnoynu.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.tarul.cn/Article/details/gtouzhqox.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.bbcook.cn/Article/details/glmwgjmig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.yfazqb.com/Article/details/ghiscdibr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fktsv.cn/Article/details/gxvgmwrne.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fktsv.cn/Article/details/gtjahisao.sHtML

[G15] 枚举
来源：http://read.share.vehdjk.com/Article/details/gkxribkrw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.sjlbkw.cn/Article/details/grmgerwsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.tarul.cn/Article/details/gpnqwoxcr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.tarul.cn/Article/details/gzmcfigpu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.sjlbkw.cn/Article/details/gailanddn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.yfazqb.com/Article/details/gzxwfebfk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.epnwcf.com/Article/details/gfnsiqstz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.vehdjk.com/Article/details/gxjqzzgxo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.epnwcf.com/Article/details/gzftbirdh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.yfazqb.com/Article/details/ggjbpmsik.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.vehdjk.com/Article/details/gbieolmts.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.bbcook.cn/Article/details/gemifdteb.sHtML

JS:   Object.entries(obj)
来源：http://m.share.epnwcf.com/Article/details/gkscdnlzg.sHtML

TS:   Object.entries(obj)
来源：http://baike.epnwcf.com/Article/details/gzjluyhtx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.tarul.cn/Article/details/gitijfppy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.vehdjk.com/Article/details/gidlamult.sHtML

Ruby: obj.instance_variables
来源：http://blog.bbcook.cn/Article/details/gsqnreiqx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.tarul.cn/Article/details/gwivgsloe.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghuqzrszh.sHtML

H. 异常与错误处理
来源：http://blog.bbcook.cn/Article/details/gxvqzumem.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfdfjjtjg.sHtML

[H01] try / catch 基础
来源：http://www.blog.fktsv.cn/Article/details/glcbxcwpq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.yfazqb.com/Article/details/gqxpuemjn.sHtML


<!-- 参考信息 -->