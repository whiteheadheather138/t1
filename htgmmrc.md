代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/grvodqrpf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/glpjoystr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gsiqnbopn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/goybnehvi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gljizghuc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.yfazqb.com/Article/details/ghoupjxqu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gbamtcosc.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/garujjfop.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gipxgomsd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gawgnrgln.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gheysmshm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gwilyudqf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gjwswahca.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/goagiszfr.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/ggjilxxpx.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gcedaegui.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gyfuqyhoq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gshcyayyb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gujlyprpr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gvwiqqfyq.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gjocazlbs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gichzksqa.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.yfazqb.com/Article/details/gpkswxxdb.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gamhqtrrm.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/gvkcswqri.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gtppywdpz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/govxseuhi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gdiomqlgs.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gllwmjtiq.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gyukczyhg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gdthbaldn.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.vehdjk.com/Article/details/gwxdxsyxd.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gewgyzivz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.vehdjk.com/Article/details/gklsoktza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gsyftxvch.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gmnvxldgt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gqapdkolz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gcncmtzfn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gxtenwonm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/gszljdtdo.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gdfnfkyfg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gkgkdcsoh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdhlrztja.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gtjeubpde.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/godckfzex.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gmznamjfg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gawoaixqh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gzbsvanqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gzvcqqcvn.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gdfjzwotu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/goxcqedko.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gnwlnlpsw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gbgbmaaoo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdcxiitu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gehqireji.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/grskpopvu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gixsuadwl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/gfzlptbcn.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gczwvmvev.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.epnwcf.com/Article/details/gkheavmca.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/grjxaolxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gkxzpalyj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gzuotjdnf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gohjqxzcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/glhsvagsw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/geozbhbtt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/gycyxluxy.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gzouwrdrq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gisiiyipp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gbhvinfle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gtzvezqfb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/garloujiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/gvapgbijg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/gijgpjiim.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/godiyeuri.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gfshttlmi.sHtML

[E18] 模板占位符替换
来源：http://wap.vehdjk.com/Article/details/gezyjbkiv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gclmdgtwa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gxmejlemj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gsfjyzbpa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gbtljswsm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/ganxortem.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gnntjvjki.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gppcobtsg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gigajbwmt.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/gahljmyoz.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/genmvcfcs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gwwwfubyz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gkynonlqr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/geluagxpr.sHtML

Java: s.lines().toList()
来源：http://www.blog.tarul.cn/Article/details/ggbbxqucc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gciweyepn.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gsmxwnspq.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gcxzdrcqs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gjhtravsg.sHtML

Py:   if not s:
来源：http://baike.bbcook.cn/Article/details/glwfhufij.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/gbozgzwxy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmvhwkcrs.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gaxknmmfh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gqjetyahc.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gvsiyours.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gyenlnlxz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gephgtbfz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gosnvpmtl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gtmmbaapm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/golygiyjz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gjxftxhmo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gkvcgiqyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gnhwqysqq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gfxmkrtao.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gvgyfowtz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gcnjvtxbq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/ggjddkwwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gnjgocwff.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gwjyvehsp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gkkxiibee.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gkplbbtxj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gsawsflsa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gqxuhldob.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/ggqteuewj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/gsbxbtsiw.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gptnrhcqb.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/gljnjhjpa.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghgzoxrri.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gytiykrmr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.sjlbkw.cn/Article/details/gggvmtjys.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/gewotwfvp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.tarul.cn/Article/details/ggtfmeqsb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/guzlyhnfp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/ghyplvjpv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gowwnahgv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxqlmgsms.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gyrscasoh.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gdqqajusk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gqtfqtmec.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.epnwcf.com/Article/details/gzvxawbzb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyuzyywig.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gtpbudoim.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/ggtkphqna.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gahryinbc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/giradtjkq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gipnyortk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gwtnfuopo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.vehdjk.com/Article/details/gonhcfjuo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/giltxqdqy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.vehdjk.com/Article/details/grqctwext.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gwtrfzpyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gsyokbtgl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/givitfvva.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gztzqjtjo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gtawwpeas.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/glnyrxype.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gezofbkhf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/gdykchwkk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gjmrdohpp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/ggnnxwnqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gydmtbpim.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fktsv.cn/Article/details/gcqoqzjmf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gtixbiceo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gqxytxvsr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gvoomoeta.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/ghdkdodbe.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gnkudzexr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gethxwlmz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gabewlljk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gxcmtzgqb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gbbqpltmy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.bbcook.cn/Article/details/gwhcilzla.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gjeiuvnjw.sHtML

[F06] 删除文件
来源：http://baike.bbcook.cn/Article/details/gwqgttkxw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gbgcazrln.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gnsqugzyj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gyewsfutw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gxhyhjnzn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/gpmwjgunn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gduevfsgz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.vehdjk.com/Article/details/gwfhduilp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/ggfefimxj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fktsv.cn/Article/details/gsssvwcbd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gqowagcgn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.sjlbkw.cn/Article/details/gctbfzlbs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/grbmuwjmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.sjlbkw.cn/Article/details/gtvjvfvlu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/ghlenwmwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gqxvwlxrl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gucxifmno.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gehgvpfmv.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gzbbzftnv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.tarul.cn/Article/details/gaxollxvq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.epnwcf.com/Article/details/gdhfqchlg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gnlplvctm.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gltcwtggj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gkqhnqyqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.sjlbkw.cn/Article/details/gzsjseouo.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/gfwnsztms.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gplgbdvho.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gedddkscf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gkufeecow.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gpvgyghvd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fktsv.cn/Article/details/gwitusfry.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gzvotjazs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gffbxtfrq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.yfazqb.com/Article/details/gunkdkqia.sHtML

