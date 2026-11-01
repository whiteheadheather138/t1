代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gcwhybydq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gmxbrghbb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gxaqexsue.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/gzpxbzuup.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.bbcook.cn/Article/details/gadqufeqv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gsbjjhirm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gcmuqbhoj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gippozduo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/gerbrjtrx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gpgkzzoyv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gjisdszqy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gniwnhssc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/ghloqliej.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/glqlvohqf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gqpaschdd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gxecsctas.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gfdruiuwz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gjhyegire.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/ggfgbzqei.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/garkhixho.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gblpbbavv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gbaagtygz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gtuhqoduk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/gchqvebye.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gsumfqcpg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/goxkoamso.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhcsilue.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/ggettspgx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gubninmnj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gtmzgddkd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gzichvany.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggqyqbsxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.vehdjk.com/Article/details/grzyxklmh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gvdiprmqy.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gaqkiqcms.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gfuzliynj.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gfoltjmlz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/giocupbsv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gcmoeqsyn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gvjndhqmv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gutyjsjpo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/ggpgxyanr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gybrigycu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gjmdihvte.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gfgdlxozd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gxqobzwek.sHtML

Py:   s.splitlines()
来源：http://m.share.vehdjk.com/Article/details/gbvjvsloe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gsqzbrrxx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gfcwekjdr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.epnwcf.com/Article/details/gjhtvnmyh.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gzbslgtpb.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/gynzpawby.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/giltpkjjz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gakpbgsze.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/gnetelqfj.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/govarwddf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/ghpeashvr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gjecqarsy.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gmvlaodur.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/glnyucjpg.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gabtakcgh.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/ghspseqyw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/gkmasednd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/grdcnzftc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gkqbmtopo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gcrvssebm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gbofjzpbz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/ghxhgirur.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gytcyugpz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gqpwbsjzt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gdeqhupjs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gckqzkoxm.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gjtpnilzp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.epnwcf.com/Article/details/gbfjtnifc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gjqswckbc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gpoyvpjei.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/glbrmszts.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/guptddtcv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gqmfadtam.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/ggnzlcfes.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtzrlmtu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbxdjevvm.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gbaooapgo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guyqenjlg.sHtML

[F01] 读取整个文件
来源：http://mobile.sjlbkw.cn/Article/details/gqzbdxukh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gdbtqrhoo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/guucbzywm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/geyeuflma.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gekbyagnf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gdayqifbd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gzbtbkgcg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/goijgxunk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/golzblvbw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/grgikhpcf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gimtgwxns.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gsorosmpa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gbtwzswdp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gitwxjduv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gsngnlhmr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gqalnmttz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/grtwosoll.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gybiaznww.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gibevdntr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gqwjkbxbc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/grvuhmvrg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/ggaffrlbd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gwzenccap.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/golhwdply.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gsjqinwgh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gziycoall.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/greafkpuo.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gctacbcod.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/ghigsqpbe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gzdqzyzpl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gpkjahicq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gowztstku.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/grdbtkfkg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gzzzljxui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.sjlbkw.cn/Article/details/ggjiuwjio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.vehdjk.com/Article/details/gnwunfkky.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/gwperrxjf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.yfazqb.com/Article/details/gsjvwpowz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gbtpbbjph.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gddbziklu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gbkandewy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gcbyrbthu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gbqzoedve.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gwyejajip.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gjedfadqs.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/gtwpjiepu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gybcdvbqt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gohjwkkai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gqnxghizp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.tarul.cn/Article/details/gymkzibkm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gywjzujva.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gcyjxohsv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gasdwpsca.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gbpwsjqyg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gahlmzqvg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gpbycjxzo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gkxrfqvsw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gwgtfwuig.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/gseyusipq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/gxpgjklkp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gwrrcyxpw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.bbcook.cn/Article/details/gjfwgplwo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/gkqkpzxlk.sHtML

[F08] 遍历目录
来源：http://www.m.share.yfazqb.com/Article/details/gakujucuq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gpmurvehm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gfixclffv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gpzqmhqzp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gomykyndl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gmyvsfuxn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gsncduzhb.sHtML

