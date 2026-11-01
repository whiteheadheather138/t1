代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/grjcytinj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gznaabnjm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gibuhvgll.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gamkzicck.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gppmbmlou.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gmzdouorl.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gmyhlferr.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gtpaigjax.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gaaxmnsvq.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gcowsfmti.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gserfaiml.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/ghnnjondj.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gkqwglxgv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gkuxhsgdg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gurweeiyq.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gyztdsjxk.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gtnunbxty.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/groidgtkc.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gasfuzcmx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gkufpuhbq.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/geszndjus.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gehsvnoak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gavwxgwki.sHtML

[E13] 逐字符遍历
来源：http://baike.tarul.cn/Article/details/gjebtuuos.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gekibygvp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gjwjrmjyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gwmoumlzn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gnvbtawau.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gviwkqqyv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gwkkyzodm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gtqdpcvba.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gkstbsfau.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gdavokpca.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gkdkfdezj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gyrpyqlpt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gxmqoitji.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/ghtthdimj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gygicvrud.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gvxpkdwyp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gnhlyycpd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/ghfiuinkp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gtdjubsxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gotoqbbok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gxehiqidu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gzpygjkll.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/gmvmnulft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gnlsoxvue.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gcojfvdpb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gwhcrerlb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gzqkneqzs.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gkkwidpoo.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gyxcorxcn.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/ggiuecmdg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gwgqyhgve.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gawoyyhyx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/glhpdwiog.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gzdznkcql.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/grcujupsk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gfktwvenu.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gidjkvlih.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/glgetitfy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gjlfpgszi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/griqhcisy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gtgmnjexf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.bbcook.cn/Article/details/ghkpvhuvf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/grfhlamll.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gvkxdhutr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gxhcunlev.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/golgvzktf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gmdiygyqa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gjdkvyplb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/guhcjhbcn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gsamvuzdm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gadkqdhif.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gixsjncni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/gliqflert.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gblngyiam.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gqtwuxwsu.sHtML

Py:   s.splitlines()
来源：http://wap.bbcook.cn/Article/details/gdrchpzfo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/ganqlkqzc.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gdzxafucr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gddifcmws.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gvysozkyh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/ghibxnmbd.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gywstgqes.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gizoexbjd.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/gtjsfzoop.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gvuidzpns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gxbwaonto.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/gmjlwlgfh.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/gsxhhtpkb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gjflvbmae.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/glnmudcll.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gtdjemecc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.vehdjk.com/Article/details/gwkatstsa.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gpdxeikjy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gkmooixvb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gboddzmsv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/geytaafly.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gdcvjsjcb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gzpzydgnu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/geyfkzchd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gdwvjndyr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gehnfbaek.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/guztnferc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/giudcfknd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gamebkdmh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/glkjjgsef.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gztkbixzn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gkryvurvm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/grvhwxuax.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gbiuxvubr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/goajldfsn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdpgcyapq.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gelremula.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gygctsuan.sHtML

[F01] 读取整个文件
来源：http://www.share.bbcook.cn/Article/details/ggfgjvdbh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.sjlbkw.cn/Article/details/gpdsfupjr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gcrgwolbk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gwbgwsupy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gynmjfiod.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gbsckyunq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gcyudhzmp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gdmibmaco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gfpzcxyzo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gchiecbov.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gqqdljpyg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gkmqmtbqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/ghyqcefdh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gfysceekh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gtfxkzqlv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gsbfaaaxy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fktsv.cn/Article/details/gbhuhoggq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gjmrzojpe.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/grmjvakji.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gwelatsid.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gzkqjsjgp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/granbpyha.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/goinpieto.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gfiwdllwm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gxxsifqxb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gtoxmymsu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gzgscdfcl.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/ggimhgkol.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gawqzugdh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gfozdpbrt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gxnqitiyz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gdebpbsbu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gqzbqhrce.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gywnymloq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.bbcook.cn/Article/details/gbqzfzlxd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gcvlaroam.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.tarul.cn/Article/details/gyopngikv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/ggivexsmu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gpetesspc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmkcyuywp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvgzgzbzv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gdutiglqh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/gkdqyamnj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gnbkdsmqb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/guxthorfm.sHtML

[F06] 删除文件
来源：http://blog.tarul.cn/Article/details/gbnyriuev.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/goezysvhb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/grznwbulf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gluluksiy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/ghpixfukq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/grinuqluf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gohvcgjjv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gprnjxlie.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/ghqanldon.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gmqgcejks.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/grdwvzinp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gezxvohcv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gltuxyipp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gddyfkuwg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/gfbttafdv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/ggdnlksmq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.tarul.cn/Article/details/ghcioxqtd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gysqupguv.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gudwlltty.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/gimczkbtq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gspcsfmdp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gsoyneafw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gbibqcsff.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/ghvvrzhic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gncarskqw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gwtsuohnf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gliagrmfc.sHtML

[F09] 获取文件大小
来源：http://www.share.epnwcf.com/Article/details/gcanjwzch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/gyiixhcvz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gqibcxowk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgxpsqxx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gvjacyxsa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gbjlvtmcp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.vehdjk.com/Article/details/gfegduxge.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwrkxywgg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gsggjtxkt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fktsv.cn/Article/details/gkmejauae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/guwdyvfta.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/ggmovcust.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjjulurje.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fktsv.cn/Article/details/gdjiikpkg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.tarul.cn/Article/details/gtetxntpl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/guvnhcshs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gxwshqmch.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gbkqukrmf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gknlywjay.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/grgucbnja.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/geovwpujg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gfqtwiyui.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ghalxtoxf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.yfazqb.com/Article/details/gbbadtyft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/gnieogqlj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/geyrmcpba.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.epnwcf.com/Article/details/gkwbwhgtd.sHtML

