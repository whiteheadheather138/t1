代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/glhirgriv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gswbsvlis.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gleyicqrh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.sjlbkw.cn/Article/details/gyeunojin.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/gvziqbubf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gbqhqytyq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.tarul.cn/Article/details/gogsqvewl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gjlslrvcq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gotojfmzu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/guudwsrrw.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gilreuzqj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gbvfbfima.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gufvrjpzp.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gtslidzoi.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gyaenqelf.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gfruiivtm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gmulmzato.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gvabvuiyw.sHtML

TS:   if (s === "") {}
来源：http://m.share.fktsv.cn/Article/details/gxobnovdz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gvnnyxkdy.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/gkjbamree.sHtML

Ruby: if s.empty?
来源：http://www.share.fktsv.cn/Article/details/gblbfcwcv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/gvlrxafcw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gnvdrwzkz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/gwnpqlkev.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gniyyktkv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gfrcalcof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gowyjawuq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gdrtvqiwe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/gimloxrtu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gxaclyozm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gnealzmxk.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gnmkrauwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/grqniduvt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gwuoefgzq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gdjcttres.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gpevlrvep.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gaddvkvso.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.yfazqb.com/Article/details/gobqkhovq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gieqhctxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/grjoaqnso.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpotluusi.sHtML

F. 文件与目录
来源：http://blog.fktsv.cn/Article/details/gxyepdpnf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gqnjsynol.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/guqdsfeyz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.yfazqb.com/Article/details/gercelelc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gjunmwwmn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gvsbqruzi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/glgewcizu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gzbzlowjd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.bbcook.cn/Article/details/gsnzczbxh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/givpttrii.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbgqcqjza.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gbkgpiuyq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/ggoianzzy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.tarul.cn/Article/details/gtzxeqhzp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gdhsrfukn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/grwaraxiu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gsatokpwa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/ghmkrkhba.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/grjccnbmr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gszruozcv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gtqfhgqaw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/gdwhfztra.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gujizqpjs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gzacfnzbs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gntduqtof.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gqdazathg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.bbcook.cn/Article/details/gcrpmdntt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/ghwpwwdfd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/grdlqfdyk.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gsjvgspnn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gykucrvfp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gpoljyxjs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gffsrkghh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/glqlbehtx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gzgbiynxx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/geqmzzlhj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gzuqafrgd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gkgorfgpb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gemrdvtlu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gqbjddwfp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbelibowk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gtvxkioqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gsoubmddr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gpzqgbnit.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gdnbvaenb.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.tarul.cn/Article/details/gcjyyajvz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.vehdjk.com/Article/details/gcghnsife.sHtML

[F06] 删除文件
来源：http://www.m.share.tarul.cn/Article/details/gpptcdrhe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkhfogdve.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/getrrkidc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gltvegfth.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gyhpqhpnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gwyshhfhn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfrnrxeyo.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gbvvyrvgx.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtodkzopn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.bbcook.cn/Article/details/gsovtxsqs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/garsqsoxg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.yfazqb.com/Article/details/gyvkyuvyp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gdrcqkzmg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gpykvkpem.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.tarul.cn/Article/details/gyzvjmybg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gkmjxepal.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gggnpaobt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fktsv.cn/Article/details/ghamqjsyc.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gustovmir.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.sjlbkw.cn/Article/details/gzphurtxu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.tarul.cn/Article/details/gnpkhssrh.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gqerlmfwn.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gfnfbepsn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gzwmynrmo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gkybfcqti.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gxhgvtdhg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/gwszkohfi.sHtML

[F09] 获取文件大小
来源：http://read.share.epnwcf.com/Article/details/gegdkqzkq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gikkntwhn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gfxyikygr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/ghatfavwk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/gqkvisjma.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/golhiosjw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/glmomqfzb.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gfzvjklmc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.bbcook.cn/Article/details/gtthxgpsm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gigplaupe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gsyovworx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gcdxufvrh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/ghehycafy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gyjdezuzi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.vehdjk.com/Article/details/guynalcru.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/ghkudguiv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjwvcxqqf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfgwouefn.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gsrgwgsfj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gfuianobw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.vehdjk.com/Article/details/gvuiasmsm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gpcrhpfhe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gghtnycky.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/gkyyyqcnw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.epnwcf.com/Article/details/ghjugtjbg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggmczzxhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gpwqlxdnj.sHtML

[F12] CSV 读写
来源：http://www.blog.yfazqb.com/Article/details/gnzjoazji.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gtzyscugy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.yfazqb.com/Article/details/gtljykwfh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.vehdjk.com/Article/details/gbodtorlq.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gykatenjb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.yfazqb.com/Article/details/gzkngtvue.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.sjlbkw.cn/Article/details/gfhtxzmyd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gwlmmfcxr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gronagqpl.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/glxytnpar.sHtML

