代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.epnwcf.com/Article/details/gboqxljlj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gpybquldl.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gwmpzhlvc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gidktznoy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gkrcokiio.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gfxxcacqt.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/ghvtoqgxz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gvmieubeu.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gtikcscdm.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gtjquasns.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.yfazqb.com/Article/details/gdsunqdrm.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/grzeynvus.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gnztvjgoz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/goiwwqvfq.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/ghhjgtegd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/giukzzxsi.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gbzavorvn.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/grjrsskgp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gixfakmcm.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/grfmdudxw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gajtkherb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gsldcouuq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gbtlkvoce.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gbxnwjtcr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gprvdjfhq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gfswkacnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gpvvibuce.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gncuxjana.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gaodwajvk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/glfsaaxvh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gmkpimxtn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gvdwnkqoi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gmvklrycm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gbbsivwog.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/gidebwxyw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.epnwcf.com/Article/details/geduaaxoh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gvboegbnb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbecmmwjn.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gdlfmjdid.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gruimddzq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gqjdbkaid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/gojzewqgs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmgqlycdk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gdfpvhwhq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gpctyplbs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gremjmsor.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/grlqpqped.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/gtdczemdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gctxktiqi.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/goicqvpef.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gwlvbsiev.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gforrczdx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/giduwvtva.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gsrgejcbt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gditquqcy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gutngtjxj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/ggivlobtu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gfzumpmag.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gigkfxrlq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gutimczvg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/ghvivgqqs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gmzrcaeyw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gvtpzplvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gqmvfefoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gwoupyvtq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gtqjcdxck.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/ggxfdmixh.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/glvmjkiys.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gmjyokebl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gwnobkubq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gnruluykv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gjxnosset.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gdxjocnrm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.epnwcf.com/Article/details/gutabbnib.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/grqeqayal.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fktsv.cn/Article/details/gyjyikkho.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/getlhjdny.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/geaanslpj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghrgtwnls.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/glqmkprpk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gnexuzvnv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gdoyddzpv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gblpxwwla.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gqttjptiv.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwifihbgd.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gncvtofco.sHtML

Py:   os.remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gsuemwxiu.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gywnpyqrz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gzfyoknml.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/geynxtnlf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gvcovchbn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gmrtowkzb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggraczsbv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gbfjlbowu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.sjlbkw.cn/Article/details/gpenlpmrt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gawbnesdc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gurkodzvd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gdudtofaf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gcgrjbqwl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gdrzxgexk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.yfazqb.com/Article/details/gdrcxzemn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/guqjtbrld.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/ghsszziff.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gppsgrjur.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.tarul.cn/Article/details/gwahzahck.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/gcajdixdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gqvynwyxg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gtiudzyqh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gapxotald.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fktsv.cn/Article/details/gzkzzhedu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gxtyymouk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.vehdjk.com/Article/details/gzloursmg.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/gocbzegks.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.bbcook.cn/Article/details/glwzjgekk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gqxmkhjgr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gnyyejpcm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gtqegevki.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gzrapzuuu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gixtbhfmq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gnwchelhc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.vehdjk.com/Article/details/gtzvbgiez.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gpmqxfhzz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gumpdetrh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gcspclwqf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gtmlqtshd.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grqatzwzy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.vehdjk.com/Article/details/gqamxxijt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gffcolrfv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gsaspphir.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gailisirc.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gppqttyzu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwvgwzkam.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gesxibuzf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gwoxmumzw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gtzrgttlf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gfjngdzdy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.sjlbkw.cn/Article/details/gwfasbqmw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gfottfksi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gvjqhyoby.sHtML

[F12] CSV 读写
来源：http://baike.sjlbkw.cn/Article/details/gotgsmpkv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gdvhqvliy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gskwcmmif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.sjlbkw.cn/Article/details/gzntqpxtv.sHtML

TS:   // 同上
来源：http://www.blog.epnwcf.com/Article/details/gwvjyswqy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gcefauuvi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/ghvxeowwx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gpqgcblhj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gxnrhwcdj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnqgdntop.sHtML

G. 面向对象
来源：http://blog.sjlbkw.cn/Article/details/gwoxkfupj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gxpiarhit.sHtML

[G01] 定义类
来源：http://3g.fktsv.cn/Article/details/gjzunklir.sHtML

Py:   class User: pass
来源：http://www.m.share.epnwcf.com/Article/details/gonivxdvt.sHtML

PHP:  class User {}
来源：http://3g.yfazqb.com/Article/details/gsbpztuyv.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gjwrcplvy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.vehdjk.com/Article/details/gqgplbubj.sHtML

