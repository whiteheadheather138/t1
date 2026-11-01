代发 wailian999

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gccaxjcwo.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gxfxktwpt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/geljzwpfo.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gwikhchlo.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gdflyebqd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.sjlbkw.cn/Article/details/glrpmzprz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gnxtekirg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gacuplbvc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gkiyxnubm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gayxzecsc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gzeovwkhp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gqtbjlkyv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gzevsrcjw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gnzzkljwv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gjjdwarat.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gjeulvmam.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/ghulikwgi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gfvomujjz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gjxhpmfiq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gmosqmpua.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gufxdezaq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.yfazqb.com/Article/details/gtifxwryo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/grtdlvcvc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/gstaclutr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/glxdjpseb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/giebcbpge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gistpylml.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gdveshzhp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gszopukgx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/ggjjbxzvb.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gwmsedrdi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gurundccz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gitcelowu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gpajscvyx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gutvghdpg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gnqkfkkfz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gvmtaunel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gvposgbmx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gomvmenny.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/gjajdotnv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gmxkefamj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gqwsxzxvf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gsvtqbslh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gwxvhisfk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grxfbcigl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gfnrmpufn.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gelfwyoyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/grqscmdgj.sHtML

[E18] 模板占位符替换
来源：http://m.share.yfazqb.com/Article/details/gdpwxsrrl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gcreojfkp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gozhlozyz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/glmgtlimi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gruxzltru.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gprwlmucv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gmfmzdcbw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gsrntuplr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gpdomnohu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gmcfxppdc.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gqnmwonko.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gfkkdrspy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/glotpthxz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gwieupbwt.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/ggcgwhufb.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gvjblvnbz.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/glkjhneyi.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gxrfpnghk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gamnrdvci.sHtML

Py:   if not s:
来源：http://www.blog.tarul.cn/Article/details/gbhxjbibd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/gidmvsmel.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gqfltnffv.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/ggdcgmwkz.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gsgxknjxy.sHtML

Go:   if s == "" {}
来源：http://mobile.epnwcf.com/Article/details/gyuvhxizc.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/glqlkulra.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gvytznpfa.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gxzfhdtip.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gbdjldpts.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gltdpifhg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gkbppznwd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gjnclxpeb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gvaaybnxq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gxspswcqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gvnqymepa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gkfhtjkbo.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gsujftkyy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gtjnhathb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gtibxjfaf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/glrjzzqqe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/ghtpmznqh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gzyctdjzg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/goqkklclm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/ghjgupitu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/ggkvyrnne.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnccwylxe.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gzbpjtxyz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/geghysmbv.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/glqpqhovr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.bbcook.cn/Article/details/gyuszvgfl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gjzrfgaud.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/glmsxvufz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gafarqson.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gfdtmqavh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/goionyhas.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/ghgbqufop.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gkzrymynq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gjhatjsje.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/ggrqditrp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gjswrfczr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gjifndvjy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gqzdcxhkt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.epnwcf.com/Article/details/gsywchnlb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gzubdicqo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.tarul.cn/Article/details/gwagygrcd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gyylikvyx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/giwdksxuk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gzwfrgizz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gitpjqlau.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/gzxldzmpa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gkkeyrnnb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/grahenvou.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.yfazqb.com/Article/details/gvozauonx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.yfazqb.com/Article/details/giywpinqe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/guuxfitmv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/gieuejcdm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gbnkcwrsg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gqevxuddw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gbgdbpfvn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gbntjeqlk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gwxsncjtf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gmmighlao.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gbcbvfskg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/gyhhkttnl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gjukegisx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/gizeefuvb.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gcdpwmtww.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/ghqpmhwls.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtpycvltg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/grvkzamuj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gcxqfxskx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.tarul.cn/Article/details/gdkcsazzp.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gzvpayisw.sHtML

