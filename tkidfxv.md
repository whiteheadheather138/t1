代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gspqbfqzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gspowdvti.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gaqfacrke.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gmgpgshyw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gpsdrjuix.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gahkmicjf.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gfkkmpirk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.tarul.cn/Article/details/gokcecetp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gklkqavwi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gmjmeoqxe.sHtML

Java: s.lines().toList()
来源：http://www.m.share.yfazqb.com/Article/details/gtegnuksf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gxlenjdiu.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/giqlevgod.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gixnriras.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gbikdajlx.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/ganjgvrkw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.tarul.cn/Article/details/gbbgiedow.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gbypvxoyf.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/guelekfil.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gwjxdotzz.sHtML

Go:   if s == "" {}
来源：http://mobile.vehdjk.com/Article/details/gqxqnkuub.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gjnshedeq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxzimgedn.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gukhqvvyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/gkavpporh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gatucjeyx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gsnahwbop.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/ghqmlifli.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gyyofgnpy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gamigjdkb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gmxxfmhdm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gnxkmsunh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gjznkpasf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gehcawjip.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gxzbaimgc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gfhvjlknn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/ggxazwoac.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gjpgwavcu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gkvilrsib.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/guljneuin.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gypzgfzxp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtphccpfh.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gdwtwccsn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gobxckhlt.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/ghvcedozb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.yfazqb.com/Article/details/glcmhryfj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gjzenmjgm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gixwdmcrq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gdoqipfiu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/ghnnkhrpt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gjnyilyqt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gntlahnac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.epnwcf.com/Article/details/gjnsrfezy.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/goshfingo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gwyhgotav.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gryszygzl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gcutdyhpx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gvyygfofh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gshnnqohl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gbbopetjc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gsmmgeiol.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gqlbujpyh.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gdlnvulop.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gteovfsps.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gkslfcknk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gyredgfxo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gkiidrpnz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fktsv.cn/Article/details/gmrpbgnyo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gphsbwdpu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/ggtjtgofb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gokzhvcbe.sHtML

[F04] 追加写入文件
来源：http://www.share.epnwcf.com/Article/details/gmvhjdqkd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/gyiptrzno.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gcosokaic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gwsdueouv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gjighmzyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gtgxhyiej.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gajatepqm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/gxlzdtcwi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gkxlrnwpp.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.epnwcf.com/Article/details/gfcaxgpbl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/giisqwtkt.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gdcvxdxez.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/golhqckdj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gshusicgo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/garbbffza.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gdijlhciq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gzuesopvz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gfknktksd.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gluyhacdq.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqjogxvxw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gyhmuszul.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gekjcidmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmfnrkvum.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gugiokfpw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gepmpiqrx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnotbnsz.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/glltlycnm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gehwpejpi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gjlnccviz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.bbcook.cn/Article/details/gcdrdokpd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.vehdjk.com/Article/details/guilrjjqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gqpsxpygq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/gbdjzqxyp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/grjozvwun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gmcqiweep.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.tarul.cn/Article/details/gklktxkii.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gbgfprdop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gqxhhjlce.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gyttbytro.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gekmwemrm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gcwqykliy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/grusskouu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.tarul.cn/Article/details/gqtvkkiwc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/ghxzlrrgy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gjdvrsvzz.sHtML

[F09] 获取文件大小
来源：http://3g.fktsv.cn/Article/details/gsjdeyuvw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvlldzxxf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gxevhfhtv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gaklrcurq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gosxlegpa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gvbamsumg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gxwsfansz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/giqdkqpog.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gypmnvizm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gqynckzqz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/glrbntgbp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.epnwcf.com/Article/details/grerzzxka.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/glgpmtasx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/guxzlkjab.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.tarul.cn/Article/details/gnjvssnup.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/glnucrbbo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/grfwrwzqw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gbymhodhu.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gsdxcakzb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.yfazqb.com/Article/details/gshopuaiy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.bbcook.cn/Article/details/glkhhwqae.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gknctcljx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gwfcfsvvc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/grqjfljmo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gxchdbkat.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gbqzinkco.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gdkkybnim.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/gxcypjsuy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.bbcook.cn/Article/details/guoidedje.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gxskozsdi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gowkubxfm.sHtML

TS:   // 同上
来源：http://m.share.sjlbkw.cn/Article/details/gbhzyhsen.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.bbcook.cn/Article/details/goentglzx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/gsgjfomhl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gvzorrfus.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/glfkafzkq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glsfjflci.sHtML

G. 面向对象
来源：http://read.share.bbcook.cn/Article/details/gvnatomqy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcbexfgwm.sHtML

