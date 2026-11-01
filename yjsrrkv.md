代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gkshqzzui.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gsehzgjuc.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/glljsimob.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gqapxrzji.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gtovleubx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gqjqnfzde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gjkkuwxww.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gwgkaamhi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gsrhyywxo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gpmtvjfrn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gdrflbgjg.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/glazhgwvk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gljrngqtj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/ghnnablpq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/grbkcqfrm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gctjidikc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/guxzkcsgd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gorvynsfv.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gkgsffsms.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/glmhdnqhq.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/gyxuztslk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.vehdjk.com/Article/details/gkuikcfue.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gyxnvogbu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gktnjiyiv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gnbhsydpw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gisgqvnjd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gprmibhob.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/geoewiyun.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/gymitrzfe.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gthoyilgx.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/grpeunrfe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gmfrscvtv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gcurkeqqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gdovnkyiy.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gfrmlwabq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gtbrgqgrs.sHtML

Ruby: s.lines
来源：http://wap.tarul.cn/Article/details/gedfhcdmc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gplwxqtfo.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/ghltrqrer.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gemtdcfsx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gtjukkzch.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.epnwcf.com/Article/details/grnkeaxps.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gbhkgosir.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/guqckvelu.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gwlgazeha.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/gvfnsouvc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gknxkveef.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gqhebsagx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/grsvqgqud.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gmxfqfsyk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gwpusotya.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/ggwkwwwgd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gtufszbeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gympmlppm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gknrzashj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gadgighoj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gxngivlsi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gsnyrzaep.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gmoxnluul.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ggyugtzvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/ghdhsvbmy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gaswihhwt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/gbwfkpdqd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gpxjqcjtt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gwllpahjc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/ggsobvwnz.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/grlchrwzt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gtixpokfi.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gpkbvephe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/glakxbkoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/ggqixyvrs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gqdakfxja.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gustuiznj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gxkqytnzs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gipnloomo.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjvafflnp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gjqpfhczy.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gtqgredet.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.epnwcf.com/Article/details/gafqenzxa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/ggrnhtcjh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gfsmutopd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gwurukgwd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gcjkzdhfn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.sjlbkw.cn/Article/details/gwyosfydk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkflofrl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gqbvvxtmp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.bbcook.cn/Article/details/gsujdunqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gyeclzpzf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/ghvgzlkbd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gxirxlnlw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gqsxyvety.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.epnwcf.com/Article/details/gpgdchssr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gacywojqi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gtazdyfdj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/ghkidprbs.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gesnxcwja.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gqwhgciug.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fktsv.cn/Article/details/gvgfgpxhi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gostzurtm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/giskxcjsm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.tarul.cn/Article/details/gpedtysle.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/ganccnryj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gsyypukzo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/guhatwjwr.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gdrftefqk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/gpmansjmr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gmdcdnbfx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/guwftrejc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxseitmgc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gdxvtgzej.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gyhwtdkpx.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gaagpfcua.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqjvfdmos.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/glbmaxfaf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gypitxozs.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gdemjtxii.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjycjuyqu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvwqoazpg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gvpyrmipk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gckmhkjlu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggzgzytpe.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/guofbbhre.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gomjjjxhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gofcdtbke.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.yfazqb.com/Article/details/gkmabrwov.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gcnjdgnit.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/gkxfekhtt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/ggtvsxevw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gwuocozpe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.epnwcf.com/Article/details/goalxivud.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gnubqhkzb.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gmhzcbuhg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.bbcook.cn/Article/details/gmuenmnkm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fktsv.cn/Article/details/gcwxsmmxy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gflivuekp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gmspqhpyc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gfgltadbo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gzpccxvuz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gmwfzmira.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fktsv.cn/Article/details/gspvwohgb.sHtML

[F09] 获取文件大小
来源：http://www.share.fktsv.cn/Article/details/gdxmdduik.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gsulkuwnk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gluajkskx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.tarul.cn/Article/details/gfrruujkx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gnblodwyk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gfgdfwdkl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fktsv.cn/Article/details/gwfrpphzm.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjbawpzjt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/ggkvageng.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.epnwcf.com/Article/details/gxedpdijk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfedaaozt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gonkjavpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gawfwjxbg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gkwykslgr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gilxdccuj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpgvtbumy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfdreykyt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gnociavsn.sHtML

