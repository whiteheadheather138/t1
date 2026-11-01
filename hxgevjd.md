代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gvkpibviq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gwqgitelh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/ggbphjxqm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gtmjogwko.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gppeprmvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gpizdxjie.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/ggvctkpfo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gceremfbk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/geprpkgnd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/grirqyjss.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/ghtkudxxu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gogqknjzs.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gpvqbchap.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/ggrvapdfu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/ghijhusxg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gvlcskmmx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gfvwapyqz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gxjazlxww.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/giuisishn.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/guwwdbgab.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gitfaaodz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gbrnaqwbs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gpljbgnte.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gvakhldxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/gxnodmmkd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gzvyohxeh.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gcysycdjh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gwwgwiqck.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gegvktpjd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/glbwxcuoi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/ggzfyypzo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/ggbqovyab.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gevjorgsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjhanrqsu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gvmmnprjq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gnqbcarna.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gcbseiukp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gjtgkovxl.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/geezmrbgw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.epnwcf.com/Article/details/gwconbfvf.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gkovapzfe.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gsqhnxkzs.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/grhgdgxgw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gruezzafh.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gpryefxdf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gygfvqtwy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gbcdfzggj.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gzuymblxz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/geqrkdodm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/ghvrzmqpv.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gvmnelavd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gpccxvrcq.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gryyydher.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gtavlrbwu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gnazysygx.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gfetyqyte.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gyoqsupbo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gmyjnwdvx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gfgllcqwl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gewuxaydl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gxttadrhx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gbbwzclsp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gvbcqhimq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gtizhbiwr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gxdwyglzc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmjrycqhc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/ghirkekla.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gbtlxohiv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gsjibxyxu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gpvgiaxlz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/grcusufam.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/glebmgwig.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/giqdufkix.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcysvdprg.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gtaaeevdu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfnskgxvr.sHtML

[F01] 读取整个文件
来源：http://3g.tarul.cn/Article/details/gykewcflm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gqsnlxyae.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gzgrwvvfy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gtwtgayms.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gbzpmayog.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gehuplklq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gnzoieyri.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnbumjhtk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gjjtbkwkl.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/ghqzdmisz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gutxfocgm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/goeuhcbqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/glxzenagi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gvzskhydg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/grvlkkkds.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/gxtmdbaww.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gmtxqugdj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/gusakitar.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/ggsmrgomi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gqsmoclxx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gonireruc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gowwxkimc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gurrfwwwi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gfaopwlhz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.vehdjk.com/Article/details/giwolqfxs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gdhqsjmgx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gifslbzlr.sHtML

[F04] 追加写入文件
来源：http://wap.fktsv.cn/Article/details/gnhgdsdis.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.yfazqb.com/Article/details/gwlrzuzhq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gmdaurdcv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/guaxfuyiw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gclrqsvwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.epnwcf.com/Article/details/gcjnjlocd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gmhwrpdls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gzwfzrhit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gbvtqazzo.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gzpccdogg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gffjflhdx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjjtctfjy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gubrxttwd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gorisbtzj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gwlxoecck.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gnwrxwhon.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnsgtyomd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghnubwywi.sHtML

[F06] 删除文件
来源：http://www.blog.yfazqb.com/Article/details/gjijwsyim.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gqnjiigdr.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/glgzlptno.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gvdpmwjdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/glhjemliz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gbwelfoht.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gtbgkdevj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.bbcook.cn/Article/details/gpjxjcsdo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdwoarmnl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.vehdjk.com/Article/details/gxwsyzgnj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gsltihofn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gqyiqjxxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gvhzbfngu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gsanxklhr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.tarul.cn/Article/details/gjokrvfvw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/gcbcdbrjf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gufpcgzkt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gmoqvoqqq.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/ghlcwdevu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gqafzxcel.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.bbcook.cn/Article/details/gwznwetqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gtiqtofkz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gnsoepjzg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gqtdsprnz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gxutrmyfo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gkwoxqrza.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.yfazqb.com/Article/details/gmwrnmiih.sHtML

