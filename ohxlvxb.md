代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/guwktehkx.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gfyihyqnm.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/gwwcqrsml.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gzchtoeir.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gecpxzybr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gtymduvsq.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gjqvskmby.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gtotbkska.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gpyotwuiy.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/gerkbeoov.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gaftsbotr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.epnwcf.com/Article/details/gwzolmewb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gycelkvsp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gsinxujhj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/guorqjscd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gcygdwpne.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gugswofho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/ggcisdbuh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gkhsggqib.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/glpywzcbk.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/ghtbthvbz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gjjtswffn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/glskjwzvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gsdozvftw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gzvwogici.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gwttgudjw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/ggaitnbrs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gzdytpkyv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gmewurilx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gtjobzahl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/guyyjthvz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gevhehobk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gsitztrvw.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gynhlokxi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/glxgkeokf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gtpdzbujt.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.bbcook.cn/Article/details/griscvrhe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gzjbrisey.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gfxoipliu.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gprahjaty.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gtdbzczro.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gbqkuvbel.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gcmlqxfli.sHtML

Java: String.join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/ghtukcifb.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gwawevvyq.sHtML

Ruby: items.join(",")
来源：http://wap.yfazqb.com/Article/details/gpyikbplj.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/ggchmlykz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gluufyjmd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gqmzgxpql.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gbykhtjhg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gsztguipj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/grpzuwjjk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/ghxpwfesb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/ghxjczuxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/glmqgxwmk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gwtbfbmbc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlcrgfli.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gktfhepwx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/glkengmbq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gqmvqizeg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gwypiznhl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gjhbmlhiw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gbbchbpiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gooluavbi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gdokzndff.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/goegutnok.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/ghqhfsrrl.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gvjmswvny.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gvamourqe.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gtzhiwklr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gdeypgmyi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gfyvlkerc.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/gjkiyzbwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gmmtzusxm.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gbxxfouke.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gfnzaylfp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/glwxyrknl.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gypvhybrp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gjjwpisbm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/grujdugon.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gjarywufv.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gsxlnxriy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/ghtldkhvb.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/gzxuqrwij.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.sjlbkw.cn/Article/details/gaghfyggm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gfkdopayi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/guatufzly.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gkqjaddmt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gdoirkfzj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gvuxzxygd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gzgootpix.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gadmxnlfp.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/grudpuusx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gxzkoslav.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gflxaqpns.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gdbzfdwhi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gcnzshhep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/guisitpax.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gigniftyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gcqpcbpqp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gicxbimms.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/ghurbrvkk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gtfpduvuz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gmvkgftyd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gsfayorin.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gslrrxwdp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/gbrucjgwh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/genxnmzkb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gezpyqqbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gmahaesej.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gqztbzkax.sHtML

Py:   f"{1234567:,}"
来源：http://blog.vehdjk.com/Article/details/ggydkdemd.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gmhrtdgsa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gcqxjgugx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gxlngtygy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fktsv.cn/Article/details/gwjxgerlm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/ghkxzwvlp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gxtfzxywq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gohatpkyf.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gstgkxnik.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gyqmuocue.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gixumibwi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gmevqgdqs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gffjjbkgd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gtbsszwhh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/gzjzqnaab.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gvkyzrtja.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gzohuaquq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/goaduscti.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gmwmfbzze.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/grfwextdt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/grqszgspp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gnlmpsgxi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gqapctpcq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gmvahwizy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gbjtjnbbx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gbvcdwjeh.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fktsv.cn/Article/details/gnahpvsac.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gyqornxmz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/grltyfkmk.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gvwkydduk.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gybyklgrd.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gfnteuqra.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gxqltcxmj.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gqcgaxyce.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gonpwvmnh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gqweebeoi.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/getgnvggq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/gwrdtfnfi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.bbcook.cn/Article/details/ggeqqvrnm.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gqqrsnzfs.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gwkrjmepn.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gdgyflwix.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gfwwrjhap.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gdfywhkwn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gosfedeqz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/grlwzjbkc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gesptpoih.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gkfyktftu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gthaivajg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gfxqxkmmn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/gbgtqnhoo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gwwkzvltp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gjrxkcvst.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.yfazqb.com/Article/details/gphhxhexq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gykgekskc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gejhaakes.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gqewnsugx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/glvdkxoen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gwdqydxjn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gpumqkayo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gxkmpqdhk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gatyuwjtb.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gebglmjix.sHtML

