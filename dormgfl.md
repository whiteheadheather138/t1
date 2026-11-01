代发 wailian999

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gzomwkvom.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gbzptpaot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gukjkgavh.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gbslwqkkw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/gjbiubzwj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gidpvbvjk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ghhogauvq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/ggdvjwytm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/glaiofekl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/gjeuutjpc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gbvtnnkqo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.tarul.cn/Article/details/gaiczbjiu.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/gdqvjhshv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gwcuzngmk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gwhfufecp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gisodwmqg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/ghwlcanjk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/gxidijntk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/gnldttnfp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gpyqyzmwz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gsfxfzjnz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gvbybwyca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.epnwcf.com/Article/details/gjrirpxbc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gmxuagzwk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.tarul.cn/Article/details/gxgdsmntv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gruqohflv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/ggamklvtz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/grskaifqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gudydpboo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gyzkawodp.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gkpxxisls.sHtML

Py:   f"{1234567:,}"
来源：http://blog.epnwcf.com/Article/details/goygioroi.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gxudolxkc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gqfsmwlnq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gbbtfxobw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gfdjceuxs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gdpioafxm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gjrayuqfr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gqqcudwvw.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/goherdxwq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.epnwcf.com/Article/details/gnoximvuu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/ggvauhalf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/grczgwmny.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gjuczcaqo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gkrdsyzig.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/guxctsqxa.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gxqenyoum.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gewxlbydk.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gibxmqtwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/gyzetfosa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gcjzwjgkk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/ghfumfxjh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gayixrccx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gblbrxkjv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gzstajnlu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/ghurtgpwr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gbaglbply.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gqcawnsus.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/griliaabk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gnckmjcwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gsaajfcqd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gccnwjsuj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gospltzhz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gxjhvuxpg.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gkksgejwf.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gazzzuwul.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gimejpppx.sHtML

Py:   if not s:
来源：http://m.share.yfazqb.com/Article/details/geclyvrvx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/grnfclorh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gppgibyzi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxzkdxzpx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpgbhafyb.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gnfmwnssq.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gnrtpvyws.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.yfazqb.com/Article/details/gyjcjoigt.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gaoujqbod.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gnztbqywt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gcidlcmzd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gqsncpbbr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gbgkaxwla.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gxjpwszih.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gsrkwgzrx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gkbewqhyo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gbrptzxzo.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gannwwouy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gnwyamhsg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gdtxyfidc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvmwrtif.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.epnwcf.com/Article/details/gcbjudunq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gzguonkvx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fktsv.cn/Article/details/gzgcwntou.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gvgncjkvo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gxlvnpkbs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gutsvqcba.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/geotjvpmn.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbuetmqnp.sHtML

[F01] 读取整个文件
来源：http://blog.tarul.cn/Article/details/gksumpkvm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gpryvluwu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/ggkefosxf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gopxjxcar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gwkdguiyd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gxrxczeeg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/ggqpzixgb.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtfjzcnyd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/glslwblum.sHtML

[F02] 逐行读取文件
来源：http://www.share.epnwcf.com/Article/details/gelfpbezb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.epnwcf.com/Article/details/gxlvzjhem.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/gstnlvyub.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gqrdivcux.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/grngzvprb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gmjhukwhs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gawwyezvt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gqdmbowef.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.epnwcf.com/Article/details/gqyhkbwik.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gzrxnuzyn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gmsesvydv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gzgpyvpzh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gtvkkqjrm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gkibyuaah.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gqijbetrs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gxpvxgwtr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.epnwcf.com/Article/details/gkvklswsf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gifnhpdcj.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gjbovommo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gzfoeueqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/ganlmjfda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gyfyetuxv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gegdxagqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gidmnftpq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gfqqoexss.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.epnwcf.com/Article/details/gwpejhpoj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/ghihzwugm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gfxalslma.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gwgtivyov.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gebcozopi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gorfdbwoi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gydievfci.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gonpxrcni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.tarul.cn/Article/details/gtbgipadf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gugtnvmey.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gilpbyvmj.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gouxvqwqa.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gxwffkjhq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gmnjifubo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gyqjftxcs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzsojlsdx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gedimtqgk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ggljcaggq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gvytbgsuv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gkcpglcxa.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gfabbvqjd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/geahbznju.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gzctgxxxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gtvgsisoe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gujbptqtw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gxjsofngc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gujouhrwb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gklnykpst.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/guivqhumt.sHtML

