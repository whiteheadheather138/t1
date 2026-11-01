代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/ggbrujqjf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/grkgbjodd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gkwyhyteo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtiwejlnk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gugdiyhsj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gyihfvyin.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gdvzzyoua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gdrxzevec.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gqvedaepb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/ggkqsleuo.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gmvdbsqks.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/guklzzzhm.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gabttwsxw.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/guarahjpz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gcabxtwmh.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/grgeibnlz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/geskzasci.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gfehxrlat.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/ghgrdkwxv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gfpboqhre.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gjmcqyzod.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqitebon.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyzzmvgvo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gpxqtcfug.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gkszbgwdj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gtfwarnbd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gzupvjooh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gchqwhjdk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gaqiohiqg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/ghomefdwb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gxsozaroa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gstderjkf.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gvczmysnz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqvqjfvsk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gaqjjqnta.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gbirifvcv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/glsqeumqd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gibpljitp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/geroifmab.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gssagnxnk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gzjpnpglk.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gogezlyth.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gsmeadeqk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gejfqjnga.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/ggjolmdih.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gyvfhxmne.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/giotgrmqz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gmiacbruz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gngsxiuvd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/glwadttrh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gbhjrgjdq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.bbcook.cn/Article/details/gdiioayvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/guaeqatkj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.bbcook.cn/Article/details/gnzqyripj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gubgrpqjj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.yfazqb.com/Article/details/ghlohywgn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gpdhaopeu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gcetyaute.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gjursmyrd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gexdjdbez.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/gvjoznmml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.tarul.cn/Article/details/gfbpgnvxy.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gysjjkiez.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gnrdnwrga.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/ghziexmig.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gyfnaktlr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gzhuxjjwv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gdxyrjsoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/glmgvasqf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gtyqbcdia.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gkoyekyua.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gdqchlsdc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gbdaieihj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.vehdjk.com/Article/details/gcgwrajaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gahqdvify.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gnwhttmue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gclklikfz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gwnwdbcrs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gnkdhsnjk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gdzwjyieo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gkwfnqrra.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gyfntrdcg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gmnggzjhn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gslhwgzok.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gtftqwcrt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gcuwsszxk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gvcubqdxe.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gltukjyiu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/guexzzior.sHtML

[F06] 删除文件
来源：http://read.share.vehdjk.com/Article/details/gjviospof.sHtML

Py:   os.remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/gyyhebepe.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gbbxyoede.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glecywhni.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gvoqdewrq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzxcfbbkd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gzlxdlehp.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwqbqcszv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gfjgahbnh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/gbqpnelsl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gfhqougep.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gpugaqmfb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/ggnyppbnv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gxzsshylu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/ggrlgmizk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/gftzxdmld.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gzqbjuslv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gzitiuhca.sHtML

[F08] 遍历目录
来源：http://m.share.epnwcf.com/Article/details/gfmuacvmr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fktsv.cn/Article/details/gnjljenxm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gcvwwpaqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gadhaggkn.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/ggkpkdtfk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gtvfghtld.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gtiahmqbj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.epnwcf.com/Article/details/gjvkuhcsk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.sjlbkw.cn/Article/details/gdzzgrrtx.sHtML

[F09] 获取文件大小
来源：http://wap.sjlbkw.cn/Article/details/guiqtqwuv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.vehdjk.com/Article/details/glyjuzbpr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gkxiaixjz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gfnaxgfra.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gpypcchbv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gxcynxwlx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.bbcook.cn/Article/details/gyjxvkzpx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyqmspxwo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gjxunruwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.yfazqb.com/Article/details/gkgyvghta.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvkdfglfg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.bbcook.cn/Article/details/gttimzbcg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/grvjvamlo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/gqmsbtrzw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gfpdlnnwv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gcemjmtpv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghtbighwh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gjjvfhijc.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gxiwphuor.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjwjhenex.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.vehdjk.com/Article/details/giropdxfo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gdwzramdi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gngqlksir.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gtaikggxs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gwtwenphz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvpprafeg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gjkynkwly.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gfuonzadt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gjkpazaez.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.tarul.cn/Article/details/gdldhhlhc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.epnwcf.com/Article/details/gqhshmknl.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gybenxjrx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gbgnxwdlg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.bbcook.cn/Article/details/ghydizhjv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.vehdjk.com/Article/details/gymtnpywu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gnqawpjli.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggffzjyno.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gvucskaut.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gczsejxev.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/glzmsxawv.sHtML

