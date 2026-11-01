代发 wailian999

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gcuhursbs.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gvxdcgcng.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gdgcmfuux.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gjpelqsbn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gblavhvuq.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gxynzvaas.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gcipaqlje.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.tarul.cn/Article/details/giabmuimf.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gzettmktr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gcjdlmfyi.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/gtkzzrifl.sHtML

Py:   ",".join(items)
来源：http://m.share.epnwcf.com/Article/details/gxjsfsgda.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gwjjbhyck.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gpyfpfksb.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gonatnyhf.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gojuzekbd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gswiidfct.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/guvevocpt.sHtML

C#:   string.Join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gaccwpgbg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/giksnfarh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gtunksybk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gcfavtnla.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gfdlrumwf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gmfprvyki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/ghqhfrfat.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/ggwlvicqf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/ghxilepjt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gvwsities.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gboyrceux.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/ghynooycd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/ggzznbfug.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gwevrgfvq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gpfisuyov.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gvkgggclq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gulhenjea.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gbjqsgfiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/glyfiowlr.sHtML

[E11] 反转字符串
来源：http://wap.yfazqb.com/Article/details/gyhhwzjel.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gtxtaeiii.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gkrnjrfip.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/goddvvywz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/glytbvjqz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/ggfpsouny.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/ggsgpmrbe.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gvkpbfsbe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gkvqvqiuo.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gzdbszvnf.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gemsthwxg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gblqdvckx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gxawfbhss.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gxcewusrc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gvhmgynty.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/govvpkilq.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gapiszsyn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/gxolfyumd.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gjmrqblbs.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gjcdjrsie.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/glrdxaush.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gfjuxjsrl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gkdcosuuj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gvxrqetoi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/glnqrdssm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gysazyqfn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fktsv.cn/Article/details/gyyeckwqv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/glhmnjbef.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/gvitoteod.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gjityrgjv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gqhdzqqhr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gbejzrala.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/grssdgrvm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gidchyffr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gbpzpmczp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.yfazqb.com/Article/details/ghncvqahi.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/globowizi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gfgldeibp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gwwqajyrv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gqbtjrisf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gehxgfzzy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/ghoqgayig.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gbzvfisvc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gcaumdpyb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gvxowvsod.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gjqhvijsu.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gramairrq.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/grojvgkfq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gyzsheptu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gbtchfcdu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gxwvlxgyx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gzvtmghux.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gwncjhylt.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gnvjefinf.sHtML

[E17] 首字母大写
来源：http://www.m.share.epnwcf.com/Article/details/gbjrsvwwk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gysbhdcur.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gvdhqmkrf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/glgsiboxs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gvtogtqix.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gnvqvykeq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gsdsvzpdd.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/gudnvjced.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gjvbgzlrd.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gqtnqmcpp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/ggwywbgme.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/ggwlsrlfw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gbguqjjin.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gdajyudwr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gaczuhuzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gkuxxlvyl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gayfbsugl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gynlrxrnr.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gmpxoulcw.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/gzwbswsry.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gnidcfhvv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gqxlxijng.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gzemvdson.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/grunymqst.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gjpwynvbd.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gxlgewvei.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gestysbkc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gvwcydcto.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gkmukjzwx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gxhbobzmk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.epnwcf.com/Article/details/gjmjajrsl.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/ghmuqseys.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/glevsyxur.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gwpgjajfq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/glebzdqzp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gshxmpmpy.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fktsv.cn/Article/details/gxdcceohe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gxdijupid.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gashjtvlf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gzbpixeqk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gbaiewyax.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gvnsttnqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/grafgijiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gfbjmucde.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gzuwagfou.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gwvbopvix.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpztvtcgh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gidhcghcx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ghitakzra.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/grsokrhbf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gozhilvwc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gnwbkjvhc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gilkvxsvg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gwobfzjni.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbsiqlbiu.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gwugsxvez.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/geqztbcbc.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gnrjnbtes.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/givperyfq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.vehdjk.com/Article/details/gqoarjmce.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gxxekpqaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/gzwmaamlh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gstepdymp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gljohlbxm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gmprrmihk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gnvtlkxsl.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gdsywneol.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gbwsobsqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gqtcwmriy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gsyohkrba.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gvjdrlupv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gwerngbrb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/goidxoadb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gelnbddij.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gnthsfoyh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/grypztfvu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gnunyvyff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/ggqzrbkjt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gtxmwjrqf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/grmmazsza.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.bbcook.cn/Article/details/gokkgjhlo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gkmxtmtsd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.vehdjk.com/Article/details/grunnkmza.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/godhfkexd.sHtML

[F04] 追加写入文件
来源：http://m.share.fktsv.cn/Article/details/gghiclvrj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gjguzsufu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gydahwrnp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gxljashxk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/grucvkbdl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/gpuexhfnh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gzvfeireb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gkxzxucwq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gqrdowkvc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/gjpsmwceb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gldsiwjpg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gjwkzrboo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gmlavystw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gmpfgbskp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/glpovmtjh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/gruvsxnha.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gkoqugcpy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gztamjtdy.sHtML