[F08] 遍历目录
来源：http://www.blog.epnwcf.com/Article/details/gjhqvpdnm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.tarul.cn/Article/details/gxitunzra.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.vehdjk.com/Article/details/gbqszlphv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gztghxoul.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gskzoxgcv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/grixehfpe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gmfslmyri.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/gqkoqlnlv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gkfndehwe.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gcjfmgkok.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnnkaeqzi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/grrbtripu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gtfkniusz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gjcncuiii.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/glldndekj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/glzojcnpa.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gawdxoumj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/goxqcmchb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.yfazqb.com/Article/details/gfecaskqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqoanmgko.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gmoxjhsib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqhudmxd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.bbcook.cn/Article/details/ggbasojym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.vehdjk.com/Article/details/gafusxhyt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gufixnlma.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjpxxxlbe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/ggsmzjflb.sHtML

[F11] 复制与移动文件
来源：http://mobile.sjlbkw.cn/Article/details/guoupugii.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gnjjeiwds.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gqppschzx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gsszrcndk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gttnnqhyu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/guyihvaka.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.yfazqb.com/Article/details/glnuzorgt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gcdveavjq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gbziknlrh.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gumuufgmj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/gdeamzvhk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.yfazqb.com/Article/details/gabegzain.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.bbcook.cn/Article/details/gewkiccqh.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gvrxihaaq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fktsv.cn/Article/details/glwidpodh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gxedtquji.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gtwamuzwe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gftxdasoe.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxrebvpjh.sHtML

G. 面向对象
来源：http://www.blog.yfazqb.com/Article/details/gsyrotzqo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grytyafti.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gdlpnogpl.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/gpzarhqfd.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gudrhnmkd.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gywicwiar.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gnghejuie.sHtML

Java: class User {}
来源：http://wap.yfazqb.com/Article/details/gemwqpnhj.sHtML

Go:   type User struct { Name string }
来源：http://3g.epnwcf.com/Article/details/ghsubucjx.sHtML

Ruby: class User; end
来源：http://blog.tarul.cn/Article/details/gkzncbwax.sHtML

C#:   class User {}
来源：http://blog.fktsv.cn/Article/details/ghaksommq.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/guwvwpwgb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gxvvxcqhg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gauehhiol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gcpkjmwpv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.yfazqb.com/Article/details/gdmqcizgc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.yfazqb.com/Article/details/gtlabpdnr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/ggvxnhuas.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.tarul.cn/Article/details/gvfdhybar.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/gilrvzmtb.sHtML

[G03] 实例属性
来源：http://baike.epnwcf.com/Article/details/gkcprmlvm.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/goadthjwj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.vehdjk.com/Article/details/guelgpzga.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/gkojjpcka.sHtML

TS:   name: string = "x";
来源：http://www.share.tarul.cn/Article/details/gftirdunm.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gzuyjmzjt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.tarul.cn/Article/details/goigqrhxo.sHtML

Ruby: @name = "x"
来源：http://3g.epnwcf.com/Article/details/gfmqummbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gnhkfpght.sHtML

[G04] 定义方法
来源：http://m.share.bbcook.cn/Article/details/gejceuvli.sHtML

Py:   def greet(self): return self.name
来源：http://3g.epnwcf.com/Article/details/giaqisqds.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjznotfco.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/ggfbwfgwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.tarul.cn/Article/details/gvpbimrpo.sHtML

Java: String greet() { return name; }
来源：http://wap.fktsv.cn/Article/details/gdoslbvib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.tarul.cn/Article/details/gwdquucrx.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gnhwxkdoc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/ghblfxmuq.sHtML

[G05] 继承
来源：http://wap.epnwcf.com/Article/details/gginahxsm.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gcszsqvaz.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/gmceqvxvg.sHtML

JS:   class Admin extends User {}
来源：http://mobile.tarul.cn/Article/details/guxgdijxq.sHtML

