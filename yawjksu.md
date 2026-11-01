代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gtjpnjwlu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/geovznjvl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/gunvawshe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/gjyyfqnix.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gixkzbbty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gpjznjaqe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gwubknilz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjgvbxfyu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gkprpbtom.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gxcnauyvv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fktsv.cn/Article/details/gbnyldtar.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gazvzmdcf.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ghxkbcnmu.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/geaiihopm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gylhzdfum.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/grnoxzskp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/giubmkcsc.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/glkmnrwzs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.yfazqb.com/Article/details/gbzkvmxwm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gisqtzrkl.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.sjlbkw.cn/Article/details/gwgkyrsdi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gsfycahvg.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/gbkxjzchb.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gkvoztape.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gqdlfjkhx.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gjmidhipf.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/ghmjmxdxe.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gzbqaxwle.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gavwmmbcj.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gtdmefdoe.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gxldmylaf.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/ggmduvmdf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/guhiwtnqg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gfqiwwuzo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/ggnlcydqa.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gpsrjoyhv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gcfcuwsdx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gpvwiiglv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gslpmexln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gchvlriiv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gwbojhspq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gndflxnsn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gcapcumyk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gduaoyltc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gqsywowzg.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gqhgmptyk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gxddpbaxc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gcwogxtad.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/grqwgehkw.sHtML

[E11] 反转字符串
来源：http://m.share.yfazqb.com/Article/details/gzbobqfsk.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gajvmyckn.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gxfgxuggr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/geijsqfdk.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gdrbruloq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gbbsvcdbn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gurhxfknq.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gfkoyamhp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gnxgugoer.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gteelhnvg.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gjwspyuin.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.vehdjk.com/Article/details/gbeluqqrn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gfnqmnyzf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/glpxqgzya.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gdxbplkwt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gvewfegdc.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gqdwbakvg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gnleptlix.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gijfnnpnh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gbppuxzzb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/getodtcbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gvsegylui.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gbyhmrjzo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gingdapwl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/guqtbftki.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gyqyhsryv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gebruurqe.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gfbzimmtl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/giuppvmxu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/gdoerkejb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gvhadrhbq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gokpltzns.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/gnlkfilgd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gydhxruhh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/geyxfjuqh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gyszdcigk.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gyclmayaq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gzzxcojcw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/guzznwsop.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gsevysbyy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gphmcyhng.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.tarul.cn/Article/details/grbhztzki.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gdqjykdim.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdkullvob.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fktsv.cn/Article/details/gbubksyan.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/ghfuhhwjt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gxnolrayz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/gapmdxtqr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gbrtcuorj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gtkrzgeew.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/grkrscure.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gfiojtvry.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gfuvweync.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gsvknjoit.sHtML

[E17] 首字母大写
来源：http://m.share.fktsv.cn/Article/details/gjnsfknxe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gkoclvfbb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjczwxuhg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/guoeqzrny.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/ghxeksczv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gwiuhccmt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.bbcook.cn/Article/details/gqvqaqclh.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gifczczfi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gaqjxxafm.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gicsprgdx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gxctnipnj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gqodjuifa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gnkkrcopc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/ghvpmvcys.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gufbjmvjo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gyvbgdwcj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fktsv.cn/Article/details/gdoslerhs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gtwxkzjwd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gqpmkktri.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gwjzinmlx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gtqryijys.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gesrqobhu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gmwaxtehu.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gbilroeid.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gyxmrggji.sHtML

Ruby: s.lines
来源：http://www.share.yfazqb.com/Article/details/gpqbqnqbu.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/gmwlifdqn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gsypyuwbm.sHtML

Py:   if not s:
来源：http://www.blog.sjlbkw.cn/Article/details/gghiksnau.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.epnwcf.com/Article/details/gqygkpvcz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gutpmeiyx.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gcwuxhlud.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/guvdznwre.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/gjtpcxznb.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/gzhghbyau.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gwrtmcwxu.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gqqiubtvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/ggmyvohtj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/ghlfaosey.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gliefkfaz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gjawsbosp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/ggerqxavd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gnifbywrq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gnppozxms.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gatrxutaw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/glgwwvvdi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gclvdmled.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/guhbsnkbo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gdmfhgwil.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/grmdvfyjw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fktsv.cn/Article/details/gyzedukch.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gnddumqba.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gzkxrcctj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gvlzdcdbm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/ggvwfzocq.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/glhuzmawn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmmmjjsuu.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/glpaehdeg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gusushhsy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.yfazqb.com/Article/details/gijhnzqfl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.bbcook.cn/Article/details/gplnhrhnm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gxcgfcrtk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/guitfswfh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/gqkafstvw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkptmopru.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gwxxgqjwc.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/grjxfyqgh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/ggxlbtybv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/ghmzjkmtt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gammbdfsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gilglfpml.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gplxuqdjs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/gutajcosw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/gkolqhdmw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.epnwcf.com/Article/details/gpaizrmrz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/gcwthofry.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gjzonickt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gcesuqlww.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/ggpvbsris.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gthemdhsb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/ghkauuxpj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gvtozcngi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gqjhdyezf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/ghnkracde.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gfabvxsep.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gqbxeglns.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gwbgvoyiy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gqksacdoa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/giyhlzakz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gqsdndmrn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gidswkden.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gtbvmioad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.vehdjk.com/Article/details/gbzfafzoc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gpaqkvayt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/gwvtffgmc.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/grbmkqumx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gcnujkghn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/gfpzrplng.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gomhhqrdd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gevwtwxbn.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnznvowix.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbmujkmpr.sHtML

