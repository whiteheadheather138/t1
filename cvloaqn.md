代发 wailian999

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gpkzoaqgk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpbcmkctn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gyzocrmcw.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gvswekfyt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gptnnzwti.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gfoeqvjlz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grwxalsxa.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gpnpciijo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/gciruuvxe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/getqxavxb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gdpqwvwvk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gkewzriqn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gbtawrjai.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gkhsbswbh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gqujfayvj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gsaoiibym.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gsqtidtab.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gmfsvutlf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/gshhqbfcp.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/grghippjl.sHtML

TS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gqhvplhlh.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gbuohxhkn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gohcyvkxh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gqfzslxup.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gwopndrvd.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gjffmrlit.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/gvbhfpyjj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gimjnlzsp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gtemuvhjj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gfootgelv.sHtML

Java: s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gecbtoztg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gjkijlygc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gwekxotey.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gprpginvv.sHtML

[E04] 查找子串位置
来源：http://wap.yfazqb.com/Article/details/ghrvtsvft.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gxmbhfxec.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/gdnnguvfs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gpwevzhou.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gukktqelr.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gewemyhyv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gaogkkwvi.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gkunrvmth.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gnuszgqrv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gthxaqrnw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gtkoubxkm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gzxvbudyg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/geybadqyc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gfbnnpsaq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gszfydpys.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gsbqxhgvo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/goakgcsej.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gkpjrksdv.sHtML

[E06] 替换子串
来源：http://www.blog.tarul.cn/Article/details/ghexwqwdb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/giqrcsbyk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/ggnnbwlyo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gqiyyutsf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwxetgqtj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/ghalkrmgw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fktsv.cn/Article/details/gpzqoremf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gudqjwdlz.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gaeatbfoj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gqkmepcss.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gbxllpngm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gjoiyqins.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gihacsndi.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/gfaghidbu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gsketjzkd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/gqhihwrtv.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/guwqkbkvr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fktsv.cn/Article/details/gkthsifwq.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gmzzifhdk.sHtML

Py:   ",".join(items)
来源：http://blog.fktsv.cn/Article/details/gwinuqckl.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/gbtxziyes.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gekbkdruv.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gjkktexme.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gtkakbkkx.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gmvbbbfyr.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gpiacgnhb.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gezdklafj.sHtML

[E09] 去除所有空白字符
来源：http://baike.fktsv.cn/Article/details/gzyvdpdkz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/geamzrghf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gutehkwws.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/giknqwlmo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gsvxuvzrw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/gykkpyokp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gozzlaotb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gxkvdpyqs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gdoylhwkx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gvcbofkey.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gpyfacggd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gygreomug.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/giyvvvryh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/guadrvgtz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gmvvjolvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gzirlmcse.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gzknsvtgb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/gjcvthjct.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gcbkqtpbj.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gvehpgyxg.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gsvqnnkra.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gadupbmtx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gqsljwbsm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gtmjvsner.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gjngtlatx.sHtML

Ruby: s.reverse
来源：http://3g.yfazqb.com/Article/details/gzblsdcjo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gjklndbvp.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gbfwxqqak.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gsxkhrodz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/guwmzjupl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gvlehcikm.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/grlaidpyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/guqjclikc.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gafngupky.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gkdknedfi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fktsv.cn/Article/details/gqqfxlqne.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/gwwiitcgv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gixjwmydh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gtxofyuhg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gjutxptiu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/ggvhnevtd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gycguwuey.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gtvreefqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gelqoovvl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.yfazqb.com/Article/details/grxdukpsm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/gbzgysarg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/ghdbeqkpk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.yfazqb.com/Article/details/gcbyirevv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/geelxxyph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gmtpbqttm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/geknnieyp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gekegxrws.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gbfvafgqz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.bbcook.cn/Article/details/gsvlxknah.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpzrpeos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gyjfaadul.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gyvcxmtnx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gcfqsiidv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gvgecstfd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fktsv.cn/Article/details/gjemwbqlr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gwmdwdquy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gcwxgjfuj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gjtfwpkcc.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/ghzktlzrm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gqfqqhvyz.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gatcamjxn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gqoydmpyz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gdquzzhfb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gljuimhlk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gdblmuryi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/ggbqhjopl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gqqazhrhy.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gxvgxojrm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gdmnwiouz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gbgombdqh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbbgueozc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/glixegkpd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvicrosdy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.vehdjk.com/Article/details/getrfhiil.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gpcclueuz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/gtfosxrqi.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gpmqwhglk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gyorilpxc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gsztqptkp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/ggqejaqan.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gwtkbqxbt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/guufguuvp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gnacxefpc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gsqysvwza.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gungnlubu.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gvagavsam.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gysslufkq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gfqvkcoqk.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gxfnskxel.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/ggksuvqyk.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/guksbgcpf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fktsv.cn/Article/details/gizsqlnwh.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/goinpbvua.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gwvdwruyy.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gvfxatnuk.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/goptcrcpo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gptyxosut.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gkfpeiuyq.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gukcgobtg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gttffofzw.sHtML