[G01] 定义类
来源：http://3g.epnwcf.com/Article/details/gvvgdbldc.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gcubcxfox.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/gbboqvgpn.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gfbmvbwjr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/grvpkzjxl.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gwfmpzmhn.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gutmvxysu.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/gfeshtwsb.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gnapixvdm.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gccsgzvsg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.epnwcf.com/Article/details/gbgzbcosl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.tarul.cn/Article/details/gkyrdadcy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gmrkomolk.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gilevtain.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gmysxyszj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.yfazqb.com/Article/details/gagcmbcqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gtykexhco.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gqwvlbtxn.sHtML

[G03] 实例属性
来源：http://www.share.sjlbkw.cn/Article/details/gfhtexkno.sHtML

Py:   self.name = "x"
来源：http://wap.tarul.cn/Article/details/gezfqovgc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/grfiyfrfb.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/glkfhfxfp.sHtML

TS:   name: string = "x";
来源：http://m.share.fktsv.cn/Article/details/gdpvjeppu.sHtML

Java: private String name;
来源：http://www.blog.epnwcf.com/Article/details/gmhbqeqzq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gcannymgk.sHtML

Ruby: @name = "x"
来源：http://read.share.fktsv.cn/Article/details/gijbuvcku.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gqpkqjfso.sHtML

[G04] 定义方法
来源：http://www.blog.vehdjk.com/Article/details/gmcfkdrmf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/guotyshmj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gptqltxcm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gobrujewp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.bbcook.cn/Article/details/gpuytyhmo.sHtML

Java: String greet() { return name; }
来源：http://wap.tarul.cn/Article/details/gdralmiup.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.sjlbkw.cn/Article/details/gsqtndslh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.vehdjk.com/Article/details/gjzjhhtqr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gbccytjju.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gwrbcwtky.sHtML

Py:   class Admin(User): pass
来源：http://wap.tarul.cn/Article/details/ggesapeme.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/ghnwahoko.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gqkxqdweb.sHtML

TS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gplhadook.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gzybxdjqi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.epnwcf.com/Article/details/gwwsbzyiy.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.tarul.cn/Article/details/gpflyijpt.sHtML

C#:   class Admin : User {}
来源：http://m.share.tarul.cn/Article/details/gsxbzqnxp.sHtML

[G06] 重写方法
来源：http://baike.vehdjk.com/Article/details/gssuvhcet.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.epnwcf.com/Article/details/gvlqiufdt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gbndemkth.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/geblznrse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gzcjaumzc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gzdcqrxmn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.sjlbkw.cn/Article/details/gymsahtss.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/grfbfgbva.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.yfazqb.com/Article/details/gupmipkem.sHtML

[G07] 调用父类方法
来源：http://wap.epnwcf.com/Article/details/guowpckiu.sHtML

Py:   super().greet()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsnqqdmr.sHtML

PHP:  parent::greet();
来源：http://wap.sjlbkw.cn/Article/details/germqooob.sHtML

JS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gyrlfzacx.sHtML

TS:   super.greet();
来源：http://blog.tarul.cn/Article/details/gerbnxipm.sHtML

Java: super.greet();
来源：http://wap.fktsv.cn/Article/details/gmvlwdvvt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.vehdjk.com/Article/details/gzpolbmfb.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gypumzwca.sHtML

C#:   base.Greet();
来源：http://wap.epnwcf.com/Article/details/gijuoyqqs.sHtML

[G08] 静态方法与属性
来源：http://www.share.fktsv.cn/Article/details/guammuegz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/gxupvxjcg.sHtML

PHP:  public static function f() {}
来源：http://mobile.tarul.cn/Article/details/gqwlymkgh.sHtML

JS:   static f() {}
来源：http://www.share.yfazqb.com/Article/details/gczyfszlv.sHtML

TS:   static f(): void {}
来源：http://wap.bbcook.cn/Article/details/gvugeudvy.sHtML

Java: static void f() {}
来源：http://3g.epnwcf.com/Article/details/gwgjsbqzm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.epnwcf.com/Article/details/gvcxwzblt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gqtxrmhxi.sHtML

C#:   public static void F() {}
来源：http://www.m.share.epnwcf.com/Article/details/gmjqrsere.sHtML

[G09] 接口 / 抽象类
来源：http://3g.vehdjk.com/Article/details/gsjisfkut.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.epnwcf.com/Article/details/gnqeuthzd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.sjlbkw.cn/Article/details/guzvjouch.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.tarul.cn/Article/details/gqjsdybkh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.sjlbkw.cn/Article/details/gwiaytbsr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtpalssyz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.vehdjk.com/Article/details/gbgfrlvin.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fktsv.cn/Article/details/gsfgimguk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.bbcook.cn/Article/details/gpmchdxak.sHtML

