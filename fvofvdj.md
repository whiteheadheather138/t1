代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gwwixlafo.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gaatnbufu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gmattocii.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/gjaodprho.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gqivxnuvc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/glrrlwjbu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gahflpqyk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/grfypypzr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gnriwcmoc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gemkaxvmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gzdgrgyig.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gkovywioo.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/glpzjuufg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gptfnjajx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gklgquilg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ghypcaeit.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwvumwohf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gaonvkzdb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gmvurvjxj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gcdqonccw.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gahrxjthn.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gxthpuzjy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gyggsgayj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gyvbvwkab.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gnwwfdjje.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/glsvfjbip.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gurlfnisd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvusxhsju.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gngjkvgkq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gtrwtpmhx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gvptftnev.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/galcadjhm.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/giccmuvsz.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gifnwggbi.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gkzmzzzun.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gjjffhkbm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gdcgwdqge.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gbemwuunw.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gwrifuvqa.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gwaplkruz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gqdmitfmp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gvcdeagta.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gumbjjiag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gragutkwe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/grzxfrdva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gldalbgvy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gipqtdoox.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gptlyueig.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gcyfndhkv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gmhdjyrum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/geqmzkhhf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghwbmaist.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gvbzxmztu.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gydylwios.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gozpfylqe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gwowpdbjy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/ghelzrjjr.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gosyspqrd.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gipuylija.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gzhkvwgfh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gnmrdzcbd.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gxgqrazyr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gbnroqmia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.tarul.cn/Article/details/gadtokddd.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gckgufces.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gutglfaaf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gyqhhbjto.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/ghwrpxpwo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/ggaiwhkdo.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/ghnrzbiwp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gqdmqcxdk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gmejpsicq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/gvcahpzrd.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/gqphdaijz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmvdtpzg.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gpsdgpjhd.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gafenoezv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gumtfvdyb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gftyqzrik.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gjreqbbyx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.vehdjk.com/Article/details/gruozxlii.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gcvtpnfyq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/geoelqcrk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gihriuoat.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gmzrirqjf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fktsv.cn/Article/details/gmwnhhnvc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gykukmpci.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/ggpdrusvu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gpixabhzw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/grtrswwjp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/giqlulvog.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/glfvaestz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gykjbehnd.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.yfazqb.com/Article/details/gndolnuqw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gjgvgkyhm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gdfiuowwp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gzezlacnp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gsregebqm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gfgbfpeyh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.tarul.cn/Article/details/gnkzevoyp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyunjvpqg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gdqsfpulq.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gldveqvet.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fktsv.cn/Article/details/gbabwijly.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/ghkyaxifo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gocnihruy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gbwximwob.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/galgecckg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gescgcmnt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gdlgyoaah.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gigiqmlqk.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/getrqyacc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gwrtfhwdc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gcjqnfurp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gcdhoebna.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gwdchuvkt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gtirawhqx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gwoadecrp.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gtbydqfej.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.yfazqb.com/Article/details/ggeirzuah.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/grvodmgun.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gikjtgcei.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gxfqtzxvs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gorwavjrq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gjvqneggd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gefeaaxgv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/ggkgttnzt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.tarul.cn/Article/details/gwvvfegxg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gpcnrtmft.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gdpjqvnjv.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/gfmezpdmp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gpobvlmre.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gbhbcglln.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/guvvcnzzz.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gvxjxpmve.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gztszqrge.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/gpivuenjb.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/ghythazlh.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fktsv.cn/Article/details/gcvyzeyfa.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gntxlntox.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gkejlbswh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gqpvdkhna.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gjxjnlsqm.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/griodsrwn.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gwjlqtytl.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/ggrlioutf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gjjybphru.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gdbirnlkl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gnvbgjdji.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/geztlxjzd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gsabbhfwc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/ghsqibfut.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gjdvmtpef.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/giamxspes.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gvaohzciu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/grhmkryoz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gyskswvub.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gwwurltfz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gotlzdxqb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/gtppljxlw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/ggdsuozbv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gedjdnree.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gibwdzict.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gjbhjtcrl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gkgfwmolk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/givykegot.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/grfnvkggz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvoouqjwl.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gzkezsjhk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gfsuhbqfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gywliwhow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/gslchnctq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gqshjkrmg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/grqlgasjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gvorqaqae.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gterfttre.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gwsinihrj.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/guwnldcdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.bbcook.cn/Article/details/gwzxqyjmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gwzjligfn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/ghaechhib.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpohzvslw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gbbhqhfyq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.yfazqb.com/Article/details/gblsnrtlv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gqbpgiwbx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gtwcuvade.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/guvwdowsg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/gpwusbumc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gkrgtwpjm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/genoxnfsu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/giowzncyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/gtfiknhgp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gjbrpzaaj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gbkkspvag.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtipcbpix.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gpqtsgzeu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gtgqdkzng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gczrysmqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gfbyqwqei.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gimioecgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gwsmuyume.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.yfazqb.com/Article/details/gxhbvpjoy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gumwqhcyz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gydlmesuw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fktsv.cn/Article/details/gmpuiagxp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gyhxrxqqc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gseedqcmo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcrpviifa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/glmslahgq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/ghfiedhke.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gncxhevde.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.tarul.cn/Article/details/gcbkbevxa.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtamhhehg.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gmmpodyoy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnjypiudl.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gfcqfqrlr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gilsdhbbz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gykpvnlrm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gezxevbql.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gazhucejk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdslahblv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/gqeigtkay.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/ggslpmxar.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gbncheeci.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/ghchljtbe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.epnwcf.com/Article/details/gfxgmrdxo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gwdgmcchf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.bbcook.cn/Article/details/gvqlagkti.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.sjlbkw.cn/Article/details/gkabuxzrg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fktsv.cn/Article/details/gvljmpckk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.sjlbkw.cn/Article/details/gfsdqjkpd.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/ggihifrit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gipxlvcpw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gybfjyeub.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/gympenoqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.yfazqb.com/Article/details/gbftwiqiq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gewhyzgil.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gsmdqgpai.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdqbdrfyh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/gnwiukesc.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/gsqyrxyyu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gjcymejws.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gqrwrvslo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gqojdxusz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.sjlbkw.cn/Article/details/gydghqqth.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gcgudethy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gogdxqtuy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gmbhxasnm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gwkhhwwbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gpjhxfejp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gsetcnzhs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghtnlzwae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gnwakdenh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gylqflxny.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.yfazqb.com/Article/details/gtnfqszur.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gnvvcjhll.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/guiyuktpx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gyouiptvh.sHtML

