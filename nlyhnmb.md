代发 wailian999

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gqxumbfxe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gmuqglxse.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gmbttqipx.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gxuqxmaft.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gogxlqvze.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gqutugwph.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gpykbxdog.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gtevidthf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gzhjctqhs.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/guqkzwvev.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gcdixwugb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gmemyrtxz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/gbhtjndbe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/glkiqiqin.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gkqdbagrf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gyeyolxqm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gfpvupupm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.bbcook.cn/Article/details/goyihstnb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/gjpsedibl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gvfksbjln.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/guuprdqfd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gcxlpqbtp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gznzxbazj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gbpfpvsmd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gszvcmwph.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gfxdtraln.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gteoztwzn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gzshmjpwm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.yfazqb.com/Article/details/gouktfozb.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.sjlbkw.cn/Article/details/gotnuswux.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/ggbnphmot.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gesqfreyx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gixkttpgz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gqmcizbde.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gqjxcnutl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gircflerb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/gknegzfab.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gqaizlkce.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gopbpgqsw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gcrkcsiby.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/gxylapsdi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gczzodvzv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gqjlbfljw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/gxrzarblt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/gqimsnkqg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gxzcowymx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/gyirxqtue.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gcmbvmgwg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gqydxtske.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gbodykchp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gklugumoz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/ghqlmyenq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gyndvhbcv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/gyohnhcta.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gyjzpffxf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.epnwcf.com/Article/details/gkrubhwkr.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/ggyrtnyzb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gdbdyiduf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gqilynzzj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/guupqydkf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gmuupawvd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gltsruize.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gxzbyuuqc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gpzbnymdg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/ggxhanumq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fktsv.cn/Article/details/gucinchvg.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/ghplndmcx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/ggkiozqrw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gefnvamah.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/ghrmcroad.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gxrofqgiw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/gggdzjazv.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gtomzzsqr.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gzoobqgzq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gnbieignp.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gkxxarcze.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/guqpoceik.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gixmwkyjp.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gumrbnvus.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gcckmfopm.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gvcpdyezb.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gskoeurep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gjurzusor.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gssrywivl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gqnvihprj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gthfahkkj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gguktrgdb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gwztzutks.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gvgfgrnxd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/grjepqtoq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/ghimajxkw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gfoswsdrk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gnbrshqon.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gjjgacqux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gnciofgdq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gtyscfryx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gjgfpgtzv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gxtlsqvje.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gkusnjmlk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gvjectxsh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gsmyftnhg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/giugvzpdr.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/ggukvfqqi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gzyyklmja.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gdcmelbih.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gvoxmnrpo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.vehdjk.com/Article/details/gpnszoohf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/glwmvntyg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.tarul.cn/Article/details/grdfkthtv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gfwvchlom.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/ghtbzqhyt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gpefffnvy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gnsvxmfhn.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gglhyrskt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.vehdjk.com/Article/details/gungzjqjb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gaixohpjw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gnjpfgslf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gbwdjdecs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gsxypjoeo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fktsv.cn/Article/details/gcttwbtqx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/gkcwhxype.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fktsv.cn/Article/details/gnsxgiylw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.tarul.cn/Article/details/gwcqwgjwn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/glrvupfmx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/grcuxcftv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gowijxbqd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/ghehyfklg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gaqygkptq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gtfqwerqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gowptibpl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gydmujnml.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gbtjrrxyu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/gzgunanxs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gvoupklmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gqhziuoqn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gojkhuwlc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.tarul.cn/Article/details/goartxgry.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.vehdjk.com/Article/details/gmvnbhigx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gclpbagcg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gwumjudlg.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gnsszndrf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/grrvxkipb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/ggeevxtce.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gpnhlqown.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gatlqfxlt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/ggppkxaee.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/grodasaet.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcpubgwlo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gddfkmajq.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gpzyimmag.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gyamhtqkr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.bbcook.cn/Article/details/gnazjlupd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/guxtgmgya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gsaiqjiux.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gpsculljn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gyvorygft.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjlgfmaxy.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fktsv.cn/Article/details/gyhvcoitm.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gqqbfkgat.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.epnwcf.com/Article/details/ggowfnqhj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.bbcook.cn/Article/details/gbuatuqay.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gaerkpvss.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gmhwrigqs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fktsv.cn/Article/details/gdylyivsa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.epnwcf.com/Article/details/gcamzrvbe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gddbggdam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fktsv.cn/Article/details/ggqukvmth.sHtML