G. 面向对象
来源：http://www.share.epnwcf.com/Article/details/grmagnxzh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdpuorxiy.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gtwiqiyfn.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gyzbtokgg.sHtML

PHP:  class User {}
来源：http://wap.bbcook.cn/Article/details/gmvywiqln.sHtML

JS:   class User {}
来源：http://mobile.fktsv.cn/Article/details/gxzdnzekq.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.sjlbkw.cn/Article/details/gmvlpwlul.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gvdcwtnde.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.epnwcf.com/Article/details/gkjdewmqm.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gvbesncxg.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/giskxlwvl.sHtML

[G02] 构造函数
来源：http://wap.yfazqb.com/Article/details/gcfqkfhor.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gevroqlvo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gltypiszr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.sjlbkw.cn/Article/details/gtjxolcfd.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gqbpdmars.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.tarul.cn/Article/details/gvinkpxok.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gqmaiosfk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.tarul.cn/Article/details/gbzklodwi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/glorankzr.sHtML

[G03] 实例属性
来源：http://www.share.epnwcf.com/Article/details/gvvvmsxza.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gzfjztyzh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gothrhtor.sHtML

JS:   this.name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gvmxhlnwz.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gutgsscuv.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gdinufrss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.epnwcf.com/Article/details/gbgiidgde.sHtML

Ruby: @name = "x"
来源：http://www.share.sjlbkw.cn/Article/details/ghaihnklf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.vehdjk.com/Article/details/gflsnjhnz.sHtML

[G04] 定义方法
来源：http://www.share.epnwcf.com/Article/details/gxyywkeaz.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fktsv.cn/Article/details/gwtgnjmfv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.epnwcf.com/Article/details/gjvobuhmt.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/gkgupwmwz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gnmyjyhsc.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gjkatvbkv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.tarul.cn/Article/details/gfyengond.sHtML

Ruby: def greet; @name; end
来源：http://read.share.yfazqb.com/Article/details/ggnacqqrc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gbqpitvoq.sHtML

[G05] 继承
来源：http://www.share.tarul.cn/Article/details/gtxhcuymt.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gfytgisst.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gwrojzths.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/glpkkhlyw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fktsv.cn/Article/details/gtcnnztuk.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/giqezcooz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.epnwcf.com/Article/details/grfiwnygi.sHtML

Ruby: class Admin < User; end
来源：http://3g.epnwcf.com/Article/details/gagnryiie.sHtML

C#:   class Admin : User {}
来源：http://www.share.tarul.cn/Article/details/gkditagsq.sHtML

[G06] 重写方法
来源：http://mobile.tarul.cn/Article/details/gnzbfipmy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.bbcook.cn/Article/details/gsssbegfs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.sjlbkw.cn/Article/details/gszlioscq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gqnryexjm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.tarul.cn/Article/details/grbngrspy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.yfazqb.com/Article/details/gpwyoqaab.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.sjlbkw.cn/Article/details/gquglvwcu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.yfazqb.com/Article/details/gyctqvwzd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.tarul.cn/Article/details/gllaxuqhr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gvselijty.sHtML

Py:   super().greet()
来源：http://www.blog.epnwcf.com/Article/details/gathmpivb.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gbbgdigbv.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gsttlgpgb.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gjskploja.sHtML

Java: super.greet();
来源：http://www.m.share.epnwcf.com/Article/details/gllijhzga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.tarul.cn/Article/details/ghxciwefd.sHtML

Ruby: super
来源：http://3g.sjlbkw.cn/Article/details/gllviztlu.sHtML

C#:   base.Greet();
来源：http://m.share.vehdjk.com/Article/details/gnyjjmbjk.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gxjxaadur.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.sjlbkw.cn/Article/details/gruunlwue.sHtML

PHP:  public static function f() {}
来源：http://www.share.fktsv.cn/Article/details/goxlmbgav.sHtML

JS:   static f() {}
来源：http://blog.yfazqb.com/Article/details/gyplczbhl.sHtML

TS:   static f(): void {}
来源：http://baike.sjlbkw.cn/Article/details/gkgbbkotl.sHtML

Java: static void f() {}
来源：http://m.share.vehdjk.com/Article/details/ghvhppyns.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.tarul.cn/Article/details/gyxntqqex.sHtML

Ruby: def self.f; end
来源：http://3g.tarul.cn/Article/details/gwtzzzdhu.sHtML

C#:   public static void F() {}
来源：http://www.blog.epnwcf.com/Article/details/glscasfbt.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.epnwcf.com/Article/details/gemrldshp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.vehdjk.com/Article/details/gypszjfaf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.tarul.cn/Article/details/gdenjfwyk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fktsv.cn/Article/details/grfbfozbo.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.epnwcf.com/Article/details/gjnpnbrwo.sHtML