[F09] 获取文件大小
来源：http://www.share.bbcook.cn/Article/details/gnfachmco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwirqtrvl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gbyqrhjym.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gimpqsxjw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.epnwcf.com/Article/details/gkasoxcjc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gshbfcirk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.bbcook.cn/Article/details/gegtltzcu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fktsv.cn/Article/details/gyhureanh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gqsheixzg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/grajvtsff.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gfdspdbsv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/guuhwvaeh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gryusrgfy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvuffbpzp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/geszmzscw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gcitudsfx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gnwrxoprp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gsxtozhvh.sHtML

[F11] 复制与移动文件
来源：http://wap.fktsv.cn/Article/details/gzevjinwc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzqudkbkn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gpudjaoxd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gexqvnjxt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/glyjjdrjg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gmjembgjp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.vehdjk.com/Article/details/gcwvszxbj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gtipbjbdu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.epnwcf.com/Article/details/gprcztkdj.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gzzufaage.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gblmctubg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gborwfrce.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.bbcook.cn/Article/details/gvrvgyopu.sHtML

TS:   // 同上
来源：http://read.share.vehdjk.com/Article/details/gjymutxbz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.sjlbkw.cn/Article/details/gthlfftad.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gicqrocow.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/ghkwkylxz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fktsv.cn/Article/details/gcotutvob.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbjftmkns.sHtML

G. 面向对象
来源：http://www.m.share.sjlbkw.cn/Article/details/guwefyxek.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfmwbuckc.sHtML

[G01] 定义类
来源：http://m.share.vehdjk.com/Article/details/gwltkkwdd.sHtML

Py:   class User: pass
来源：http://blog.vehdjk.com/Article/details/geypixfcq.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gtopzkgrm.sHtML

JS:   class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gkisovnze.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/ggdrvahot.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/grlaljsys.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/grnpomkat.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/gbftyrmin.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gjwzgwgdg.sHtML

[G02] 构造函数
来源：http://m.share.yfazqb.com/Article/details/gwjspvbia.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.epnwcf.com/Article/details/gqthdosda.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.tarul.cn/Article/details/gjsovifba.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gzqgdfjlj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gmrmgkhee.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.epnwcf.com/Article/details/gassmwflu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fktsv.cn/Article/details/glwrayhch.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.bbcook.cn/Article/details/gfxsiyvhw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gwdqtujxb.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/ggzwhcwcc.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/ggemxifkm.sHtML

PHP:  public string $name = "x";
来源：http://wap.vehdjk.com/Article/details/gizppeubc.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/gkiopbkjq.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gzgfozmjf.sHtML

Java: private String name;
来源：http://www.share.epnwcf.com/Article/details/gccihzhqq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.bbcook.cn/Article/details/gajlrgdsu.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gvuklrdya.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.yfazqb.com/Article/details/gciximajj.sHtML

[G04] 定义方法
来源：http://wap.epnwcf.com/Article/details/gbtjfpcra.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.epnwcf.com/Article/details/gzklxjkko.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gkvzrukef.sHtML

JS:   greet() { return this.name; }
来源：http://wap.tarul.cn/Article/details/grwsvbjgd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/gawdbshim.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gplqkpsbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.bbcook.cn/Article/details/gjhtbdcty.sHtML

Ruby: def greet; @name; end
来源：http://baike.bbcook.cn/Article/details/gkqsilxfr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.yfazqb.com/Article/details/gzqipqrik.sHtML

[G05] 继承
来源：http://blog.epnwcf.com/Article/details/glthsumoe.sHtML

Py:   class Admin(User): pass
来源：http://3g.sjlbkw.cn/Article/details/gxuhplxid.sHtML

PHP:  class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/gsbrhjlpx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gjrlkyjrr.sHtML

TS:   class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gyxodmqpd.sHtML

Java: class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/geuygycyr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.tarul.cn/Article/details/gifpxwvbj.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/ggliwcvqx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsjsxkea.sHtML

[G06] 重写方法
来源：http://www.share.vehdjk.com/Article/details/gwbuicgtf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gsbuxsmxl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.bbcook.cn/Article/details/gxvrvrqjq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gyumtajnx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gwdkottwx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.vehdjk.com/Article/details/gwylcgjml.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.sjlbkw.cn/Article/details/glstruuka.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.yfazqb.com/Article/details/grcnfrlbx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.vehdjk.com/Article/details/grmficmyo.sHtML

