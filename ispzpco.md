代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gxmhibwjx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gnobbwcjk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.tarul.cn/Article/details/gfdrjroxv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gbrruyrrp.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gmjfpiwma.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gjhrnjvzn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gulvobfzj.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/glmasormj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gmtntogtf.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gammsmmtc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gjvmhdlop.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gzlsfinrl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gmhldyaru.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gfnwsdbbt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/gvsyolnzu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/ggozxoczj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gajpwwznr.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/gsglbfzer.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gsyebgzfz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhlkqxyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gogrpulky.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gllkjbgnq.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gkjohislp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gilcjzork.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/ggkpkyqop.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gykxkvfha.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gamnlegvu.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gltuexeal.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gqbahlxwo.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gqaartsus.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gcopvpqwc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gcrbknanh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ggputoxsv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gilcnsilx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.bbcook.cn/Article/details/giombqbbj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gwjfpuxjz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gykstuazy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gmkifiqma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gemtuulhz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gsksvrora.sHtML

[E06] 替换子串
来源：http://www.share.sjlbkw.cn/Article/details/gxhwwqpbh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gnycvcgzy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gusccybbu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gaysepudo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gslavhvon.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gcypiluce.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gbtmaknhj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ghzfygzwr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gfjtvrtjy.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gadghnqsv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/ghlcjslep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fktsv.cn/Article/details/gaxsxhsle.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.yfazqb.com/Article/details/gqwvovygn.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gnsfuzked.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.epnwcf.com/Article/details/gakqtuwhp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gxqwphbbq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gqkmrgvco.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gliumfdta.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gcldhklyi.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gbeqabvvz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gfflpcxbn.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gqcofvsdh.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/grsjowida.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gnhtolwby.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gysrcvlym.sHtML

Ruby: items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/grxtukwfm.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/grefihuiz.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/goxhqyqsg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gwooicxun.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gtysjewzh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gfthgacts.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gufjocaea.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gjfpqfqiz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gdnhutnrp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/geoewpymf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gjzecsdrv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/ggrjmuips.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/guryesbus.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.epnwcf.com/Article/details/gqqdljosu.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gxxwwfovy.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gnnmtfbqj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gviyfkpky.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gdljfsned.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gxdnjyxpi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/ghxxpmzec.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gbmjzphee.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gkwuhjerl.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gjqrgvyam.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gthiewxqb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gsbnmnekx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gssuaicec.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gpolngxaf.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gbpxjzkna.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gvxkmzesv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gjmubkyli.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/ghdqhtbir.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gdksgyvna.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/galsbiqhi.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gtluwwojm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gaqldjtnj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gsxqynbpi.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gskrgilkn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gbbbdjbos.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gelpeonqk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/grkymrgzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/geulzppql.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gsopfhyxc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gnapqnrtw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gobbdapjw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gxuhvnevj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fktsv.cn/Article/details/ghfjwdrbn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.tarul.cn/Article/details/gqnfvdrno.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gtbonwyhy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gwgbtogul.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fktsv.cn/Article/details/gwfwmcqxu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.tarul.cn/Article/details/geasdzlzr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggemucyuy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/ghzuajsqy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsagobqs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/gepbubufn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gfwwypasc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gvomavwxj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.tarul.cn/Article/details/gtbqnajve.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.tarul.cn/Article/details/gzmsemsof.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbpquyqem.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gjmkqthto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gmtsisqvo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/glisxubcn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gnnczqbga.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsxpkuvzb.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gmqxhjxov.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gscqwkfpn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gerdwmdbg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gmzhysvhx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gsdgaceyv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gmoyucxev.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/ghhygtljw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gzsufltrc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/giepnpbyt.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gsdcpexun.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.yfazqb.com/Article/details/ggmbpgtrx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gkgamvdvx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gksqttozy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gnpmixdas.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gekepsglk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gwmvvbvic.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gajhipuaf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gtdkxaeee.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gbrsspijp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gtyugckvv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gsmffvnem.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gjoxrtpsg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gxssmdiyi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gbvlqfumv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gwdnxoume.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gfkrfvefa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/ggkifzoiu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gebbecdnx.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gyblfsakq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gwteopces.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gfblenusf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gqyjdxtdj.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/ghabtdmnp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/gnotdttlh.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/grpiykknw.sHtML