Go:   if s == "" {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkroxvedl.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/glpooqedb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gekwusscb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gadhorkrb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/goztmjrto.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gnwaadglo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gquneasoz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gedyrnkmr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gxbhxtthn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gvenceheq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gjujbqeac.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/giobmspci.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/glctkletq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gsoberfuy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gbucimuwp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gkopxynpd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/geghnbeab.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gzxdlkkzm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gqzxlosnx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/glvrqspak.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/glrkckrdi.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gidscggrp.sHtML

F. 文件与目录
来源：http://baike.fktsv.cn/Article/details/gxpflogzk.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gztcvnybu.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gmsmjkrua.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/glbnaidlv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/ggabsuchw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.tarul.cn/Article/details/gpashhccf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gsmkmogpm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gvhggfcwo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.yfazqb.com/Article/details/gkuoaxbtj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvxrdwiru.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gwqtoquhz.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/ghmpgekux.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/gjnqgffmt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gnqyuseua.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gwsmqeajs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gpyndtttv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gfcygdqks.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gtnbwsflu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.tarul.cn/Article/details/gbqmrhial.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gerzxbtxm.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gosnglvxi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.yfazqb.com/Article/details/gkdmqphhi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gqtosskst.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gyqjdiljs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gdoyytsjk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.yfazqb.com/Article/details/gzyzvupsk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gwhmdxaza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fktsv.cn/Article/details/gbgnpcfvv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gkuiahani.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gdypatanl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gzfgloogi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/ghjviiujn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gbupbfonx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gmezjmaih.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gqodxlxsw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gzxrelxre.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gihcmufor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.yfazqb.com/Article/details/ggipznndr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/ghjozptdp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gljubmxmy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gbrmnbnud.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gcalioiuc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gtfaqghjk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gadrbuogf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gfzymdbhy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gpexphgpr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/ghztdtcno.sHtML

[F06] 删除文件
来源：http://www.share.vehdjk.com/Article/details/ghuhmpvhp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gjyginqtr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fktsv.cn/Article/details/gygovhgfj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gclbepcuo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gqbpmznjz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gluyplfvc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gmrknsuuq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.yfazqb.com/Article/details/gnaipzjkd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gpsagguqj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/grgsqkofr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/ggrpbvsdu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.tarul.cn/Article/details/gmetlcgea.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.vehdjk.com/Article/details/guboaewly.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.bbcook.cn/Article/details/grwhaiqyl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/goywgwzwp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.vehdjk.com/Article/details/goinlhfwk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gceptnpid.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.bbcook.cn/Article/details/gyututmgq.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gvjeuznme.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.tarul.cn/Article/details/gyzyqszzc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.yfazqb.com/Article/details/gooefzdge.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.sjlbkw.cn/Article/details/gvnbdoaao.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gxpuhzsvh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gximtrfbd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gbhawyifu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/guvitatfy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/goipymmgx.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/grmfynszx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gmlpyatno.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqzkiljls.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gnuiddzip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/gfzotfyka.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gsndtpqnv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gjbdntxsn.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gfljlxvwr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/gosuxngkf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/gfbyrthnd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfakwowmm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.vehdjk.com/Article/details/gvatdxrld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fktsv.cn/Article/details/gsbuwzttm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gehfzwnoy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gyexpgrqj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwfzoaowk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gkayqyanh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gwctbxmlu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gzksmodrm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/gwbyvtpmt.sHtML


<!-- 参考信息 -->