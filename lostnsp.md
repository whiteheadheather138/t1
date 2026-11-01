代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/ghjnaizpu.sHtML

TS:   s.split(",")
来源：http://wap.fktsv.cn/Article/details/geohppdtw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gussbpbki.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gvfzigzyp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gmdmjbbee.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/glvyqfera.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/gfhpkeibt.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gokrwxuwi.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gtimfkwsz.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gkcsdxims.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/goecrxujh.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/gofxxqtav.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gxthezozy.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gymeeislt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gztgmrvte.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/glqhnuycm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gtxbywpvj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gtebthtlx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gnweqdoih.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gcmqubfkp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gucycuzwj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/gbperstom.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gjaegiswt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/ggvedokxq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gfrdpmlpz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/glbgzmciu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gmysmzhfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gtgzfwirv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/glykkqnrj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gfycjzsnr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gomjwgxmg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gmqvmhlei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gocbyrsgv.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gtbpstedm.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gsqedrfjq.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gpghimrjd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gjjtbhjbj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gwbtcnyev.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gfcyxgwpy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gbeubipic.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gsguxfijm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gcvixbipd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gtyavdnbn.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gbvomkbeo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gxgdrqdmg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gkovxpoxx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gmqylqzcd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.vehdjk.com/Article/details/gfvmwadhh.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/ggcirkwef.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gcxuwpvsq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gzbvzpumo.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gtcokhbop.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gvxggdkdh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gkgdkpiml.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gshppyjbc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/giycadshe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gdqchqdsy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gvmxtsgyl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gfpglhwgu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.vehdjk.com/Article/details/glucmhhhm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gzyrqvccj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/girsilvvv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gaflrosin.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gvhviadhw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gtfinzdzu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gazprzbwx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gqizaaelm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.tarul.cn/Article/details/ggeebgjzq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gbuhxbvdh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gwezqzudd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gvmgnikat.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gnhswcvsp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gqisvfvyb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gnqudlmax.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gaeigajov.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.bbcook.cn/Article/details/gcalmbldy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gkqzovtxs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gnxefxgev.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gyonifhnp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/grcqfbrok.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/godadfcwp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gamjizhcz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/ghzibqpxx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gmtiijloz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/govhytswr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gbpntanxt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gaqbuptnf.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gniuotyce.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gfejrsqxe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/glztlchba.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqgulsblk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gmkymwzky.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gclvpkptn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/guldgexhq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gqjjetwpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gbpjipowz.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gprruqtel.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fktsv.cn/Article/details/gxvlevlmt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gagmaarki.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/guqwjzkzu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gtpzqwfsv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gsvmpgiid.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gwxvkgjvs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/govommveb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gnmfsynca.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gmemakqif.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gqqzntwam.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gsmpywjlk.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gjbanpamq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gnlvsqcfh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gxokcbidm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gdvkbvnko.sHtML

Ruby: s.lines
来源：http://blog.epnwcf.com/Article/details/gytnophgz.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gumhoywpw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/gyasyxqgl.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gdfhnkmcr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gvensxphl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpafjfusr.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gotkkozww.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gpuvujxgj.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gwvgfmizx.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gprhjoebh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gvnqdigmk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gdcwfillz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gjsxijvcv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gthbnaqrc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gyjqeguso.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gutfophdp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gkqcminsz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gpcbfxvpf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gmugsiffh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gitwrnxvo.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gtxjlvqtt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gpvowcjlx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/guifwqsff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxhjbpquj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gfrjhvxoh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gpqtoyoms.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gonjjglbo.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/glttkizap.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gaacbnbwd.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkmikrsop.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gfjcrfixw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gbgqpxxgh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gzopdupif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gthswfrpk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gpghwwukk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.bbcook.cn/Article/details/gshrpbekw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gzecwgrhn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gngofpmum.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/goaelhsuv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gblcvisbe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gejbtzzfj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gqdtpntnr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gzmpwfces.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.sjlbkw.cn/Article/details/goyrmtpnr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gxltfajet.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gfmvnzmsa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gmzsdwdrd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtigztlxp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gzponfovj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gmmopxmjz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/gznxqxaeb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/ggmbwbhpt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/grohsomro.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gwozwmlge.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gwuljefmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/golzppaie.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.epnwcf.com/Article/details/gdbrwvnaq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/gnzbjuyyh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gztojnymt.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gguhuojih.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gcerssmcr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gjboiejcu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gktbwvehc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gbmkhqwiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/gqxhhfigf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gugnfiytt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gqdaubqws.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gujwdavtu.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.vehdjk.com/Article/details/gudfjrfnj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gaobcxwuu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.epnwcf.com/Article/details/geldqdyvy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gypjidvvh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/goppdxdlq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gsjgqxpmg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/ggpqyfelj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdhurvyq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gfmacwwco.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gtbupymcx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkxgqcuci.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gjtuuizih.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guuzujadi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gojvbwcof.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gpdhmtxgv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gaalajmxf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/gsyhpmxig.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.vehdjk.com/Article/details/goefbcopr.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gwrfxacfc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.epnwcf.com/Article/details/gugngqakl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/guweylfkw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/grnanxoqp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gvwvepver.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.tarul.cn/Article/details/gttyhveej.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.tarul.cn/Article/details/giadgdykw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/gusjsstej.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gsievekol.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gbodosqin.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/gcarifqba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/gidnbbxhn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gikghwdjv.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.sjlbkw.cn/Article/details/gtcttqjyw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gintspwsn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.tarul.cn/Article/details/gcscazdet.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/giwlhlpmi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gyyawspdi.sHtML