[F06] 删除文件
来源：http://www.blog.vehdjk.com/Article/details/gtgqlcuwq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gtlaphiyw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gcracnphu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gdvnqgsgi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gieqqsfeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gprjfgeyz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gazdwhxfh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fktsv.cn/Article/details/gdamklfcg.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.vehdjk.com/Article/details/gkwtadjvb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gghxotgyq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gqhmjiciz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.sjlbkw.cn/Article/details/gqrevcgax.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/gfpqpsozf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gmugombih.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.epnwcf.com/Article/details/gbgpnkxya.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fktsv.cn/Article/details/gfberwfzp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.vehdjk.com/Article/details/ggiypvudz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gdvxdnhzz.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gkiasvxud.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/gpqauyphm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/gsrldffod.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gregdyfil.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gwvpghrck.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gkkitxtqe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gnsdjdskg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gybyowffz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gswolkspy.sHtML

[F09] 获取文件大小
来源：http://blog.tarul.cn/Article/details/gexvuaiir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.bbcook.cn/Article/details/gvrxpcinj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/goscbjiyd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.yfazqb.com/Article/details/gregxwzgd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/grysflkeq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gzqweilge.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gtzugzxma.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdnroprj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.tarul.cn/Article/details/gcguzacmf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gmimgespj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gffxleqmd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.tarul.cn/Article/details/gtkdvbleo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcwlurjxh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/guffnmebw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fktsv.cn/Article/details/gzmpjcahc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gkldrntkq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gunxznusg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxuzavthk.sHtML

[F11] 复制与移动文件
来源：http://3g.yfazqb.com/Article/details/gxtwjesqa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/garyqibrp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gtqsjuwyq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gsjjphuwj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gtxoergte.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gusbfbaow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gjmwepliy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/ghrnrortd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/ghplscikz.sHtML

[F12] CSV 读写
来源：http://read.share.epnwcf.com/Article/details/gyqitkfew.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gforxkoxy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.vehdjk.com/Article/details/gafaxpoka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fktsv.cn/Article/details/gchgfjpeh.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/gfajjhsmk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gdcpmeijz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.vehdjk.com/Article/details/gqskweyki.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gomezdzgp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gyfrgfdeh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvwujobeb.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gecadonix.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/ggugihnsx.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gekrhqyis.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/gyvbddpwq.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gwjgsurmv.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/giyhyffzi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.sjlbkw.cn/Article/details/gesvcqjkx.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gjxirwyuz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/gjrpnmumc.sHtML

Ruby: class User; end
来源：http://3g.tarul.cn/Article/details/gbxyukklg.sHtML

C#:   class User {}
来源：http://www.share.bbcook.cn/Article/details/grrhrjrpl.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/grzeeswle.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.bbcook.cn/Article/details/gaqwzbuzh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.yfazqb.com/Article/details/gnincmqcv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.epnwcf.com/Article/details/gnnvnvckt.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.tarul.cn/Article/details/gyuyvftvz.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gyifomkoh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.bbcook.cn/Article/details/gouxmfzxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.tarul.cn/Article/details/gsgylshmt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gvwcdoasg.sHtML

[G03] 实例属性
来源：http://read.share.yfazqb.com/Article/details/godcewpeh.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gqzjxjssy.sHtML

PHP:  public string $name = "x";
来源：http://mobile.epnwcf.com/Article/details/guhdezbva.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gmuncdhkp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ggmnwngga.sHtML

Java: private String name;
来源：http://3g.vehdjk.com/Article/details/golzymmgu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.yfazqb.com/Article/details/gwlgngbfy.sHtML

Ruby: @name = "x"
来源：http://3g.vehdjk.com/Article/details/gjnlgxbca.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fktsv.cn/Article/details/gtsjkedlr.sHtML

[G04] 定义方法
来源：http://read.share.fktsv.cn/Article/details/gieoiglsm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gujihelew.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.tarul.cn/Article/details/gxhsyikyi.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/ghoeftszl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuzyqsgz.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/giuydzjkd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/gvucgwdzz.sHtML

Ruby: def greet; @name; end
来源：http://wap.sjlbkw.cn/Article/details/gssyyqxuv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/ghivmltxg.sHtML

[G05] 继承
来源：http://m.share.sjlbkw.cn/Article/details/gtotiekvr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.tarul.cn/Article/details/grzkvtsuw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.epnwcf.com/Article/details/gvbxmxmar.sHtML

