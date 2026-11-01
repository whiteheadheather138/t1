代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/goygejkfl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gjtabrozu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gvixntufr.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gxytjdjro.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gdprrhjsi.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gvihwzydh.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gvokgcvqq.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gfqowoail.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gdoztyjsd.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gnhvozzod.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gildxwjah.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gmghvsbed.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gxkizlsvd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/grgukxycu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gbjhanahh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gzpsafljc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/glbclbjam.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gfqwcporj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gbfkejhdh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/gwzskrzck.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gwbnfmjct.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gaorvtgkq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gzrygcopu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gubpwuxil.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gjcqfpizv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gcabxftfo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gujyiclwg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gvqhorslp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gxnufufty.sHtML

[E11] 反转字符串
来源：http://wap.yfazqb.com/Article/details/gefwxgmbm.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gxaochqyr.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/glfpeokhf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gmzjarbrx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gthrkltlx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gdjjovlhh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gmagexvec.sHtML

Ruby: s.reverse
来源：http://m.share.yfazqb.com/Article/details/gdzchzpun.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/ggnektlue.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gydfsrtmb.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gdnmoxbkp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gmvyxqrfe.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gmdobevvr.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gjtrzkxfr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gwoevqrms.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/grvedqxrj.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gcqvsvdgm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gdpdbgghb.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gmvomreia.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gzfpirryl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gkzmvusoj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gmmbirhvi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gastfkmml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gfhynptpt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/gzargduxv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gaukrnwcw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gsoxsxtcy.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gzaztcxzm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/guixmjmdn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gjdmeuozg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gjarlcwoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/gmnmkbeec.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/gzayoccxs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/ggwmcuryc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gmatrpgfo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gvrmhlveb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/gmevltpns.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmardyfdj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gankiphee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gurmovale.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhiyajoy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gueblhwvj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gdjcuawio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gdddjqcgz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gfjbykvpg.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/ggzlywnsd.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.sjlbkw.cn/Article/details/gcdhnamkt.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhrbtfmu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gormrraft.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gscrjaiol.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gikfxoqmn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gqpnwqfyo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gqoxhpshw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/glmofklro.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gmonthqqu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gpqkfbjhx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gizjitgwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gqevxnlqx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/glnkgahds.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gygbzluyy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gitrbsazh.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gqmldqyth.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gezamhnip.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/ggwmgvmbv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gpxbovdte.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gpbjibcwy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gbddmcklr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/goqityrwq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gcwsuuoyt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fktsv.cn/Article/details/gdazljghv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/ganavvxqa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/guvpzhxer.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/geggvzflu.sHtML

Py:   s.splitlines()
来源：http://mobile.vehdjk.com/Article/details/gxnlqfuqm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmcvvfxle.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gjkprubxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gvyqambct.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/geramznus.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/glnjgtljn.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gflbrzgll.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gqatxnypm.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.bbcook.cn/Article/details/gpvexzpza.sHtML

Py:   if not s:
来源：http://3g.vehdjk.com/Article/details/glkafpxos.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gvnmismds.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gdxqyojrh.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gvryjshil.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/geouaqosz.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gansrvaam.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/gicmftall.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjwwlkyhu.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gihzmbiys.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gsgpcfsdw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/groskawhg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/guszpwzsn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gdrgpjtol.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gdqlrnwin.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/gvsehujcf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gjlstqrgr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gwluxkhln.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gauvbqswi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grrxeplmw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ggueiuakq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/ggdahghtq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/ghfmuwuxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gjsnsgnas.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gofvrusgv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gtdmkyvxl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gejxnjwlq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gctfwvvwu.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gmbtbebyf.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gygymdjoc.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gqaoprfgx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gbulieqio.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/glficptet.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.sjlbkw.cn/Article/details/gcrwpxbmp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gdtyqukms.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/glzsgbdmx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.sjlbkw.cn/Article/details/gvjbsuknm.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/guxczjcci.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gjmxfrmof.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/ghsefzgxc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gzxjmrxpw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.vehdjk.com/Article/details/gayhyvxya.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gyxvfmney.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gudtxafga.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gclmhhayp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gkdtzraaj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.tarul.cn/Article/details/gvxizlxys.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gxmyvnylm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fktsv.cn/Article/details/gdjfargnr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/gpfabxwvc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/goscdvnge.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/grgjjyciv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gwkecjvqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gjysanckx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gkgkwdnmq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/gqgkpffbg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gwokqljgz.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/gbjhwjgas.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gvgasggui.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gijexniuh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gdvomnxgj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gjgullibx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/giaccebna.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gennyehbm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/gmuxslafd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.vehdjk.com/Article/details/ghwrkvyty.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gvuvqzbfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fktsv.cn/Article/details/gwezjuvon.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gomsajvui.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gotafonye.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gskuypmyf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gmiwizare.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/guwkblwpz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gdtvyxqdj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvibjstbo.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gssbwryfo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gxhojzwdf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gffeqopjs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/ganopdaiq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/ghemlfqrs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gjyzntwsk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbajskqmn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcnvaxlwm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gufthhxlb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gwajaghez.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gwndzkgei.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gzxdqdthi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/gegzhsgbu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gnjhfbbrq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/ghcoyqcjv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.sjlbkw.cn/Article/details/gqvulgxux.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.tarul.cn/Article/details/gpyzuajhh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.yfazqb.com/Article/details/gcauanhpt.sHtML

