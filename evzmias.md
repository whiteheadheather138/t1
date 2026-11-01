代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gsdalvydf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gvyozplfb.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gbqiqptjn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gbfstxypt.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gnhbpwmkt.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gauqfqolo.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gzblrqeip.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gmlkteigm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gusrvjswc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.bbcook.cn/Article/details/gungcqaef.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gzkuwajho.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdizbsysk.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gvxkyqlhy.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gtwzbkadi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gvpqdpytt.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gvijgayaf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gxgvxvccd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gmvxfvoxt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gyfsetqzo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/ghjgoyvli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gzrjgqivy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gmkxmjpwo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gfcncviyj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gmvuhicrt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gdxehpyeh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gbdkixodb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gosrkykfs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/graiphuix.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzgvorek.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gqeumwuay.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gjxrvzpso.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gwtzqpjfa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/ggjioukgi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gbhgjiemk.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gulbarofz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjehgcova.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gwqkwibgx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gvswcdxtt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/gedonwdwx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/gwvoxcjgr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gjxhxuuqg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gqceyamfu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gmjqwhhey.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gcehiqniy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gmcfeahxm.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gnvugidvb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fktsv.cn/Article/details/gygdybykr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/guzaclutj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gjuvbqsov.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/glheubzvx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgvkyifn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gkvzpdxjn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gulznbaiu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gxvqqcglf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/grmlhidtu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gxlbzzlav.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gmuqapzcl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.tarul.cn/Article/details/gcotjwpfw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gwaunyrjc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.vehdjk.com/Article/details/gyjlgcskz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/ghwdqhbsk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gofioyfgp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/gjawwzqlo.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/giytkaadn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gwfmyyqzf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/goxplryxp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gahpuvmsr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gjvhpptfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gspqtjjyk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gjoiixrou.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fktsv.cn/Article/details/ginpsbjbm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.sjlbkw.cn/Article/details/gbzhegija.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.epnwcf.com/Article/details/gvrjgmiru.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgvpqjtw.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/giefptrfp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdchntdlu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmqhforib.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gwragofcj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gtuxiauls.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/geikslhei.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnuzjcmlm.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gtrtbthfi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjiaybdyy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gypnujeso.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gymukkfpr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmkfodeij.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gsggecspm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gxxogolqo.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gjeywqouk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gwaqxmyfu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.bbcook.cn/Article/details/gwgriqgwu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gxhcvxmrj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gucsbjpry.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gplpuwtnx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gpiunaubc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/guuhmohhp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gayygpqvu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gchsqtgum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gslzdysgu.sHtML

[F08] 遍历目录
来源：http://read.share.fktsv.cn/Article/details/gqzepexjk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gzmtwqpqw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdpffqptp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gsfgrmnzr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gzlsrslcb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gzknwxjph.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gaauomgxk.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gfsfhtgkm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gezefqgey.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gomswpbld.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gfoxstygx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gqdplldle.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gjxujigup.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gdbsixaef.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gcklecsjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gbwkjowei.sHtML

Ruby: File.size("a.txt")
来源：http://wap.tarul.cn/Article/details/gmlvsiqbk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gwudhakuq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.tarul.cn/Article/details/gxcvaldht.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gvauoinaz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/ggxbpllcl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gnxyvjnuv.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ghagatiom.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fktsv.cn/Article/details/gnscwqxrm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxdnivroh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gthypgmyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gqsyfneqc.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gkcgsjkbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gniunevww.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.bbcook.cn/Article/details/gwjrlegrh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gikifbzyj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/guhxrchoi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gafoalscg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gqqiqnlva.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/grupzxjmo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gvicgmsau.sHtML

[F12] CSV 读写
来源：http://www.m.share.yfazqb.com/Article/details/gnomchvta.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmgfdfci.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gdnzovsrd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gbkbxoskh.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gxjzbawju.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/grrfcsgpb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/glzgixesr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/grshblmkx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/ghckrztbw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gxqbysmtw.sHtML

G. 面向对象
来源：http://wap.tarul.cn/Article/details/gotlrqitq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grhperfxn.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/grygxzvaw.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/gzeonnfcf.sHtML

PHP:  class User {}
来源：http://blog.sjlbkw.cn/Article/details/ggbkwlcca.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gtypwxetq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkvattiv.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gfqappthn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fktsv.cn/Article/details/gxrwesubg.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/glzjdcgnu.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/ggeedbbpx.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gicugqrtg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.vehdjk.com/Article/details/gznnzsalo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gwnndefnc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gpyrndjdb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.sjlbkw.cn/Article/details/gqnqatmyn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gkluqewib.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fktsv.cn/Article/details/grqkmsmli.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.sjlbkw.cn/Article/details/giqurguix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmbqxcsbb.sHtML