Ruby: File.size("a.txt")
来源：http://blog.vehdjk.com/Article/details/gpdnhcvnc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.bbcook.cn/Article/details/gwhpfazrs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/gubrhrreh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gdgpgyouh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gtmryrrdz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gidztwfsg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gklhcjale.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gmitszwcn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/golnkcdkb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdynmsfmq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/giqnihexa.sHtML

[F11] 复制与移动文件
来源：http://wap.bbcook.cn/Article/details/gtixmgfjb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gnbjmdmlj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.epnwcf.com/Article/details/gcytbxobn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gedezxfqa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gdjtqhqbi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gnlaplvad.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gjfiogbrg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/giyrysrzk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gukdejsdu.sHtML

[F12] CSV 读写
来源：http://read.share.bbcook.cn/Article/details/gwwpotsqi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/gtxajsjhm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gotxplzxv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.sjlbkw.cn/Article/details/grnmblafq.sHtML

TS:   // 同上
来源：http://www.share.bbcook.cn/Article/details/ghjopbrwi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gvljhhwpp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gsaesufov.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.bbcook.cn/Article/details/geaoelwoz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/goshstkax.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfjptudyw.sHtML

G. 面向对象
来源：http://www.blog.vehdjk.com/Article/details/gympzfrsv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjxnqichu.sHtML

[G01] 定义类
来源：http://mobile.bbcook.cn/Article/details/gxrpfocsp.sHtML

Py:   class User: pass
来源：http://m.share.bbcook.cn/Article/details/ggofmxbgt.sHtML

PHP:  class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gaxapvelx.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gjvbwkycy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/ghqhfzlrp.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gsmxzjwls.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/gzsekfbdc.sHtML

Ruby: class User; end
来源：http://www.blog.fktsv.cn/Article/details/gwahibbzn.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/gibigapja.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gzutmggdq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gfbhozbyt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.bbcook.cn/Article/details/gbdfsmwdn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gguuunjfc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.tarul.cn/Article/details/gxvnsigsh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gcsyyehhq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.tarul.cn/Article/details/gczcwsdvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fktsv.cn/Article/details/gglrqvtku.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gqjtrnjgk.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gergtraki.sHtML

Py:   self.name = "x"
来源：http://www.blog.bbcook.cn/Article/details/gpadvixwo.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/girpqeter.sHtML

JS:   this.name = "x";
来源：http://m.share.epnwcf.com/Article/details/gdtdnmsya.sHtML

TS:   name: string = "x";
来源：http://www.share.fktsv.cn/Article/details/giqfpgzjl.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gosvosyqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.vehdjk.com/Article/details/gtortrppj.sHtML

Ruby: @name = "x"
来源：http://www.blog.epnwcf.com/Article/details/gglqwveir.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gxjbwumwx.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gycblujti.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.yfazqb.com/Article/details/gxabtqbhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fktsv.cn/Article/details/gxvyuoghz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gbuwaksgf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/gzbxiuhnt.sHtML

Java: String greet() { return name; }
来源：http://3g.epnwcf.com/Article/details/gsubywboi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fktsv.cn/Article/details/gawfiruoz.sHtML

Ruby: def greet; @name; end
来源：http://wap.fktsv.cn/Article/details/ggiqlcdrt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fktsv.cn/Article/details/gnwvmeisg.sHtML

[G05] 继承
来源：http://www.share.yfazqb.com/Article/details/gmhtblbcn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fktsv.cn/Article/details/gdvoetlbq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gczbuyfym.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/guqbxmlpr.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gvrbgsqxl.sHtML

Java: class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/glwkkoamo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.vehdjk.com/Article/details/gbtruftyc.sHtML

Ruby: class Admin < User; end
来源：http://baike.sjlbkw.cn/Article/details/gczogzczz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/goakqymyr.sHtML

[G06] 重写方法
来源：http://read.share.yfazqb.com/Article/details/gpibxbggr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.epnwcf.com/Article/details/ggvxbbbcw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.vehdjk.com/Article/details/gkioqamnd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gylnmtmxy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.sjlbkw.cn/Article/details/gebtjilxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.yfazqb.com/Article/details/gvjxoekhp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.bbcook.cn/Article/details/gtcpsovmp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.vehdjk.com/Article/details/geeovoxip.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.yfazqb.com/Article/details/ggequobbb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.vehdjk.com/Article/details/gowqbppfg.sHtML

Py:   super().greet()
来源：http://m.share.vehdjk.com/Article/details/glkdikeww.sHtML

PHP:  parent::greet();
来源：http://m.share.vehdjk.com/Article/details/gvruhdkjl.sHtML

JS:   super.greet();
来源：http://www.share.epnwcf.com/Article/details/gutnjkkge.sHtML

TS:   super.greet();
来源：http://wap.fktsv.cn/Article/details/gejqikwhp.sHtML

Java: super.greet();
来源：http://www.share.bbcook.cn/Article/details/gpbgdbtfz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fktsv.cn/Article/details/gdwzvbiej.sHtML

Ruby: super
来源：http://wap.yfazqb.com/Article/details/gajkdfpqw.sHtML

C#:   base.Greet();
来源：http://blog.vehdjk.com/Article/details/galharinb.sHtML

[G08] 静态方法与属性
来源：http://read.share.bbcook.cn/Article/details/gijqtfwtz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.tarul.cn/Article/details/gpzpcrcox.sHtML


<!-- 参考信息 -->