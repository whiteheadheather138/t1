代发 wailian999

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/gjbyvhcae.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/glbhtxobp.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/ggmeixhva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gclrrigbv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gtirmsiyg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gwatfxptd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gonvacwgj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gsixfblbw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/ggqxarsza.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gybmcbbhk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gcglyubej.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gsyffnogt.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gployrcuv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/ghpwobfvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.sjlbkw.cn/Article/details/gorqvbyvh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/ggppjboeq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/glmnaaspe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gqpgifrsq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/geejpnuvb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ggsesbfgq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gixindegr.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gjnakbbra.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gkpjhfjun.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/ggyibmbqg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.bbcook.cn/Article/details/gclyqjzvh.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/ggvhnlnby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gtvknnovj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gnlrajsdi.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gcaepygzz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gylttowfn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gtvxqugac.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gbwjjnayn.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gqcokvphz.sHtML

JS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gajpuukwh.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gqtjgdrig.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/gckojemsg.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gwrsbfbtl.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gwiwjrblr.sHtML

C#:   string.Join(",", items)
来源：http://m.share.tarul.cn/Article/details/glgdbqhlb.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gaeamgkwy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gghbzgumr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gddzumlbt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gaqjaqksg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/grjblhtyj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gpoqfcgfn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gqyctxgyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/grjplkbgg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gvzqkcdti.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gsjmdmjxm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gbcjzafvq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/goecphadc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/giuemscaj.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/givmfxged.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gwfkamwwp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gojlkwjsn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjxnnqfdq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gkkmwpaqp.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/giysskhwx.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gdtompruw.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gkpdbatxi.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gblvlpzim.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gdybokvnk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/givsfoxqv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/geszwsbtq.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gejpbbiws.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gozohtiww.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gwnhhplnc.sHtML

Py:   s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gztvrkpos.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gezcsucnl.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/giutlgkop.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gmcavhmgh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gremrmdhl.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gwbrgywfy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gdzgefqcy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gdfuwotty.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gybesvuzf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/gdnxzgkwz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.tarul.cn/Article/details/guxltshpy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gqeoiftxb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gicpvjxcu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/guamafozi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gjaufxnxj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gpodoxhry.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/groehscoa.sHtML

[E14] URL 编码与 Base64
来源：http://3g.vehdjk.com/Article/details/gmwduhisj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gkekdwhgp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/ghyhttrhz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gdlotqkoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/ggaijlsru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.epnwcf.com/Article/details/gvbbthzpe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/guulqjjdk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/ghyvzzmcb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gmeybbxwd.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gpfbnbvse.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.tarul.cn/Article/details/gkhcsipav.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/glliqmvkj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gmkvvvvgt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/glivujaod.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gkcdaaapg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gmopzptbm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gbppgulqp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/grmzeivct.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/ghutkvoec.sHtML

