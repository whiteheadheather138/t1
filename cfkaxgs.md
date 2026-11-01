代发 wailian999

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gjxpvbhig.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gsgiqwlny.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gmfupobsi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gjprnauta.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fktsv.cn/Article/details/gxspawxrs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gtigsfgmu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gemzgwmig.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gqqamnqmm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gcypzrabv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/ggrvgqfyz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gmnndmljs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gyhwzhrav.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gbgjvwbxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gbrpyaktc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gonbbpljr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gllndfxwf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gngnzvvwr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gznlomlgb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gdujzayni.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/goddohhuj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gooqhsodp.sHtML

[E07] 按分隔符拆分
来源：http://baike.yfazqb.com/Article/details/gbkckypsz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.epnwcf.com/Article/details/gmaddvpsf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gjedgpqab.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/gtlvaduel.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gwqyseyhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gvrgknotf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/goeueehtv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/gyaqriwpz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gnugrfidh.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/guxtttpyr.sHtML

Py:   ",".join(items)
来源：http://blog.fktsv.cn/Article/details/gnsuhwuvn.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gelbbcnth.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gulcsrqgg.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gicdcujth.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/glmsjqosa.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gwlswtcvg.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gkzoqmlqe.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gpoqietrz.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/glskidgpk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gpvgjcxiw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gthtorrne.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gydgddiim.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gfhfbqyyf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/geqymojsg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/ggkhwrqwe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gxfddkqfn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gsuxgwhea.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gzlvnqwmo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gicjnlpdp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.tarul.cn/Article/details/gorjrfcwv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gjildznrk.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gokneqpuj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gafwmhyrv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gqhplimcz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/grwwvmpfx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gdbomeckw.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/gtapeluiu.sHtML

Py:   s[::-1]
来源：http://blog.yfazqb.com/Article/details/gbxkvofev.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gcadyhevp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gcxrfaexr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gkorybfyw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/ghpovixsi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gneqxscyt.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/geeueecpt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gzbzkcsnu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gdbxjjden.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gkmgsuxwc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gaegbrjyl.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gaicnyxwk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/glaqpvusz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gbylmpseq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gfunqkqei.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gbnenpaaj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gwnwubaon.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gxsjcwffm.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gmgjujsad.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/ghmifkqgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gijgbrilh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gvuoxmcdv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gqacwdtdu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/geujvizgc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/gpwghiels.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.vehdjk.com/Article/details/giwzbwnhc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/ggofhhjcg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gexkszxxy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gffkeuhjs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/guymgdcan.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gnjizwiqs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gogpumpck.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/goqcngaae.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gshqzdlsg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/ghykoxdlr.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gysdkajbs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gnmnfteka.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gmjizndsa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/gmzltfokw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gwuvrmyqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/guyvgauub.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gspxvnuyu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gsbnbjmwt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gfgeyftda.sHtML

[E16] 数字千分位
来源：http://3g.fktsv.cn/Article/details/gkyuqzulo.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/giesxxhgt.sHtML

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/gwwfpbroy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gwvjnxoab.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gvwtxqykz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gclycxqae.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gchooqgul.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fktsv.cn/Article/details/gloyiwjwk.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/gppmksorw.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/glegdgeqt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gxautiofe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gjefffhdj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/gogyvnoyw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gawicpvhd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyuhpmtfz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gwgtvddgy.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/gkxisxfld.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gjsronmol.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gnvinyolv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gcpgitsmg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gcqwwtzds.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gclqcjkpd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gjsmnncuv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gxtfmpzyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/ghenzzhgk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/gyikndnvk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gobamufry.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gwvclisce.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gwfbbsslw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gpjuotbnz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gbdaksrtr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gepkvzzll.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gaujigpsw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gxkvsfvfj.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gnsiwhwrd.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gxmmtfymx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/gshajaggi.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gwhunfwlk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.sjlbkw.cn/Article/details/gbxdsocii.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/ghtkujuld.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gdvyzrydw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gguhhgckt.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gpisqwvyt.sHtML

Ruby: if s.empty?
来源：http://3g.yfazqb.com/Article/details/golahldyy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gcjgwmsst.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gnnryiail.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.sjlbkw.cn/Article/details/gnglklvdc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/givhqapgn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gexnshibe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gfktxnwzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gohhkzomc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/geipqwxoz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gnavyyqzv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gmgdqayhn.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/gzysqrqle.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gnyapdcww.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gqpolfhws.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/guwkxfuxh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gywsodboe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fktsv.cn/Article/details/gvkpfgfzc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gfcxvnkcy.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gzchntlon.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/gjpbvprtv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbotmpoxn.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gqwdfemzg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxchesklm.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gxvyvcmdc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/ghqwoqnpq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gudhyoxyj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gllnesevd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gnwnjbolu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gfytvzlyy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gutltdadi.sHtML