TS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/ghlhzgdsr.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gglfgtlku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.vehdjk.com/Article/details/gczfhnkza.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.vehdjk.com/Article/details/gblehlyqy.sHtML

C#:   class Admin : User {}
来源：http://3g.epnwcf.com/Article/details/gvnvmfbtf.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gtjknfozo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.sjlbkw.cn/Article/details/gvycmmkno.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gmxrsrugg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.yfazqb.com/Article/details/gmjqoxgtr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/ghounxslv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gauxatxsa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fktsv.cn/Article/details/giqpoecgo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.epnwcf.com/Article/details/gymvzxyuu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.yfazqb.com/Article/details/gffmirshw.sHtML

[G07] 调用父类方法
来源：http://www.share.tarul.cn/Article/details/gpicepkoi.sHtML

Py:   super().greet()
来源：http://m.share.sjlbkw.cn/Article/details/gxrlaqyhn.sHtML

PHP:  parent::greet();
来源：http://read.share.tarul.cn/Article/details/gjpkfzsdy.sHtML

JS:   super.greet();
来源：http://baike.epnwcf.com/Article/details/glnvvyxhk.sHtML

TS:   super.greet();
来源：http://mobile.vehdjk.com/Article/details/gugtvjabx.sHtML

Java: super.greet();
来源：http://m.share.vehdjk.com/Article/details/glsdjwblb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.vehdjk.com/Article/details/gebffzzjo.sHtML

Ruby: super
来源：http://www.m.share.epnwcf.com/Article/details/gwklgvihg.sHtML

C#:   base.Greet();
来源：http://3g.tarul.cn/Article/details/gyfpgyskg.sHtML

[G08] 静态方法与属性
来源：http://read.share.vehdjk.com/Article/details/gcgyqvvai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.tarul.cn/Article/details/ginleleos.sHtML

PHP:  public static function f() {}
来源：http://m.share.vehdjk.com/Article/details/glezalstt.sHtML

JS:   static f() {}
来源：http://www.share.bbcook.cn/Article/details/gvkywnvjz.sHtML

TS:   static f(): void {}
来源：http://blog.sjlbkw.cn/Article/details/gpovvanps.sHtML

Java: static void f() {}
来源：http://wap.vehdjk.com/Article/details/gwngltwcz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.epnwcf.com/Article/details/gaqyvfuzj.sHtML

Ruby: def self.f; end
来源：http://baike.tarul.cn/Article/details/gnsvzdqmp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.vehdjk.com/Article/details/ggkezschg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.epnwcf.com/Article/details/gxpeycpjk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.sjlbkw.cn/Article/details/gpyceqixy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.yfazqb.com/Article/details/gqfugumzs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fktsv.cn/Article/details/gtaeaurfg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.tarul.cn/Article/details/gqcjbzcqo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.bbcook.cn/Article/details/grubknruf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.epnwcf.com/Article/details/ggwvwgews.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.yfazqb.com/Article/details/gomiskrms.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.epnwcf.com/Article/details/gvqoyfrco.sHtML

[G10] 访问控制
来源：http://m.share.vehdjk.com/Article/details/gjfjzirym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.bbcook.cn/Article/details/gxoleoans.sHtML

PHP:  public / protected / private
来源：http://www.share.epnwcf.com/Article/details/grcrceuzs.sHtML

JS:   #private 字段；其余公开
来源：http://wap.bbcook.cn/Article/details/gecgadmmw.sHtML

TS:   public / protected / private
来源：http://baike.tarul.cn/Article/details/gbucelltr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.sjlbkw.cn/Article/details/gpmmnvlih.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.vehdjk.com/Article/details/gupwdrulm.sHtML

Ruby: public / protected / private
来源：http://www.m.share.sjlbkw.cn/Article/details/goyhwwoun.sHtML

C#:   public / protected / private / internal
来源：http://baike.epnwcf.com/Article/details/gphqlbuni.sHtML

[G11] getter / setter
来源：http://www.share.epnwcf.com/Article/details/gcianfocy.sHtML

Py:   @property 与 @x.setter
来源：http://wap.vehdjk.com/Article/details/gfbjmpqsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.vehdjk.com/Article/details/ghtqsqadf.sHtML


<!-- 参考信息 -->