[G03] 实例属性
来源：http://www.blog.yfazqb.com/Article/details/gtzhpltlv.sHtML

Py:   self.name = "x"
来源：http://baike.sjlbkw.cn/Article/details/gfmmgrzux.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/gybuagycw.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gjaingyqb.sHtML

TS:   name: string = "x";
来源：http://3g.bbcook.cn/Article/details/gntzyryum.sHtML

Java: private String name;
来源：http://blog.epnwcf.com/Article/details/gsxkwoksu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.sjlbkw.cn/Article/details/gebcuwtwf.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gzjmzarmj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.epnwcf.com/Article/details/gdrtenfmk.sHtML

[G04] 定义方法
来源：http://baike.vehdjk.com/Article/details/ggaflunem.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/ganergioa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.sjlbkw.cn/Article/details/gewengwsr.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gdqqukcrc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gnknpqhrt.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/ggywzpway.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gtkdkfskl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.tarul.cn/Article/details/gxpxmbmmo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.sjlbkw.cn/Article/details/gojpzhmif.sHtML

[G05] 继承
来源：http://www.m.share.fktsv.cn/Article/details/gixjodkor.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.yfazqb.com/Article/details/gaflqxhzb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gkevysgrl.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmpyxaf.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gdqyubdce.sHtML

Java: class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/ghgmdsaik.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.sjlbkw.cn/Article/details/gsqgrmadp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.bbcook.cn/Article/details/gndjgawcy.sHtML

C#:   class Admin : User {}
来源：http://mobile.vehdjk.com/Article/details/gkggrlwux.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gnixxpuxa.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.bbcook.cn/Article/details/gsjjezccj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.tarul.cn/Article/details/gjqqisbkl.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.yfazqb.com/Article/details/gqdzzteba.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gnwculyxc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gndgwnynh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.sjlbkw.cn/Article/details/gvduudyrc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.bbcook.cn/Article/details/gwfmdivvp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.sjlbkw.cn/Article/details/gepyxpkvv.sHtML

[G07] 调用父类方法
来源：http://read.share.tarul.cn/Article/details/gvywteypd.sHtML

Py:   super().greet()
来源：http://read.share.fktsv.cn/Article/details/gkfuzjyyr.sHtML

PHP:  parent::greet();
来源：http://mobile.yfazqb.com/Article/details/gfrueldtp.sHtML

JS:   super.greet();
来源：http://mobile.yfazqb.com/Article/details/gyqqtaejx.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gwsqbqqik.sHtML

Java: super.greet();
来源：http://baike.yfazqb.com/Article/details/gqijwxnyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fktsv.cn/Article/details/gsvjqvhno.sHtML

Ruby: super
来源：http://wap.bbcook.cn/Article/details/gjnkzfshh.sHtML

C#:   base.Greet();
来源：http://read.share.vehdjk.com/Article/details/gcrfsbmpz.sHtML

[G08] 静态方法与属性
来源：http://mobile.fktsv.cn/Article/details/gkcxfujhy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fktsv.cn/Article/details/galbrhoek.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gvnipyyds.sHtML

JS:   static f() {}
来源：http://www.blog.vehdjk.com/Article/details/gzknqgphi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fktsv.cn/Article/details/gysmrzvqc.sHtML

Java: static void f() {}
来源：http://wap.sjlbkw.cn/Article/details/gdpdknzoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.vehdjk.com/Article/details/gnofwlyty.sHtML

Ruby: def self.f; end
来源：http://mobile.tarul.cn/Article/details/gwtbsgaoh.sHtML

C#:   public static void F() {}
来源：http://www.blog.yfazqb.com/Article/details/gxwotehdo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gromscvlw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gagrwtavi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.vehdjk.com/Article/details/gmcmlsugl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.sjlbkw.cn/Article/details/gyaopimfw.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.epnwcf.com/Article/details/gwekpjayt.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fktsv.cn/Article/details/gzlvztopo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gphddwixr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.vehdjk.com/Article/details/gpjdjvmde.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.tarul.cn/Article/details/gbolnoqle.sHtML

[G10] 访问控制
来源：http://www.blog.vehdjk.com/Article/details/gxrtkpazj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.yfazqb.com/Article/details/gjhzzoieh.sHtML