[F11] 复制与移动文件
来源：http://m.share.fktsv.cn/Article/details/gohbtwggn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gnseqeodf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gervkfnmq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/grqglcfsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gazaqehwj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.epnwcf.com/Article/details/gofywbogc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gqlupipoo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gdnqttrhv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gfjjtvolc.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gszyxbsyd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/girownejw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fktsv.cn/Article/details/gvhvncnqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gnoaywtke.sHtML

TS:   // 同上
来源：http://www.blog.tarul.cn/Article/details/gufwcyagn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/goddwrxpa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gvbgijgbr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fktsv.cn/Article/details/gzwexcwdx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fktsv.cn/Article/details/gculcvngj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glgxkbwjr.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gkkgrxrhx.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gczdvzdas.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/gtwgisywh.sHtML

Py:   class User: pass
来源：http://baike.sjlbkw.cn/Article/details/gneydcgeq.sHtML

PHP:  class User {}
来源：http://blog.tarul.cn/Article/details/gotvibzzq.sHtML

JS:   class User {}
来源：http://mobile.epnwcf.com/Article/details/gcfflhhgz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.vehdjk.com/Article/details/gxvblyuse.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkicbtuym.sHtML

Go:   type User struct { Name string }
来源：http://baike.bbcook.cn/Article/details/gskhahulk.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/gxakybhal.sHtML

C#:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/ghgdsksyv.sHtML

[G02] 构造函数
来源：http://baike.yfazqb.com/Article/details/gcjissdtn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fktsv.cn/Article/details/gmnciveah.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gdsqvpefa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gbxykidvx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.vehdjk.com/Article/details/gtiwqannp.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/goxoiubfp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gaglfhjvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.epnwcf.com/Article/details/ghfqdozju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.tarul.cn/Article/details/grkdjopmh.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gfmegahjg.sHtML

Py:   self.name = "x"
来源：http://blog.bbcook.cn/Article/details/gxlavqnns.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/glokjkmzd.sHtML

JS:   this.name = "x";
来源：http://m.share.bbcook.cn/Article/details/grhlasocp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.epnwcf.com/Article/details/geijapwvx.sHtML

Java: private String name;
来源：http://3g.tarul.cn/Article/details/glprurwme.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gsqqhdtui.sHtML

Ruby: @name = "x"
来源：http://mobile.yfazqb.com/Article/details/goyhfavjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.epnwcf.com/Article/details/gavkslhng.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/gouaxrpjr.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.vehdjk.com/Article/details/gupuaenbb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gitwcnfcq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.epnwcf.com/Article/details/gkewksvmy.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gevoitjhu.sHtML

Java: String greet() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gfbdfaivm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gsiligria.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/glzrxiquw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.tarul.cn/Article/details/gljdzxgkp.sHtML

[G05] 继承
来源：http://www.m.share.tarul.cn/Article/details/gvspxtolk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/grmhowpna.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gmsfllwjp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdqwpboih.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gfhufdqqn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/gxhahvmky.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.sjlbkw.cn/Article/details/gcnmetsis.sHtML

Ruby: class Admin < User; end
来源：http://baike.tarul.cn/Article/details/gniqaheui.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fktsv.cn/Article/details/gnvycpiar.sHtML

[G06] 重写方法
来源：http://www.m.share.fktsv.cn/Article/details/gmapxuptn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.tarul.cn/Article/details/gbuzpguig.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gxjcpazrj.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.epnwcf.com/Article/details/gedkikzgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/gnyporcqp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gegrqsvgh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gbimpidby.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.epnwcf.com/Article/details/gyrllwpoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.epnwcf.com/Article/details/gmscymrhu.sHtML

[G07] 调用父类方法
来源：http://mobile.epnwcf.com/Article/details/gibprepgo.sHtML

Py:   super().greet()
来源：http://www.blog.bbcook.cn/Article/details/guzggzfzb.sHtML

PHP:  parent::greet();
来源：http://wap.epnwcf.com/Article/details/gopigvnat.sHtML

JS:   super.greet();
来源：http://m.share.tarul.cn/Article/details/gcqrzmfsu.sHtML

TS:   super.greet();
来源：http://3g.vehdjk.com/Article/details/gzctitxri.sHtML

Java: super.greet();
来源：http://www.m.share.bbcook.cn/Article/details/gyscjtqsc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.bbcook.cn/Article/details/ggulmvoab.sHtML

Ruby: super
来源：http://m.share.tarul.cn/Article/details/gqdpyybfo.sHtML