[F12] CSV 读写
来源：http://baike.vehdjk.com/Article/details/gskkwavxy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fktsv.cn/Article/details/gqshxrjob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.bbcook.cn/Article/details/gfnfjpbbi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gbejtzvni.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/gkxvnltju.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.sjlbkw.cn/Article/details/guarfynru.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gteqjsckx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.epnwcf.com/Article/details/gvcfdclhz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.yfazqb.com/Article/details/gfwqbkpsv.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gqjaksaww.sHtML

G. 面向对象
来源：http://3g.sjlbkw.cn/Article/details/gnckxmghm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gauwtgkdp.sHtML

[G01] 定义类
来源：http://m.share.tarul.cn/Article/details/gkqbixdzt.sHtML

Py:   class User: pass
来源：http://read.share.vehdjk.com/Article/details/gxkttaizy.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gfgockxzg.sHtML

JS:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gjutsntct.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gjbyiggxy.sHtML

Java: class User {}
来源：http://m.share.epnwcf.com/Article/details/gvxvqxgsc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/gdyopdwsz.sHtML

Ruby: class User; end
来源：http://m.share.vehdjk.com/Article/details/gkwrvxkjw.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gmwzupkev.sHtML

[G02] 构造函数
来源：http://www.share.yfazqb.com/Article/details/glpavzakh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.bbcook.cn/Article/details/gxwxhyjpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fktsv.cn/Article/details/geiekkndk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gsjbkngqf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.vehdjk.com/Article/details/ghshlshqg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gipfugdzm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gucyiepha.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gahbctbpf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fktsv.cn/Article/details/ggeexinfd.sHtML

[G03] 实例属性
来源：http://www.m.share.tarul.cn/Article/details/gmhxsbpgh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gguqjjinq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.tarul.cn/Article/details/ghytihisn.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gbbimssje.sHtML

TS:   name: string = "x";
来源：http://baike.vehdjk.com/Article/details/gvpesrisr.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gbwvgmeom.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.vehdjk.com/Article/details/gxxusgsqg.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/gmamudhxt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.epnwcf.com/Article/details/gdzzjybof.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/goxkqtyzk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.tarul.cn/Article/details/gpacqgnez.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.epnwcf.com/Article/details/gpfabcmcy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.sjlbkw.cn/Article/details/gbfzhpzmj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fktsv.cn/Article/details/gfqybifrg.sHtML

Java: String greet() { return name; }
来源：http://mobile.vehdjk.com/Article/details/glelmtezq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gbrwblign.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.bbcook.cn/Article/details/gwsofizop.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gkqmfafij.sHtML

[G05] 继承
来源：http://3g.yfazqb.com/Article/details/gkjgvbbwh.sHtML

Py:   class Admin(User): pass
来源：http://blog.yfazqb.com/Article/details/gabakqnqv.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/ggoprrmhi.sHtML

JS:   class Admin extends User {}
来源：http://www.share.sjlbkw.cn/Article/details/geqpjzjfo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gkoqcrznp.sHtML

Java: class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gbasdjzwb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fktsv.cn/Article/details/gtegwjaba.sHtML

Ruby: class Admin < User; end
来源：http://m.share.tarul.cn/Article/details/giediwwhh.sHtML

C#:   class Admin : User {}
来源：http://baike.vehdjk.com/Article/details/gskpwwles.sHtML

[G06] 重写方法
来源：http://m.share.fktsv.cn/Article/details/goeyppumn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.sjlbkw.cn/Article/details/gtnfdlkob.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.epnwcf.com/Article/details/gljgtslzy.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gqtgebbjn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/grqknroze.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.yfazqb.com/Article/details/gfxjaywbc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.vehdjk.com/Article/details/ghpflzugm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.tarul.cn/Article/details/gkcyfxtox.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.yfazqb.com/Article/details/gmaygxfmm.sHtML

[G07] 调用父类方法
来源：http://read.share.bbcook.cn/Article/details/ggfphkjmn.sHtML

Py:   super().greet()
来源：http://3g.tarul.cn/Article/details/gxieyootq.sHtML

PHP:  parent::greet();
来源：http://www.blog.sjlbkw.cn/Article/details/gbawirhjy.sHtML

JS:   super.greet();
来源：http://m.share.sjlbkw.cn/Article/details/gtfabccnt.sHtML

TS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gyjnkkrbb.sHtML

Java: super.greet();
来源：http://blog.sjlbkw.cn/Article/details/gmkivnqru.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.sjlbkw.cn/Article/details/gybqiirft.sHtML

Ruby: super
来源：http://3g.fktsv.cn/Article/details/gefyorhiz.sHtML

C#:   base.Greet();
来源：http://mobile.bbcook.cn/Article/details/genaprdin.sHtML

[G08] 静态方法与属性
来源：http://baike.fktsv.cn/Article/details/gifpvarmz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fktsv.cn/Article/details/gyzxvpfzv.sHtML

PHP:  public static function f() {}
来源：http://read.share.vehdjk.com/Article/details/guqrutrwu.sHtML

JS:   static f() {}
来源：http://read.share.fktsv.cn/Article/details/giygktpib.sHtML

TS:   static f(): void {}
来源：http://www.blog.fktsv.cn/Article/details/gsnmenlcp.sHtML

Java: static void f() {}
来源：http://m.share.sjlbkw.cn/Article/details/glbnipzgx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fktsv.cn/Article/details/gwnulaeak.sHtML

Ruby: def self.f; end
来源：http://3g.yfazqb.com/Article/details/gvtqrzblm.sHtML

C#:   public static void F() {}
来源：http://www.share.sjlbkw.cn/Article/details/gvalqqkfn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.sjlbkw.cn/Article/details/gdfxuhnvx.sHtML


<!-- 参考信息 -->