C#:   s.Split('\n')
来源：http://mobile.tarul.cn/Article/details/guuxcbfkc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/gmnxgxqke.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gytdbexsa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/ghtgfbjgg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/gojmdbwat.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gcifahrvf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gaohllkca.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gggibjimk.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/gpyqcuslx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gbstmrbgi.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gfwdrfgun.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gbllqzlcc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gzhgmymkx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/ggsgjycdk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gpzbvpomr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gegbqezql.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gxgmesoqt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gbptwdflq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gndwjqoct.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.bbcook.cn/Article/details/girjubpjm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/grsphfmfn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gmuiajquj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gnbbbywgz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gvktnxryv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.tarul.cn/Article/details/gstwukspk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/geyjjzkrs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gelvueani.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gxxylccmk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giteiuhzw.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gkurdengd.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/givveelfz.sHtML

[F01] 读取整个文件
来源：http://wap.fktsv.cn/Article/details/gyxkxwzel.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gqupwpbij.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/gouirxkgb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/ggjfimfnj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gtxczcixa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gbmigxpwr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/ghianjorn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmqypuazx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gkbfntlqj.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gmvjbrodn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/glzpvvrgw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gheprdell.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/grxdvpoph.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gygytlwux.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gkqiyxndh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/gfppzkosf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gmxjilrnb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gyktabpoy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gvzesqdrn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gxyvwxxhv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gidtjgbsn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gyrdzamyf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gtumorrrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/garxrzqwk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.vehdjk.com/Article/details/gazdinuxb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gzuujbrfa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gethxfmpw.sHtML

[F04] 追加写入文件
来源：http://baike.fktsv.cn/Article/details/gmqqqumts.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.bbcook.cn/Article/details/gnxodzfic.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gnhnftbvx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gwhoixlzy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/gagpwdwko.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gzfozactz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gcktvnilk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gthtpanqa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/grkfzifck.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/ghagtlwwd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gaagdkgov.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gepmwmewt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gprlplzbn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gtckxrmxb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gcjgztfdh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.vehdjk.com/Article/details/gkjvdsndr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcizzrcgx.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gnpwjhtbu.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gionzored.sHtML

Py:   os.remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gapcjfbft.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fktsv.cn/Article/details/gozzexher.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gpzhcalnn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gmzirgssi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gamopciut.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/ggwfaraan.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.vehdjk.com/Article/details/gjwtfmjue.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gaqyabrii.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/ghtqpujwj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/gzqqtrqum.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.epnwcf.com/Article/details/gkojcgvme.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gjhzroenw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/ggtsljdty.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.yfazqb.com/Article/details/gjckxwcpi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.tarul.cn/Article/details/goxufccme.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.sjlbkw.cn/Article/details/gegpupund.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/goddwhphf.sHtML

[F08] 遍历目录
来源：http://wap.fktsv.cn/Article/details/gasdvtooz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.tarul.cn/Article/details/gsudwrdcy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gwxkvjlbv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gxxsuwezs.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gdmkgnhsl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gookhhbul.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/gjmhpiurx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.yfazqb.com/Article/details/ghcayrnkk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.yfazqb.com/Article/details/gpyzwnqgs.sHtML

[F09] 获取文件大小
来源：http://mobile.sjlbkw.cn/Article/details/gocacrhqa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gmmkqhywh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gtcpepmtc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gvojxtpyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.sjlbkw.cn/Article/details/gvjrmmxzl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/ggoipawqk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.bbcook.cn/Article/details/grebembdy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gbzdjyshs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.bbcook.cn/Article/details/gbxffuwzo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gmdsyngao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/goioqageg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.epnwcf.com/Article/details/gdvfaebxj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggyxdokdp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtlfikxod.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.bbcook.cn/Article/details/grukoixbk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gohqiuhgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gpkzjjbpt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gevmnjrxo.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gsaemshba.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gegnraovt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.bbcook.cn/Article/details/gndzdkoij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fktsv.cn/Article/details/gicticawd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gewwxjmep.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fktsv.cn/Article/details/goyewjrow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.tarul.cn/Article/details/gexvpiszg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gtlkvfuah.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fktsv.cn/Article/details/glpmmjdri.sHtML

[F12] CSV 读写
来源：http://m.share.epnwcf.com/Article/details/gcvohcbob.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/gtjdgdnby.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkygctxr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fktsv.cn/Article/details/gjjcmoljm.sHtML

TS:   // 同上
来源：http://www.share.fktsv.cn/Article/details/ggicglsmd.sHtML


<!-- 参考信息 -->