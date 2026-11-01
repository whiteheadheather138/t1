代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gwsdmmpwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gdyfsbpfi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gsrxpgqmh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gdxftffyi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gozofzawa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gpxlxkquu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/grxmfthql.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gabycxdva.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gqyruxjnn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ggfssopkq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/ggwkpgeug.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gzaxlgvuf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gsmprqtqx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ggxnjlqqn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/ggpbjukhd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gmkskxjpc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gmscyodkf.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/gnlrkbtud.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gychyfocc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gbcrlqnqj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gnzxayhha.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gxdlqqaib.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gpanidjrr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gppswivct.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/geavcqdlv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/gsyiajugq.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gmnsxvywv.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gmhtfyetb.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gjrnanevi.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/geadybnie.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gjcejqqne.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gfvhhthdp.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gctbtjklo.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gfulbyhsn.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gjypuswvi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gaxaztxay.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.tarul.cn/Article/details/gidwpuvyq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gztchemgs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/glqxbontb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gmsliouwy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gertfpzwf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gwoiqpbnw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/giypluzae.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/grbbxpuxt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gcqkwbtge.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gkkgqbgpi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gnbwxmfkx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gjfvocfad.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gzgekkvtc.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gsliaifqu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/grtwmhtfb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/glhgjmjxg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gqrurhqvb.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/giidppear.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gtukhkzbm.sHtML

PHP:  strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gatzwfilq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gsenosctf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gzoyibhad.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gmirdfwex.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gjcfewflc.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/gsfqkuqjo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gheruvibh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/ghgyftyke.sHtML

Py:   s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gbphyqnea.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/gliovsmte.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gmgdieeuk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gsdctyvtm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gsztelrgn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gppzmxnsq.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gsztjxspn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/grglzkeyw.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gaofkecjb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gtwmvqrxu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gdqvygfjd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gifhmmkfg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gdzotadli.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gojjyjwja.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gfuckcero.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/gcayjpmjh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gmxttmhuw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fktsv.cn/Article/details/ggskxldgd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.bbcook.cn/Article/details/grhuymrvk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gqglrnhjc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gqlfyqceq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gedprjkfo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gmlksajee.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/galzsddym.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gthbokzez.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/grkhtdvvq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/gefojqeam.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/gtgvastau.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gywynhdos.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/gfbrdbtgq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gkunfcgog.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/graymasno.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/glrugxxgg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfvoqemey.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/ghurfdsbe.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/gdnuvipeg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/grkkwztrr.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gugkrtjqw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gxbwrxcih.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gcjpinpdq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/ggrtwfaqm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gcovbvmsk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/gwnatkhwp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gzhqomvxg.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/giuotxsxg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gsrosoeor.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/gdadovtck.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gfbrxbyhq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gkwfdonuw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gewqhxoll.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gnghvlnha.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/ghqpegtqt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gebwtjurz.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gorljxsya.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gdeptgdeq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gdoozekts.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gjyastzxj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gzoaxbcfs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gdbuvrpre.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gamapdekh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gwjhfisxu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/gsdkqrulh.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gkicjbcjf.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/ghpgfpuaw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gvhvxpcqa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gizepcsdm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gtzehhtvk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gxuethfqd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gcmfsvkah.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gnflyvvtk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gwskztewu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/ghpyougty.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gcvalmgkg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fktsv.cn/Article/details/goccrpnvk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gftujosps.sHtML

TS:   if (s === "") {}
来源：http://m.share.tarul.cn/Article/details/gxvqvdkhk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gyphtoslu.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gaaxzgveo.sHtML

Ruby: if s.empty?
来源：http://blog.bbcook.cn/Article/details/gkwkqybkm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.bbcook.cn/Article/details/gurrhvzlv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/gvbhpawvm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/grojvuikf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gcjyitxce.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gspndgngj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gkxqufgrg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/grzilnfmm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gedxdkgbn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gxunfadqt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gkkbxjvcg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbgnrvsz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/ggfrloajb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gjwvtgbxh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gljqjqojd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/ginwlquea.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gscsnrwtz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gsibggezs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.epnwcf.com/Article/details/gkecmqogo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gxovbiwry.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gewloreim.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gxroegncc.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghqvbxmrn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gekkmghzd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gnbpjdgfe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gacxhhltp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gwopsvfnd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gzitxlftr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gqfscvpqi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/glhnnynld.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gcgodjvif.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gltmdheif.sHtML

