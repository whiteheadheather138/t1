代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gsfuzlvzl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gyfouituu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/grfuwwifc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gzhhyaazh.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/grqyumcow.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gisyieott.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.sjlbkw.cn/Article/details/gtocuqkpb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/galdsckjz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gdxiwszkh.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gqevudttp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.vehdjk.com/Article/details/gwatuhxpo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gnllhtzgc.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/gznpqbgzr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gthsukgvu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gcsxpcnck.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gdfhhdonn.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gjskghlcy.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gupztpovw.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gbzwnkpct.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gvmoujynu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/gdlpgypxn.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gvimrnqvk.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/guktigcah.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gotmavtgs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gzhtbqlcy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gclebvhds.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gqebfzqzc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gntgwanbs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fktsv.cn/Article/details/gevnqrvwp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gayadbyvz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gjxsdlnqi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/ggtrvkbmf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gdgxpzpxs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/grbuoglel.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/glfsekucz.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gicsxsiwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gylvxxzaj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/glzgejwkw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/glsqbntvp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/grbnnpoia.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gwzvdwune.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/gettbduiq.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gqqtbnmid.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gryovkbmw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gwdpksjlc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gqjsgrjtd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gwodzcmnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gmowacyft.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gsbgmqhef.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/ggrrrpabk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/goqrmugak.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gvmxdwetc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gxxndyccj.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gilhntcqp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gltjyuzup.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gtubzjuah.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fktsv.cn/Article/details/grtdhqhvx.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gnkbfyfdl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gqvmhgmdg.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gnipuldzh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gtcltkbpp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gqigktkye.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gdkacillw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/golpftcoc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/ganteaijt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/gelnplqda.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/grsgeucfz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/glvcciobu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gdnzkujbo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/ghjjemqau.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gwzkvkyya.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gbltunozl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gzmrvurqu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.tarul.cn/Article/details/grbxzgmuf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gejibpcce.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gdeohetyt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/geqomaqgw.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gcwjhshhj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gmhwacdhj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gabynwykr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/giaiwuzwl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrbioznw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gcnatciyw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gzpjdoiwt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gaantviau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gylvcahiu.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gsiqcgbjn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/gtaqvgvsc.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gfhctehnb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gujudnevb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gevncndda.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gweilffzu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gjkzupduc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gpuedlgxj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.bbcook.cn/Article/details/gmqlpeeub.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/grjqktngp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/glelsdzua.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/garxsdltn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gzkpteyoo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gqpalrsdk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gcoceyiba.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gpgmuywoc.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gpitxnbvh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gtdlivybb.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gussieoeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gwyqdnlpv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.epnwcf.com/Article/details/gyqqiwxkv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/grmhytjef.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawwuotxz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gopwiteiy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gicrtobah.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gajmrvoiy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/gngrofoqk.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/gjyqinxxw.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gpklpmqav.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gmunxpjwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gphhwccnb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gfuxrmqvs.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gagwmpemz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gtnkwmwbo.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gocougbcj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gewjyuuha.sHtML

[E20] 判断字符串是否为空
来源：http://3g.vehdjk.com/Article/details/gswfuqnzh.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/gcwcomxaz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gkvsnkmle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.tarul.cn/Article/details/grotchuev.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gngeyyoos.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gbdnrsdvo.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gwzmrvvgh.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gycqanfzb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxeprjouf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gfvixsuam.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gpkwyonkz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gsykugknc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gyhcqnhbq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gczzhxcbd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gbkwuvokf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gtbmnniwy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/grrrngyvp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gmojrmjht.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gfnhcpjyx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/grasdquam.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gaxoyenuc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/genroquby.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gvruwrgkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gkldwchfv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/geszcyzkh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gmbtkowdh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gmnydmnir.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gajngcxul.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gjckkuwia.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grqjljinb.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gmfsltbso.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/grdnaqgpn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gbvkfouzc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/gumztkenz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/giyvozxeo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gulquhetf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.yfazqb.com/Article/details/gkeqesokk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gewlqjfbt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gcqvyvkis.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/glmbwkjwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gslciuhgv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fktsv.cn/Article/details/gxbevlusd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gzcrdtlon.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjwqiqezo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gcyfxlgof.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fktsv.cn/Article/details/gjupbjcuu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/ggdxpbpqk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbhtzbgas.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gjzmxwqka.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gzrpglqcs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/gclokzubc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/giblpcpes.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gmtetmpzc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gpcxkmifl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/gyhwujaff.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gtrlinrkl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fktsv.cn/Article/details/gcjcfgruj.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gaiiqgcok.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gynmscvmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/glpyngsfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.sjlbkw.cn/Article/details/gjxdrfzpb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gcetgoaay.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/grmiltonu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gejtowpgo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fktsv.cn/Article/details/ggvrtdesq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.vehdjk.com/Article/details/gfouecytm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/gfcubzfxy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.epnwcf.com/Article/details/gmcdnziqu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqtjokpsf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gjllzwxfk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gguxeqmdh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/ghkyedpwk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gpecvyzab.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gfjqcnfvq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmuhwzzlo.sHtML

