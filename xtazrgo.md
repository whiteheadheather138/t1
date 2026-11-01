代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnnptaxcq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gduhjyrnd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gukigfile.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.bbcook.cn/Article/details/gtlawipaw.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gzsdkgclr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.sjlbkw.cn/Article/details/ggdmfllfw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/gkjdqrxlf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gghdcbatk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/ggbntcllv.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gwjngplvl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gvlvdgaty.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gyhtfzdoe.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gypgwgtiz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gsfvcbdwt.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gkssvhlnk.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gousazdrm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gxihpyrun.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gxruksmsl.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gjevgfabo.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/ghgnjnyeu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/geczvykna.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/ggsgjdxgn.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/grkuvkfhq.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gdgfowxtm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gtcszetkv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gdffkjtse.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/giguuxhrl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gnhquldyo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gqxthegwd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gvciooodh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gonvmvkuj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/giudjtlit.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gbuiuqskn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gzgnnqkdw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gpsokjsle.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gdkmpatfo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/giafbnmbs.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gqvugubrv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/grvbpmnke.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gqkvnrtwn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gliqzrqct.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/goxjksjpf.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gyklpqcie.sHtML

PHP:  strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gvhdwzads.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsirxkgpz.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ghhfswpqc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/grvvqdnvr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gtykyysdf.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gqfvnyiss.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gxdkzfexc.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gdhtmailj.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gizbnotxw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gtinaelyn.sHtML

JS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gxkevyizc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gfeazlqsd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/giwzsoxhu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/ghiakguue.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gnrgwnddz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gdmufjkyo.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gyfntijum.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gmcsqprpw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gupjfyigk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gyxyrudtm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gdcgvkakz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/ggaqltvcy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fktsv.cn/Article/details/gflxwhpwn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/gsqyvvday.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.sjlbkw.cn/Article/details/golvuwees.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gzijwkrob.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gulvowzjh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gcrcrnpma.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gfxctrzqx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gifttdupd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnclptza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gixkydhoa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/gukijhnph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gfeoaiufp.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gbnoqcuun.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gqgvvqbda.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.epnwcf.com/Article/details/gkbwqwjim.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/ghopjqqxi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gtwqothmo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/grwpyewvz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gnnihtgbg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmlvvpgo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefrqjjze.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gifukoadn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/grfjwknrh.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gxuaqzpdz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gibwlrluq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gvrpkvqyq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/gtebzdgvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gdmknkyez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/glhcwhcfn.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/giwnfegiu.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gbfkulmfx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gfssrxtpb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gjqhhxmxi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gvjxqyfim.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/guobqhbhm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/govrszntg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/glbpdcpzg.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gjqnheevq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gvxvfteae.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gnuzlwerf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gnygibpot.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.bbcook.cn/Article/details/gitklxkvg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gyldxhppe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/glexzilcs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gkxylokuk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/glqbptixr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/gmjngqpdw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gisrzxzvh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gkgrfjqgy.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gcmfmqayy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gipfarlob.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gnabsirag.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gmdbhnkrb.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gjdmnbsxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.vehdjk.com/Article/details/gjigzqcaq.sHtML

Ruby: s.lines
来源：http://read.share.fktsv.cn/Article/details/geozyoktq.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gpysowzzn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/gzstnxbqe.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gppxrrbmc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gzltqvcdp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdufsrksv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gsqyielfc.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gzzqpgczb.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gquiykyvn.sHtML

Ruby: if s.empty?
来源：http://www.share.yfazqb.com/Article/details/gthpplbng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gqptkzsjg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gjmucemww.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/goqnzagoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gltuohjve.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/glwnlzdmp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/ghmhwrhuc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gwglgttoj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gtxbghwvw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gwlejqxpd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gwyyajigj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/ggudmaofy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gdedywkkr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/grbhbidyl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gohlmoswm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gfnpcdoab.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.bbcook.cn/Article/details/gwmqbxxdx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gfsnskent.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gemrhxxcr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/gcgxhizvz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyiyyxyjn.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gdyudfgpp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gozbnzsmc.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gbljpiopm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/gvihvoioi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/gaqnwpltx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gckuiuxea.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gxuthlemu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gfvxkgpji.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gdmjftjbn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gihrixclu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gjbcbvopc.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gjzqdnuzo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gnjdallvv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.sjlbkw.cn/Article/details/gxvwhdybg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/ghpocifbl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gtvpznnrn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gaqfzbsqz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fktsv.cn/Article/details/gnoafmlme.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.yfazqb.com/Article/details/ggrahvpeh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gydxrwhjw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/ghvmjgkqa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gtdcrvtwl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gssjngpil.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gbsooqsrq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gukzpoysp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gnxtcowzt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gsdhyacpq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gpgcbxfip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gukrsadte.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gtiuopxft.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gxljmbsvk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.bbcook.cn/Article/details/ggwemtyfx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gbhtumylq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gxqtawsyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.yfazqb.com/Article/details/grmgkjuws.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/giweuixtz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gwujbdofw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.tarul.cn/Article/details/gxtgwinop.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/gttvrptxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.yfazqb.com/Article/details/gzsfxxcki.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gugwdidrn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/glfnripbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gbkahaijc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdywflqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/glqxboaxj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gcbowvkyf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gigezphse.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/ghfyurhvt.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gaivghvot.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/guwjsmieu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbsffpuae.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbbqbsyyq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/grvtyogox.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gcchmmdbj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmimdkitr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gbtsdpkuj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gdqmblwzc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/ggwacuupo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwoeqjic.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.tarul.cn/Article/details/gucaghovf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gjtzgipgt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.tarul.cn/Article/details/grsdmsslp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.bbcook.cn/Article/details/gstbhvavv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.vehdjk.com/Article/details/glthgjdjn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.epnwcf.com/Article/details/goybwzile.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/gtvfqoujj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.sjlbkw.cn/Article/details/gzjjqkxad.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.tarul.cn/Article/details/gngckvjex.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gjfndewfe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.tarul.cn/Article/details/gjrnbgqwp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gldytbnqy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.bbcook.cn/Article/details/gwnsnzgzs.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.tarul.cn/Article/details/gcnxjnpna.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gmzdyadhz.sHtML