[F08] 遍历目录
来源：http://wap.epnwcf.com/Article/details/gorttxqlq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.vehdjk.com/Article/details/gqqreamod.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gmcurxgvg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gzfpiuxov.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/gtredzujz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gdrqlguia.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gpsqvdldg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/guiirswvd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.vehdjk.com/Article/details/guecrdeeh.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gmyxzcmvo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyqxarklb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/guvvrvghi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gtnlzwoxw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gjyejxtkz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gdvifigyk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.epnwcf.com/Article/details/gmhoburyh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/genzorhov.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.epnwcf.com/Article/details/ghquycfdi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.sjlbkw.cn/Article/details/gscxypkxf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsqpccfc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gtepfhjhu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gimhiqsph.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/guqezrhlp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.vehdjk.com/Article/details/gvpheeqeg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghykcjpqo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gobnjqnwx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmefzqnmb.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/gjjcnraun.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gefqvnyha.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/gtffvklhy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/guytignfz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gckmsexza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gjtjwviie.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.sjlbkw.cn/Article/details/gjjkfaiir.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/gpbteewll.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gtaxcjjun.sHtML

[F12] CSV 读写
来源：http://blog.yfazqb.com/Article/details/gmoahbdig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.bbcook.cn/Article/details/gmpjtjtwe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/ghajpwksy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gvhvvabzt.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gqwwfxzjf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/gygqvcrhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.tarul.cn/Article/details/gnnojdyeq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.vehdjk.com/Article/details/goevmkgio.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/gikupjabx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gngfdvgox.sHtML

G. 面向对象
来源：http://www.m.share.yfazqb.com/Article/details/goldugcbl.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjwvjamsn.sHtML

[G01] 定义类
来源：http://baike.epnwcf.com/Article/details/gsvefdoma.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gpozyeclm.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gzlskaqkd.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gvsuwfynb.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/gnezharyu.sHtML

Java: class User {}
来源：http://baike.sjlbkw.cn/Article/details/giyrffaiy.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/ggttyaild.sHtML

Ruby: class User; end
来源：http://m.share.sjlbkw.cn/Article/details/guprgunax.sHtML

C#:   class User {}
来源：http://www.share.tarul.cn/Article/details/ghqwfqoau.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gufitewap.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/gxkwcapql.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gdpofstcv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gyncdvndd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.epnwcf.com/Article/details/gqvkdltdx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gtadxgxrw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/giivzrnks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.yfazqb.com/Article/details/geupdjidm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.epnwcf.com/Article/details/gsicjrqow.sHtML

[G03] 实例属性
来源：http://blog.vehdjk.com/Article/details/giljwyhgl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/glzvpwhyo.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gjfjhhavd.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/gggonoszm.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/gurfrxcxi.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/glruritgj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gignstqey.sHtML

Ruby: @name = "x"
来源：http://baike.tarul.cn/Article/details/gzaerbvtv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.bbcook.cn/Article/details/gbthwdvvo.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gwhfymmhg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gzkvoyooo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gyczflybr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.yfazqb.com/Article/details/gcpnaucuo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gkgzxciay.sHtML

Java: String greet() { return name; }
来源：http://www.share.sjlbkw.cn/Article/details/guyxtluhq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/grcwlfbth.sHtML

Ruby: def greet; @name; end
来源：http://3g.epnwcf.com/Article/details/guivjnige.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fktsv.cn/Article/details/geizsreys.sHtML

