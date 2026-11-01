代发 wailian999

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gqbtzxowp.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gznkfxlpo.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gnzfelqhe.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gskbbcltp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gewgeklsp.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/ghakrizaa.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gctqduqlm.sHtML

[E09] 去除所有空白字符
来源：http://wap.sjlbkw.cn/Article/details/gadpvistt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gjkltpkrn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gzymvgpqt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gpukyjcjl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gfvvgzguy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/geymlhybg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gbdpmobnm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/ggjgetwmi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.yfazqb.com/Article/details/gmlpgopvx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/guauvmnow.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gpvpmtjon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/ghoepvttn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gmmzqodep.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/glfcedkfo.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gahvscmzu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gxyfwasvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gkleyqbkr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gvmyrosft.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gowookakc.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/golzumxjk.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gczisqmwa.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gsnvtpijs.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gaehdkhoe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gqnzjbhbn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gdgdocahv.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gizlwojsl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gherlnctx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gldlqwcnl.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gizwprnjk.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.sjlbkw.cn/Article/details/gsfevqivj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwskqvde.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gofonxlfh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gmfmcgink.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gfqsnzymd.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gxgicizur.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gzsvitwfh.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/guyvwnkyr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gokachdwe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gdpwvdrrn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gxxsghhxd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gehfzewhd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gpsaixvth.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gwjxxgyzw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gyrtwrqmc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gkjgehvho.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/ggyoylshs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gtqpzejuh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gxjsitmjf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gxqajcdjo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gnhdwlkad.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gczlljbfu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/guhvubmgj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gapgctigt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/ghtonexsy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gzirjcspg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gamznllsu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/ggceoxvdz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gldxhnvuz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gfeiiqmfi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.yfazqb.com/Article/details/guqgtlows.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/gfhdvobmd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gmfhbkkfd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gctaulcbi.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gfhvrgcwd.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gydtgdntk.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gkqhrhxsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gyyibrhyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gzghplaee.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmqowuuy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gdnjseuoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gyeshkjgr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gcmcpdwml.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gropvdsjc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gxduugcts.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.yfazqb.com/Article/details/gulmuyqnb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gufkyugtr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gjvrpvnmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.bbcook.cn/Article/details/goizcejkf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/goriddigu.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/ggqritght.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gwpfmdrzn.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gumapjlxk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/grtotbcjy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/grbagtzjj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/givofdtyo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gpqocmezr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/ghfyzuqjw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gbjoevpas.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/gnxxioxai.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcyxbarx.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gcgzmnilg.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gbrhuhacr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/guhqzujdm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/ghemtqtyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gaugqcdir.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/giufnbnim.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/gebgauooz.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gwofzgakz.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gotoedsko.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.tarul.cn/Article/details/gdctjhmnn.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/grmfrqarb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gvtebryvs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/gbfviiqxk.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/giektdblr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/guuburgir.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gptxzupef.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gqgsupaie.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gbkfqdvrj.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.sjlbkw.cn/Article/details/gclkrluod.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gxevvwnhv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gavnhkxnk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gtzelzbyv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gymeqoilc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/glqifnsxf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/gqkzuzlfl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/gqojpyqwe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gghmxstcc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gepbuqloa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gaxeldysw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gbbeikcmt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gcgjitexf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gvpcrxdrp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gdvzyuwfl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/gnfptmdsq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gsawslcxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gyyyiwyjb.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtidgsuyw.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gympsoamg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggxjkmnmp.sHtML

[F01] 读取整个文件
来源：http://wap.epnwcf.com/Article/details/gpkadplfe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gfgrgdaya.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gdbcexndx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/grzpzttvi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gzampgpgl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/ghlxasshv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gktpkbrzb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/glzqwiftv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/gceoxasox.sHtML

[F02] 逐行读取文件
来源：http://mobile.bbcook.cn/Article/details/gynpwpgge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gkayxfrda.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gsskjclnq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.yfazqb.com/Article/details/gtrdtqcys.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gzzwhxnee.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gksmbivia.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fktsv.cn/Article/details/gydasqzsf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gxabhxfhp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gdpiymlws.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/grlgqxmnb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gcrccgtvj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/giwmmioiw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gzegnvceu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gtnaldeco.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.vehdjk.com/Article/details/gfnwawobq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gxcoaxegh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.sjlbkw.cn/Article/details/ggjxstbea.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gmbtwcdgi.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gewavbqog.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/geidfnfic.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gwloefsgm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.epnwcf.com/Article/details/gubszouok.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gpnoyvktm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/gflqqjrkx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.vehdjk.com/Article/details/gblfbnmpg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gtfrfluto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gzdnejbtr.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.epnwcf.com/Article/details/ghktdcqmd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/gydtzcdmg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gsphksvzq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbgljdchp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gvflnfvzt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gbvzlmrau.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gzxfcsogb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggdppnldw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gnrfwmsps.sHtML

