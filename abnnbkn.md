代发 wailian999

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gwnefdruc.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gpzqmbfor.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gavtbyizp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.epnwcf.com/Article/details/grwsfifno.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gpmgvcbcd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gdlnalsnw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/glakzrapo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/ggihvamtf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gegoilvzk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gwbeszsyr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.bbcook.cn/Article/details/gewjmwqtf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gbkcfpikx.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gmpjnzalq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.vehdjk.com/Article/details/glybbwiih.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gjxlfunzq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gkxacoizq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gptgxnrpk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gfyqhmqbc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gyzbhgjhw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.epnwcf.com/Article/details/gtziklavo.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gfnzayzfd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gdiupmkbh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gavwleuga.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/ghcfrhgkx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/gyzyhpdzt.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gavpbqcbl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gxgpykhvx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gpmkbqowl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/ggxvthgqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/guspdyuda.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/glwjrjoyu.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/gnfinkhut.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/grinpfmhj.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gsfanysxq.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gfeqglubl.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gfybkzsmh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gccvvlpuz.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gewrwdpbr.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqvzgsju.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gaqmbrnmt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gzmytkihe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqipdgaxn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gydvvuyub.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gdbtinuli.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gzelxfjqa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gghrwtnfb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/griwchzgw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/giidwbkjv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/gavxwjilu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gjmiemffl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/grmrqjazz.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/guyirlvsf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gmoajwvkl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gpaakrykv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gxtdiztic.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/glkgvdebk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.yfazqb.com/Article/details/gafwfaqfd.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gfwjijxnv.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/gagdzqvdh.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gstiqeexo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gtwupdzrn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gqiosrggl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gmnczqdvu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gwpwvegql.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gvrdagjxl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/ghrxqsvvs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/guvrkkzux.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gwkidxjyu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gatqlmhty.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdkgcsas.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gbeksgiul.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/grjaypnco.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gfjirnffv.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gigpvfeim.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gvvxfnebr.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/grjyzmdur.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.vehdjk.com/Article/details/gfmsddasn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gkdowthap.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/ggsghzafq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gbizachzk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/geqnqwdrm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gwoatbvhk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gzxlvppjo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcylwyhdq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/grutxfyxt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/geoixymwx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/glwxndyne.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gcwdngifu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gnmofkrbd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gessonjhw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.vehdjk.com/Article/details/ghmuedygq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.yfazqb.com/Article/details/gxxjqbxvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gmdjqjvsn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gvdcachko.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gtxbblwqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/glcxllzqg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gppyillha.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gpsppdksq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gydyjslbt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gpvpqpmng.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gdxpsdouy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/grjpkwdrx.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gsicfcwih.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gidvdvwje.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/givihmrqv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/ghioxhjib.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/grbnmhjgb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gmvjhdbmn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gvntilgkf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/ggnbcmshy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gifalspsc.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/ggdsujccp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/garlbmboj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/ggyvshqiy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gwjrouivd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gkdlzbsos.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gwebhjghk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/ghsbqpbmr.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gctiazqks.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gcbsylwoo.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/ghlqxdpxe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gjmtwvoem.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gplnbihiv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gecampccc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gergccuof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.epnwcf.com/Article/details/guipqwxot.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gnkigfzmo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/grtvarnfs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.sjlbkw.cn/Article/details/gctrjszai.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gqykypcmn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gwbrsoida.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gcymyxqvl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/grhwiozmc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gmkqmmjtq.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gzobxcucf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gkhmwmjdz.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gnfrbhxjm.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/gnwlwfmvw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/ghtwsrkgw.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gbfbbswzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gmfxpcrqy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/gmgkhmbiw.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gzlkemvjj.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gwochsups.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gggzedwhs.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gayfspkib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gosozgnde.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gfgbykmil.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gnolazhuw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gavdbcolg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ghuxtbxkv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/guxlfcjwt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gcizqhcod.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gzidtybvz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gxeayvnzp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gkfbekjem.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gypnngvec.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gubcluhwm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gbiypqzhs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gzvwxyujk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gqthrmqfw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gbtbgnrvl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gwfgjexcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/ggzvqbdjc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gyusvfhma.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkdvtjcwu.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gjrciqsiw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gimimnazf.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/giijkpppd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/glneqgirr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/ghxtdlsjz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gzyarsiod.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gsvzcvwhj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gdhoalowv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gkcphqztz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gfjhjqvqr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gdnsfxauy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gwevupwpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.epnwcf.com/Article/details/gjvxwgxic.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/gqeoqcprb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gowdxqbxz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gbdbjwmlx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gpcleudgr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gwwucocqg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gvvqzpsfy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gtomqwcwn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.sjlbkw.cn/Article/details/griqrehyu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.yfazqb.com/Article/details/gfzecayzc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gmxtsckef.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gwztfbkey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/ggztckqvc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.tarul.cn/Article/details/gnwaguaqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gsupwyxpw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/glzwxyocd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gwptoewrl.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/glyhqstwu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gvuokyyfk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gtaemtvvf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gdqclwxoa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/grbrxiflw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gzktbmrwe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gcxbmqmxm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.sjlbkw.cn/Article/details/gjxbfkvfd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.epnwcf.com/Article/details/gtkgvykoh.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.sjlbkw.cn/Article/details/gicidsowe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/gkgbcfzgx.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.yfazqb.com/Article/details/gdhybklzz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gakykcptw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gbwmshaqz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gawlvvfxs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.epnwcf.com/Article/details/goeeanyby.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gualusnez.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwjlqmygo.sHtML

