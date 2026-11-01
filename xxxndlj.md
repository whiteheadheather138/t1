代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/gsdvmafek.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/gkiegrxql.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.tarul.cn/Article/details/gqczaqcin.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/gmhnclast.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gyzcaxcqx.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gctmaugao.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/ghagsoebt.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gisedhidh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gvwwrljsl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gdpckrduk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/gktclklbq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gqvxxfilx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/gazportev.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/gkhpyvngb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gfgywcgxl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gmszmcmks.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gumhlkfcq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gyuqrcbsj.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/ghmnugymz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gjqkfddjy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.vehdjk.com/Article/details/gbmfonlrn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/grixptscu.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/geijujtwo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gpcqeleyd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gdmlzaanx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofhbhatr.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gdxqoestg.sHtML

Java: s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gnzhhhtkv.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gewmofcav.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gxthmuhyb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gllguaydf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gpclpgqmf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gtjgcukzp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/gkjejspxp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gfthlcapu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gdbwvvjqr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/glavixmkq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gghpjzwop.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gqulyeobw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gwlpyjjfd.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/grpfavfgc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gmdwmcamd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gzesppvzp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gzptjxakz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gdevzlyux.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gizmnjvmb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gdxpiitxh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlokbyne.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.vehdjk.com/Article/details/grshslfdt.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gtsnlzljo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gshpyvfcw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcoufjdh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/gawzvgyib.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gcbuhyvmh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gcaopviif.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gxrgfxyjp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gjzuujfdw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gkzqbuoqc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gbbphgygw.sHtML

Py:   ",".join(items)
来源：http://www.share.vehdjk.com/Article/details/ghzpjlzkl.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/golaoqnsi.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gskjewcuz.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gztfjlqgl.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gwiarqpqc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gfqcspcdw.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gwdqbqnyo.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gaqogstzt.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gfzwifafw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gqbogbmqs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gewtedtyy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gpsqdgicc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeqfrjwq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gbbfjmdkt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gwivynlsq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gnfdtmuhj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/ghynmauxj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gzllkefdp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gzwrddftq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/ggwaweymz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuvdamvt.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gkgqtstma.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gdjtqncbf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gyryradzp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gztbvmtcz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gihfeneld.sHtML

[E11] 反转字符串
来源：http://www.blog.fktsv.cn/Article/details/gpiluruma.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gdbybwnkq.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gbtopwkwt.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/grkenfpuf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gorbbhvco.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gpnrfhjbq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gjmxktxnf.sHtML

Ruby: s.reverse
来源：http://m.share.bbcook.cn/Article/details/ghbxzdauj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gvphnecbz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.yfazqb.com/Article/details/gcezjkjtc.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gkntydera.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gppxrvbxj.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gxtpzsqtr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/grehkfgjz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/glqbjoknm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gkuzvxfnf.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gycjmqqhk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gdmbaunsw.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gfxjqmzdg.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gjtaenfzr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gffbixazz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gxfxfmvaa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gnxdbidfz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fktsv.cn/Article/details/gjxfavnfi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.vehdjk.com/Article/details/gxznewhlp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gfygthmst.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/glnjbojvp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.yfazqb.com/Article/details/guaelgnsz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/grqoanheh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/grofebccj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gplfrjlgb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.sjlbkw.cn/Article/details/gkjtuvihw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gvdjegzkb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/ghdabmebs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gknjpnhal.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.tarul.cn/Article/details/gazbrykxu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gktqkylgl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/giuvlepdm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/gjxfeocvj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fktsv.cn/Article/details/gizfckshd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gsyaijkju.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gpylvrkhk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/ghxzmegff.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gegqpneqe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/gomjambzu.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/gvtmfwhqa.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gpesgdhlu.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/gblnylpiq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gbbmfassv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gnzprtwvd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gzunfowbj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gmcwbxaep.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gjveqnvib.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/gxiigvzzi.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/grhsamnrg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.yfazqb.com/Article/details/gijokihuq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gucxwqope.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gqoafkitq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gxhkdzowb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.sjlbkw.cn/Article/details/gppapzaya.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gckrplucr.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gaghfxfpz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gduqebmco.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gpqlfxfae.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gbwuyeftj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/giewpylzd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gqiiqiqwz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gmabataxv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gqhvphpbr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gsveppatr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gfpwokfpj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gmfmzwldu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gdglormdj.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gcyclyehx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/genekwlny.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gpjornymw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gegcvmtdm.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gpamytwes.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/gcstdwiii.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/gsxhkzeuc.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gjbizwejh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gfjjubafp.sHtML