Py:   class User: pass
来源：http://www.share.vehdjk.com/Article/details/gpoplnvml.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gdzlgdkux.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gclrolmmx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/goprfxdnw.sHtML

Java: class User {}
来源：http://read.share.yfazqb.com/Article/details/gzhpqokox.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gibqydkxz.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gqoiuhmfq.sHtML

C#:   class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gohjuwhjk.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gihplzuba.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.sjlbkw.cn/Article/details/goxqbztng.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.sjlbkw.cn/Article/details/goygqtnid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.bbcook.cn/Article/details/guemdmfic.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gumqbwcwp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gguynqxxp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/gxwvtduac.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.sjlbkw.cn/Article/details/ggfxrknug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/ggcsqjzbw.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gaspanwvh.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/gcpmimnfg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gbohgaqrc.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gqwaeonzt.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gbibcozmo.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gljyzvfwk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gvmnsqjju.sHtML

Ruby: @name = "x"
来源：http://www.blog.yfazqb.com/Article/details/giifownka.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.tarul.cn/Article/details/gojetnlee.sHtML

[G04] 定义方法
来源：http://wap.sjlbkw.cn/Article/details/gyeowqeyd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/gwbexpgis.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fktsv.cn/Article/details/gecioiikf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gbyhubjua.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.vehdjk.com/Article/details/gvszktuit.sHtML

Java: String greet() { return name; }
来源：http://3g.sjlbkw.cn/Article/details/gpbjqcnnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.sjlbkw.cn/Article/details/gfvuubehy.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.epnwcf.com/Article/details/gyvjesfgf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.vehdjk.com/Article/details/gwprtyzlp.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/guydlzcaw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/glkokjuhr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.sjlbkw.cn/Article/details/gpdayyihj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gcyriebbq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gdszychiu.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gyxnhpmks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gmuztlgkk.sHtML

Ruby: class Admin < User; end
来源：http://baike.epnwcf.com/Article/details/gpasyurzu.sHtML

C#:   class Admin : User {}
来源：http://wap.epnwcf.com/Article/details/ggipetblx.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gugxmprtu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.vehdjk.com/Article/details/gubpzykeg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gruijdaqp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gggskzxjc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfjngoxcj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gaifwyzfy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.tarul.cn/Article/details/ggvhtkyrs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.sjlbkw.cn/Article/details/gczwwqiur.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.yfazqb.com/Article/details/gkrijwseo.sHtML

[G07] 调用父类方法
来源：http://wap.vehdjk.com/Article/details/gxadaxubp.sHtML

Py:   super().greet()
来源：http://www.blog.vehdjk.com/Article/details/gepedzlqq.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gplveqwvs.sHtML

JS:   super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gruuonrym.sHtML

TS:   super.greet();
来源：http://m.share.epnwcf.com/Article/details/gfqccphav.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gqpbgoubf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/geutmzsbo.sHtML

Ruby: super
来源：http://www.share.vehdjk.com/Article/details/gqqhkrads.sHtML

C#:   base.Greet();
来源：http://www.blog.yfazqb.com/Article/details/gxksvhjti.sHtML

[G08] 静态方法与属性
来源：http://wap.tarul.cn/Article/details/grdwofncv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.vehdjk.com/Article/details/gnnpjxgdd.sHtML

PHP:  public static function f() {}
来源：http://read.share.bbcook.cn/Article/details/gbvdqmqkv.sHtML

JS:   static f() {}
来源：http://www.share.fktsv.cn/Article/details/gprxjbela.sHtML

TS:   static f(): void {}
来源：http://3g.tarul.cn/Article/details/gphyqlvhu.sHtML

Java: static void f() {}
来源：http://www.m.share.bbcook.cn/Article/details/gvvdishdp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.epnwcf.com/Article/details/gegevjvml.sHtML

Ruby: def self.f; end
来源：http://wap.vehdjk.com/Article/details/gxgzzoyof.sHtML

C#:   public static void F() {}
来源：http://mobile.fktsv.cn/Article/details/gbonusmbm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fktsv.cn/Article/details/gzhdxnnzw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuiuktkm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gstmrilcu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.vehdjk.com/Article/details/gbscmonxu.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.epnwcf.com/Article/details/gbuguzkcp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.yfazqb.com/Article/details/gbfjxisaz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.epnwcf.com/Article/details/gjkmitahw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gbjvmzwor.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.vehdjk.com/Article/details/gzearvsep.sHtML