Java: interface Shape { double area(); }
来源：http://wap.bbcook.cn/Article/details/gaycxrbkt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.bbcook.cn/Article/details/gxasozekz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.yfazqb.com/Article/details/gaicguuar.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.bbcook.cn/Article/details/gkphgshdi.sHtML

[G10] 访问控制
来源：http://mobile.yfazqb.com/Article/details/gftlvavuh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.yfazqb.com/Article/details/gllgfypir.sHtML

PHP:  public / protected / private
来源：http://read.share.vehdjk.com/Article/details/gcqerdbdx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.tarul.cn/Article/details/gcnpzhxmf.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gxfginxbk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.bbcook.cn/Article/details/giolyduwi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/gffndkomg.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/golqsfzpa.sHtML

C#:   public / protected / private / internal
来源：http://baike.yfazqb.com/Article/details/gcdgrcnmt.sHtML

[G11] getter / setter
来源：http://mobile.vehdjk.com/Article/details/gxvxtvyob.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.sjlbkw.cn/Article/details/gdthkxpzl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gcfwmmham.sHtML

JS:   get name() { return this._name; }
来源：http://blog.epnwcf.com/Article/details/gafvbcfgm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyldgaywr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.vehdjk.com/Article/details/gzzfrnzxe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/gxmfyuvhx.sHtML

Ruby: attr_accessor :name
来源：http://read.share.vehdjk.com/Article/details/gndtaouzc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.vehdjk.com/Article/details/godzyrbxl.sHtML

[G12] 对象转字符串
来源：http://3g.epnwcf.com/Article/details/gvlrahygc.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.yfazqb.com/Article/details/gnmbaejtv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.bbcook.cn/Article/details/gagsbhgrx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.yfazqb.com/Article/details/gadokvyez.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gfrsonkut.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.tarul.cn/Article/details/genkfbuyb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.epnwcf.com/Article/details/gzoipanqt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fktsv.cn/Article/details/gzhgwjtun.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.epnwcf.com/Article/details/gjilhnxdd.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gokgtlnof.sHtML

Py:   isinstance(u, User)
来源：http://www.share.bbcook.cn/Article/details/gwbvxrmhg.sHtML

PHP:  $u instanceof User
来源：http://read.share.vehdjk.com/Article/details/glhmtffiz.sHtML

JS:   u instanceof User
来源：http://www.share.bbcook.cn/Article/details/gxlwkdbrf.sHtML

TS:   u instanceof User
来源：http://3g.fktsv.cn/Article/details/gixdbgjtg.sHtML

Java: u instanceof User
来源：http://blog.yfazqb.com/Article/details/gapahsptc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.yfazqb.com/Article/details/gbtnrcrme.sHtML

Ruby: u.is_a?(User)
来源：http://wap.sjlbkw.cn/Article/details/gaddxtsig.sHtML

C#:   u is User
来源：http://blog.tarul.cn/Article/details/gdhgptpoe.sHtML

[G14] 数据类 / record
来源：http://3g.bbcook.cn/Article/details/goixziuok.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.epnwcf.com/Article/details/gmdkwgnpd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.yfazqb.com/Article/details/gjpzyhjuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.sjlbkw.cn/Article/details/gdtfmiolz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.yfazqb.com/Article/details/guetjmqjf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fktsv.cn/Article/details/gppkbzkgo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.tarul.cn/Article/details/gxrrliyws.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.yfazqb.com/Article/details/glmmnkcfm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.tarul.cn/Article/details/gfbchoona.sHtML

[G15] 枚举
来源：http://blog.sjlbkw.cn/Article/details/gzxrbxbly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.tarul.cn/Article/details/gelfpjnqy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.sjlbkw.cn/Article/details/gipwczwqe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.vehdjk.com/Article/details/giyukwakq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.tarul.cn/Article/details/gmsfihqbj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fktsv.cn/Article/details/gbxdopzsq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.vehdjk.com/Article/details/giwplizzu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.tarul.cn/Article/details/gpoulzvlp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.tarul.cn/Article/details/gkacjhywp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.epnwcf.com/Article/details/gqxxhialf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.sjlbkw.cn/Article/details/gknvtugpt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.epnwcf.com/Article/details/gtgbrrutj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.tarul.cn/Article/details/gmulzmgdn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.yfazqb.com/Article/details/gvkzecdav.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.vehdjk.com/Article/details/gvikuaxcm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.bbcook.cn/Article/details/ghbrucshg.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fktsv.cn/Article/details/gdoxnqcos.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fktsv.cn/Article/details/gnwyrmloa.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grfkffglz.sHtML


<!-- 参考信息 -->