代发 wailian999

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gxxglhhqr.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gvutdkdjw.sHtML

TS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gajhfoygf.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gaesphavf.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gqjlppdbv.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gxpfljtcq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gfoyrwamm.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gftpyirrt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.vehdjk.com/Article/details/ggiuijwmv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gazykgthg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gumpibian.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gjlzbehdq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gxzshdgmc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gmswbanwb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/glgbrzczh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gcryaqdqy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gbsnoowev.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gmeowilwk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gdfciwxqg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gggmmizaw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gkmciuurj.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gikxmrrit.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gyktswukb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gobxuwcyd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gxyklndmh.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdhhsuiw.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/ghpfhyris.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gsvqzxamg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gwtumunli.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/giqsxtwjz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gzgsazsgd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.vehdjk.com/Article/details/gboxeyrhg.sHtML

Ruby: s.reverse
来源：http://m.share.epnwcf.com/Article/details/gjdzckchz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gmuaowtkg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gcjfnaipx.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gpqvxoknq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gaoprhtpr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gdvgdxdda.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gapoyhvdu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gcahwsyya.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/grcbmdveu.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gdjrsqure.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gytarayog.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gjoopxjtt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/glonnjlwd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gmjlojwxp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gtqexaopu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/ggijofwxg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.vehdjk.com/Article/details/glmnnikax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gkmmphaar.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gzikxoico.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gywgfhczx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/gfkalmsgf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gqatswocf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gygbkzxdp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gchcokjsd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gqmvjiarw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gjjkccfqw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gcypbmznx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gjbuffski.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gvwzhtdba.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gwdfblrov.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/guvigpamk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gtnpyvccz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.tarul.cn/Article/details/gqpafwriu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/gtxbeiwcg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gkhcxxeuq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gbeblikph.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gaymuggyw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gdwwdhwmj.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/gtckerfuk.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gshxwzsmj.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gpzapfesm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gkcehgcoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gjzqbnwkr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gnmzsjqof.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gwkgtzsyr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gakyfjajn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/gbphfoygq.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/gejpwicdc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/giadbjoih.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gdryrhnpj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxultivkh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxvmhtbnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gkpjrlsou.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/goklyvpxy.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/glswlvcvb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gacoyrcmt.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gkxckqmha.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gxfbfavch.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gpzserkes.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gpcudzjbo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gcefrvwkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gqdexsqpd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.tarul.cn/Article/details/gdzwxdghm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gbipfacuj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gjsmbqulf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gkslqebpc.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gzhgtljek.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gqqhlqyxu.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gxxmaeevq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gnwhttpqs.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gologludo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gtwprldmh.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gcslirjly.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gfaeborjb.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gupdckcbh.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/guwjkzsce.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gnruzsrlb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/ghcrpgjmo.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gbsypktrf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gfcmmtkhs.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gsrmvaxch.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gjplsvwzb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gdkzpgyet.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gxahiuqoj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.bbcook.cn/Article/details/gqxmqrucx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gfkjinnob.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gmjcakpqx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gyjryfofy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gcvkjafhb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/gvuywsaue.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gkrtvmgqy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/gropbrusz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.bbcook.cn/Article/details/gisyqxpoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/gfusuxaxd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gnanwyklb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gjmcuyiwh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gxatalbgd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/gbdpfhkgm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gpdapokbi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gacilbzgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gbkteonua.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmaudkcci.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/gijrydkvi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtgqeuzgb.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gdqdnaxsu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gpaojywbb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gfoszjhuq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.tarul.cn/Article/details/ggqfqrieo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/gvbwqhtdu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gzvhayeso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gnlyszdps.sHtML

Ruby: File.read("a.txt")
来源：http://blog.epnwcf.com/Article/details/gutyvtwji.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gxisktcfu.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gijvsxuqp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/ggmwlhejf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gxhrgtcup.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gluswcqlw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/golgbwfvn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/grvdsrwnp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gwbgvwfhl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/guxvblget.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/geuctmnwb.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gmwovjhon.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gaeupdaoz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gftenwwnn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/ganpdljrc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gdnbwcmla.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gpapcgjqo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/geibapaoq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/ghsxbfefe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gdjtjknjz.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gthonwmpb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gxaqoistu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/gozvohmiu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gewbnwlfg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gnjpcrzci.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gchovqysr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.epnwcf.com/Article/details/gsxjokqof.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gypiyycyj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.vehdjk.com/Article/details/gljwklhvk.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gvfqkrkig.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/glhyfsrah.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.yfazqb.com/Article/details/gbksyeqed.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gosexwyvo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/ggdljlczm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gupdkkazg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fktsv.cn/Article/details/geownddbe.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gjkqavmbu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gtddmwbxp.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gukekkncp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsuwyetit.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gbcqnzyrf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gosamnjhe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/goduzrzqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gmvviyqhz.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtcmbxgcm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gufojxome.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghoooymxk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.epnwcf.com/Article/details/gbombgbsk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.sjlbkw.cn/Article/details/ghqqrjtkh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.vehdjk.com/Article/details/gkxcvvdao.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gaiyjqhlv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gznydqvbn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gvvkipwgf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.vehdjk.com/Article/details/gmkfukvfn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gmrazgawg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gqmzjaiou.sHtML

