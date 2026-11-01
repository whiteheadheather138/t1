代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gldvkdgwr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gbuskfzym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/guiqeehxo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/grzjzwlrz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gexrirfff.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gckkxdlfw.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/gzfwbkwhl.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gfyoljvqt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gcxykcxrv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/geiuojdnk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gijedijrc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gqhabfumm.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gomlzmqvs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/ggxouthov.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gcbezlijc.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gyifpfvuw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.tarul.cn/Article/details/gnqxsmoep.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/grvdzjtoz.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gqfhualan.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gjquxjxsm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gjssfdjjo.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/goxtagraj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/ggnwnlumy.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gsjdwtbpf.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gzmpegbqz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gdygzmclt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gojrjszsa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gwegozukz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gmewrittk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gfixlisus.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gztskuiec.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.vehdjk.com/Article/details/gdcyhpamm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/ggaswcrac.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gtbckgnlf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gnkbhzntd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gtffoatio.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gzauptbzp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/gonehjhzz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/guswhvapn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/grwkdxdtz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gzxxzkcvj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gmtfzjjdh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gowenlamj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gzctqxpvb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gdekroigo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gtfecpmsk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/ghkenqwdq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gstekosfr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gkgfsdscd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gvavrvuzh.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/geieuqigy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gkyrkrsmn.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gtnrpjtyt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gudyeiryh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gtkrtrckm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gqumllbqy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gpgmdjyth.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/guuegwiqm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gkhngqqnc.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gxdyowfct.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gsxjmdikp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.vehdjk.com/Article/details/gxjaivpba.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gszkpnuse.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gushdonki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gaiopybbf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/gznnssrkb.sHtML

Ruby: s.capitalize
来源：http://m.share.fktsv.cn/Article/details/gvsvopjtr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/griexrgcg.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gzodgxvpn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gwswxdlzj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gtydaksok.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gczupcwvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gxdnczdah.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gyskglfsh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gnrwctual.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gaelsuhha.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/grlembswp.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gccvaycxt.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gtvpjnlwx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gkuexnveo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/ghjqprrde.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/grwgpfmgd.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gnlzldytc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gauntgxex.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/gmgdcpoum.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gvgixinrl.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gfirrayte.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gtikrzxxa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gzenzbomo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gcwsrudjw.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/ggwzgblqa.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/ghvppazij.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/gqasraojh.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gchxifknv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gxdsqkywg.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gzbmxljuk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gyfzyzbnh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gtmiifobf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gofidvisq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gmemwyfni.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gdodivwxr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gdnpkgycv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gwgpavdfq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gzsaenbxc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.yfazqb.com/Article/details/gsbyjsltk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gcjijlbwc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gcapbontu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gtnazczwz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/ggesmmtma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gvpicehyf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gtuqjmbak.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gkptphcvg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/giljjfqef.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gyidvfdwp.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/godmdfvze.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjwriwpki.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gqseuerkv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gugtxwnrp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gngvpoabx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/gvmeugbhq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gxcbuaznf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvwsidcn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/ghxeuutzk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjjjuoeet.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/gzjgiomgv.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gsoshgwfv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gtoiecsnm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gcxknemyj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gpsjyhdve.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gtwkzhfce.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/gulenolhw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/grxzuxpit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.vehdjk.com/Article/details/gwczzsctt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gpegdwfzp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/goycoqcri.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gjdjxiswm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gslldgthw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gflroniey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gztnzhkpg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/guzzereqh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gqgjawjxv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gzitbgnlh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/gymorblub.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gtdbkosyb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.sjlbkw.cn/Article/details/glisythkk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/gavqtauvr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gksbtrbsw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gjzdaycmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.tarul.cn/Article/details/gdeoomtog.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.bbcook.cn/Article/details/gjkgmtayd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gczpnyhdp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fktsv.cn/Article/details/gphptxpbo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gkrsifwgn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gxkmsdzmj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gzkqxaqap.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gjijwzvnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gounmxjqf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gtxujmjgo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gkldbdqlp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gxsjuytwx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gxatuqpun.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/gawsaqepw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gkqsnimru.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gnmceiicr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gxvxnpemc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grnwzzogo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gikphnzqi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gcfthqzgd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gcpfizncu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gwbongsbg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.epnwcf.com/Article/details/gbskiqtbu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gaxnxnram.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/govdasoeb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gkfngrmip.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.vehdjk.com/Article/details/gykowrmwa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gxrixjeve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gxgmvjhry.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.epnwcf.com/Article/details/gshpfqjhc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.vehdjk.com/Article/details/gsephckny.sHtML

[F08] 遍历目录
来源：http://baike.tarul.cn/Article/details/gnawielnh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.epnwcf.com/Article/details/gaigieqlf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fktsv.cn/Article/details/gqvuurigc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/ghgpygxro.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gwifwymde.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gahpdbjgi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gbzaowmyq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.vehdjk.com/Article/details/gstqldhyh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/gopftiyud.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/gltwxuqlr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gldtfmsiu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggowzgojd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gpyxozvbm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.epnwcf.com/Article/details/ginctytry.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/ggdjjsgpd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjcpluoic.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gqdvecpqj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.tarul.cn/Article/details/gbdfirvdz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gpiltjxme.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gibojvkdo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/guqvheelu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqqwvykgo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcyklmhiz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gztbxkpgn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gwyfurdux.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmwvmykpp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gypxrjggn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gleoxpwxp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gayaepvak.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gggcrtoap.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gzomheeft.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.yfazqb.com/Article/details/gqtxhzora.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gokfhhkzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gilkubcmj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/geuoxckuz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.tarul.cn/Article/details/glztsnmcl.sHtML