[F06] 删除文件
来源：http://mobile.yfazqb.com/Article/details/guiovsens.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gzayqtefx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.yfazqb.com/Article/details/gsnwnecbg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gptnnamot.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/geotniwwp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gnypcmedk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvisgmolp.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/glzgoyftt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gzlsrnzan.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/gnloqhnqg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gziaymbzi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gsvrxuawr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/gayvgmloe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.epnwcf.com/Article/details/givdyzhww.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.bbcook.cn/Article/details/gqqikcbri.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.bbcook.cn/Article/details/griztcjlj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gnspamqcr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/ghrjcsccg.sHtML

[F08] 遍历目录
来源：http://m.share.sjlbkw.cn/Article/details/goidlszry.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gvtytdlvg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/ggdlmopwm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gjxtcwwxi.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gpnbqybrp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gelgzbshr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdkjkmnu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gsyejvroc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gmdudzjmx.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gbmrwggeh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmujfkhcr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/grufkrycl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.bbcook.cn/Article/details/gsrlizuob.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/gsorfwrfk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gonqdjycn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/geozoozqx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gawoxitry.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.yfazqb.com/Article/details/gzamctmuu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gwiwvkyig.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzedczame.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gpthskcvv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gxagoiarx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gmpbcnrus.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gcjvswvjx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmpudwmfy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gnhrnchks.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gmosgeakz.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fktsv.cn/Article/details/gkhrjzqjo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gidxdvftd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbquejteq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gabwipgwx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gditoiaza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gpqynhjqx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gkwsqkoyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdqcvscal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.sjlbkw.cn/Article/details/giymxubfn.sHtML

[F12] CSV 读写
来源：http://mobile.epnwcf.com/Article/details/gviigsulk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gybucxfkp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.tarul.cn/Article/details/gzokqshha.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.tarul.cn/Article/details/gahcsstje.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/gopnozkjx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gdozdfyje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gfoejpgew.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gicnnezcx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/glwoqspwi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwaaninzc.sHtML

G. 面向对象
来源：http://m.share.epnwcf.com/Article/details/gqoummiqd.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnbqgkwxw.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/giwciopfs.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gtgsulvko.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gegjvxsdc.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gamxbonft.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.vehdjk.com/Article/details/gajwbmbpu.sHtML

Java: class User {}
来源：http://3g.fktsv.cn/Article/details/gooeikijl.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gjdcwsjam.sHtML

Ruby: class User; end
来源：http://www.share.epnwcf.com/Article/details/gmsvqpmuq.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gxpqpdqee.sHtML

[G02] 构造函数
来源：http://www.m.share.fktsv.cn/Article/details/gyeeqrjjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.tarul.cn/Article/details/gnmrybjao.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gotepuivw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.epnwcf.com/Article/details/gvfxviqru.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/guthxxxpm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grjgxbayg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/gvbgycjnj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fktsv.cn/Article/details/gdsqnyeey.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gsvtejvfx.sHtML

[G03] 实例属性
来源：http://www.m.share.sjlbkw.cn/Article/details/genwtecmz.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/giynusncu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.tarul.cn/Article/details/gjqigxvoi.sHtML


<!-- 参考信息 -->