Py:   f"{1234567:,}"
来源：http://baike.tarul.cn/Article/details/gugjjhdol.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/giepmhfhx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gbaimmoht.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gocodmmfh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gikmjyrcm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gdzinuaqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gemrcphoj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/glajujrrk.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/gatvebhhd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gzjivltjj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gawcreynw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gidwaxiai.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gimpmtpjh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gzfterday.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/ghwduvhku.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/gvglixnmh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/gqntmcyjp.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/girzveqwm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gkflqcfwc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gtbvhfkby.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gjhzabega.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gdccyvyrq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gqebshgjj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/ghvuvcjwz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gniyqkqvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/grmewbtkb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gypkenmso.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gimylwyia.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gofcmxmhp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/ghglapomz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/gceefnkbd.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gfyselkrw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gusxfpqfa.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gtepcmsgj.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gzazhogjs.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gvwtjinnw.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gqpybcgke.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gwgyntvxo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gmnmvigri.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gwnexrvul.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gtzwzazoz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gclqiaiev.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gjwbqbhjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gcafaicgw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/grcdoanth.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/ghfcdlemm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gxmgrhbes.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/grimjvkop.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gohvdtarr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gpjpjvpsu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/geanfrqhe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gzbkydccu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gwmwfyvfn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gwxfabjcm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/glzjyrmtq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gdvhfxkoh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gagxevelw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gpzmbdpzj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gtowpicti.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/geofvlanz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gjhqvripc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gqtdhaywg.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggqtsvchc.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/giugopixu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gghcdzrix.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/ghfjtcduh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gogkczhhd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gggxsdafc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.sjlbkw.cn/Article/details/gecnexgtc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gelkgmacg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gugatsoso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/gxnwkrotl.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gggbljdxg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gydecptmm.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/gfrpilyls.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjiemcgr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gctdxzgnf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gupuqchrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/ghcxgxqlo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/geahfprow.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.vehdjk.com/Article/details/gxrgothuy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.sjlbkw.cn/Article/details/grtbhvama.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.epnwcf.com/Article/details/gfycguvfw.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gsozcohrw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.vehdjk.com/Article/details/gxgkuveiz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gvbecbvxy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gaeqeqwbg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gsermcfar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gfsxkpaxn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gszagulng.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/goqxvbobs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gzsfwqsil.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gbtaznxyj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gkkchsanb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fktsv.cn/Article/details/gkupvzwxb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gqbmskchh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/giggmllxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gdheozich.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fktsv.cn/Article/details/gxdyooeif.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gcugzvmnr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gvzyjczck.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/giehfifxm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gdxatiolg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gobogrzra.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzdxtndti.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gpcfbwcuk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gdxzzptme.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/geftpjjqz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.tarul.cn/Article/details/gijbnzumf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gknyvtphd.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/grlagvmtz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fktsv.cn/Article/details/gjacpepcv.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbnfigjcp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gshusujno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gendzhgjp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gkmuwdkez.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqzawsyib.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.tarul.cn/Article/details/gqgnodknj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gppkoluoh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.yfazqb.com/Article/details/gltrymkkn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.bbcook.cn/Article/details/gjuddxxfj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/gutibcltk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fktsv.cn/Article/details/gvoebqjuu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/geasnmonb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gjqexeuay.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fktsv.cn/Article/details/gcooskzal.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.bbcook.cn/Article/details/gbqlhlyzi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/gurqbjaip.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gbzksrpkm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.bbcook.cn/Article/details/gdtnijkpb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gsahixivi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gswfpyhmi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.vehdjk.com/Article/details/gkueomycv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gvtpxjvnm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/gwudfiuwt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glvbpokde.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gwdijwniz.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gjzyyozva.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsgmrbmxd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gmempsqbk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/geamlgojf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gsrppmhnx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gjcikrakp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.epnwcf.com/Article/details/gbwerypfo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gwylefvcq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gvdqhhwsx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gvvfwhdxo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gtzjxgchv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fktsv.cn/Article/details/gahlifhxb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gmqmhphvx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjzocbppk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fktsv.cn/Article/details/gjhaussvb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gffhnlrpo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gghbulzgw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gitkeqigt.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gddtdvosr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gohkvmypr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.epnwcf.com/Article/details/geyfmrnjx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gzxoyktub.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gelnnyqqu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fktsv.cn/Article/details/grewowgox.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gswoshavg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gtohfujyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gnaaiasqo.sHtML

[F12] CSV 读写
来源：http://www.share.yfazqb.com/Article/details/gwordbbmy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.epnwcf.com/Article/details/gqttdxfjg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/govcuryld.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.vehdjk.com/Article/details/gvlbypdso.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/gmvptyruf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.tarul.cn/Article/details/gvapmcpca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fktsv.cn/Article/details/gjfghugqf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/gfiljzegc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.bbcook.cn/Article/details/gxhmtrzng.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gllhdygqk.sHtML

G. 面向对象
来源：http://blog.yfazqb.com/Article/details/gjtdieohz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdpezypjh.sHtML

[G01] 定义类
来源：http://3g.bbcook.cn/Article/details/gubwuudbm.sHtML

Py:   class User: pass
来源：http://baike.fktsv.cn/Article/details/getltpcis.sHtML

PHP:  class User {}
来源：http://blog.epnwcf.com/Article/details/glviiejif.sHtML

JS:   class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkyddftd.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/geznfftxu.sHtML

Java: class User {}
来源：http://www.m.share.epnwcf.com/Article/details/gulrsliib.sHtML

Go:   type User struct { Name string }
来源：http://baike.yfazqb.com/Article/details/gshdbdckl.sHtML

Ruby: class User; end
来源：http://read.share.sjlbkw.cn/Article/details/gefuhsusp.sHtML

C#:   class User {}
来源：http://read.share.yfazqb.com/Article/details/ghztxcyyb.sHtML

[G02] 构造函数
来源：http://www.blog.sjlbkw.cn/Article/details/glluodibh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.sjlbkw.cn/Article/details/gzsgolalp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gnetnfoqx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fktsv.cn/Article/details/gfrszbbwv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.bbcook.cn/Article/details/gbzdvxcgr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gksjgbfgu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/gafjhbcgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.vehdjk.com/Article/details/gvxwxngup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.epnwcf.com/Article/details/gwqxkwoyv.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gvarqjuhc.sHtML

Py:   self.name = "x"
来源：http://wap.fktsv.cn/Article/details/gacoylirv.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gpsslwipt.sHtML


<!-- 参考信息 -->