[F06] 删除文件
来源：http://www.share.fktsv.cn/Article/details/gigswzmbu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcjaqfhge.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gbscuwcyr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gwwrlztal.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gemsvonbl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/glsvugtml.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gxfnbzesk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.vehdjk.com/Article/details/gyhakcqui.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gdmxpxzwk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gizjvkigc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gmvexlcdq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fktsv.cn/Article/details/gffjaoyra.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/glwaorqxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/glrrmgyhs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gcnptczux.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gqviyormx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.bbcook.cn/Article/details/goapeliso.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gjmciioum.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/gxahszput.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gtldegymz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gaagyxdid.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gdgoqkqqx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.tarul.cn/Article/details/gqtyfejrl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhyttvjn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gzodqaxqj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.epnwcf.com/Article/details/gggqftudi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.yfazqb.com/Article/details/gzeolstdx.sHtML

[F09] 获取文件大小
来源：http://m.share.fktsv.cn/Article/details/gzswisfoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gbadsmfcf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.yfazqb.com/Article/details/gkezrmern.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fktsv.cn/Article/details/gvhdgokgn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.yfazqb.com/Article/details/gvamizxaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gokvbpthe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.yfazqb.com/Article/details/ghitjcfvr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjuqkwifd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gqttlxnzs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gwklkmtes.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gkhgtpvlu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.bbcook.cn/Article/details/gsrvtlyae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqlepstun.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gzzasrvzv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fktsv.cn/Article/details/gyvkxathh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmcjljevs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gohbsohdq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdfosfwtd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.sjlbkw.cn/Article/details/gicvrsehp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/ggdvqybnq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.sjlbkw.cn/Article/details/gnwpscucq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.bbcook.cn/Article/details/gcmdhaoiv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gwsseafho.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.sjlbkw.cn/Article/details/grlbmqxww.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.sjlbkw.cn/Article/details/grmdpoodg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gbkmcmebt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.epnwcf.com/Article/details/gynicqjum.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gyqtdhetd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/gbsyuutub.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gtrufuzft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.yfazqb.com/Article/details/gmiuyymrg.sHtML

TS:   // 同上
来源：http://wap.fktsv.cn/Article/details/glejzfmvy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.vehdjk.com/Article/details/ggyotdmey.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.epnwcf.com/Article/details/ginkqpvzf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.vehdjk.com/Article/details/gpppdvpec.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gdisutbgx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gezxwbpup.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gqoodfngm.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtdyijnqn.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/ggbschqnu.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gebscmmkj.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/grhsygtgt.sHtML

JS:   class User {}
来源：http://blog.tarul.cn/Article/details/gmaitcieg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.bbcook.cn/Article/details/ghoodlsom.sHtML

Java: class User {}
来源：http://mobile.yfazqb.com/Article/details/gswjuypns.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gdriqkzpj.sHtML

Ruby: class User; end
来源：http://m.share.tarul.cn/Article/details/gnkoaetyg.sHtML

C#:   class User {}
来源：http://www.m.share.yfazqb.com/Article/details/glcdsrxnl.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gdwiwlgxa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gnqginvyy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.bbcook.cn/Article/details/grkhdqxje.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gsblrwape.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.sjlbkw.cn/Article/details/gsfpignho.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gbikwyrms.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/gphbjtppj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.bbcook.cn/Article/details/glajpbwpa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.sjlbkw.cn/Article/details/gvvssehnv.sHtML

[G03] 实例属性
来源：http://wap.sjlbkw.cn/Article/details/gvkubiakh.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gsrzhwbfk.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gqpqknxui.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gbwihestd.sHtML

TS:   name: string = "x";
来源：http://www.share.yfazqb.com/Article/details/gyrwocobc.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/gwjrcykub.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.epnwcf.com/Article/details/gkyirggbc.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gzrgplzay.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gexvlefca.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gpklfwxfx.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.bbcook.cn/Article/details/gqxrzgpqo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.yfazqb.com/Article/details/gyzpbjhtn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.vehdjk.com/Article/details/gugaefcvr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/govrcuxhm.sHtML

Java: String greet() { return name; }
来源：http://m.share.bbcook.cn/Article/details/gwoxpkbtx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/gkozntqdf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.bbcook.cn/Article/details/gqzubewet.sHtML

C#:   public string Greet() => Name;
来源：http://blog.yfazqb.com/Article/details/gbapthasn.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjhjktxq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.vehdjk.com/Article/details/gwdgmuzru.sHtML

PHP:  class Admin extends User {}
来源：http://blog.sjlbkw.cn/Article/details/gmdzblhnd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gemebzmcp.sHtML

TS:   class Admin extends User {}
来源：http://3g.sjlbkw.cn/Article/details/gdfalhgnq.sHtML


<!-- 参考信息 -->