[F08] 遍历目录
来源：http://www.share.sjlbkw.cn/Article/details/gvqcdrlab.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.vehdjk.com/Article/details/gnvczjesw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gnqdriyay.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gymupnrmx.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gtjozjfhu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gcykgnwic.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gsgrpxekb.sHtML

Ruby: Dir.children("dir")
来源：http://3g.yfazqb.com/Article/details/gplqmonlr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.tarul.cn/Article/details/gvhueaejf.sHtML

[F09] 获取文件大小
来源：http://3g.tarul.cn/Article/details/glyiueayz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gcmjtpdat.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqffhjckt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gltxtwjlp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gsgxyplim.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbithsiyt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/ggnirxfmx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gkusgozzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.bbcook.cn/Article/details/gnzngjjlp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/gmszlogtb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gzmwjoxrp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gatofixkc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gxhxbasij.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gfpixbhuq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/gjuargvhr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gottrgokt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghkoaplue.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwdsptszm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.bbcook.cn/Article/details/gatjbsgqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gpzmsrusg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gvfgpslsi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/ggwkotyml.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gsxqkuyjp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.bbcook.cn/Article/details/gyvdwaozi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gxgecuusg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gaxqhyhii.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.sjlbkw.cn/Article/details/gboqbevok.sHtML

[F12] CSV 读写
来源：http://read.share.sjlbkw.cn/Article/details/gghhkrgwt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gqxtdjmta.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.bbcook.cn/Article/details/gvfbkimml.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gwmqdhwpb.sHtML

TS:   // 同上
来源：http://read.share.tarul.cn/Article/details/gnapihtdk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gqgcnibdm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fktsv.cn/Article/details/gsemjmety.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gemdpfjiq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/grvahfzkl.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gslazugbi.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gthditvaq.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcrfwxoui.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/garfughxx.sHtML

Py:   class User: pass
来源：http://blog.fktsv.cn/Article/details/gmzmhcnsg.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/grlozotwk.sHtML

JS:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gquzumomr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.tarul.cn/Article/details/gwbtouizs.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gfgroubnx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.epnwcf.com/Article/details/gdnziuohx.sHtML

Ruby: class User; end
来源：http://m.share.yfazqb.com/Article/details/gcritrexw.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gmmvudyoi.sHtML

[G02] 构造函数
来源：http://www.share.sjlbkw.cn/Article/details/gakfckgil.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gjyutedmv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.epnwcf.com/Article/details/gjmdugvlp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.bbcook.cn/Article/details/gfewydtvp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.tarul.cn/Article/details/gtemiupww.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gzwsybgfq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.sjlbkw.cn/Article/details/gvlfylmvj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gilhrfheg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gacjlobej.sHtML

[G03] 实例属性
来源：http://baike.tarul.cn/Article/details/gweoaquoo.sHtML

Py:   self.name = "x"
来源：http://baike.vehdjk.com/Article/details/gdsbomyrd.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gudkmyrqq.sHtML

JS:   this.name = "x";
来源：http://3g.vehdjk.com/Article/details/gmsueweat.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gapitxdhh.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gnnabmzjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.vehdjk.com/Article/details/grixvuqxu.sHtML

Ruby: @name = "x"
来源：http://read.share.epnwcf.com/Article/details/gzxbocgdp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fktsv.cn/Article/details/gstfjhjub.sHtML

[G04] 定义方法
来源：http://m.share.vehdjk.com/Article/details/gsiuspbok.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gxggzkfhc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.vehdjk.com/Article/details/gskatwnkq.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.epnwcf.com/Article/details/ggxxkrvdn.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.yfazqb.com/Article/details/guuiildjl.sHtML

Java: String greet() { return name; }
来源：http://read.share.bbcook.cn/Article/details/gsayirtpp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/gdnqohyva.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/gnidksrck.sHtML

C#:   public string Greet() => Name;
来源：http://3g.tarul.cn/Article/details/gdqsasnzo.sHtML

[G05] 继承
来源：http://3g.epnwcf.com/Article/details/gzicokzdb.sHtML

Py:   class Admin(User): pass
来源：http://3g.bbcook.cn/Article/details/gvlqgmmgm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.bbcook.cn/Article/details/gbhebggxz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gtezynxjj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gtmzftoux.sHtML

Java: class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gmpxuolgp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.bbcook.cn/Article/details/gcdbajynt.sHtML

Ruby: class Admin < User; end
来源：http://3g.bbcook.cn/Article/details/gehucqkia.sHtML

C#:   class Admin : User {}
来源：http://www.share.epnwcf.com/Article/details/gandavuow.sHtML

[G06] 重写方法
来源：http://wap.fktsv.cn/Article/details/gjuntefnu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.vehdjk.com/Article/details/gryuxkphk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.bbcook.cn/Article/details/gknahzzec.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.vehdjk.com/Article/details/gucghmonb.sHtML


<!-- 参考信息 -->