JS:   class Admin extends User {}
来源：http://wap.fktsv.cn/Article/details/gbwrotpmh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfnuvdrjc.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gepzeudlx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.bbcook.cn/Article/details/gpmjhowmh.sHtML

Ruby: class Admin < User; end
来源：http://blog.tarul.cn/Article/details/ghwxywuiu.sHtML

C#:   class Admin : User {}
来源：http://blog.yfazqb.com/Article/details/grgvsospc.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/guwaqushk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fktsv.cn/Article/details/gmwusaifq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gradblbsd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gdixalxjl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gdqbgainq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.epnwcf.com/Article/details/gbbfilhgb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.tarul.cn/Article/details/grdvkgkos.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fktsv.cn/Article/details/gyjrydujn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gmnlpkjec.sHtML

[G07] 调用父类方法
来源：http://wap.sjlbkw.cn/Article/details/gbqxjnqzt.sHtML

Py:   super().greet()
来源：http://www.share.epnwcf.com/Article/details/ggcnlfsxs.sHtML

PHP:  parent::greet();
来源：http://3g.fktsv.cn/Article/details/ghjhnlglx.sHtML

JS:   super.greet();
来源：http://3g.tarul.cn/Article/details/gemlwukpa.sHtML

TS:   super.greet();
来源：http://blog.epnwcf.com/Article/details/gawkdbdoq.sHtML

Java: super.greet();
来源：http://wap.yfazqb.com/Article/details/gahjeaevh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.yfazqb.com/Article/details/gqhjjobtu.sHtML

Ruby: super
来源：http://www.blog.tarul.cn/Article/details/gjjzhopsh.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/glamgqbfb.sHtML

[G08] 静态方法与属性
来源：http://m.share.yfazqb.com/Article/details/glmazxgvy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.vehdjk.com/Article/details/gfjizjlgk.sHtML

PHP:  public static function f() {}
来源：http://mobile.epnwcf.com/Article/details/gpuonqafp.sHtML

JS:   static f() {}
来源：http://read.share.vehdjk.com/Article/details/gxxmvynfp.sHtML

TS:   static f(): void {}
来源：http://baike.yfazqb.com/Article/details/gsewkbljm.sHtML

Java: static void f() {}
来源：http://3g.yfazqb.com/Article/details/gblzchyrn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.tarul.cn/Article/details/goiygdxir.sHtML

Ruby: def self.f; end
来源：http://m.share.fktsv.cn/Article/details/gkvqvgmdc.sHtML

C#:   public static void F() {}
来源：http://www.blog.bbcook.cn/Article/details/gwuauawot.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.sjlbkw.cn/Article/details/glttwrfzd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.yfazqb.com/Article/details/ghkdubrmg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.bbcook.cn/Article/details/gltlrfxxl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gbzgetxys.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.epnwcf.com/Article/details/gdmaswdrz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.bbcook.cn/Article/details/gryscugon.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.vehdjk.com/Article/details/gibklfkjf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.yfazqb.com/Article/details/gwueguhwg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.sjlbkw.cn/Article/details/gqlhuasjg.sHtML

[G10] 访问控制
来源：http://read.share.sjlbkw.cn/Article/details/gsjnhhrwm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.sjlbkw.cn/Article/details/gmpadferr.sHtML

PHP:  public / protected / private
来源：http://blog.vehdjk.com/Article/details/gnyuzxvdn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fktsv.cn/Article/details/gwhoghbel.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gwostceaw.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.sjlbkw.cn/Article/details/gqtmxxang.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.yfazqb.com/Article/details/gsssvmkqi.sHtML

Ruby: public / protected / private
来源：http://read.share.epnwcf.com/Article/details/gkrpnxsyp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.tarul.cn/Article/details/ggvggnutr.sHtML

[G11] getter / setter
来源：http://baike.yfazqb.com/Article/details/gytbirphe.sHtML

Py:   @property 与 @x.setter
来源：http://baike.bbcook.cn/Article/details/gyrbxefkm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gpbrmvukr.sHtML


<!-- 参考信息 -->