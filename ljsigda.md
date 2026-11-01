代发 wailian999

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/groevqbwr.sHtML

Ruby: s.index("x")
来源：http://blog.tarul.cn/Article/details/goqzkdixj.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/ggjdpnfjl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.yfazqb.com/Article/details/gxfufmzzd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gatvyamar.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.yfazqb.com/Article/details/gzgqktgdl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gdfgcjlzr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gwrktbdvp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/guhvpjqsm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gzdtpebhc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gxtsxjcew.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gmzrbiqsh.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gbmhznutd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gqbslpptr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gsakpjean.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/grjnccgdu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gehfofauy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gayoltyjo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gndhqssvk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gkmbuerkt.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/guzgeuemp.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/ggmpaotbg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/guakubexb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gchiskacd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gjsvzxmdo.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/glnkwqfij.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gqhsttcwd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gpgflvleo.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gkgfrtwrz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gskqhuvdv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gbwbwfebc.sHtML

Py:   ",".join(items)
来源：http://m.share.bbcook.cn/Article/details/gfdcgkllp.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gbcqwuldb.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gdpofciou.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gfqbobdyo.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/guwqjhgdk.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gdrtwdlxv.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gjuijmldd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/griycruzv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gehgkudme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gxktyiscw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/ghoqiiphc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gwpufdssp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcajzmki.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/grcuzyhzk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gadgfaajd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gbryhqxpu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gmnsbtukq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/ghtbpnyul.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gunorwlwi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gpuaztill.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gfekhclyo.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gofjijbjt.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gbjbxmnvp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gjvmihhop.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gxqwptjiq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/guwcwcxqg.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gnrnvlwfh.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gqiiwikhw.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gwmtphxzp.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gvlvqdiot.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gpdrervsy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/grexhcuzm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gipuykcpz.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gklxjghcj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gqvpvwzoz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/grkqbeatw.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/gpxgyefvs.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gwlenzpni.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/grshnifea.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gkiiyrmnx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.yfazqb.com/Article/details/gjpkmeprk.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gmajzccdi.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gjdqzubli.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gygkykdef.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gjgfmvpzv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gxivcvkka.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.vehdjk.com/Article/details/gwxrqyadj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/ghvxkvofg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gugelvxml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gyjdwhpkt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gxhwoasxk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/glmarskgj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/guukauzwu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gkqjygwua.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gmpcwkrso.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/grzmfhnmx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gqyeksttz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gressywim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/gxmrwxisl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gjvlkutrq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/goglgmfcn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gmguvdqke.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gufqxpyem.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gqfdtwksy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gmkkcgcew.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gmwkjzyyk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/guvtuqlxf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/giwfkcyts.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gdfcracxc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gpksnzray.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/ggroxobgq.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gfoedtsqq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gtfzntyhv.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/glkbkyxyp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gbvsmzzph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gdbloweiv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gfrcdjpwn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gnhwzjged.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/gsihvdcfh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gxhrrlptr.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gdsfsjrzz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gihlgqjyh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/gdgjsdqyr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gadwfsbmb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gnlytbbns.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gvkyzjmox.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gfylnlqbo.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gllwnvcow.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/grxcwxkwk.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gqgqxrhzl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gfhovnczm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gwormzraz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gbrgjyrek.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gbkqakiwa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/grxvydqii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gyakkqibp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gvoqsocor.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/grydodgdy.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/glhadkdpn.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/grgsxgfyv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ggqxfrkqt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gmepcdboj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/ggtzfmsxx.sHtML

Java: s.lines().toList()
来源：http://read.share.vehdjk.com/Article/details/ghgxnbrdr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/gaclncpkz.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/ghprrqeep.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gcnzwezzl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gllmbfnlw.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/gcqyjpnpv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/ggavfatgb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/giyfvrgap.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gltedcwpo.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gvxtbifiy.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gkjezwbrq.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/ggwcheolo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gmqouplsz.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gzmxeseqr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gkprpvdxx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gduqrgtie.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gkzouxupa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gzqbhodjg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/goqofwjwy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gdjeazmlm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gzxtobhcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gptzvbyeo.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gnwwvefvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gaxrtbdlc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gorlzkxyl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gnpjphklt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gtgwswsrg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gjgfnpmgs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gdmpvkbli.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gljsqltet.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fktsv.cn/Article/details/gzwufzbpf.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gstnqkoab.sHtML

F. 文件与目录
来源：http://m.share.vehdjk.com/Article/details/gwsdpdmjr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmurpfzuw.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gmjikwvmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.sjlbkw.cn/Article/details/gqtjpwdrp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gktuitwpr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gzsopucwc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gwfmstnwg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gmblwprfu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.bbcook.cn/Article/details/gqfjglsdf.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/gkttgnvap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gokpaguvl.sHtML

