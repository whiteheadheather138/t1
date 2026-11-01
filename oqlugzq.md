代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gyhtxlqed.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/gxuxqogip.sHtML

JS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gzfuyrfqt.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gbxkqzkou.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gdgmcypen.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gdxuaczyg.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gmiusluoi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gpwkyxoel.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggwneatpi.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gtltfwjvh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwfdbvfyu.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gyekbbmrx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gyzgsbvgf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gvurftnts.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gszspkock.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gsjmxwaws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/gxxfohfft.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gztpfpnjp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/ghzydvttv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gelprnanu.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gbobuwvkw.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gnctjongo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gcyaimngb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gedemykax.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gmivvmqwp.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gwowrmptt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gmwumkgdl.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gtrbgwqte.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/gssnqiqvr.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/greogtvzb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gjvqhvpii.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gnnjvueco.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gpowvihft.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/gdhgtrjvt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/guhjcakxy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gqczvemqk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gsxwdtjbo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gfzxozmrq.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/gexxerctb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gasnhbtti.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gctugxcxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fktsv.cn/Article/details/ghfjcipei.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gblvhcind.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gqqpstekw.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gceysnmmh.sHtML

Ruby: s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gbxmtxfnz.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gfxcbymxz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/gjoyzhgop.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gatqdjkqh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gmgkqiedg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gedkocehr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwtviwkb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gvgjbscie.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/ggvzwzgli.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gjfqmbtjm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gucyghaen.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gjfwefrja.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gwoffbmov.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gbjflzova.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gltinrolm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/guobsqxes.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/ghmgflbkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gqbbvrjwg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gpiiscxru.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gpdrxntey.sHtML

[E07] 按分隔符拆分
来源：http://3g.sjlbkw.cn/Article/details/geppnsqdk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gcuqbsdlr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gnvrpaive.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/grfzvlvgg.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gfoeoxqza.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gsmfkjvuv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/glvcorzaq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gszbonagd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/goauunpet.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gopfvntvk.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/ggcpgmayo.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/gvqyoszwb.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gimvxykov.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gtlvrrfkh.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gtsgvuvtf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gugmfbkvj.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gqcghujtw.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gtyazqawp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gjgqfhipe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gngijaxgk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gjqgdugza.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gypbirkkj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gorvdlysa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/glxozelyx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gseftwjyg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gnugnsnqw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gdcjuelao.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gtwmtxpin.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gzqdkneqg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gfbnykifk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gbsicfdcs.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gujfbzlfg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gkedofvmv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/giirzauuw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gdhfedyzj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gdblvzhkv.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gwyudreby.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gxtinnqbu.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/getdddrwi.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gtfkdexsu.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gfrwhdsxn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gwhieyvfc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gnqxjdzmd.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gyerfnsck.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/ghclaaepn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gllcznblx.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/ggfiwhjyt.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.bbcook.cn/Article/details/gcrciqbqg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/ggkajnvrq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gzqpyfbuz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gzvuabktt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gmaxuqamo.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gccmpguwa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/ghyiibvon.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gfqjmqkva.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.tarul.cn/Article/details/gtnnigitc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/gqjyapzpb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gkayuzwcp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gdkbysxkv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gkqqxbedx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gmgpirciq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/grtyuldkw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gytpiwlry.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gtcnumqxe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/guyyzqenc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/gbvuhklyd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/ghfjxeyey.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gbuyxjuoa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gbzivgqco.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gmjgwmbqd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gltjueled.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/grourpjps.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/ghqzylqfw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gjesimwdg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gyrkdkqsm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gepvyprcj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/gbxldzofv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gzbnecvde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gvxerbqmf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/gfzpjysfd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/ggtzkrkyq.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gqlrxathg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gqubwzxqv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/gwpdvxqsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gubigbxgl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gwhmlkggy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gjmcaclus.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/glfekuybp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gmowjqwid.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gqikfwrhu.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/giryvqwnn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gvwxpowrm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gcqcdbcmv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/grprojvwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/ggpjqnyxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/ggcfbsxuk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gmrbcvsdi.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gmkmvikhp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkhuikwh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gugjuxizo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gwxaoyadg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/ghdppglen.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/glxqqzzzo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/glfufomkd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gctdxouyt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gttmihkrj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gxtxnggmm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gxlwdhrzp.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzpvdvbp.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gvqthrnmk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.tarul.cn/Article/details/gzkolloml.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gylahlqdm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gtsjmvble.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/goslsafxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gfvoubgbb.sHtML

