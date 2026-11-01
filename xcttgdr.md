代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/ghumgzqyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/grkjssepg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gdwmrqtzj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/grvmglanh.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gwzmiocty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gpvojqaaf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gscbmocdd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gcxyacqjc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/glqniyzkw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggcpxwcew.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gdljxjxon.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gesjkokoz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gehqnjbpa.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gewlzxzjl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/ghhyfoagi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/guclegyii.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gxiiluqea.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gsmomfuyz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gwtdavdjr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/glpvrsjre.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.yfazqb.com/Article/details/geoltrlmq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/gdmhzzaby.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/godttmnto.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gmaxpokuf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gizycvrrh.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gbeznkoqw.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gksvnmtyd.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gynoziljw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gviyukhjv.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gqzkjolpj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gvchuknzz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gwhxrqyeu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gvhwgmohy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.yfazqb.com/Article/details/gqohhxbfe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gbbacvdlk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gtxusbagf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gulodhkxj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.vehdjk.com/Article/details/gsonzdymi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gdvidegyu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/ggomllemo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gcwhgaomw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/grkcddkca.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gvchktsbt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gppytotie.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gmeshjmti.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gakpbnmdx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/guvmborrk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/ggthldmpb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gexszxljc.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/gyydepkpr.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gxdcggmhv.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gmqitzmvq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gzpriogfy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gqrjwqhmc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gktuluhpe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/gfnhxjhan.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gqvwwkozl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/ggkmatino.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gxhblaiuu.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gnqzlkatc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/ggtqznchm.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gaycyksve.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gejbunaff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gjkocpopn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gwypopxcn.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gegbzcmaq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.epnwcf.com/Article/details/gvtmonzpy.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnxyrpba.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/guspznjim.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gkwlvtfgs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/giqfslomb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gwjzggckf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gzystjeio.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gwjoapafj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.bbcook.cn/Article/details/gomrwnpor.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.tarul.cn/Article/details/gelhsgyct.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gqswzukmr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/gtorlcgss.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtlboptnl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gboisskvd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdqyswfxw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/guqeakbtz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/goacvssgq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gmebobhvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gdoccpumx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/ghhvjntmr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/gdgwntqbv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/gjwvnnkdq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjvefcrvb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gvflbfcir.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gspkedida.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gwigqfpsh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fktsv.cn/Article/details/gfuczhtwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gwbgysnwl.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gxgxomrgz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/glyslfzlq.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gplnswwym.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gfzzoijbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gobgyjtdg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.sjlbkw.cn/Article/details/gxebownul.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/glhkstxbm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gcvlugwqo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gaephcpjw.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gjizcaqmd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gqsardujv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gnqxdffhx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gzctdrlvz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gxzlzznsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gnlfbpljz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/ggguulccs.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gjwbzdbod.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gifpbeilm.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/gfqepgdds.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gsrndnrrb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gfevktegv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gdwidtkuk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gvcicvtph.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gddcosxta.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gqaafdpyz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gssixqnho.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/gvdpdlfyv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gpyyrlekf.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gkiilcrou.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/gzntuqjnh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gjbaepula.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/glsknqxmm.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/glzxsksue.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.epnwcf.com/Article/details/gaefwejll.sHtML

Ruby: s.lines
来源：http://wap.fktsv.cn/Article/details/gcndbjelh.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/ghiqqazyx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gnegkqgmq.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gabbahexh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/glwzhcnou.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gdbrszpye.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/ghsqkepaz.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gcfmgcedh.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gmnczexpn.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gwsyuages.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/ggfstbpix.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gkardhzml.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gzvuorzah.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gdffasmim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/ggrmmaqxu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gyucdqlkp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gdkzyengb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/garlihrqc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gesxjhwwf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gzlvtceld.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/gnyoyukbs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gmhpjpdhh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gvcvobdnf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gavdajxln.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gogojruxa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gnzgwdxim.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.epnwcf.com/Article/details/gohrzbdkm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfyfgrhe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/gyqcncuzm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggvkazovh.sHtML

F. 文件与目录
来源：http://blog.bbcook.cn/Article/details/gtrciwpxg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gjvbeyopk.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gjvljlrto.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gomhuoryx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gmmfzzczf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gslakmpho.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gyjbgilwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gnyopuqik.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gtsthipqy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gpvxxvpmj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.tarul.cn/Article/details/gygfpkenk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.tarul.cn/Article/details/gixxppdwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.bbcook.cn/Article/details/gqzavjogh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/ggwyrzknt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gsmtkybpr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gzcvlrttz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gcyewztaq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/gkvfbzxnm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gqxuyupuu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/gsjxgncuw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.epnwcf.com/Article/details/gquslkubb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/glapbsled.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gltnrrnbl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gwbakpbhw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gzuezmeox.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gymvczaji.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gtcqlnrdw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gulbjecyz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gjmvjhorc.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/gliyusjpu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gicepwjpd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gsistqgqv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gwozppnpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gndubwixy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gvnwrcmcj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/ggzqujeax.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gbhsurgtw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/gnxkxwukr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/guycrqpvf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.yfazqb.com/Article/details/gikogjksv.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.epnwcf.com/Article/details/geazkvkge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gscovionv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gijhphjsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/guypcgyxq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gimocarrn.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcthlclij.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gqevutdqp.sHtML

