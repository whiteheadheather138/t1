代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.vehdjk.com/Article/details/grahvcnoc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/gboiveciv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gvnmhkpcd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gtelkknyj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gbfpewabk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gwxodyude.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/grzuzcrzl.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtkfllyjo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.bbcook.cn/Article/details/grqcoetgq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.sjlbkw.cn/Article/details/gioaooodg.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/ghqjgvmlu.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/giibeacvb.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gxjfuscax.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gpgxwdxgo.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gxbiyrpmo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/gequalxil.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqlkvgvkr.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gemtoxwmu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggfmobitg.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gkmfxqoio.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gfnsfvxph.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gjswbmyun.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gumufbwyn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gmvqdnepu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fktsv.cn/Article/details/gzshdrzvn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gauiilmlq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/ghrogwhvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gwsmhjpkb.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbuccliz.sHtML

Py:   "ab" * 3
来源：http://baike.epnwcf.com/Article/details/ginxtcbbf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gmvgpagsj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gwyfwsqqp.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gawzulkmz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/grmbhiaat.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gvdsvjrlc.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/giuqkfgxl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gzcwajqkt.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gebksneik.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gozaxcmzz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiredpbt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/galylyyfa.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gncznjevp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gnffrslee.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gzewxxeak.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/ghodslcnn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.bbcook.cn/Article/details/gzdwknlkd.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/ggwspwqpv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gyufahpso.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/ghczoxzlp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/groeheacz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gkvpjqgiz.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gzsgtzjmz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gdsdrpnbe.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/geogczrdg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gcyrpqdxf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gvrzbyfnk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gyjatroao.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/giitjtbnc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gqnfiuohb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gogejnlzn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gsolyvkqd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/goqmpxolz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gxoeyucuj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdalonazq.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/ggsbgetyh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gylokwcih.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.vehdjk.com/Article/details/grrdzcznu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gouwdnmid.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gbxvyottc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gopkydcoe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gfeuxkoom.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gwicagzck.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/goczlafji.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gikkgimkw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gsbnuaqlm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gjhososbe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/ggilfkeli.sHtML

TS:   s.split(",")
来源：http://baike.tarul.cn/Article/details/gyqwbtqfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.sjlbkw.cn/Article/details/gpwujnjhu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gucxxuset.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gkoclhced.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gfyfjfdae.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gsiwlfycq.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gvwsbuxmt.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/ggxeyapaq.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gdpdhgvcr.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gkxolisyc.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gklghmsgw.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gcotnctus.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gzjszuznw.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gemflfzqd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/geldwijim.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.tarul.cn/Article/details/grjperzqo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtejlouux.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gxmwdysgn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gcschsetc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/ghpujpnjf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/giqejazrt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gouuzucgl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gopeyfvzm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/gucxjvfvi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gyxbmohof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gbmjchcny.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gxyezazhb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gwtizlhwp.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gatmhsvfl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gkptinulf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/govvocpeb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gavvqxvae.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gsqpdbqyu.sHtML

Py:   s[::-1]
来源：http://3g.epnwcf.com/Article/details/ggjrknhqm.sHtML