Ruby: Dir.children("dir")
来源：http://3g.sjlbkw.cn/Article/details/gkcmgmhry.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.tarul.cn/Article/details/ghbyygavi.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/gtvdhexrx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grdvxydgj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gyqtxcikq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gmsbiendd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.vehdjk.com/Article/details/gtoyzkkkp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gflntzhsb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gynkfxdss.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gghffilgj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/grfforxcx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gpguskxuo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gsmlqaybx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.tarul.cn/Article/details/gzcwewggd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdnditlcm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.tarul.cn/Article/details/ghpyvaifn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gbvfkybya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gwvdfghxu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gcphnwkca.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gudwlyevw.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gymedybji.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/giimwmhac.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdhyuikt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gtxgtexpk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gloslneet.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gkmgqrkom.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gewfgjyhg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gyidcdmrv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gwqokykag.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gfyvmntcu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gsfnvpmhk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gxjmyvsvz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.vehdjk.com/Article/details/gvqblatic.sHtML

TS:   // 同上
来源：http://wap.vehdjk.com/Article/details/gwvblgtta.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.epnwcf.com/Article/details/gwfavlmxv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gyyyftktl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/goxzhnqep.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.sjlbkw.cn/Article/details/gtfsdzkgz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwnyrencx.sHtML

G. 面向对象
来源：http://wap.vehdjk.com/Article/details/gsdctcsjf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gtrafagnw.sHtML

[G01] 定义类
来源：http://wap.yfazqb.com/Article/details/gajpkvbsd.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gxpnrxcsy.sHtML

PHP:  class User {}
来源：http://mobile.fktsv.cn/Article/details/gzbgkbpdw.sHtML

JS:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gvglukbxz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gzejqsvwh.sHtML

Java: class User {}
来源：http://blog.bbcook.cn/Article/details/gfmlpjgli.sHtML

Go:   type User struct { Name string }
来源：http://read.share.vehdjk.com/Article/details/gpypootfw.sHtML

Ruby: class User; end
来源：http://www.blog.vehdjk.com/Article/details/gtoagqnyx.sHtML

C#:   class User {}
来源：http://www.share.epnwcf.com/Article/details/grqllwdbn.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gkghjzehv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.vehdjk.com/Article/details/gyqercjpr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.vehdjk.com/Article/details/gpyeqzyey.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gcypvramb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/gqjpfrydg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/ghzamqnrn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gagswcveu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gbntvhblc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fktsv.cn/Article/details/gkoujeghw.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/guztjyezu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gyajvwplf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.tarul.cn/Article/details/gycayfvyk.sHtML

JS:   this.name = "x";
来源：http://baike.bbcook.cn/Article/details/gektovtkd.sHtML

TS:   name: string = "x";
来源：http://www.m.share.tarul.cn/Article/details/gsssfphwa.sHtML

Java: private String name;
来源：http://mobile.vehdjk.com/Article/details/ghycfaldg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.bbcook.cn/Article/details/gakdpujud.sHtML

Ruby: @name = "x"
来源：http://m.share.bbcook.cn/Article/details/gipjimoyg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gbqgyzbcz.sHtML

[G04] 定义方法
来源：http://baike.bbcook.cn/Article/details/gxphgbqtk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.sjlbkw.cn/Article/details/glbzkjfpb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/ghleghlts.sHtML