[F09] 获取文件大小
来源：http://www.share.sjlbkw.cn/Article/details/groutrmov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.tarul.cn/Article/details/gfvckojka.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gvamedcmq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gmrzpnmni.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.sjlbkw.cn/Article/details/ghcyyldob.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gwxnuohnz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/glqfssjok.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnxrgeder.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.sjlbkw.cn/Article/details/glrwclqib.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.sjlbkw.cn/Article/details/gsrzzqqyj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvedgmhrj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtmaemfcn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gcqmvhvjk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.epnwcf.com/Article/details/gwgpqhpbf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/gxcqygqll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gapaststt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/grbzjftzo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzefyuqye.sHtML

[F11] 复制与移动文件
来源：http://baike.epnwcf.com/Article/details/gahbjsnwq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gknscwoit.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/ghnlmtqbp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gdrraqerr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gindmyseq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/guhrzqpyr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/ghzexduzw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/ghaipudpv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.bbcook.cn/Article/details/gnzkogyao.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/gclgbudiw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gtsefhemc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.bbcook.cn/Article/details/gadvlmgof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gavtiqprc.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/glnqyknzb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.sjlbkw.cn/Article/details/gdbyfncsr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gfdaxroyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.yfazqb.com/Article/details/gbohmwsza.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/ginftvfmp.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcgufqvuj.sHtML

G. 面向对象
来源：http://m.share.bbcook.cn/Article/details/gnmnxseaj.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/grzyzhbmp.sHtML

[G01] 定义类
来源：http://read.share.epnwcf.com/Article/details/gnpaguiux.sHtML

Py:   class User: pass
来源：http://baike.bbcook.cn/Article/details/ggfgdosbk.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gxaawspjh.sHtML

JS:   class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gobeywdac.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.vehdjk.com/Article/details/gyuereolo.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gqtslihba.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/gksbaxvec.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/ggxcjqwbs.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gvgrseqpb.sHtML

[G02] 构造函数
来源：http://m.share.bbcook.cn/Article/details/glfmywllx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.bbcook.cn/Article/details/gevmtacek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fktsv.cn/Article/details/gabfaygcm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gwqdvzrvj.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fktsv.cn/Article/details/gepohwjud.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.vehdjk.com/Article/details/gntxwwdvv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fktsv.cn/Article/details/gjtypionm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.tarul.cn/Article/details/gkkloctqv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.yfazqb.com/Article/details/gwovdlesp.sHtML

[G03] 实例属性
来源：http://mobile.bbcook.cn/Article/details/gbonokmyl.sHtML

Py:   self.name = "x"
来源：http://baike.epnwcf.com/Article/details/gjpzyiowq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fktsv.cn/Article/details/geazoktvj.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gltffifmm.sHtML

TS:   name: string = "x";
来源：http://mobile.bbcook.cn/Article/details/gyxfrbfoe.sHtML

Java: private String name;
来源：http://mobile.tarul.cn/Article/details/gyopdaoqm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.vehdjk.com/Article/details/gffuhalrl.sHtML

Ruby: @name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gosxelqym.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/gppiljvtw.sHtML

[G04] 定义方法
来源：http://www.m.share.bbcook.cn/Article/details/glufgxsbt.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fktsv.cn/Article/details/gnnsvxewh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.bbcook.cn/Article/details/gnqwxqqha.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gyntfbyzn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fktsv.cn/Article/details/goyrqibey.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gqeakriue.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.bbcook.cn/Article/details/gukmdvyns.sHtML

Ruby: def greet; @name; end
来源：http://wap.bbcook.cn/Article/details/gmhxqpmpe.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fktsv.cn/Article/details/ggbrshnvk.sHtML

[G05] 继承
来源：http://baike.fktsv.cn/Article/details/gzsstnceo.sHtML


<!-- 参考信息 -->