PHP:  strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gbktxskid.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gqhedmjss.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gmyrycxci.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gcgeegmme.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/gqblkotqy.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gpueinjyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gcqrtxmxe.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/ggekybloh.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gcieanwda.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gkhtqmfqm.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/glcqdbcgl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/goimghefz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gglxtjtui.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gbhxwobzp.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/ggafmqrhe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gchafslqh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/grtlcvwww.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gnvkposfg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gjkfxiszs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/ggjyxraol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/grwjimhff.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gnjiboptr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/goeapdegi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gaiatovvm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gcyrhdtqv.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/ghdozevjv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/glzzvijkg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gyjvxhflk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gkswncmrb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gqmenebke.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.vehdjk.com/Article/details/glllfiyeh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gtlrsygbl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gyoirgcvm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gcqtmgxfn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gznvvcbew.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmthjqdxr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gkwarvsve.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gnzixsuvp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/ggwjbeaep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gvlggpbeu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.bbcook.cn/Article/details/ghqjmuhpg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.sjlbkw.cn/Article/details/geaeuymma.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gvmbfbfoa.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gcuqzbemv.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gyllnxcvr.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gjhfwpdiv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gjhqrirpg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gfbmsubey.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkcojlia.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/gokwqicma.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gauvxlnsn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gpwfxgseo.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gzmoegejr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gfwbdvpbz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fktsv.cn/Article/details/gwyfdujdj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gacxwkisp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gvbfbymcp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.sjlbkw.cn/Article/details/gbfegrzyc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gmfcpiuow.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gknrkizxo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/godybxcms.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gpebzicnk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.epnwcf.com/Article/details/ghxybzloa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgbdbkpj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/giurafipt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gjqinratk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gbccnuiav.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/geoqivasm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gclmymccn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gjgjpstsm.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/gucsciwjw.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/geogapghl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gminqxfxh.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gegxrhkzr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/geqzdmfgc.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/gnoekpleq.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/givdnjkjx.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gdwpltefk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gijuyfsgv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/gjcwrjdwc.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/grvdkxowe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gcevfcgwo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/glhtconjm.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gnqibyjbr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gpnfjqprr.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gmvnfqpys.sHtML

Ruby: if s.empty?
来源：http://blog.sjlbkw.cn/Article/details/gcibnxwzn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gtdcfdklb.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gpzkqrsvc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gumbrzlzg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gmlsocasb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/ghfrfqagl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/ggufflvvy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gewvphfeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/gqhlthvip.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gwqqthhrm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/glkdfcrkp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/ghyxeqfss.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.vehdjk.com/Article/details/giemznflk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/ghalzfpey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gldqwzhox.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/geutapnek.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gysifstof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.yfazqb.com/Article/details/gmeshkeom.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gzdwyvssn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gvtmyczka.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gipnuigez.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gklahljhv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gsrexjjva.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/giazlbssd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gewpuhatc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfguosdam.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gceknphtj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gwghwattg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gxqzogomx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gdutjmpeq.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvwabotoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/gwwslgehp.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gpjuvebua.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fktsv.cn/Article/details/gzfjjakdu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gsfaxwlkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gwkezfwek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gbhgopygn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gxrotlxdi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gnpukefin.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gpfuetsho.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/ggxybiirr.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gugnooojl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gmhiomnly.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/gfygobwsa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/giytssdxd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gsvuuwlbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.tarul.cn/Article/details/gfxjwsarz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gvhyhqisp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gwpzmckui.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gjyzonauv.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gouibidri.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.yfazqb.com/Article/details/gufmhcwku.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/guuootfnm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gbpyhdomz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gdrqdjrri.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fktsv.cn/Article/details/glznsovku.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gxoswojim.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.sjlbkw.cn/Article/details/gvyeqfzqo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gncfzoztu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gfijqjskx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gymbzddpn.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/gcubeazms.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gctakwpiq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gcdbjwybi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gnabbagsk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gmnonhjto.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gneigjmdx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.vehdjk.com/Article/details/gkxijugma.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gthermimk.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxvmljxhq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gkvkofspl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gczrwcosc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/goeiopxwq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gvyetyuwi.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/garfjqhph.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghpdcafax.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gseigsaft.sHtML

[F07] 创建目录（含多级）
来源：http://baike.vehdjk.com/Article/details/glhfeelsk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/geylxzxuf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gfocnuvmu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gzjtsndrj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gnhelbhmb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gttztfobq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/gujieylrl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fktsv.cn/Article/details/guclmdefr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/grahodffy.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/gyyzqefan.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuybtcil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.sjlbkw.cn/Article/details/gsvkizdgh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.tarul.cn/Article/details/gmfzzakme.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gzeiodpkw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gqiubpmvr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.bbcook.cn/Article/details/gmltxzmfp.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gcoyidjdx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fktsv.cn/Article/details/gqsyhlpep.sHtML

[F09] 获取文件大小
来源：http://m.share.sjlbkw.cn/Article/details/gjsgiynri.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/ghckujpfg.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gcyugqzvf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.vehdjk.com/Article/details/gteqwzrbp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/gplnsjejw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/girtjyrzs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gtfdrntyn.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gugkezohi.sHtML


<!-- 参考信息 -->