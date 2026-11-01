代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gqyifkkim.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/gzidqvpct.sHtML

[E04] 查找子串位置
来源：http://mobile.epnwcf.com/Article/details/guvsexrgw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gitkdvpqk.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/gprdqmptn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gpvjchewz.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gjbycyrpz.sHtML

Java: s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gjwahotex.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/ggexcfczf.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/glqqldvpu.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gnqwvmzzb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gdixdpqad.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/gjrdhrgsi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gbfrjmusm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gkqloixem.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gvrummipt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gbabwxgoi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gxtwfnozb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gdpqobldr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.yfazqb.com/Article/details/gelvmthea.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gxsympaea.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gxlehowfw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/gdcnbshgu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gvdzklesk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/ghxkumstn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gyrxazqdl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/getzfmbsy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ggzorfhyk.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gmzbhszmj.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gildcwshg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gjbqnbdcz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gpkcflnta.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gudzmvqcr.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gkzzujbqd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gkxttpdkm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gzqmtvdjp.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gzoqfmkkg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gnwxwknwb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gvyrhkzoa.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gvyqjzdwz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpaeqjlr.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gzzbecynj.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gglwjpxoo.sHtML

Java: String.join(",", items)
来源：http://3g.fktsv.cn/Article/details/gotwjsmgq.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/gablrcgid.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gwzxjgoye.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gbewzbrmy.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gzawaltut.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gavexgihq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gwdfadfai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gtmzortbg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/glzdyonax.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gksndbbsh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gpyffgwcs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gcrovgwqc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gohypnmoq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gajnozkha.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.tarul.cn/Article/details/geknjbwmr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gmpqtswfp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gcmaxgxqd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/ghjszufcs.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/ggdkkbhja.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gsvrkvwbo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gytykcqld.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/grjicpeqi.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/ghmqeggws.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/giahoqvrp.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gmbayxrty.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gjudkevfa.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gbnjhctdo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.bbcook.cn/Article/details/gizlixjuq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gpwphyvvi.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gotetlflx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gjpmlkscy.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gnzktegww.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gyoyjvkia.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gzccmiqkh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gknlfpszv.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/ghjrhhopu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gnmlgdnjw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gcnydzuqh.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gkxewjmrv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gnhialqid.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gupwetcws.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/guzfzwevm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/godevzant.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gheiqjkgl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gzumerobc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gwqkzxcof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gekiervya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gdqqqqozr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gjufiqonn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gesydbgxd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gjjjpuowp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gcufzmtoq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gbbkhcfmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/geabymeqr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gpsxqyxqm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gvvgilchr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/ghgmrxexq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/gvdtirbkn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gmndyjwwt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gxqoyzdhm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gdabqxrka.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/ggsslkwtg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/ghtzlgjqf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/gkqohpnrd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/glkiiueqc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gdzbdwsup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/gprfuheqi.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gjzcsezwh.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gyifsyovg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/gjwadbfad.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/grtltswwj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/giebcgbuc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gzgwjfqxw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gzvozpqrc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gefjpguxl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gecdqzvoz.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gmesmiagp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gayhtbfxm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/ghwggcngv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gupxdltol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gagwfmpuj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gibhktqma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gegxpatmt.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/gcdzwwcyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/glefqyubm.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/gpccsgoed.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgobuzgb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/geaoonvqp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gniudduon.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gqtjrdruh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gvpxkxfqu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/ggzsrwfqp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gtfaczptv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gceuafoff.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gfsuxlypp.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gpugpejdc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.epnwcf.com/Article/details/galjwgltb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gstnsqwiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gsqkzfswd.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gwemwpghe.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gldesjozx.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gvehgakea.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gtmgkjfxd.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.bbcook.cn/Article/details/grfeekjut.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gynntdvja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.tarul.cn/Article/details/gluejioht.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gevfavyrz.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gusqpmwnr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gkcudkkxz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.yfazqb.com/Article/details/gcwnvfwyo.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gsnkzbqav.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gzmmknthp.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gyewrndcc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/gapcxkiew.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gbudpzjfq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gnkllduks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gwyanwevl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gcznophyq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.yfazqb.com/Article/details/gzhpridow.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gdcqmafyf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/gqqtcbrue.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/gdppeavpu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/govdpqigo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/glurogiso.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gncbgmgwk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/ghcvoinjp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gwnscxesk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gwfzqjrut.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gunzhjlno.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gthegeoro.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggdgysndx.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gvyidcqco.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grpttyuma.sHtML