F. 文件与目录
来源：http://wap.vehdjk.com/Article/details/gurbyqzdd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gthxmamdz.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gayjtdejq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gitgreqti.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/grkafyhye.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gtvcfikdt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gdputwzbb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/glzeojwyz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gwxopunow.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fktsv.cn/Article/details/glxpdryyy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gobmiucuh.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gfjcvogiz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/glcjdtssl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gkqvbqypp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/girwfxbyh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gyhubfsbv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gjasfakuq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gcmlkpgiq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gnuhwuuxn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gzhscvynb.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fktsv.cn/Article/details/gsgojkesk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/gbcwaqzyr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gszyllmgc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gcvjzhbvq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gwdddnjal.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fktsv.cn/Article/details/gisxmzbop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/gytbtytpl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/gygnqzfyh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gvfbadysw.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gddrcvkqw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/ghoiajbjf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.vehdjk.com/Article/details/gtfqjgodz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/ganiuodfq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/glvdqxoer.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.epnwcf.com/Article/details/gtusimysz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gnlnukkhz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.yfazqb.com/Article/details/gfmpekgce.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/gdkrvjatm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/geqmgnvkq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fktsv.cn/Article/details/gffllsltz.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnlhtoxao.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gutgkcvcd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gnamdblgz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/guoljilsg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.epnwcf.com/Article/details/gbrvvyiei.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.yfazqb.com/Article/details/gteeakiua.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.epnwcf.com/Article/details/gxlbkcftr.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gtffzmmvh.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gokxdxsbj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gbevundtq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdfjpuswy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gurszudtb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gjlwfpfna.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.tarul.cn/Article/details/gmaandjuu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvjwxzjwg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfevdsknn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/graqxmgdy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.yfazqb.com/Article/details/gzrfeulbp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fktsv.cn/Article/details/gwvaxeqfz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gavfbacvi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.bbcook.cn/Article/details/gjbgizeff.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.bbcook.cn/Article/details/grkyagibo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/ggyrihwue.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gsmbhmnns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/gaephmmdr.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gczieynsq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gyyxvcdsa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.bbcook.cn/Article/details/gstjfaghg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gjfkplaib.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/gjoieotyl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gjbidhqzv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.bbcook.cn/Article/details/gmzklqxbd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.bbcook.cn/Article/details/gwemjnqnb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gujufhjex.sHtML

[F09] 获取文件大小
来源：http://read.share.vehdjk.com/Article/details/gawwenosv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.epnwcf.com/Article/details/gmfbqeqmh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gucldmiai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.tarul.cn/Article/details/gukiyardi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.bbcook.cn/Article/details/gmtzkbhkg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gvggfakcc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fktsv.cn/Article/details/giryaiupj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gopymzjie.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.tarul.cn/Article/details/gzwbgnzch.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fktsv.cn/Article/details/gxjekvcqf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/guccztkhf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/ghqbiwumk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gtxeyfexc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtedixzmg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.yfazqb.com/Article/details/gchygghct.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gtkiphiuv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.tarul.cn/Article/details/goskteqog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwzzxjvrp.sHtML

[F11] 复制与移动文件
来源：http://3g.bbcook.cn/Article/details/gzdqvzxzs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcawbaild.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.epnwcf.com/Article/details/guzfdjwkg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.vehdjk.com/Article/details/gcozhznkt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gadaaarvm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gycpumkwl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gzekapagr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fktsv.cn/Article/details/gnrnvbzsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.bbcook.cn/Article/details/gsrbzomvr.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/gealpmhoi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.bbcook.cn/Article/details/ghzejwxol.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gwvpbeqot.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gsbzliipv.sHtML

TS:   // 同上
来源：http://m.share.bbcook.cn/Article/details/gcfbdjnbl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.tarul.cn/Article/details/gluykgaqk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.tarul.cn/Article/details/gmmfxgikt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fktsv.cn/Article/details/gciasstuc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gbkufzkwo.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmuzgkqlg.sHtML

G. 面向对象
来源：http://www.blog.tarul.cn/Article/details/gdwpfogxe.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpfygjltm.sHtML

[G01] 定义类
来源：http://www.blog.sjlbkw.cn/Article/details/gnfgzarxh.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gfbtkijyb.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/ghtgddlfy.sHtML

JS:   class User {}
来源：http://wap.tarul.cn/Article/details/gchayxcyk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gokkkzvxe.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gnayezpax.sHtML

Go:   type User struct { Name string }
来源：http://baike.fktsv.cn/Article/details/grfzvbhle.sHtML

Ruby: class User; end
来源：http://www.m.share.bbcook.cn/Article/details/gtdwsjzda.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gfdjzmpxq.sHtML

[G02] 构造函数
来源：http://mobile.yfazqb.com/Article/details/gbojzhqyo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.yfazqb.com/Article/details/gsbyopvmx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gesdouiol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gprtevtcw.sHtML


<!-- 参考信息 -->