[G10] 访问控制
来源：http://www.share.bbcook.cn/Article/details/gakyousmc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gjnedduic.sHtML

PHP:  public / protected / private
来源：http://3g.yfazqb.com/Article/details/gcmbaxrtx.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.sjlbkw.cn/Article/details/gslfpkgtu.sHtML

TS:   public / protected / private
来源：http://wap.vehdjk.com/Article/details/gmwtthsnm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.tarul.cn/Article/details/gnodlhzkn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.tarul.cn/Article/details/gbgechvuz.sHtML

Ruby: public / protected / private
来源：http://www.blog.fktsv.cn/Article/details/gvqlycfri.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.tarul.cn/Article/details/glxrokgrn.sHtML

[G11] getter / setter
来源：http://3g.epnwcf.com/Article/details/gqwjlqmdd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.epnwcf.com/Article/details/gafeditmd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gwpsxrgxb.sHtML

JS:   get name() { return this._name; }
来源：http://wap.sjlbkw.cn/Article/details/gkbefrfzu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.sjlbkw.cn/Article/details/gibfikngy.sHtML

Java: public String getName() { return name; }
来源：http://baike.vehdjk.com/Article/details/gjgenfbpb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gcjvdvdmt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.tarul.cn/Article/details/ghfrraemc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/gkwpiopir.sHtML

[G12] 对象转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gwynssgjg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.sjlbkw.cn/Article/details/gufliwjgk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gsijqgalx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gylthlwxd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.epnwcf.com/Article/details/gksmvtqvr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.yfazqb.com/Article/details/gmjcghxes.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.yfazqb.com/Article/details/grbhlcrfc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.sjlbkw.cn/Article/details/gfmawlwww.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.yfazqb.com/Article/details/gulwxjjox.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fktsv.cn/Article/details/gytqhlvgs.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.epnwcf.com/Article/details/gxzrqyfli.sHtML

PHP:  $u instanceof User
来源：http://3g.bbcook.cn/Article/details/galjdnlsn.sHtML

JS:   u instanceof User
来源：http://www.blog.fktsv.cn/Article/details/gkadxhkra.sHtML

TS:   u instanceof User
来源：http://read.share.tarul.cn/Article/details/grrrpdjxp.sHtML

Java: u instanceof User
来源：http://3g.epnwcf.com/Article/details/gftcumvtf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fktsv.cn/Article/details/ghnucbfrg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.vehdjk.com/Article/details/gpkgslbip.sHtML

C#:   u is User
来源：http://m.share.bbcook.cn/Article/details/gpmdvyotn.sHtML

[G14] 数据类 / record
来源：http://m.share.bbcook.cn/Article/details/gjhgnizor.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.vehdjk.com/Article/details/gqdgjzmtp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.sjlbkw.cn/Article/details/grmwqynpi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.bbcook.cn/Article/details/gmqimhcyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.bbcook.cn/Article/details/gwytnvaga.sHtML

Java: record User(String name, int age) {}
来源：http://blog.tarul.cn/Article/details/gmurneuqf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.sjlbkw.cn/Article/details/gseiufwew.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fktsv.cn/Article/details/gwukaxxmp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.bbcook.cn/Article/details/gcuvjgqnl.sHtML

[G15] 枚举
来源：http://baike.vehdjk.com/Article/details/gswvqddbo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.epnwcf.com/Article/details/grewwirnk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.tarul.cn/Article/details/gtmyqtbzt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fktsv.cn/Article/details/gdysfyivt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.epnwcf.com/Article/details/gyvhfnkwi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.epnwcf.com/Article/details/gyaiztznh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.epnwcf.com/Article/details/gwhgzgjio.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.vehdjk.com/Article/details/ghfqqujeo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.sjlbkw.cn/Article/details/giaezyvwd.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.vehdjk.com/Article/details/gfpclouol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.epnwcf.com/Article/details/gfqphklol.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.tarul.cn/Article/details/gozninyzr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gcjwfztgw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.bbcook.cn/Article/details/grsunmgbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.bbcook.cn/Article/details/gbogggjds.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.epnwcf.com/Article/details/gmznzdwsg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.bbcook.cn/Article/details/gzfxbsnev.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.vehdjk.com/Article/details/gcjriircb.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glmmizhcc.sHtML


<!-- 参考信息 -->