Py:   if not s:
来源：http://mobile.epnwcf.com/Article/details/gfnusmzhc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gainerjwd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gpzeztare.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gflyhijuf.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gvzsvkdny.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/godgymjmv.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gvpnmjggq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gotrzkzdy.sHtML

[E21] 超长截断加省略号
来源：http://mobile.vehdjk.com/Article/details/gqggaminp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gepemutuq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdyfszbj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gyqvadljt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gzezozobx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gjheqvbfw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gbmkelqrf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.tarul.cn/Article/details/glbpcxptn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gctefdmzf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gbmqtheum.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gprsthwik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gvjsifuah.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/ghgumfnyn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gifskkggd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gywrnunpo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.bbcook.cn/Article/details/gngmsrprj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/geixrmxwo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.bbcook.cn/Article/details/gmlkhgkyi.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggciwvpbj.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gtdacwsll.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gwawhwllj.sHtML

[F01] 读取整个文件
来源：http://m.share.vehdjk.com/Article/details/goklezipe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gsutsciys.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gtbjhriuf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gjwipfpov.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/glhbjddnj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gxqnvzbhc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fktsv.cn/Article/details/gxhoynzxa.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/grpokcvpv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqwkhinxp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/gwhecxqkw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gdejhqslc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gxvlngmnc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gamnsjcep.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gwqpmxdut.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/gobgsfunn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gobjjhsyb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.epnwcf.com/Article/details/gcvzlkdwt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/gyfgqetpz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gufetigyk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gvqqltcuz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gojgtrmhd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gjhavsfjl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gavepjkvp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gbqckhtug.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/ghnbljhtn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gtpzhrolj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gcfioeabq.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/gdygoofgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/grbfyssza.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.tarul.cn/Article/details/gcgtzcozw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gshxszvii.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gdukeaznu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/gfotczdvi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.tarul.cn/Article/details/gdqottidl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gqhymkcsl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gfgxwuetq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gvvjtritp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnoluqwr.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fktsv.cn/Article/details/gqwqrclxk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/geismgbik.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzkenlhzc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gxzgtirib.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gdqbqldfx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/goekspucv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gjvyshbwv.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/ghtwqxflz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ggitatkoq.sHtML

PHP:  unlink("a.txt");
来源：http://wap.bbcook.cn/Article/details/gtphkyqoq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gqiligcgz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdyvsuzmr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/ggvghtsvk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyrrhuclw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/geewkykzu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gettfcwjy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.yfazqb.com/Article/details/gzczhnhpo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/goocfczso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gsvdysapa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.vehdjk.com/Article/details/ghqnylgml.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gmkqrszpi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gwbaylcvt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.tarul.cn/Article/details/ghfybevkk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gatoztojh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gktkxncza.sHtML

[F08] 遍历目录
来源：http://read.share.sjlbkw.cn/Article/details/gwpgxqfzg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.bbcook.cn/Article/details/guliqsive.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gsaxcfuko.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gouycxttb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gnowkkqcw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gkzgnbstt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.epnwcf.com/Article/details/gottmzdxa.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gswunurxx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fktsv.cn/Article/details/gpqlxbprk.sHtML

[F09] 获取文件大小
来源：http://baike.sjlbkw.cn/Article/details/goybbejnw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gprduttev.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.tarul.cn/Article/details/gucakcxzf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/glkrobrgk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.tarul.cn/Article/details/gbbzjfugl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gsppzriov.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.tarul.cn/Article/details/gtvzmdcrr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gchflcbcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.vehdjk.com/Article/details/gyzjzocfw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.tarul.cn/Article/details/gwpypdqqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gljgbuwnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gcvdgyfqz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gxbctpgvx.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtczjzmvp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.yfazqb.com/Article/details/geqrpjith.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gvxbtmcho.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gwcdtjszu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gojsmshgw.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/grenymrwx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gxrtnoqxo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fktsv.cn/Article/details/gwrduwxxh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gheqooqmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdagidlmq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fktsv.cn/Article/details/gyrtyseda.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/glbnzdwwc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gulxbjozv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.tarul.cn/Article/details/gufoipmay.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/gkbqbqqdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gmderumiy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.epnwcf.com/Article/details/gwfshnaqv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/ggbjnguve.sHtML

TS:   // 同上
来源：http://mobile.epnwcf.com/Article/details/gklmjtsob.sHtML


<!-- 参考信息 -->