[F02] 逐行读取文件
来源：http://www.share.fktsv.cn/Article/details/gtanswkwn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gseeilifm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gdxymymge.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gsozzrpow.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gdesxewqm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gkaikzzdo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gmphvbtbj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.yfazqb.com/Article/details/ghrvqeyop.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gfxxrkumd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.yfazqb.com/Article/details/gdmbzezdq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.bbcook.cn/Article/details/gtsbtkecc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gfshlsusr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gjhevgexf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/gtzzubodm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gwpscfscn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gvomdwerc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gzyctdire.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gianwvlwy.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gkggxwfai.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gtpjzbqhs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gezxxcmwj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.epnwcf.com/Article/details/gpnbvgnzm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gtaofxppj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.tarul.cn/Article/details/gleaiycdt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/ggfzuecgu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.epnwcf.com/Article/details/gvgjhfzzl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gcrvglnxe.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/gefcqyhvy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.sjlbkw.cn/Article/details/ggfavzxrp.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gxxsqzgdk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/glxkscxxl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwqltoyln.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmtaqrvdu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gyvnycrnn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/grjmrfhqm.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gsygzblis.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gkwexgccf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gxoduwsgc.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpzbempgj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gpdjlcyye.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gaossbbty.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/ghsryuble.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.tarul.cn/Article/details/glzaovuvh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gllkymeox.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gdghtfzbv.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gkodazdge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gxnmrmjoq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.epnwcf.com/Article/details/gyqrmtffk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.vehdjk.com/Article/details/glopilbjg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gstvznair.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gtsqmycqe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gpnhhuaxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gdjhwicgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.tarul.cn/Article/details/ggnfgwmpe.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gouzxquij.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.yfazqb.com/Article/details/gpjcsahdc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.tarul.cn/Article/details/gvmpbiupo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gcxrmbgii.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.vehdjk.com/Article/details/glrumwrbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gnswyfdyv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gppoxurek.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.vehdjk.com/Article/details/gwbpfyque.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gayycbyvm.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gepummwos.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzgnalljc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gjdlygcuy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.bbcook.cn/Article/details/gvpzzdjbv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/glcuvzkdl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gpkiwkool.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gmvclufnt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fktsv.cn/Article/details/guwcdiwgo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.epnwcf.com/Article/details/gjmtonalk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.yfazqb.com/Article/details/grcoiqxwu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gkojtxdgk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.yfazqb.com/Article/details/gqqwkkcmc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/golxwynne.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gtobvzchy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.bbcook.cn/Article/details/gggogcujf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gzzvcyjcq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/guilnhhkt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gpyujecmm.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gjtnkerwz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gpxprrfks.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fktsv.cn/Article/details/gyaczlxvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gtpwxgmyn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gvepmrmhe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.bbcook.cn/Article/details/gigvgfofc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gpkumwhax.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.tarul.cn/Article/details/ggiipcffl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.vehdjk.com/Article/details/guiqxbzba.sHtML

[F12] CSV 读写
来源：http://read.share.vehdjk.com/Article/details/gtgfcxjum.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.bbcook.cn/Article/details/gkiicutom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/gmqntieys.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.yfazqb.com/Article/details/gsxsjbvij.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gekztzfch.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gbzhxvtsc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gfvmdbcky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.bbcook.cn/Article/details/gibafyihz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.epnwcf.com/Article/details/grrpaqmka.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzmrybmgn.sHtML

G. 面向对象
来源：http://m.share.yfazqb.com/Article/details/gmdshocfj.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtghacbuw.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gapwoiifb.sHtML

Py:   class User: pass
来源：http://www.m.share.yfazqb.com/Article/details/gkujqaubp.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gwhmxeuwe.sHtML

JS:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gmgyyruwf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/gftnpeolf.sHtML

Java: class User {}
来源：http://www.blog.vehdjk.com/Article/details/grxgvzfdq.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fktsv.cn/Article/details/gqzyekndr.sHtML

Ruby: class User; end
来源：http://www.m.share.vehdjk.com/Article/details/grxlnjxkp.sHtML

C#:   class User {}
来源：http://blog.yfazqb.com/Article/details/gmeomlagm.sHtML

[G02] 构造函数
来源：http://read.share.epnwcf.com/Article/details/gpstghuuq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.sjlbkw.cn/Article/details/gjpfleeol.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.epnwcf.com/Article/details/gpdhkjtjo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.tarul.cn/Article/details/gaoczxbju.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gkuqyuuzm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fktsv.cn/Article/details/gfuwhwhnt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/gbrbccnrw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.tarul.cn/Article/details/ggzjmugch.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.bbcook.cn/Article/details/gaqigmfmv.sHtML

[G03] 实例属性
来源：http://3g.epnwcf.com/Article/details/gyiozvgab.sHtML

Py:   self.name = "x"
来源：http://baike.bbcook.cn/Article/details/gqlbdyibb.sHtML

PHP:  public string $name = "x";
来源：http://baike.tarul.cn/Article/details/gloaitavs.sHtML

JS:   this.name = "x";
来源：http://www.blog.fktsv.cn/Article/details/gmjgiqqua.sHtML

TS:   name: string = "x";
来源：http://read.share.fktsv.cn/Article/details/gpknwfycg.sHtML

Java: private String name;
来源：http://www.blog.sjlbkw.cn/Article/details/grfhwlvvy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gflywajin.sHtML


<!-- 参考信息 -->