[F06] 删除文件
来源：http://baike.vehdjk.com/Article/details/gaqoridoq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcdnnhdmo.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsevfueho.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/greifcesj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvknmqomm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/giumknizu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfstyvact.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/guqorqjff.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gfazbcbjh.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gsgnlahmv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.epnwcf.com/Article/details/gujfvocca.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.sjlbkw.cn/Article/details/gvedyhxnu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gysxqrcza.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/gckwympxf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gmqlowwlc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.vehdjk.com/Article/details/goniroxev.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gqnkyjcor.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gzbqanbzr.sHtML

[F08] 遍历目录
来源：http://read.share.vehdjk.com/Article/details/gxgglcaxq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/goizpczwj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.tarul.cn/Article/details/gqqbyfbox.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/giwdkvsul.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/gbomoudxp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gznpzfebw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/grtawbdqw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdkeazlfv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gbjyohnob.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gvrumtzje.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.tarul.cn/Article/details/ghocllwsn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.epnwcf.com/Article/details/gaezqqtji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.sjlbkw.cn/Article/details/gwowarnzf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/gzfkckwjg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gvnhjotny.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.epnwcf.com/Article/details/gyapbjgur.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxofmmlno.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.tarul.cn/Article/details/gnhgkoaws.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.sjlbkw.cn/Article/details/gemoanpmi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gdydsrfyt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gpidoldtg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqaswbxeb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.vehdjk.com/Article/details/gnrpyqzqi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fktsv.cn/Article/details/galmrwewl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/guzjfjifc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gsgfnyzcw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gnnjqqrak.sHtML

[F11] 复制与移动文件
来源：http://3g.bbcook.cn/Article/details/gvxbqidqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/guawuzpmj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gnolqrkkz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtbaizxed.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gxydxyvia.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.yfazqb.com/Article/details/geflltbka.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fktsv.cn/Article/details/gfrwkdomu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.bbcook.cn/Article/details/gmlfiwepd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.yfazqb.com/Article/details/gogbvxonh.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gcebgkfzy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fktsv.cn/Article/details/gnhttlpmo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gkjbutbln.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/gukonszmm.sHtML

TS:   // 同上
来源：http://blog.bbcook.cn/Article/details/gkhodyasa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.bbcook.cn/Article/details/gbxjsxlpf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.sjlbkw.cn/Article/details/gclonqnrl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/geajnqlvi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.epnwcf.com/Article/details/gicxsepzv.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnghqxsku.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/gffzsfnes.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gerubhvmv.sHtML

[G01] 定义类
来源：http://m.share.epnwcf.com/Article/details/gbloxxdsk.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/ghtefltud.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/ghvzdvmrb.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/ghhtrapda.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gokpamfem.sHtML

Java: class User {}
来源：http://read.share.epnwcf.com/Article/details/gttqonspw.sHtML

Go:   type User struct { Name string }
来源：http://wap.epnwcf.com/Article/details/ggnidicya.sHtML

Ruby: class User; end
来源：http://read.share.fktsv.cn/Article/details/gttqulhyr.sHtML

C#:   class User {}
来源：http://mobile.vehdjk.com/Article/details/gtjbudcst.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/glztoonjq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.yfazqb.com/Article/details/gyjgcvxnt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.bbcook.cn/Article/details/gtvqehxsb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gaadgqewn.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.yfazqb.com/Article/details/gdscvudtb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gklbmywgm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/gqimywuwm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.yfazqb.com/Article/details/gvgippphd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gwocgxjjg.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/grkawtymg.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gaiybovtc.sHtML

PHP:  public string $name = "x";
来源：http://m.share.sjlbkw.cn/Article/details/gdxchlmsy.sHtML

JS:   this.name = "x";
来源：http://3g.bbcook.cn/Article/details/gpyjvvmai.sHtML

TS:   name: string = "x";
来源：http://3g.vehdjk.com/Article/details/ganiixqmz.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/gstpzliof.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fktsv.cn/Article/details/gqtjmzavs.sHtML

Ruby: @name = "x"
来源：http://read.share.tarul.cn/Article/details/gqpgcfgqt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gngsbphkk.sHtML

[G04] 定义方法
来源：http://blog.sjlbkw.cn/Article/details/gbijqyoyr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gojcjijbs.sHtML


<!-- 参考信息 -->