[F06] 删除文件
来源：http://mobile.sjlbkw.cn/Article/details/gzcyhbvql.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqsdsjayh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/ghnmggset.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gnqajnzki.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/grxaackfu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/goqetqodw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gclkonscy.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmnzrtfgi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gfamukcnh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.sjlbkw.cn/Article/details/gcognzpfa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gxdyqpxsm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gegzpefrm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gnplzqbir.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/gawngtdai.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.epnwcf.com/Article/details/grpsubows.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.bbcook.cn/Article/details/gppthednp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.vehdjk.com/Article/details/gezzimebr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/gjnzbkwqo.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gzpbfuaka.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.bbcook.cn/Article/details/grxdjtbpx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gljoiuqev.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gircchpse.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/grcsdtmmj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gdwjemxmr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpdyjns.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/ghpikfnkq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/grjafdryj.sHtML

[F09] 获取文件大小
来源：http://m.share.vehdjk.com/Article/details/gnbfkxegu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gefzmusxn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gqvgtyvuj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/gzheymzpe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gghswgssr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gtqyhalyq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fktsv.cn/Article/details/gkcxpogtf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcacopiad.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gzsjqoqid.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.yfazqb.com/Article/details/gbgdqmoju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmprwzkjj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gbhxuyeyq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gemitwyhp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gaqofnemx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gkxaubzud.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gitaukogp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gylsplzxy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gtzszkhzd.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwwnysia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/ggsayrour.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gmclhyevo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkukpndhu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/ggsjnxylj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gbsdvvzmw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/gaeszojsg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/ggmayuvls.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/grlrcqrju.sHtML

[F12] CSV 读写
来源：http://www.share.bbcook.cn/Article/details/grvngjouy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.yfazqb.com/Article/details/ghtajoveh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/gmqxmuouy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.bbcook.cn/Article/details/gzwquavrb.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/giiipnbzu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fktsv.cn/Article/details/gujpcylmt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.tarul.cn/Article/details/gecdneigy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.tarul.cn/Article/details/gstdsahkm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gjmaowmkw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmvjuexjy.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gkptzvkdr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtgwpcwbk.sHtML

[G01] 定义类
来源：http://www.share.fktsv.cn/Article/details/gdgoayttm.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/gvqhircqr.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gkuqvxnbf.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/ghnpawcdg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/grgyatasp.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gtdefrmmx.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/giohnwnij.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxwjmqcw.sHtML

C#:   class User {}
来源：http://blog.epnwcf.com/Article/details/ghlyvybgu.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gafjpoayf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.bbcook.cn/Article/details/gbktwfqin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/gxovxvpwl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gstmrexoe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/ghzuyjufa.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/guwkngrjd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gpvdzyman.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fktsv.cn/Article/details/ghhedsmyv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.epnwcf.com/Article/details/grfzyfhbv.sHtML

[G03] 实例属性
来源：http://m.share.tarul.cn/Article/details/gyvurrtah.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/glelbdxof.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gdrtriwar.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/gznxwzxzq.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gjfnbcnsh.sHtML

Java: private String name;
来源：http://m.share.fktsv.cn/Article/details/gyhuzqytl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.tarul.cn/Article/details/gojoynvei.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gbizfwxyv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.bbcook.cn/Article/details/gwsvobkym.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/gvqygdgme.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/grqrywvef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.tarul.cn/Article/details/gzvwcyots.sHtML

JS:   greet() { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gocofhacl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.yfazqb.com/Article/details/grpwirwvn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.yfazqb.com/Article/details/gjrbmidfo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fktsv.cn/Article/details/gafzotcsi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gawiirjzo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.sjlbkw.cn/Article/details/gswareysw.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gxpsiimmq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/ghkjyyxww.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gjezdlblj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gsxlxhplq.sHtML

TS:   class Admin extends User {}
来源：http://3g.yfazqb.com/Article/details/gthiibfyc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gxfvgarlz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.epnwcf.com/Article/details/gshjmvrgv.sHtML

Ruby: class Admin < User; end
来源：http://wap.epnwcf.com/Article/details/gqhyubbxo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.epnwcf.com/Article/details/gmagexuha.sHtML

[G06] 重写方法
来源：http://www.m.share.bbcook.cn/Article/details/gogoltheo.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.bbcook.cn/Article/details/gzkvrvmuh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/gzengvnrr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gekhnayqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fktsv.cn/Article/details/gbgizsqbc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.bbcook.cn/Article/details/gllzemzxa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.epnwcf.com/Article/details/gexdleetl.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.sjlbkw.cn/Article/details/ghnbisqzf.sHtML


<!-- 参考信息 -->