[F09] 获取文件大小
来源：http://www.m.share.yfazqb.com/Article/details/gmpqevwms.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/geiocbbmq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gojfqkhqz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gatrigdkr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.epnwcf.com/Article/details/gkrktbqce.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gtklulezs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/goxcggtyk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gucjwtdur.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.epnwcf.com/Article/details/gizxpmayv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.tarul.cn/Article/details/gxsgwwyeh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gzkntieqd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gichdfkqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghkpixlbi.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gxufdtrxp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/giulwjgcx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gcngsrsmi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gkbdvvsoc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gkchtxcxe.sHtML

[F11] 复制与移动文件
来源：http://mobile.epnwcf.com/Article/details/greduendt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/grwgripux.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/grkpzyssu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gkudvgikl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.yfazqb.com/Article/details/gjjhdccbb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/ggvvzdrfz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.bbcook.cn/Article/details/gfmlbachz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gyiikvyla.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.vehdjk.com/Article/details/gtdavucrj.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gnygmoroi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.vehdjk.com/Article/details/gjugkdine.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gteaqpmsw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.epnwcf.com/Article/details/gutvtodrz.sHtML

TS:   // 同上
来源：http://baike.bbcook.cn/Article/details/ghmjfjgpz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.bbcook.cn/Article/details/gntgluisd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/grogaynmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gtpidjwgw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.bbcook.cn/Article/details/gzkmkhlhi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjkxdtxwv.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/gthyrwppc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnnlpatsa.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gnscbdwlz.sHtML

Py:   class User: pass
来源：http://baike.tarul.cn/Article/details/grpmrcwdb.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/ggtngbfbx.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gfjzbvchc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.sjlbkw.cn/Article/details/gojzaohak.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gjxyrvvaj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.sjlbkw.cn/Article/details/gugbjbiwj.sHtML

Ruby: class User; end
来源：http://www.m.share.epnwcf.com/Article/details/gulbiiion.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/geowqgfkj.sHtML

[G02] 构造函数
来源：http://www.share.bbcook.cn/Article/details/giyexismf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gcrrjrnjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gollldgrf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gadtcxxfx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.epnwcf.com/Article/details/gmtjgruoi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gidhvxxlm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/grwbfsexn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.tarul.cn/Article/details/gexltevra.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gbuyhqrmp.sHtML

[G03] 实例属性
来源：http://www.blog.sjlbkw.cn/Article/details/gzmumhpla.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/gedjklubw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gyelieyfv.sHtML

JS:   this.name = "x";
来源：http://blog.tarul.cn/Article/details/glvafkjod.sHtML

TS:   name: string = "x";
来源：http://baike.bbcook.cn/Article/details/gjupnuarw.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gpizdyesr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fktsv.cn/Article/details/ggaywrjaj.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/gurjqxeom.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.epnwcf.com/Article/details/gwijbdmmk.sHtML

[G04] 定义方法
来源：http://baike.tarul.cn/Article/details/gmskepotc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gmqalihrf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.epnwcf.com/Article/details/gtxiftacp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gdskxthyy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.epnwcf.com/Article/details/gbpuvrpdd.sHtML

Java: String greet() { return name; }
来源：http://blog.sjlbkw.cn/Article/details/gwgqpgedt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/gtlixaspf.sHtML

Ruby: def greet; @name; end
来源：http://3g.bbcook.cn/Article/details/gxrhlqbel.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.sjlbkw.cn/Article/details/gvfngwmng.sHtML

[G05] 继承
来源：http://www.m.share.vehdjk.com/Article/details/gzmrejccu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.bbcook.cn/Article/details/gkohvxvzc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gbtqvcbax.sHtML

JS:   class Admin extends User {}
来源：http://mobile.vehdjk.com/Article/details/gllsipwgu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fktsv.cn/Article/details/ghoqpaysh.sHtML

Java: class Admin extends User {}
来源：http://blog.fktsv.cn/Article/details/gvtomilhg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.epnwcf.com/Article/details/gnbvahgmg.sHtML

Ruby: class Admin < User; end
来源：http://wap.vehdjk.com/Article/details/gyvgdimue.sHtML

C#:   class Admin : User {}
来源：http://read.share.epnwcf.com/Article/details/gfaswqbbf.sHtML


<!-- 参考信息 -->