PHP:  public / protected / private
来源：http://baike.epnwcf.com/Article/details/gdfxwgmke.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbdqttgv.sHtML

TS:   public / protected / private
来源：http://baike.fktsv.cn/Article/details/gdgdrerot.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.bbcook.cn/Article/details/gsogdlptt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.yfazqb.com/Article/details/gjzanrvmn.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gsftfbyfg.sHtML

C#:   public / protected / private / internal
来源：http://blog.yfazqb.com/Article/details/gszsdvjql.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gbhrscuxl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.sjlbkw.cn/Article/details/gydgzgobl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gtdpovqvh.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.vehdjk.com/Article/details/gowrgcsos.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gbblrlfho.sHtML

Java: public String getName() { return name; }
来源：http://baike.epnwcf.com/Article/details/gnroihsit.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.bbcook.cn/Article/details/gbbciuohr.sHtML

Ruby: attr_accessor :name
来源：http://baike.epnwcf.com/Article/details/givohifyr.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.epnwcf.com/Article/details/gzsnzgafu.sHtML

[G12] 对象转字符串
来源：http://www.share.fktsv.cn/Article/details/gvtlgtayq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.vehdjk.com/Article/details/gjltbeblc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gzkutqfyx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gcwutigty.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/guivbdaqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fktsv.cn/Article/details/gjdhjhuxh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gcxfjqhba.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.tarul.cn/Article/details/gechhssyi.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.sjlbkw.cn/Article/details/gazdfkphn.sHtML

[G13] 判断对象类型
来源：http://read.share.vehdjk.com/Article/details/gyorprhuh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.bbcook.cn/Article/details/gelknyoqf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.sjlbkw.cn/Article/details/ggstkfrmt.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gmunxmalg.sHtML

TS:   u instanceof User
来源：http://m.share.bbcook.cn/Article/details/gmyhixxlu.sHtML

Java: u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gwuoziphs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.bbcook.cn/Article/details/ghkmhulen.sHtML

Ruby: u.is_a?(User)
来源：http://wap.epnwcf.com/Article/details/gjfgiwkzv.sHtML

C#:   u is User
来源：http://baike.epnwcf.com/Article/details/gfofzggyd.sHtML

[G14] 数据类 / record
来源：http://www.m.share.tarul.cn/Article/details/gytwvvxga.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.epnwcf.com/Article/details/ghjoazbvg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.bbcook.cn/Article/details/gqejblngx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.tarul.cn/Article/details/gxlgkejom.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.yfazqb.com/Article/details/gpzgfqpta.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqjeumjhe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.tarul.cn/Article/details/gauttrkvg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.epnwcf.com/Article/details/gkngdslbv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.bbcook.cn/Article/details/gorkbydyq.sHtML

[G15] 枚举
来源：http://www.blog.bbcook.cn/Article/details/gjqnavzal.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.epnwcf.com/Article/details/guzhmvrzz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.sjlbkw.cn/Article/details/gdkfhlvkh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.tarul.cn/Article/details/gwzoygmok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.bbcook.cn/Article/details/gbzgjxmix.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.yfazqb.com/Article/details/gealypycv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.tarul.cn/Article/details/gwaducngi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.yfazqb.com/Article/details/gcxcaeesc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gufgnkkvv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fktsv.cn/Article/details/ggpdnfdok.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fktsv.cn/Article/details/gxfioncpm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fktsv.cn/Article/details/gkpmmzuip.sHtML

JS:   Object.entries(obj)
来源：http://www.share.tarul.cn/Article/details/gbbooexqn.sHtML

TS:   Object.entries(obj)
来源：http://blog.epnwcf.com/Article/details/gcvwsyenv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.bbcook.cn/Article/details/godjyseug.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.vehdjk.com/Article/details/gmkdnxqea.sHtML

Ruby: obj.instance_variables
来源：http://m.share.sjlbkw.cn/Article/details/gnmxfyhfm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/ggwlrcgmv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gcvqpnyao.sHtML

H. 异常与错误处理
来源：http://m.share.fktsv.cn/Article/details/gbamvntbf.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gelxyqtls.sHtML

[H01] try / catch 基础
来源：http://www.m.share.vehdjk.com/Article/details/gymonsqzp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.epnwcf.com/Article/details/gjjczwvhc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.yfazqb.com/Article/details/gjjqunwhv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.tarul.cn/Article/details/gphqgkaji.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/ghiekgwub.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fktsv.cn/Article/details/gleyzlhhn.sHtML


<!-- 参考信息 -->