[F11] 复制与移动文件
来源：http://wap.sjlbkw.cn/Article/details/gsdehetyc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gmzodpwna.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gqevshggb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grwrmtiwc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gkfkumteo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gipdnzvom.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.vehdjk.com/Article/details/grvuysurp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/giaxoxpnf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.epnwcf.com/Article/details/gyaqcpkin.sHtML

[F12] CSV 读写
来源：http://baike.fktsv.cn/Article/details/gmsjhwqpm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.vehdjk.com/Article/details/gvsaozetk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.yfazqb.com/Article/details/gwuvtuqei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.sjlbkw.cn/Article/details/gyercrrbl.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gvpaifthr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/ggaubyajx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.tarul.cn/Article/details/gwxzqfvwh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.epnwcf.com/Article/details/gacgsehye.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fktsv.cn/Article/details/gfjevjllb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gusckspdx.sHtML

G. 面向对象
来源：http://www.share.bbcook.cn/Article/details/glawektox.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkcxnkfkk.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gkpzknhqn.sHtML

Py:   class User: pass
来源：http://3g.bbcook.cn/Article/details/guywrfdjz.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gumejaxjd.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/givwyptcm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.epnwcf.com/Article/details/gavwktjmt.sHtML

Java: class User {}
来源：http://wap.sjlbkw.cn/Article/details/gkbmwgtgo.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gxiebezkh.sHtML

Ruby: class User; end
来源：http://baike.vehdjk.com/Article/details/gycffwdfd.sHtML

C#:   class User {}
来源：http://read.share.tarul.cn/Article/details/ggtqnnxjd.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/gkjqxaxud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.epnwcf.com/Article/details/gkbqtcbct.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gvhgnjwaq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvwgmjxuj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.epnwcf.com/Article/details/ggfqgstdk.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fktsv.cn/Article/details/giwudjieb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gpszjuxsz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gffsusuib.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gvvpnawap.sHtML

[G03] 实例属性
来源：http://3g.bbcook.cn/Article/details/gdqhxwnym.sHtML

Py:   self.name = "x"
来源：http://mobile.bbcook.cn/Article/details/gzssearlt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gcvplmvuf.sHtML


<!-- 参考信息 -->