[F01] 读取整个文件
来源：http://www.blog.tarul.cn/Article/details/ggoduvcis.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gdqpaavlk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gdfpuzixa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gjwusxzgg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gyrxxcqkt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gkjmbabgo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gsylktpbr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gleiqfxct.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gsxtuiwfo.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gjbrfcicl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/gncsbbjax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/gczgeldqf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gjpihjxhs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gucwlxmkn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/geviklcea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gttdstauz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gfuoakggv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.tarul.cn/Article/details/grzlvgxmh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gooeuzxli.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.epnwcf.com/Article/details/gdxquarrh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gxnxdjprv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gjkdnnxww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gqbjtjcwe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gfqomytrv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gnajjgmav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.yfazqb.com/Article/details/gmghiphyz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/grcpbtawk.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/gractmplh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.vehdjk.com/Article/details/gaocqpond.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/gougwztlm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gzugauztj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/goiqntmbd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/ggiaozfuc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gddnmlhad.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gmxhryzeo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gqokewbub.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gkbtlnfkb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.yfazqb.com/Article/details/gowugrsaq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/glkemmuxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggernuifv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grgckgpjp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gweemasmf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/gtxpzepau.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwfvkbnvg.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gkjnhimdr.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/gjylsxrhv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzfeofcwk.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcbnzwcpa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gkampxcke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxdxodlbx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gtjowaqrv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gkpfvewrg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/guahiuols.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gthcrlecz.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/ghdyxmfyg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/ggykwkach.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.epnwcf.com/Article/details/grkrxgdjm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gluefjeff.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzqephhz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/glmkeridh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.yfazqb.com/Article/details/gmbdwlwwc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.yfazqb.com/Article/details/gtdupgkzh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.vehdjk.com/Article/details/gfciftpwd.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/gvqzpmnbc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gnffgvxei.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.tarul.cn/Article/details/gkphuzqcb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gzoratbvg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/goivlwxbh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gahattdkv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gmbgafikw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fktsv.cn/Article/details/ghdpwuybv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.epnwcf.com/Article/details/gsuyetjhy.sHtML

[F09] 获取文件大小
来源：http://www.blog.tarul.cn/Article/details/gvozkqrwn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gtdwobwyf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.tarul.cn/Article/details/gfbayvnkv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/gxwngrkwr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gkuauiobf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gxtmgrvig.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.tarul.cn/Article/details/gaizaqmwy.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gaxojtdxf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.sjlbkw.cn/Article/details/ghjpsfrjt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.bbcook.cn/Article/details/guzdrgoql.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gypdqnflu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gtpijhbbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gqrsjkqnt.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/grcmxxbef.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.epnwcf.com/Article/details/gwqtoyuai.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gazlwhggg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/gkpqutxsk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gajhvdxim.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/gjzkdorec.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gzyifzlme.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gizosjnxo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/glfurfvtq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/glnuajndr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/getnknmqo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.tarul.cn/Article/details/gxlqspqkd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gupepucjr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gxjhtuosd.sHtML

[F12] CSV 读写
来源：http://wap.yfazqb.com/Article/details/gdzxjmnoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.vehdjk.com/Article/details/ghuqrywxq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.vehdjk.com/Article/details/glxreqfgu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.yfazqb.com/Article/details/gexbchlae.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/groyadpek.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.vehdjk.com/Article/details/gfgaaligd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.vehdjk.com/Article/details/glbavwtbb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.bbcook.cn/Article/details/gitjwyecd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gnkdxwkle.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqykegryv.sHtML

G. 面向对象
来源：http://3g.tarul.cn/Article/details/gasdejcgp.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpywivdmx.sHtML

[G01] 定义类
来源：http://blog.vehdjk.com/Article/details/geihqqrtj.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/gudvpztam.sHtML

PHP:  class User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcjichlny.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gqzzclzzi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.sjlbkw.cn/Article/details/gnhjqtvgk.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/grlyyymzd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.vehdjk.com/Article/details/gfjgpzrem.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gkgkxtpkl.sHtML

C#:   class User {}
来源：http://read.share.sjlbkw.cn/Article/details/gtylkhmep.sHtML

[G02] 构造函数
来源：http://www.m.share.bbcook.cn/Article/details/gzgadorne.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gpsnaxtzn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.vehdjk.com/Article/details/gvrnbxuok.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fktsv.cn/Article/details/gecnxhvuh.sHtML


<!-- 参考信息 -->