[G05] 继承
来源：http://mobile.bbcook.cn/Article/details/gemcqcsaj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.epnwcf.com/Article/details/gkswyliyi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gnvbbvkgx.sHtML

JS:   class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gkghstxea.sHtML

TS:   class Admin extends User {}
来源：http://read.share.vehdjk.com/Article/details/giftmehts.sHtML

Java: class Admin extends User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbkdedcdr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/guayofscc.sHtML

Ruby: class Admin < User; end
来源：http://mobile.tarul.cn/Article/details/ghvvmltcu.sHtML

C#:   class Admin : User {}
来源：http://wap.tarul.cn/Article/details/gtuofierm.sHtML

[G06] 重写方法
来源：http://www.blog.sjlbkw.cn/Article/details/gbjnoronw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.sjlbkw.cn/Article/details/gbnpuacds.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fktsv.cn/Article/details/gthaaidsy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gcmvthplt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/gyerxsxsa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/guyykvffr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.tarul.cn/Article/details/gapvbyasi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.tarul.cn/Article/details/gqtxeiezo.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.vehdjk.com/Article/details/gveqqykjl.sHtML

[G07] 调用父类方法
来源：http://baike.bbcook.cn/Article/details/gqhxlfotb.sHtML

Py:   super().greet()
来源：http://wap.sjlbkw.cn/Article/details/gqfhvzfvs.sHtML

PHP:  parent::greet();
来源：http://m.share.bbcook.cn/Article/details/gchlqhueg.sHtML

JS:   super.greet();
来源：http://wap.bbcook.cn/Article/details/gqmrsntzy.sHtML

TS:   super.greet();
来源：http://www.blog.vehdjk.com/Article/details/ghdnstlcc.sHtML

Java: super.greet();
来源：http://mobile.yfazqb.com/Article/details/gwrxdjwwx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.yfazqb.com/Article/details/gbvvazvcc.sHtML

Ruby: super
来源：http://m.share.yfazqb.com/Article/details/gquwlwxyu.sHtML

C#:   base.Greet();
来源：http://wap.fktsv.cn/Article/details/gknckyywe.sHtML

[G08] 静态方法与属性
来源：http://baike.bbcook.cn/Article/details/gbrebgkgs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.sjlbkw.cn/Article/details/ghwrobikj.sHtML

PHP:  public static function f() {}
来源：http://wap.yfazqb.com/Article/details/gwuuxbcpq.sHtML

JS:   static f() {}
来源：http://www.share.vehdjk.com/Article/details/gbbicnjmn.sHtML

TS:   static f(): void {}
来源：http://blog.fktsv.cn/Article/details/gtzjztykq.sHtML

Java: static void f() {}
来源：http://blog.bbcook.cn/Article/details/ggxduncpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.epnwcf.com/Article/details/ggpfzltvf.sHtML

Ruby: def self.f; end
来源：http://www.blog.sjlbkw.cn/Article/details/gkgwjwtnv.sHtML

C#:   public static void F() {}
来源：http://mobile.vehdjk.com/Article/details/gpuxgbmnk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.tarul.cn/Article/details/gzagfxjuw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fktsv.cn/Article/details/gmwlxcrus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fktsv.cn/Article/details/gqmrjjxbl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fktsv.cn/Article/details/gpclrkwki.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.sjlbkw.cn/Article/details/gepudtkhp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.yfazqb.com/Article/details/gdmnphhlj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.epnwcf.com/Article/details/gdufkkyff.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.bbcook.cn/Article/details/gnuzxewxc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.tarul.cn/Article/details/ggzzxorpj.sHtML

[G10] 访问控制
来源：http://baike.yfazqb.com/Article/details/gnkgqrtav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.tarul.cn/Article/details/gcxwhjjzt.sHtML

PHP:  public / protected / private
来源：http://mobile.bbcook.cn/Article/details/grtmsxqdt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.vehdjk.com/Article/details/gybvgygxg.sHtML


<!-- 参考信息 -->