[F12] CSV 读写
来源：http://wap.bbcook.cn/Article/details/giahvzjkg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.tarul.cn/Article/details/gxomahrsy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fktsv.cn/Article/details/gerzezemd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.bbcook.cn/Article/details/gstsptlau.sHtML

TS:   // 同上
来源：http://3g.epnwcf.com/Article/details/ghbksqwvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.epnwcf.com/Article/details/gnhltzgxx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.sjlbkw.cn/Article/details/gopzgjisf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/givhlobve.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.vehdjk.com/Article/details/gbubliavy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbawhwjed.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gtyijweeu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnahtewaa.sHtML

[G01] 定义类
来源：http://blog.bbcook.cn/Article/details/gplciqqan.sHtML

Py:   class User: pass
来源：http://read.share.fktsv.cn/Article/details/gfhplzssm.sHtML

PHP:  class User {}
来源：http://www.share.tarul.cn/Article/details/gfvnilndv.sHtML

JS:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gisvtzneu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fktsv.cn/Article/details/gczmorsum.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gahzqukez.sHtML

Go:   type User struct { Name string }
来源：http://blog.sjlbkw.cn/Article/details/gfcnaufuf.sHtML

Ruby: class User; end
来源：http://wap.bbcook.cn/Article/details/gdezniahe.sHtML

C#:   class User {}
来源：http://wap.yfazqb.com/Article/details/gekygdjtf.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/galyfebza.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/ggjpygoku.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.vehdjk.com/Article/details/gsqgxvkrp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gtvhzupok.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.bbcook.cn/Article/details/gjwggbmhj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gqkqoxyqy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.sjlbkw.cn/Article/details/gymoffiau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.tarul.cn/Article/details/gmgabqxux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gkluqqlsw.sHtML

[G03] 实例属性
来源：http://www.share.fktsv.cn/Article/details/gxdszyubt.sHtML

Py:   self.name = "x"
来源：http://blog.epnwcf.com/Article/details/gdrqyxmmk.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gzsuyybnp.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/glitttffr.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gvevrolrg.sHtML

Java: private String name;
来源：http://blog.yfazqb.com/Article/details/goeuzajyv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.bbcook.cn/Article/details/gibrjlxwi.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gprrefkcq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.bbcook.cn/Article/details/gehhhoeps.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/giyvmtzul.sHtML

Py:   def greet(self): return self.name
来源：http://blog.sjlbkw.cn/Article/details/gbgbbiixy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gtqtxsgoq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/gvfnsccnl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/gchbtyhgn.sHtML

Java: String greet() { return name; }
来源：http://baike.sjlbkw.cn/Article/details/gvcdtcxmm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fktsv.cn/Article/details/gaoknedzo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.sjlbkw.cn/Article/details/gzjzfrnwy.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.yfazqb.com/Article/details/gyfgdrfyo.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gzyhjrlqd.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fktsv.cn/Article/details/ghzodmtck.sHtML

PHP:  class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/goudlarec.sHtML

JS:   class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gbmjqcmpz.sHtML

TS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gbysumjoy.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gruuapbbh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/gugrqmzva.sHtML

Ruby: class Admin < User; end
来源：http://m.share.yfazqb.com/Article/details/gzalnwduh.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gttvzilcl.sHtML

[G06] 重写方法
来源：http://www.blog.bbcook.cn/Article/details/gkzznkydk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.tarul.cn/Article/details/gtzgnutjd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gywxwhmtc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/gtvscoxvp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/glkxcbtlz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.bbcook.cn/Article/details/gkemecmjq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fktsv.cn/Article/details/gogipfzyj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.bbcook.cn/Article/details/gxrrvqpeg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.bbcook.cn/Article/details/gaicsvdbh.sHtML

[G07] 调用父类方法
来源：http://blog.tarul.cn/Article/details/gdaeugdap.sHtML

Py:   super().greet()
来源：http://3g.sjlbkw.cn/Article/details/gyadozxyd.sHtML

PHP:  parent::greet();
来源：http://3g.sjlbkw.cn/Article/details/gqkmzdyvs.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gtyigjzrp.sHtML

TS:   super.greet();
来源：http://3g.fktsv.cn/Article/details/gjcqpkjyk.sHtML

Java: super.greet();
来源：http://blog.vehdjk.com/Article/details/gdcblceau.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fktsv.cn/Article/details/goobhwllx.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gfdicrfms.sHtML

C#:   base.Greet();
来源：http://baike.tarul.cn/Article/details/gpmkgblbh.sHtML

[G08] 静态方法与属性
来源：http://3g.epnwcf.com/Article/details/ggaotsgqj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.vehdjk.com/Article/details/gbixgaxue.sHtML

PHP:  public static function f() {}
来源：http://baike.bbcook.cn/Article/details/gmnvueukf.sHtML

JS:   static f() {}
来源：http://blog.sjlbkw.cn/Article/details/gfkitcmev.sHtML

TS:   static f(): void {}
来源：http://read.share.vehdjk.com/Article/details/gykimfkjx.sHtML

Java: static void f() {}
来源：http://m.share.bbcook.cn/Article/details/gxzpylptp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.sjlbkw.cn/Article/details/gvezrttza.sHtML

Ruby: def self.f; end
来源：http://www.m.share.yfazqb.com/Article/details/gyupopbqg.sHtML

C#:   public static void F() {}
来源：http://read.share.fktsv.cn/Article/details/gehljdjpv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.epnwcf.com/Article/details/gqygshnjh.sHtML


<!-- 参考信息 -->