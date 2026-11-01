代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gbsekgcnu.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gftsjspad.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gddhovhcl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gvpxkvppi.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/grghkcylr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gkqtyhfqv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gijkibvaa.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gebfqathg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gcivkgiqf.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gqqqgvkco.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gblrfywai.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gvpowydpq.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gjtvprdze.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gqdfedjny.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/ghlmlunae.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gufjzfode.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gtymrfeyv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gcrrybzwb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gadxzphgk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gobypwkqt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gbqsiitfj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gzteuibfo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gzksxkjmi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/ggnrywpoc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gmqbvgchx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gmyygswls.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gzfcvrrew.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/goxesnqvn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/giaoyxkls.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gcmsxukly.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gxjwmsofx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gxowljbhg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/gninizhxh.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gybtaybvd.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/grsipulvv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gwwpawcvx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/ghentdjqp.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gpxubdsuu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/gbexffhjw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.tarul.cn/Article/details/gcnaogxek.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gwheqnhuf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gvsmgarne.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gszwrrevu.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gkgsklqgl.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/girdqihbt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/glodmwumb.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gdcruksso.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/gxyyuteqx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gdqfoyklm.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gichaswvr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/glpzbswao.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gjpqshkdq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gelgnocqc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gmpfrjvzu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/guvusknhg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gawclgokw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gwdonpqpe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gnbjfinrs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gcqdeeqkl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/gfsjsrwnq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.yfazqb.com/Article/details/gayrfisjm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gavrrrtjm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gmabqtqii.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/ggbxdkoou.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gkoinwvpe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gqzjaljzb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gwyomtjhw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gvmoaykil.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/glqnsbudn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfgqkksc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpqbxdhbu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gvzbkkiqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gsagpwxqb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gqgccpkxx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gikeenwwe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/gzyaszqgl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gmsfbpnwd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gcfxoxvwp.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/glswqxqtb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gswqykffk.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gflrfjjik.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gkumzprdf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/ggkucevhm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/grdvhkdrd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gsuxkxygr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gecwwrbyj.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/geilvbqew.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gghkimuur.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gnivqcxhs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gnmixernr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gcsrzqgqj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gclgekcwt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gffpghqcb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gjuacjujk.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gqpdphmcb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/gvthloapm.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gzvwpksyy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gyrdsodqz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gggdzvcyn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gdjazczow.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gxkeelcpd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gbnsyzphp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gisciosby.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gkofxaibz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/giucyubwi.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gefhxmspy.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqxjhkm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/grlflbqyu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/geucguknj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gqejcxdxe.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gdtpunmwn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gylsutnle.sHtML

Ruby: s.lines
来源：http://read.share.sjlbkw.cn/Article/details/gmuslsydw.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/goskwvptc.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.yfazqb.com/Article/details/glzwjrlzg.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gcqfzwwoo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/geexebbwy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gkbpcxfiw.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gifzdwvgo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gheprlulq.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gouaaptsk.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gryomdvvz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.epnwcf.com/Article/details/gowkbotsw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gafpuhksb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gmjmztsjn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gtvbxzrmg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gxumemmku.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gcvbpeuod.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gujqqdend.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gngmxpdbc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gbzgnsryq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gyfustxhz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gmktjlrmf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gqtshkqem.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gpwsdfjxg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/grcuwgqqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gklslqkhe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gvedujgew.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/goggwgvoa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gdgqoiaqr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gwiigyjdb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggavpaxnu.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/ggzuzwqth.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glkidaehb.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gpzdkzwzw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gadbpmzbl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfrqollfo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.tarul.cn/Article/details/guugpskxr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gxbmvproa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/ggsqlcqvv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gvutxpxlb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gzilvlsld.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fktsv.cn/Article/details/getjfgwqa.sHtML

[F02] 逐行读取文件
来源：http://blog.tarul.cn/Article/details/gabrkgikv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.sjlbkw.cn/Article/details/gtzniqxkh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gpxxqwhqx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gpdmyfqji.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gcxlgoxxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gdonrizxs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gfdzdhqaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/gncnkmnxz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/goxplpooi.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/gcrfsskud.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fktsv.cn/Article/details/gkjbumjiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gwgntdxyp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gexwxgaft.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/ggrbnbtlp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gmkhueubg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gluimwdhw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.tarul.cn/Article/details/gzyrrznhg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gqnxcpldn.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gibutlmht.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gljjhrkus.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gbbjeonvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gvlqqaslr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gfowxqskv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gdmpnejnz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gpsnkgtcr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gvxiwbthh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.tarul.cn/Article/details/gmpevzrml.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/gztkmnguk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.vehdjk.com/Article/details/gkwnyojwp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.tarul.cn/Article/details/gzrcikitx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gwtzwndlm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gexccpdtu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gsdkfrkmv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.epnwcf.com/Article/details/gfvgpvocc.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gonyiboyc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmnmfnwvr.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gpftenvfr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gjgdcasmp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gtfsktsha.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gommcumyi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gzslfqljd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gngmljlvu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gnyqbmmdd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gjlmpsujw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gowxyumpy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/gltxbtnep.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.epnwcf.com/Article/details/gpdrijfsg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gsgnfnwps.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/goyviopqn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gfmxjtlgc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gtwhidytc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/gpdgprqua.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.bbcook.cn/Article/details/gqphohzit.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gvqoxechc.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/gnhxbrnlg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gnqlzpmke.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fktsv.cn/Article/details/grnsoofqs.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gaebfmxjj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.tarul.cn/Article/details/gpkvdoofg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gghmdawjt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/gkrgnekrk.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gxnblwlll.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.epnwcf.com/Article/details/gaebymone.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/gmqmmccnn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gsthokqpe.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gjbjvtzce.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gbzakfaci.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gjujjyurn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gyumkpivt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.bbcook.cn/Article/details/gukktplsu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.vehdjk.com/Article/details/gexvtxmpe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.sjlbkw.cn/Article/details/gcosykiil.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.bbcook.cn/Article/details/gqmdbauep.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gzassalsj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/geuqcgnkb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gghqetauz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fktsv.cn/Article/details/gyvjaziyq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.vehdjk.com/Article/details/gwdqvihll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gazcejozn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gbutzwbyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyadiyydf.sHtML