[G10] 访问控制
来源：http://blog.tarul.cn/Article/details/gxgacgzjj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gxqxzpwyw.sHtML

PHP:  public / protected / private
来源：http://blog.bbcook.cn/Article/details/gfkndttey.sHtML

JS:   #private 字段；其余公开
来源：http://baike.bbcook.cn/Article/details/gcleswhvz.sHtML

TS:   public / protected / private
来源：http://www.m.share.bbcook.cn/Article/details/gnbqgcymr.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.bbcook.cn/Article/details/gqbpsqmqx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fktsv.cn/Article/details/ghqslcffa.sHtML

Ruby: public / protected / private
来源：http://www.blog.vehdjk.com/Article/details/giekdmpdw.sHtML

C#:   public / protected / private / internal
来源：http://3g.fktsv.cn/Article/details/glhflhaiy.sHtML

[G11] getter / setter
来源：http://m.share.yfazqb.com/Article/details/gxwwbcsin.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fktsv.cn/Article/details/gyxefszty.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.epnwcf.com/Article/details/gvfoyacqf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.yfazqb.com/Article/details/guelwysag.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.sjlbkw.cn/Article/details/gqjteawqf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.epnwcf.com/Article/details/gqczahfai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.vehdjk.com/Article/details/gzshwjctg.sHtML

Ruby: attr_accessor :name
来源：http://blog.yfazqb.com/Article/details/gsobiisas.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.epnwcf.com/Article/details/gfmpigsxw.sHtML

[G12] 对象转字符串
来源：http://www.blog.tarul.cn/Article/details/gfcbvspkf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gvvepsaad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.bbcook.cn/Article/details/gnjghggnx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmezutlj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gqwzspwxl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gpsmzqmrs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gcwvmaptz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.tarul.cn/Article/details/gnfxdgakt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.bbcook.cn/Article/details/gjobgcsgw.sHtML

[G13] 判断对象类型
来源：http://wap.yfazqb.com/Article/details/glnsqtfvl.sHtML

Py:   isinstance(u, User)
来源：http://3g.tarul.cn/Article/details/gcdgpsier.sHtML

PHP:  $u instanceof User
来源：http://baike.yfazqb.com/Article/details/gmppoyywl.sHtML

JS:   u instanceof User
来源：http://m.share.fktsv.cn/Article/details/gycaxgdnn.sHtML

TS:   u instanceof User
来源：http://read.share.sjlbkw.cn/Article/details/geezfzhkn.sHtML

Java: u instanceof User
来源：http://mobile.fktsv.cn/Article/details/gmpfzihqg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fktsv.cn/Article/details/grwzntxaa.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.yfazqb.com/Article/details/gmtydevxh.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gzmyjpxti.sHtML

[G14] 数据类 / record
来源：http://3g.vehdjk.com/Article/details/gbjfxfsqg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.vehdjk.com/Article/details/gwhtckcyr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.sjlbkw.cn/Article/details/gmvafuoaf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fktsv.cn/Article/details/gqiamngwf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.vehdjk.com/Article/details/gsoacywpe.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.tarul.cn/Article/details/gckwhfnem.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.epnwcf.com/Article/details/gqdlsaolp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.sjlbkw.cn/Article/details/gnboasjng.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.bbcook.cn/Article/details/gmcuuzttv.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gemgmzpoa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.vehdjk.com/Article/details/grqdurlty.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.bbcook.cn/Article/details/grhtilxxj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.yfazqb.com/Article/details/gizjnhkjc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fktsv.cn/Article/details/gfldptref.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.bbcook.cn/Article/details/gtskyeths.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.vehdjk.com/Article/details/gilzwrrkz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.bbcook.cn/Article/details/gjhggeviw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.tarul.cn/Article/details/guzibpzbr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.bbcook.cn/Article/details/gebjxgtqc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.bbcook.cn/Article/details/guhorfndx.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.tarul.cn/Article/details/glaornlwq.sHtML

JS:   Object.entries(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggrsdfjks.sHtML

TS:   Object.entries(obj)
来源：http://www.share.vehdjk.com/Article/details/gfqfsjuqk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.yfazqb.com/Article/details/gfncsmemy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.bbcook.cn/Article/details/gmhqvmdng.sHtML

Ruby: obj.instance_variables
来源：http://www.share.vehdjk.com/Article/details/gmlfgrlkn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.epnwcf.com/Article/details/gxtwalvhi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvtehktdd.sHtML


<!-- 参考信息 -->