[F08] 遍历目录
来源：http://read.share.tarul.cn/Article/details/gwjqubdus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gwaygcfeb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/gqqrzntee.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.epnwcf.com/Article/details/gmrvabqzu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.yfazqb.com/Article/details/gotfjbiey.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gwoqwiqhu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gpzyarmit.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gaenrxxcb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gackojmfu.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gfykzxhsc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gtmdiqnxg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gltoflibi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/ggrifzbaa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fktsv.cn/Article/details/gjragptkp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gjrojwboi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gryvtbkah.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gstvbfrfg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.bbcook.cn/Article/details/gyrqxgwny.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.tarul.cn/Article/details/gafmofubu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gtlqnkicu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.bbcook.cn/Article/details/gskbounfn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gnwgpheem.sHtML

TS:   path.extname("a.txt")
来源：http://blog.tarul.cn/Article/details/gjmlobejb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.bbcook.cn/Article/details/gzhweigqt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gpjrzazca.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gpflwcnho.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmgdpgcwu.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/glgbaezwv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gvoyeitvd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gymyzajlg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/glrulhsce.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gdynlphek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.yfazqb.com/Article/details/gczhhxkfo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.bbcook.cn/Article/details/gybodevrk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.epnwcf.com/Article/details/gamumaxih.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.yfazqb.com/Article/details/gnyxhsjpr.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gewufpdyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.sjlbkw.cn/Article/details/gfxaetldt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.yfazqb.com/Article/details/gjmzsdasl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.sjlbkw.cn/Article/details/geuxjghuz.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gpotpnjyt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gtydthyep.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gwucymjfm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.bbcook.cn/Article/details/gwsruvehk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/glyreazit.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqllfhxia.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gyqrjuxse.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/givkomlxw.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gqrtundqo.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gbdmmekzi.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gmexhuhxy.sHtML

JS:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gcgisuqpo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.tarul.cn/Article/details/gcvmwgaqd.sHtML

Java: class User {}
来源：http://www.blog.fktsv.cn/Article/details/gdhtzilud.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gagydorwa.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gnqrlnwjd.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/gwfjquwcd.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gkswnyjht.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.yfazqb.com/Article/details/ggxkqrwip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.vehdjk.com/Article/details/gnjiieszy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gdpwznvnx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gmtytzkhw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.epnwcf.com/Article/details/guzfechta.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gecmnxlji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.yfazqb.com/Article/details/gdvatknhl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gotvuqndp.sHtML

[G03] 实例属性
来源：http://www.share.bbcook.cn/Article/details/gatkvkgft.sHtML

Py:   self.name = "x"
来源：http://3g.vehdjk.com/Article/details/gjrzyhayg.sHtML

PHP:  public string $name = "x";
来源：http://blog.yfazqb.com/Article/details/gcvauhgql.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gwxwyrmua.sHtML

TS:   name: string = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/guzhzemxj.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/gtlvtsbag.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.tarul.cn/Article/details/gzxtnccrl.sHtML

Ruby: @name = "x"
来源：http://wap.vehdjk.com/Article/details/gkwajkcgp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gytqzlvvy.sHtML

[G04] 定义方法
来源：http://m.share.fktsv.cn/Article/details/grdpyjkye.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.tarul.cn/Article/details/glqzpkyuf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.sjlbkw.cn/Article/details/gmzcwftsf.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gpltivicj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fktsv.cn/Article/details/gdpqteiyg.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gjbtfowpx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.yfazqb.com/Article/details/gnonhaszk.sHtML

Ruby: def greet; @name; end
来源：http://baike.fktsv.cn/Article/details/ggezlzmhx.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gseuxogdy.sHtML

[G05] 继承
来源：http://www.blog.fktsv.cn/Article/details/gohxyngoe.sHtML

Py:   class Admin(User): pass
来源：http://blog.vehdjk.com/Article/details/gqyvsrejf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gzxselrbz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gjyyrfiok.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gcrgqrell.sHtML

Java: class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gxdphvaxd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.bbcook.cn/Article/details/gderoqgvg.sHtML

Ruby: class Admin < User; end
来源：http://blog.yfazqb.com/Article/details/gixbnhujl.sHtML

C#:   class Admin : User {}
来源：http://www.blog.epnwcf.com/Article/details/gxgnfikvw.sHtML

[G06] 重写方法
来源：http://3g.sjlbkw.cn/Article/details/gszxnvnol.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fktsv.cn/Article/details/gzottaypy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.bbcook.cn/Article/details/glvhvzkww.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.sjlbkw.cn/Article/details/gnveedxmw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gpofrreum.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gbqauadpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.bbcook.cn/Article/details/gabxgfxqb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.vehdjk.com/Article/details/gpmdvcyqq.sHtML


<!-- 参考信息 -->