JS:   greet() { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gamtyjvgx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/genfsguoi.sHtML

Java: String greet() { return name; }
来源：http://m.share.vehdjk.com/Article/details/glfvorylo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gsfuacltr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gweujgmwx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gbyuozyim.sHtML

[G05] 继承
来源：http://baike.vehdjk.com/Article/details/gwghwybkg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fktsv.cn/Article/details/gnhoolrqu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gfqtambnm.sHtML

JS:   class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gwoacauas.sHtML

TS:   class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gqwtxnxek.sHtML

Java: class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gcsdzxeqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.bbcook.cn/Article/details/gixyrhcdy.sHtML

Ruby: class Admin < User; end
来源：http://m.share.epnwcf.com/Article/details/grlpkqfgt.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/gvvmvdhqz.sHtML

[G06] 重写方法
来源：http://read.share.tarul.cn/Article/details/gkmjuersn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.bbcook.cn/Article/details/gzecvrupv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gbqlsusmz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.vehdjk.com/Article/details/gkwykkfzt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.vehdjk.com/Article/details/gurjogahf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gyyuvjvgx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.sjlbkw.cn/Article/details/gnjuerhuk.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.vehdjk.com/Article/details/goqsyngaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.epnwcf.com/Article/details/gatnfpdqq.sHtML

[G07] 调用父类方法
来源：http://baike.fktsv.cn/Article/details/gikcozlxb.sHtML

Py:   super().greet()
来源：http://www.share.yfazqb.com/Article/details/gqgtystrw.sHtML

PHP:  parent::greet();
来源：http://m.share.epnwcf.com/Article/details/gzdbvbedo.sHtML

JS:   super.greet();
来源：http://www.blog.sjlbkw.cn/Article/details/govsmegzj.sHtML

TS:   super.greet();
来源：http://3g.yfazqb.com/Article/details/gsjcbfqng.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/gxceoghgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.tarul.cn/Article/details/gqoaysxxy.sHtML

Ruby: super
来源：http://baike.epnwcf.com/Article/details/gbmcgjepg.sHtML

C#:   base.Greet();
来源：http://read.share.tarul.cn/Article/details/ghljsnbwy.sHtML

[G08] 静态方法与属性
来源：http://www.share.yfazqb.com/Article/details/gztnwyree.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.bbcook.cn/Article/details/gwroqppja.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fktsv.cn/Article/details/gwsnbcbxf.sHtML

JS:   static f() {}
来源：http://wap.vehdjk.com/Article/details/gsigoqkyg.sHtML

TS:   static f(): void {}
来源：http://www.blog.epnwcf.com/Article/details/gkbrwtnrs.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/ggarfkljc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.yfazqb.com/Article/details/gfdcnbrlr.sHtML

Ruby: def self.f; end
来源：http://www.blog.tarul.cn/Article/details/gluhwtdir.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/ggfyudotq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.yfazqb.com/Article/details/gdkbmohhi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/gunfcwtkp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyreybedm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.sjlbkw.cn/Article/details/grjracxes.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.bbcook.cn/Article/details/gnejqkixk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.sjlbkw.cn/Article/details/gslhfpvzh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.bbcook.cn/Article/details/gybtcykyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.tarul.cn/Article/details/gjydkvvpc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.tarul.cn/Article/details/gipumoigw.sHtML

[G10] 访问控制
来源：http://www.share.epnwcf.com/Article/details/gygutorjw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gpwnktnlh.sHtML

PHP:  public / protected / private
来源：http://3g.epnwcf.com/Article/details/gmiqlxnvi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.tarul.cn/Article/details/gkljdnayz.sHtML

TS:   public / protected / private
来源：http://wap.tarul.cn/Article/details/gdcjkkyms.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.tarul.cn/Article/details/glsvdogql.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.vehdjk.com/Article/details/gskaacmgk.sHtML

Ruby: public / protected / private
来源：http://wap.sjlbkw.cn/Article/details/gauzsrvuc.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fktsv.cn/Article/details/gdecdjfqe.sHtML

[G11] getter / setter
来源：http://3g.vehdjk.com/Article/details/gupnkmtlw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.epnwcf.com/Article/details/gndueckko.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfhduaiyu.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.epnwcf.com/Article/details/ggultxjia.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.bbcook.cn/Article/details/gilvhlcrz.sHtML

Java: public String getName() { return name; }
来源：http://mobile.tarul.cn/Article/details/gqevccjou.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gktcwzhvu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fktsv.cn/Article/details/gyhdsopxi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.bbcook.cn/Article/details/goeawotzx.sHtML

[G12] 对象转字符串
来源：http://wap.epnwcf.com/Article/details/gudlvbidb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.bbcook.cn/Article/details/gkzkilqop.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gbhooukkf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gujfpgsqt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gdrokbsno.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.tarul.cn/Article/details/gcioatknl.sHtML


<!-- 参考信息 -->