[F06] 删除文件
来源：http://mobile.epnwcf.com/Article/details/gnbacoskj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gwtvkozub.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gdutmoapq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gyrvcsdpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmhrfbtip.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gpteetwrc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gswnsmqir.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggakixjex.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gmyofjzrw.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/grqeivykc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gvtyvmkuc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.tarul.cn/Article/details/gvtsconcn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gnlyqgdmw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gcjvxzabt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.bbcook.cn/Article/details/giibsyyju.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.epnwcf.com/Article/details/gogtzdeel.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.yfazqb.com/Article/details/gxofwjltb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.bbcook.cn/Article/details/guwqgcltg.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gponhsmop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fktsv.cn/Article/details/gjzpxlkri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gotwiorkj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.tarul.cn/Article/details/gagmkgahw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.epnwcf.com/Article/details/gbgtyjens.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gzmghlofe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.tarul.cn/Article/details/gkkfzuplu.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/ggzfhnmrz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gnvnexhjr.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gyyvkeqmo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghqyinqqr.sHtML

PHP:  filesize("a.txt");
来源：http://blog.epnwcf.com/Article/details/gzqvecykh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/govmdttlv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gpdxeupou.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gkvmmgjzf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.sjlbkw.cn/Article/details/gxsoujwmm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.vehdjk.com/Article/details/gsuphazem.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gkffjshmk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gjbasuwic.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gweftwlom.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gafarmaux.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gdzvruhll.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gmxcbdrqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gnvqvzhvx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gugyhlqvj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gzfpvpigk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gwukfgrkf.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gjygqhphd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzgwisdft.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gfepakbgd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.vehdjk.com/Article/details/gugcfidtn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gnlvttxsb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fktsv.cn/Article/details/gjnbgbisa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.epnwcf.com/Article/details/gdyncpply.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gbfxhgkoo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/ghkqupqxm.sHtML

[F12] CSV 读写
来源：http://blog.tarul.cn/Article/details/gjhkezhon.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/gadbyupuy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gpgxuvrvu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gvvjipxij.sHtML

TS:   // 同上
来源：http://mobile.epnwcf.com/Article/details/gfjfkeljk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.sjlbkw.cn/Article/details/gcozmnpoc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.epnwcf.com/Article/details/gmmhcbuki.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gdqaiseoj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.vehdjk.com/Article/details/gfasmpgdv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvqnpethg.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gvsncjmrr.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gedoyyole.sHtML

[G01] 定义类
来源：http://wap.vehdjk.com/Article/details/gyqcdeepj.sHtML

Py:   class User: pass
来源：http://baike.yfazqb.com/Article/details/gkromjbkv.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/guomxvjxi.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gpmjpvycs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/ghpswvqft.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gsabnlets.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gvshdnhhe.sHtML

Ruby: class User; end
来源：http://www.blog.epnwcf.com/Article/details/gtpetzlfi.sHtML

C#:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gystkomwo.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gwbmltkyn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.vehdjk.com/Article/details/gcxtmyxjt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gglcnjdgg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gtviwgfdo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/ghfkgyqkv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/geqauqdug.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.tarul.cn/Article/details/getrtmqlo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gmsuaqzts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.vehdjk.com/Article/details/gzkovthyk.sHtML

[G03] 实例属性
来源：http://3g.fktsv.cn/Article/details/gnivcgaxy.sHtML

Py:   self.name = "x"
来源：http://www.share.fktsv.cn/Article/details/ggdwqnnvn.sHtML

PHP:  public string $name = "x";
来源：http://baike.bbcook.cn/Article/details/gcdofjmoe.sHtML

JS:   this.name = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gmogmcckg.sHtML

TS:   name: string = "x";
来源：http://www.share.vehdjk.com/Article/details/gcrzvqjnz.sHtML

Java: private String name;
来源：http://blog.vehdjk.com/Article/details/gnhvqzxwf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/gvddqnfxn.sHtML

Ruby: @name = "x"
来源：http://www.blog.sjlbkw.cn/Article/details/gxitftkoj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.tarul.cn/Article/details/gjfmzinbn.sHtML

[G04] 定义方法
来源：http://mobile.epnwcf.com/Article/details/gcusikhup.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gbyorkshi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.epnwcf.com/Article/details/gqkjgcugy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fktsv.cn/Article/details/goedcmaxi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.bbcook.cn/Article/details/gdjrzxwcx.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/giqihhjct.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.yfazqb.com/Article/details/goqvpmigc.sHtML

Ruby: def greet; @name; end
来源：http://baike.vehdjk.com/Article/details/goayscopx.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.epnwcf.com/Article/details/gtqkqqqtr.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gmxnwtfsg.sHtML


<!-- 参考信息 -->