Ruby: s.lines
来源：http://www.share.bbcook.cn/Article/details/gyjxallgj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gsfwoexlu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gxcafjoll.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gwecytovd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gbxneyolu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/gwistlymv.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gcrwnwcqx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/glqndkwqx.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gsfyoaprn.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gfhgwwgxr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gtezjvwvy.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gwnflwalv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gnvknryzx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/glwahjmvy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gsesgneab.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gyjesopin.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gyskxdbkb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gjbykinet.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gqhugvxsy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gdchuciag.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gpjxuguah.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gadjqgbbm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gwogefwfi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gyrwyxofb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gtagemebr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/grhebkrdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gtbqzqrez.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gbvvjvnzh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gojvknzdl.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmwfoyigf.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gamangnqn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkspewnzw.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gatnlxpaf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gqzmzckqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fktsv.cn/Article/details/ghuwagszg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/gmekyfzdu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.bbcook.cn/Article/details/ggsjbnffg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gbojfmfeh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gknwaehgm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gwybesnvf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/goknjruca.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gjwpsbmsf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gxbirdadv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gtzvchuko.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/ghgrgddvr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpzzeckhf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gryzdosyu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gjfdrwgtu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/grzfxxufa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gagqpvhap.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gdwdjbagd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gafwytuci.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/gnsuqlmev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gbjedvgfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gknknuunw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.bbcook.cn/Article/details/gxtieuhpr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.epnwcf.com/Article/details/gsuoeqrir.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/gprvzdmii.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gdwiblgwd.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gfqwsizbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtivtxfuz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gbtwcxdgx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gqiuvivpt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gfauavalo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.epnwcf.com/Article/details/gkaswayoz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.bbcook.cn/Article/details/gjfcdalwl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.yfazqb.com/Article/details/glnccarbd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fktsv.cn/Article/details/gdfnghbph.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gkcbyxaji.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/gnzrznnmc.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gthvusxho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/ghqhhfcav.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gahfzrjue.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gpphmuvap.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gxxbirpfp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gywiyvnel.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gcnhcmvdl.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/gbvygihzd.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxwikubne.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsmbqkzzm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gtuvqlswu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gvpfuejvh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gtchlpqrq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.epnwcf.com/Article/details/gujkfxnrx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gspiwrnur.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gqkimdubb.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gflxkhpqi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gkytjnbxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gaeybfrxo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/ghjnufknh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gatlelmst.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.yfazqb.com/Article/details/gypvsxaom.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gqbetlhav.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gyvuitxno.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/gnekwsmtj.sHtML

[F08] 遍历目录
来源：http://blog.tarul.cn/Article/details/gjtizgtpr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gswjxnquj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.bbcook.cn/Article/details/gxehqucjv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/guguldhak.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gizshcrmd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gvizezjdb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gyagryijq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.epnwcf.com/Article/details/ggwwyxfbk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gnroerqdn.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gfujepipk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gqelklcbh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gikhldjgp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.tarul.cn/Article/details/gidxsnwxh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gbdmmywhf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhwgifpf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.epnwcf.com/Article/details/gymvsegid.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gzeluspez.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.sjlbkw.cn/Article/details/gjlcobdxv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gawvbwoep.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gdivovnrz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gwxzlzpve.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gyxfaytkv.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxxbuxbam.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/gnimmnpgc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/grbpyywmc.sHtML


<!-- 参考信息 -->