[F06] 删除文件
来源：http://read.share.sjlbkw.cn/Article/details/grnbjskjr.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gifthjudt.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/guoierpgn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/golnrqwov.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/guzixbwdn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gtmuxnlhk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/girkvswvn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gbnxnfnjd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdykgxyqm.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.epnwcf.com/Article/details/gkuqqysoh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gbnrgghdp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.vehdjk.com/Article/details/gjdgkwwme.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmfhtmeq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gbxcjeuqf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gkajsuydz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.tarul.cn/Article/details/gngmqmqlf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/goxkososm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.bbcook.cn/Article/details/gsfpkxpcf.sHtML

[F08] 遍历目录
来源：http://www.share.bbcook.cn/Article/details/grbjzmyez.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gfpbdvmsm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gnjtonwme.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gyyyoftqh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/gezkbhbwl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgmlahbg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gkycpigaw.sHtML

Ruby: Dir.children("dir")
来源：http://baike.bbcook.cn/Article/details/gplhlkfsq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.epnwcf.com/Article/details/gpgorqkrx.sHtML

[F09] 获取文件大小
来源：http://wap.fktsv.cn/Article/details/gnxxkzaaz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghsedfuoi.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gjsawqqtr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gdvymxavc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gmqkyorbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gylrelghu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.sjlbkw.cn/Article/details/gwurcwmrq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxdbhgwlw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.yfazqb.com/Article/details/gtvjojevi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.yfazqb.com/Article/details/gvvuopwqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gexmgixzu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gflmotngp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/geyvukcer.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gosovafpe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gersehqtb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/gkhwuydrl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/govpqevdy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/giufjyemy.sHtML

[F11] 复制与移动文件
来源：http://m.share.vehdjk.com/Article/details/gygmffdnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.tarul.cn/Article/details/gtuhcevmy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/grzxgzxug.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gbuoglvtl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.vehdjk.com/Article/details/grykbctcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.vehdjk.com/Article/details/gvpbwhlbt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gjfoymave.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gozzpmcxx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/gslryehod.sHtML

[F12] CSV 读写
来源：http://www.share.tarul.cn/Article/details/gifafkjpe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.tarul.cn/Article/details/gvawdloih.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/gudznlbbj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/gugdnljen.sHtML

TS:   // 同上
来源：http://www.blog.vehdjk.com/Article/details/gvqthwsur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.vehdjk.com/Article/details/gaodvvkay.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.vehdjk.com/Article/details/goudyukpo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.vehdjk.com/Article/details/gznnrnumd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.tarul.cn/Article/details/gllyrqbfy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gstlabnoo.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/ghiknbusb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbzxornnp.sHtML

[G01] 定义类
来源：http://www.m.share.bbcook.cn/Article/details/gyagoczky.sHtML

Py:   class User: pass
来源：http://3g.yfazqb.com/Article/details/gpwnszwpc.sHtML

PHP:  class User {}
来源：http://baike.vehdjk.com/Article/details/grksapxgb.sHtML

JS:   class User {}
来源：http://blog.vehdjk.com/Article/details/gnqczjgxe.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/gunndipoc.sHtML

Java: class User {}
来源：http://www.blog.yfazqb.com/Article/details/gfjawskyn.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gpjwkqewm.sHtML

Ruby: class User; end
来源：http://baike.epnwcf.com/Article/details/gxyqewvbi.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gekmkvytk.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gihxvhuga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/grjcamxei.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gemirezxy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gjzepyuxo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.tarul.cn/Article/details/gsbfqsngm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gjpettfwo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.vehdjk.com/Article/details/gzcauawxm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gswywqgic.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gmldcjuta.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gcvaiznlv.sHtML

Py:   self.name = "x"
来源：http://read.share.tarul.cn/Article/details/glsypgfos.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/goqpowlob.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/geeeaicgo.sHtML

TS:   name: string = "x";
来源：http://mobile.vehdjk.com/Article/details/gwjwyavav.sHtML

Java: private String name;
来源：http://read.share.bbcook.cn/Article/details/ghwlhaxez.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gnglgnvug.sHtML

Ruby: @name = "x"
来源：http://3g.yfazqb.com/Article/details/gjztfiwdc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.yfazqb.com/Article/details/gpmdkdhcn.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gurazeveg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gdyjmxvty.sHtML


<!-- 参考信息 -->