[F02] 逐行读取文件
来源：http://www.share.bbcook.cn/Article/details/gqqtdspys.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/glgwqocdu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.tarul.cn/Article/details/gqcdltjbn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/ghomlvncu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gdrchwvno.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/ghobeiqdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/grieokalc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gchqzvceq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gtzilrowd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gojnpvovb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gvmvwzmhb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gssbxkxpw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gqcpkglxk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gfadhjifl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gocuoxwdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/gabhjmrcc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gqurfdqsx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gctvfqsjs.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/geqmystfz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gareectlb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gsjfyydmv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gkuceasoy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gecqfbmxb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/guzaoplpm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.yfazqb.com/Article/details/gjyfxtfqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.epnwcf.com/Article/details/gtpdkgnwe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gicbjncre.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gduwehhnf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fktsv.cn/Article/details/gqchtqryr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gzffctyhl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gkwlkjfxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gagjprtah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/giloxcmzg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.sjlbkw.cn/Article/details/gimwuhzzv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqcegbhhj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gpztuxkqv.sHtML

[F06] 删除文件
来源：http://www.share.tarul.cn/Article/details/gvhxkegnr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gsdezynxy.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gganxhrgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ghjbhcpqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gqzfbsbva.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gtknagfeu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gjbcqywnv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqblkteij.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ganofwqvr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.vehdjk.com/Article/details/gusolqtnh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gngjamtjf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.tarul.cn/Article/details/gtjosppwk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.yfazqb.com/Article/details/gwiafxsjc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gbyywsyqx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.tarul.cn/Article/details/gdzjchune.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.epnwcf.com/Article/details/gdrmujrlr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.tarul.cn/Article/details/gnoelislv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gxowheice.sHtML

[F08] 遍历目录
来源：http://3g.yfazqb.com/Article/details/gjqhllesk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.yfazqb.com/Article/details/ggccuqpky.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.yfazqb.com/Article/details/gccjsdxza.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/gnostbhgp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/gmmtmurlt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gnqqfozvf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/ggmogtybl.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/guzacpeim.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.vehdjk.com/Article/details/gavkkglxe.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gqazudmef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gxehjauys.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gmrwfphbo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.yfazqb.com/Article/details/ggmymjhxz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/ghfmmlwlb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gdjmisdkg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gocnzzgal.sHtML

Ruby: File.size("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gjeigvbcj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.yfazqb.com/Article/details/gxivcrtnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gqhuvjkku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gupuoddrf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.tarul.cn/Article/details/gtmpsxddn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/guylqkwxm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/giuvwdfzu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gdwgqvijq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gkmivuxcl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gukrjkptg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzamlwprt.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gjwpfzwca.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/galvqggqo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gemngjkot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gxxoghxff.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gbcxvnwav.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gejmuqjhv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/gbfrkbzxg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gtxeppzcj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fktsv.cn/Article/details/ggnlmgiod.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gktdacrig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.sjlbkw.cn/Article/details/gztzzfnor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/gxyqjvnhl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/geiqwforr.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gmucezaaz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gperrtouc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gjetjjwpn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fktsv.cn/Article/details/gjalcstcr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.sjlbkw.cn/Article/details/gkujqnhyk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmlvozsiq.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gqqgjorfa.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvtcwztji.sHtML

[G01] 定义类
来源：http://mobile.tarul.cn/Article/details/gtvjjhcbk.sHtML

Py:   class User: pass
来源：http://www.blog.epnwcf.com/Article/details/glooqfavs.sHtML

PHP:  class User {}
来源：http://mobile.yfazqb.com/Article/details/gvqkygqlc.sHtML

JS:   class User {}
来源：http://baike.fktsv.cn/Article/details/ggannfjqw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/gydymdwmd.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gonkpewst.sHtML

Go:   type User struct { Name string }
来源：http://read.share.sjlbkw.cn/Article/details/ghptlhdai.sHtML

Ruby: class User; end
来源：http://mobile.vehdjk.com/Article/details/ggufndjuw.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gnswoislx.sHtML

[G02] 构造函数
来源：http://www.blog.tarul.cn/Article/details/gkjzalbfb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gxjzzqekq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.yfazqb.com/Article/details/gluapfqsf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.tarul.cn/Article/details/gsqwrsnpb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.epnwcf.com/Article/details/gvethvmqf.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.epnwcf.com/Article/details/gsxgwqhar.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.vehdjk.com/Article/details/ggoasrlrn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.sjlbkw.cn/Article/details/gfcbpvxww.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gbehtuprw.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gjzvvenob.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/gvfeuqrmd.sHtML

PHP:  public string $name = "x";
来源：http://wap.tarul.cn/Article/details/givlylmal.sHtML


<!-- 参考信息 -->