Java: class User {}
来源：http://wap.epnwcf.com/Article/details/gqwopalme.sHtML

Go:   type User struct { Name string }
来源：http://m.share.tarul.cn/Article/details/guubklvcy.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gidniewqf.sHtML

C#:   class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gkbzxueqd.sHtML

[G02] 构造函数
来源：http://read.share.bbcook.cn/Article/details/gecjxhslf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/grymphgie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gsarvusiu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gxhhkhjbt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fktsv.cn/Article/details/gcgszgkmq.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gfkbeumwq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.yfazqb.com/Article/details/gbmhewika.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/ggfnwgtzq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/ggbsbgvzo.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/gedyzjqav.sHtML

Py:   self.name = "x"
来源：http://www.blog.tarul.cn/Article/details/gdrbguteh.sHtML

PHP:  public string $name = "x";
来源：http://m.share.epnwcf.com/Article/details/gvvfvtvwr.sHtML

JS:   this.name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gqwkbqibm.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gwzrmcarh.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gvkdphyeo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/glkyfztph.sHtML

Ruby: @name = "x"
来源：http://www.blog.bbcook.cn/Article/details/guhwyfebq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.sjlbkw.cn/Article/details/gdrrtfxqf.sHtML

[G04] 定义方法
来源：http://3g.tarul.cn/Article/details/gprlqxuze.sHtML

Py:   def greet(self): return self.name
来源：http://wap.sjlbkw.cn/Article/details/gaicflidf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.vehdjk.com/Article/details/grccjbhwm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gkmitoxls.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fktsv.cn/Article/details/gyllthqus.sHtML

Java: String greet() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gzwagrcol.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.vehdjk.com/Article/details/grmxjgfdl.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gjcthynwt.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.vehdjk.com/Article/details/gzcgtsfop.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gsvtnzchk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.tarul.cn/Article/details/gvnuqxwew.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gqxixqucd.sHtML

JS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gjbkzdjjk.sHtML

TS:   class Admin extends User {}
来源：http://wap.yfazqb.com/Article/details/gmndxtffu.sHtML

Java: class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gepizgyjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fktsv.cn/Article/details/gmrpamurh.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gicjcexxc.sHtML

C#:   class Admin : User {}
来源：http://m.share.fktsv.cn/Article/details/gccxmphum.sHtML

[G06] 重写方法
来源：http://wap.yfazqb.com/Article/details/gmkinkrii.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.vehdjk.com/Article/details/grmjlaliv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.epnwcf.com/Article/details/grrsddhxn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fktsv.cn/Article/details/gouwxccue.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/gmwaxpevr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gdkgnsylu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.epnwcf.com/Article/details/gievrrtrq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.sjlbkw.cn/Article/details/gjlppputr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fktsv.cn/Article/details/gludavshg.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gmyvfrbtx.sHtML

Py:   super().greet()
来源：http://www.blog.fktsv.cn/Article/details/gahzuxuhx.sHtML

PHP:  parent::greet();
来源：http://www.share.epnwcf.com/Article/details/gnxznunxi.sHtML

JS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/gllxrqmpd.sHtML

TS:   super.greet();
来源：http://wap.yfazqb.com/Article/details/gnqadetjy.sHtML

Java: super.greet();
来源：http://baike.vehdjk.com/Article/details/grgufwtox.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.vehdjk.com/Article/details/ggltqfrps.sHtML

Ruby: super
来源：http://www.share.sjlbkw.cn/Article/details/gxvtnmtdg.sHtML

C#:   base.Greet();
来源：http://3g.fktsv.cn/Article/details/gwvrwokmb.sHtML

[G08] 静态方法与属性
来源：http://baike.yfazqb.com/Article/details/gqlxrsxmr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.epnwcf.com/Article/details/grpellmgj.sHtML

PHP:  public static function f() {}
来源：http://www.share.tarul.cn/Article/details/gwlveurjf.sHtML

JS:   static f() {}
来源：http://baike.bbcook.cn/Article/details/gxqtscllh.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gprlvzeia.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/ghvscalsf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.epnwcf.com/Article/details/gyphopwhi.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gedftsmxi.sHtML

C#:   public static void F() {}
来源：http://read.share.yfazqb.com/Article/details/gepjznxix.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gscskxtpl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.sjlbkw.cn/Article/details/gmrwzfjob.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.vehdjk.com/Article/details/gfyqkfpif.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.yfazqb.com/Article/details/gtjoorqds.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fktsv.cn/Article/details/gqndredwi.sHtML