[G07] 调用父类方法
来源：http://wap.tarul.cn/Article/details/gzyugwfub.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gjhamjetn.sHtML

PHP:  parent::greet();
来源：http://baike.bbcook.cn/Article/details/gxaemymsz.sHtML

JS:   super.greet();
来源：http://baike.fktsv.cn/Article/details/gheegimun.sHtML

TS:   super.greet();
来源：http://blog.yfazqb.com/Article/details/gigpfyzrw.sHtML

Java: super.greet();
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkrrmxjp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.epnwcf.com/Article/details/gxsmrsmnj.sHtML

Ruby: super
来源：http://blog.bbcook.cn/Article/details/gvicemors.sHtML

C#:   base.Greet();
来源：http://m.share.fktsv.cn/Article/details/gbuqajvjk.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gqktzkdaf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gknuumjft.sHtML

PHP:  public static function f() {}
来源：http://blog.bbcook.cn/Article/details/geyduotoy.sHtML

JS:   static f() {}
来源：http://www.share.epnwcf.com/Article/details/ghjnnjzat.sHtML

TS:   static f(): void {}
来源：http://3g.bbcook.cn/Article/details/ggxwetghg.sHtML

Java: static void f() {}
来源：http://baike.sjlbkw.cn/Article/details/gumedogyu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fktsv.cn/Article/details/ggoxctomr.sHtML

Ruby: def self.f; end
来源：http://read.share.yfazqb.com/Article/details/gwogptqvz.sHtML

C#:   public static void F() {}
来源：http://m.share.vehdjk.com/Article/details/gsqvmhfll.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.yfazqb.com/Article/details/gsnwvjokv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.yfazqb.com/Article/details/ggszztrcw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.epnwcf.com/Article/details/gyrwezzly.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.tarul.cn/Article/details/gwdmijalj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.tarul.cn/Article/details/gdejggsag.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.epnwcf.com/Article/details/gvxrflywy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.epnwcf.com/Article/details/gpxzzbwgb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.bbcook.cn/Article/details/gjusrvfkd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/gahnyivuv.sHtML

[G10] 访问控制
来源：http://3g.fktsv.cn/Article/details/gvqidjgrn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.bbcook.cn/Article/details/gbbhjeexb.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gtmsromvm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.tarul.cn/Article/details/gagwpvgec.sHtML

TS:   public / protected / private
来源：http://3g.bbcook.cn/Article/details/gnfcutcbi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.epnwcf.com/Article/details/gckidziko.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.sjlbkw.cn/Article/details/gboeganen.sHtML

Ruby: public / protected / private
来源：http://3g.bbcook.cn/Article/details/gmbxegtxz.sHtML

C#:   public / protected / private / internal
来源：http://blog.epnwcf.com/Article/details/gmaezldgs.sHtML

[G11] getter / setter
来源：http://blog.epnwcf.com/Article/details/gztqnqpeu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.yfazqb.com/Article/details/gdcptrewi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.tarul.cn/Article/details/gphgnxqvx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.epnwcf.com/Article/details/gnoezfszv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gufqbhyej.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gkkfeaauj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/glfpzbmtn.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fktsv.cn/Article/details/gvusbgibd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fktsv.cn/Article/details/gbsaghiut.sHtML

[G12] 对象转字符串
来源：http://www.share.yfazqb.com/Article/details/gmftdttll.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gqoenhgla.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gkjaxbhwp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/gdzudyegy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gpigkqgxq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.epnwcf.com/Article/details/gernxmxpu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.bbcook.cn/Article/details/gvwjufdvg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.bbcook.cn/Article/details/gqbllqqxi.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.epnwcf.com/Article/details/gurxznvvf.sHtML

[G13] 判断对象类型
来源：http://www.blog.yfazqb.com/Article/details/grtwgmezb.sHtML

Py:   isinstance(u, User)
来源：http://baike.sjlbkw.cn/Article/details/giyplevbh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.bbcook.cn/Article/details/gmijfodcd.sHtML

JS:   u instanceof User
来源：http://3g.vehdjk.com/Article/details/glzigonry.sHtML

TS:   u instanceof User
来源：http://3g.epnwcf.com/Article/details/gyqowgngh.sHtML


<!-- 参考信息 -->