Ruby: File.read("a.txt")
来源：http://3g.yfazqb.com/Article/details/grrijxepz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gnimbvoen.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gtiyqxddl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/ggvqptxqe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gatmhqmid.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gxvqezqil.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/ggybcrrun.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzwxjkkvb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gpwyzfvgs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gknrqosdw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/guvrhtsws.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/gaefkjthy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gsgovcggf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gbspqhfkw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gekeipkvt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/goozuoaik.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gppwjxumn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gjmtiqztc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.epnwcf.com/Article/details/gnbbzajlx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gffdltity.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gnbisqddt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/geletyxcq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/gijpamoic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gwkupxhcf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gtxrtgoiy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/ghhmlmcum.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/grmxtypzs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/ghgfuoero.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.vehdjk.com/Article/details/gnfisdjoz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.vehdjk.com/Article/details/ggwfyicoh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gkxidxjhw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.bbcook.cn/Article/details/gonvtkwjn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gevmymsub.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gyokgivjw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gpycxhvnf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/glpsgvygj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gmmlmrfph.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gzpexbmuy.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gbxrvmbtr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvhpdkhog.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gzcnkvgqw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gseycaant.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxbvshsws.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/goztuaxwd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtraqtvyw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvfovhyts.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.bbcook.cn/Article/details/gfdmlvmhe.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gdybjcdrp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gibweamyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gchpqvuuq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gygmkgwpn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gidpedmya.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.tarul.cn/Article/details/goxpqtgmb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gxfenkyox.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.epnwcf.com/Article/details/gqoswybwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.vehdjk.com/Article/details/gacfpeauf.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gfwhdlrmc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.yfazqb.com/Article/details/gcduyrram.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.epnwcf.com/Article/details/glkwgcept.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gwnssykfs.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gtmnbalrq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gewepckfs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.bbcook.cn/Article/details/gvbpxptwa.sHtML

Ruby: Dir.children("dir")
来源：http://blog.vehdjk.com/Article/details/gqezlnldy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.bbcook.cn/Article/details/gfcmgwmzy.sHtML

[F09] 获取文件大小
来源：http://blog.fktsv.cn/Article/details/gnqtwnubx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.yfazqb.com/Article/details/gczlazkvh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.epnwcf.com/Article/details/gkfhiaikj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gfxkuakwi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gmtrmjfjc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gipbfkkuj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.vehdjk.com/Article/details/gpplwsktx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gvkwgrjnf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.tarul.cn/Article/details/gwhddourj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/guxnrkdok.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gdudpxpbs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.tarul.cn/Article/details/gaassikbz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gkjrfqspa.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzftrqmlb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/gtgginxpk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gutsqbjbp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.yfazqb.com/Article/details/glbqdlhai.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdrfdbwzt.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gdydtrdqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gitbrjrdr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gfzvwgdpc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gokdfoexj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/gjsguwqwp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gglnhdukj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/glmebxsri.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gwthyhqrk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.bbcook.cn/Article/details/gkqmnaaiu.sHtML

[F12] CSV 读写
来源：http://read.share.tarul.cn/Article/details/gveuculnb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gjuezgfqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.vehdjk.com/Article/details/gblupffgq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.yfazqb.com/Article/details/gjkwarixy.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gwnvzlptk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gjtksuogv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/ggzjkojgd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.yfazqb.com/Article/details/gyysjcywx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.vehdjk.com/Article/details/ghwlbpnge.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqbuogbte.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gtbpuhjuv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gfqyepbhm.sHtML

[G01] 定义类
来源：http://www.m.share.tarul.cn/Article/details/gzvxhxbqd.sHtML

Py:   class User: pass
来源：http://read.share.epnwcf.com/Article/details/gpybjhbmp.sHtML

PHP:  class User {}
来源：http://3g.fktsv.cn/Article/details/gzkbtfwrt.sHtML

JS:   class User {}
来源：http://3g.epnwcf.com/Article/details/gqkxxmtox.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.epnwcf.com/Article/details/ggjuooaxy.sHtML

Java: class User {}
来源：http://baike.vehdjk.com/Article/details/ghkquydpv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gekaonzwx.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/gvempdjrd.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gxdbxhzmz.sHtML

[G02] 构造函数
来源：http://www.blog.fktsv.cn/Article/details/gshuhbhrl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gqsooggnh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.tarul.cn/Article/details/gxvhtrhgy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gpgwwafoy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fktsv.cn/Article/details/gztowyuar.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gsmikbdve.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.vehdjk.com/Article/details/gvongoqan.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.vehdjk.com/Article/details/ghrdeoxdy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.vehdjk.com/Article/details/gvlabbscj.sHtML

[G03] 实例属性
来源：http://wap.bbcook.cn/Article/details/girkcwsuv.sHtML

Py:   self.name = "x"
来源：http://m.share.sjlbkw.cn/Article/details/gldpofenq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gifmjefbj.sHtML


<!-- 参考信息 -->