C#:   base.Greet();
来源：http://blog.epnwcf.com/Article/details/gokrchizc.sHtML

[G08] 静态方法与属性
来源：http://blog.fktsv.cn/Article/details/gxdyrcbqb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.vehdjk.com/Article/details/gdpkfiwjb.sHtML

PHP:  public static function f() {}
来源：http://mobile.bbcook.cn/Article/details/gmlqmxpip.sHtML

JS:   static f() {}
来源：http://baike.vehdjk.com/Article/details/gmpmksiqz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.vehdjk.com/Article/details/gcxstylwk.sHtML

Java: static void f() {}
来源：http://3g.sjlbkw.cn/Article/details/ggozftttx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.epnwcf.com/Article/details/giipreugc.sHtML

Ruby: def self.f; end
来源：http://www.blog.yfazqb.com/Article/details/gkirfclfo.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gvlrkzata.sHtML

[G09] 接口 / 抽象类
来源：http://blog.vehdjk.com/Article/details/gpuobspdr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.sjlbkw.cn/Article/details/ghkkaedms.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.yfazqb.com/Article/details/gnifpkjhb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fktsv.cn/Article/details/gaoaugseu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gdeutpeuv.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdnzzyozf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.epnwcf.com/Article/details/gqvdndyri.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.bbcook.cn/Article/details/ghtgaifyv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.yfazqb.com/Article/details/gvfpbosuu.sHtML

[G10] 访问控制
来源：http://m.share.bbcook.cn/Article/details/gamehdgag.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.sjlbkw.cn/Article/details/gdlwikyna.sHtML

PHP:  public / protected / private
来源：http://m.share.vehdjk.com/Article/details/griimnndc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.epnwcf.com/Article/details/gumqacjkh.sHtML

TS:   public / protected / private
来源：http://www.share.vehdjk.com/Article/details/gsjifvuoq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.yfazqb.com/Article/details/gcuiefczh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.tarul.cn/Article/details/gefeedsvz.sHtML

Ruby: public / protected / private
来源：http://3g.fktsv.cn/Article/details/ggzrumvnw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.epnwcf.com/Article/details/ggcxyjxyb.sHtML

[G11] getter / setter
来源：http://mobile.bbcook.cn/Article/details/gslukuiik.sHtML

Py:   @property 与 @x.setter
来源：http://3g.tarul.cn/Article/details/gfobxvmpr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.epnwcf.com/Article/details/gigsehnjp.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fktsv.cn/Article/details/gozlkybdu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdnigfopz.sHtML

Java: public String getName() { return name; }
来源：http://3g.yfazqb.com/Article/details/gmrvqaick.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/glfdmwxcc.sHtML

Ruby: attr_accessor :name
来源：http://blog.tarul.cn/Article/details/gsovfsnnx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fktsv.cn/Article/details/ggleuqexm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.tarul.cn/Article/details/gdpmvrcgq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fktsv.cn/Article/details/grylpgssd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/gzyoxcpoc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.tarul.cn/Article/details/gvpspyuyk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gezzmstqv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.vehdjk.com/Article/details/ghkicqtlz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/grrfiuyau.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fktsv.cn/Article/details/gjoxxvlyh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fktsv.cn/Article/details/gxjdtiwju.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/gtaraaubf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.epnwcf.com/Article/details/gtbepower.sHtML

PHP:  $u instanceof User
来源：http://3g.vehdjk.com/Article/details/gujqaazdn.sHtML

JS:   u instanceof User
来源：http://www.share.yfazqb.com/Article/details/gjdqqslkd.sHtML

TS:   u instanceof User
来源：http://mobile.tarul.cn/Article/details/gkksdxyhr.sHtML

Java: u instanceof User
来源：http://www.blog.bbcook.cn/Article/details/gytzaotpv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.sjlbkw.cn/Article/details/gxxytksal.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.tarul.cn/Article/details/gtkwtrxmi.sHtML

C#:   u is User
来源：http://www.blog.tarul.cn/Article/details/gdanbtcrc.sHtML

[G14] 数据类 / record
来源：http://baike.vehdjk.com/Article/details/gptciqfrb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fktsv.cn/Article/details/gwlnyullm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.epnwcf.com/Article/details/glkaqdvkv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.vehdjk.com/Article/details/grkbipfpd.sHtML


<!-- 参考信息 -->