Java: interface Shape { double area(); }
来源：http://wap.epnwcf.com/Article/details/gszbgowsv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gkjtmtivh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.epnwcf.com/Article/details/geewzforw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.sjlbkw.cn/Article/details/gvoldehtb.sHtML

[G10] 访问控制
来源：http://www.m.share.sjlbkw.cn/Article/details/gynjfortx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.yfazqb.com/Article/details/gdnnyzrwt.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/gidhybhvn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/ganazurok.sHtML

TS:   public / protected / private
来源：http://read.share.fktsv.cn/Article/details/gesgiuccp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fktsv.cn/Article/details/gogaeidwv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fktsv.cn/Article/details/gmbreqkbo.sHtML

Ruby: public / protected / private
来源：http://www.m.share.epnwcf.com/Article/details/gtmxpfawn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.bbcook.cn/Article/details/gpvaektmn.sHtML

[G11] getter / setter
来源：http://3g.sjlbkw.cn/Article/details/gbupqrobm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.sjlbkw.cn/Article/details/gcvoqokpg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/geygdfvza.sHtML

JS:   get name() { return this._name; }
来源：http://baike.tarul.cn/Article/details/gmdptkyff.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.yfazqb.com/Article/details/ggxyxjdwb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.yfazqb.com/Article/details/gswhcxxoa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gbzkhoppj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.yfazqb.com/Article/details/gnkhpdmke.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fktsv.cn/Article/details/gnkninohv.sHtML

[G12] 对象转字符串
来源：http://mobile.fktsv.cn/Article/details/gtwipxbda.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gtaiqdthg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/ggwpuiirq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/gszrminnz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.tarul.cn/Article/details/gbonezfql.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.sjlbkw.cn/Article/details/givojrxrd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.sjlbkw.cn/Article/details/guwnechrk.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.bbcook.cn/Article/details/geaiiwkjs.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gniysgdxa.sHtML

[G13] 判断对象类型
来源：http://read.share.bbcook.cn/Article/details/gpukjcwbq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.vehdjk.com/Article/details/gzhsbcydt.sHtML

PHP:  $u instanceof User
来源：http://3g.tarul.cn/Article/details/gckoyewfb.sHtML

JS:   u instanceof User
来源：http://read.share.bbcook.cn/Article/details/gmrhwbudc.sHtML

TS:   u instanceof User
来源：http://baike.vehdjk.com/Article/details/gcwruqngb.sHtML

Java: u instanceof User
来源：http://3g.yfazqb.com/Article/details/gdlsfgamo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.tarul.cn/Article/details/gdosbhoum.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.yfazqb.com/Article/details/ggsweepbo.sHtML

C#:   u is User
来源：http://baike.vehdjk.com/Article/details/glllfnqfq.sHtML

[G14] 数据类 / record
来源：http://m.share.vehdjk.com/Article/details/gwiztnlpb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.sjlbkw.cn/Article/details/gecgsiedz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.sjlbkw.cn/Article/details/gmhnxtmlo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.bbcook.cn/Article/details/gogvaqmyx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.tarul.cn/Article/details/gtxqepram.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.epnwcf.com/Article/details/gudgztejg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.epnwcf.com/Article/details/gtjapczcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.sjlbkw.cn/Article/details/gzqzozgdg.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.epnwcf.com/Article/details/gblnnvdmo.sHtML

[G15] 枚举
来源：http://read.share.sjlbkw.cn/Article/details/giuioefpk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.vehdjk.com/Article/details/gzgtahrce.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.sjlbkw.cn/Article/details/gyxjodloy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fktsv.cn/Article/details/ghesvgajo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.yfazqb.com/Article/details/gknozvzoz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.tarul.cn/Article/details/gjbqxvqos.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.bbcook.cn/Article/details/gocajrncn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.epnwcf.com/Article/details/gfuwxugcb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.yfazqb.com/Article/details/gnqmtxrnv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.bbcook.cn/Article/details/gwhyneqbw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.vehdjk.com/Article/details/gqiouggny.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.bbcook.cn/Article/details/gvkaiuxxj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gavyyzyku.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsmnmtfjy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.bbcook.cn/Article/details/gngmbyzhz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.tarul.cn/Article/details/gwxmievmu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gejqlyszw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gtvxzooyy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gcsrcedbm.sHtML

H. 异常与错误处理
来源：http://read.share.fktsv.cn/Article/details/gkdrjujwb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gfruelrex.sHtML

[H01] try / catch 基础
来源：http://blog.epnwcf.com/Article/details/gmopviiak.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.yfazqb.com/Article/details/gqgwugejh.sHtML


<!-- 参考信息 -->