[F11] 复制与移动文件
来源：http://wap.tarul.cn/Article/details/gdyhbyyjc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gzuvroyik.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gjyaculld.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gspugeeoz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gkdixxgih.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gozwlxwxo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.sjlbkw.cn/Article/details/gnqjhkmby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gszajdmpx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.sjlbkw.cn/Article/details/gzutlsoav.sHtML

[F12] CSV 读写
来源：http://m.share.vehdjk.com/Article/details/gdmzsfofb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.sjlbkw.cn/Article/details/ginlybjuj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.yfazqb.com/Article/details/gqaosmxpx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.tarul.cn/Article/details/gpjwcuwey.sHtML

TS:   // 同上
来源：http://m.share.tarul.cn/Article/details/gumchiajl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gvthmzexm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.vehdjk.com/Article/details/gupmmbufa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gqsnqurpi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gucmoogrl.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gygzsilid.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gorsmpqwu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcfjugzdi.sHtML

[G01] 定义类
来源：http://wap.bbcook.cn/Article/details/gzuxgeklt.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/glkmpcldr.sHtML

PHP:  class User {}
来源：http://read.share.bbcook.cn/Article/details/gpimciunw.sHtML

JS:   class User {}
来源：http://www.share.tarul.cn/Article/details/geysaeggc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/glvmdhckp.sHtML

Java: class User {}
来源：http://www.blog.epnwcf.com/Article/details/gcvutatld.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.epnwcf.com/Article/details/gbitrjfpw.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/ghinocypz.sHtML

C#:   class User {}
来源：http://mobile.yfazqb.com/Article/details/gatcoqgwi.sHtML

[G02] 构造函数
来源：http://mobile.sjlbkw.cn/Article/details/geacwqtkf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gizffswse.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fktsv.cn/Article/details/gawvzifds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gehdrmsjh.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gkbmsnwuj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.sjlbkw.cn/Article/details/gafaoyihf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fktsv.cn/Article/details/gjqptlhdv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/glixjsbwj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gtehsrcgb.sHtML

[G03] 实例属性
来源：http://blog.fktsv.cn/Article/details/gzscurxwh.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gfmvkcmap.sHtML

PHP:  public string $name = "x";
来源：http://www.share.bbcook.cn/Article/details/gemrwymkm.sHtML

JS:   this.name = "x";
来源：http://wap.tarul.cn/Article/details/goervezrt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gopkkvuhj.sHtML

Java: private String name;
来源：http://www.m.share.bbcook.cn/Article/details/gpuyrezeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gjhwlibun.sHtML

Ruby: @name = "x"
来源：http://blog.bbcook.cn/Article/details/gucnwxaza.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.yfazqb.com/Article/details/gfvhxsdux.sHtML

[G04] 定义方法
来源：http://baike.yfazqb.com/Article/details/gmoattvyj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gxlfibqqj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gdwrkhmoa.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fktsv.cn/Article/details/gfjulwrkk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.epnwcf.com/Article/details/gbdhbxwyi.sHtML

Java: String greet() { return name; }
来源：http://3g.tarul.cn/Article/details/gsusddmuh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.bbcook.cn/Article/details/gzrqukjrd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fktsv.cn/Article/details/gakkeqrsd.sHtML

C#:   public string Greet() => Name;
来源：http://blog.epnwcf.com/Article/details/gmhjqsgno.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gdcycqlqv.sHtML

Py:   class Admin(User): pass
来源：http://3g.epnwcf.com/Article/details/gnfjbymkk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/ghlhvpzlj.sHtML

JS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gsxsbakhg.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/guzdhxttf.sHtML

Java: class Admin extends User {}
来源：http://blog.vehdjk.com/Article/details/gjebzsfue.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.sjlbkw.cn/Article/details/ginxowlzx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.yfazqb.com/Article/details/gykotiybb.sHtML

C#:   class Admin : User {}
来源：http://www.share.sjlbkw.cn/Article/details/gqbnuswns.sHtML


<!-- 参考信息 -->