代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gdwfpadbk.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/ggftwxbnz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gvwjpyqug.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gzmyeaetk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gxrmvdiqk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gupakvbfn.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/ggnylulke.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/gfwatsqce.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/gtebymbin.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gvzcdozuj.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gjveflkoe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gknvjegjx.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gvjfdztyt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghinlihlt.sHtML

TS:   s.indexOf("x")
来源：http://blog.bbcook.cn/Article/details/gxyonvnvn.sHtML

Java: s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gamyolown.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/gmtxjkwjc.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gmexvfcka.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gibwlmbvi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gwqrjnodl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gwfydpqci.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gvbmynogz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/grrszlcrt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gnowhwemn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gonglwkcf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gnysizvgf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/garbqhark.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gzhkhpttd.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gniksnwyq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gfuavflso.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gcotfsccu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gfewhsyak.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gwwtfnowd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gfyavrlbd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gfsemwxzk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gecajikmz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/giwogvyvj.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gyssjgpmn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/ggqvtzuno.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gtdmgcuqw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gqmyuwttm.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/gverbjdlr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/grqbliswv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gqqnzztgw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gfdvhjgpx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gzkxicpfc.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gqindfoyg.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/gicosxwpz.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gpdvpyybi.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gbtieqmvb.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gpugwvicg.sHtML

Java: String.join(",", items)
来源：http://3g.vehdjk.com/Article/details/glwlqbhgi.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/ghjhnelrl.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gmhpoqlkg.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gkirzaxfh.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gyhkcadzr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/glywfdwdg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gxbfhxjjv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gzpohgjel.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gtmryjygc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gxwnarogg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gbtgdxuns.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gmneewedz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/glczgghry.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gmsjmgkru.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/grnznggqc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gtzcsfgfm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gxumhceyi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gzwmadnbm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gakzrxmem.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/guyupfhjv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/glvksxvwx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gbxglzaje.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gmsaxywuc.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gzegxcwdr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gjlhbauqo.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gjbvszvvi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkbyleg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gfsdieoqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gbjpwhsey.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gbxbbhlyp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gwxxdmwyg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gfufrbdje.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gpodnuzbs.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gpkndilpk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gekvmogvt.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gkhjuetff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gkcnkdrgv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gjbxaxlyg.sHtML

Ruby: s.count("a")
来源：http://read.share.tarul.cn/Article/details/gzpwquuvz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gdyaingtr.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/ggilagzlj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gbbkcuaoa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gcvlcgyja.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gscrjzmqk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gixmdwhzs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gdledfbfu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gplkcoucn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/giulxicga.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gxnzegdws.sHtML

[E14] URL 编码与 Base64
来源：http://baike.yfazqb.com/Article/details/gnnwvegoi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.sjlbkw.cn/Article/details/gaqxsnexc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/grrtseyyy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gtkdhbvhh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gpkgsbhon.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gkntmrdvj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.sjlbkw.cn/Article/details/gezmqhzqh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/getfbsiff.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gmukhswpk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/geibkrmis.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gnvuevjnl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gqqthsjib.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.yfazqb.com/Article/details/gzoamnqas.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gaqjxyzia.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.bbcook.cn/Article/details/gaeknpfhe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gxhrhegun.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gjjcettpf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/glwhuoioa.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gpgqoyrkf.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gclgumulp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gapvcsfed.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gwxgwefvw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gsctevwqg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gytbtmdaw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/geidwzalm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gjpwofqvk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gsklmikwd.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gnmlrxzba.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gpacxvuqk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gfmqpffhk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gfollqimz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gffoicwwh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/ghqqxdwql.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/ggffyonaw.sHtML

Ruby: s.capitalize
来源：http://www.blog.vehdjk.com/Article/details/ggphtovhv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gqjqjvxgr.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gxiiqjnes.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gtieomdtt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/grwvptikq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gsarggpsy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gfjyfpdck.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gmefhtiqc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gjorlfcek.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.yfazqb.com/Article/details/gtxdylhyp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gcsypjkmu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/gvlfchezf.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gxhzklmie.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/geyfdmpsc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/ggfabxqjm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gfmhpbebh.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/ggjrdoadu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.yfazqb.com/Article/details/gbwxngtuq.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/gaxcjocys.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gxysaptaf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gjfrhwtoy.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gqptaihgd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gxdzixgvz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/gcnxdfrej.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gqzkuklmb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gqbobbwvd.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gfvjrxrps.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gvfiphbqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.bbcook.cn/Article/details/gjnbryscc.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/gzzhhswyo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gpmnlaody.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gesmqurjp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbgagfeoe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gsphmhale.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gbemcsgoh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gavydmtzn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gkmxbibim.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gppbgjxif.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gdcafgpxc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gnpzodsjd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gwpruqzrg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gqihxltry.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gqvtmopag.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gcuypwqdu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.sjlbkw.cn/Article/details/gsbdkzqrw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gxluymfux.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gmtjvebss.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guqsqcthe.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gyvtgwwgk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbfjxnpes.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gajpavlxd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gagubqqag.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gdsqpvodj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gqaymusjq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gozbaxssl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.epnwcf.com/Article/details/glorlempq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gwjontomz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gwhelmukr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/grddhezyj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gswmhfmmi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gubkiqseq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gnjwsseog.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gdpqyalng.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyfhogexs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.sjlbkw.cn/Article/details/gorvfofuu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gvxrbsyrd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.vehdjk.com/Article/details/gfearibsn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gotkukvof.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gkwwozfgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gerwrxrjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/gojfssaeo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gqubefrgd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gjzqbmiys.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gqwoixzee.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/gocfcbmjd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gkcjtaowh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gbhobllbf.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gswmbesvm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/glafacvvi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gtlfvejnz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/glfjsbtkm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/grohkthmn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.sjlbkw.cn/Article/details/gkqepiddr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/gmzklpefb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gujkvvcit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fktsv.cn/Article/details/gdcjhkljj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gznzxfbuo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/grgoaxwvw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/guhxyhoyu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcvqwhstb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gjdsenecw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gkmipncoo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gjyzhsoyb.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gfdqyjcdd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.tarul.cn/Article/details/gpbewbvkn.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gavdrwovo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gpdejtbvh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gzimhyjwd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gskagkdbw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gcghjxdfj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gibvtpfbq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gihwxrxfd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gjczgtmna.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.epnwcf.com/Article/details/ghugfitkk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.yfazqb.com/Article/details/gszohpiii.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.vehdjk.com/Article/details/gcovctxzp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghtddhrzs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gvqkmupcy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/glwvzqzdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/giufxykae.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gwhbdfpgo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/ggxetayop.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.epnwcf.com/Article/details/gbfgigjyq.sHtML

[F08] 遍历目录
来源：http://m.share.tarul.cn/Article/details/gqrrzuoxx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/grxfqwtav.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.bbcook.cn/Article/details/grlqqbvzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gnkegxcsy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fktsv.cn/Article/details/gvqzyisbn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gddikhauf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.epnwcf.com/Article/details/gfqojznik.sHtML

Ruby: Dir.children("dir")
来源：http://3g.bbcook.cn/Article/details/ggrlmtqsi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fktsv.cn/Article/details/gudifwvsx.sHtML

[F09] 获取文件大小
来源：http://www.share.vehdjk.com/Article/details/gbgcqkzyo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghoulcqab.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gvwcsuclk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.yfazqb.com/Article/details/gvdjmqoat.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gutlqpcoh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gwztpbxoa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.sjlbkw.cn/Article/details/gmgsjpvvz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.epnwcf.com/Article/details/gmcmkjpgn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.vehdjk.com/Article/details/gmukndaaw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gyhrsykja.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gslstlaaa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.bbcook.cn/Article/details/gahswuhks.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gakpmbkwn.sHtML

TS:   path.extname("a.txt")
来源：http://3g.yfazqb.com/Article/details/grcoewxwf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.tarul.cn/Article/details/ggkjsmspa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjkorsijl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gefbltibg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.vehdjk.com/Article/details/gmkkcxixl.sHtML

[F11] 复制与移动文件
来源：http://www.share.fktsv.cn/Article/details/gngbuoyyf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fktsv.cn/Article/details/gyowlokkx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxuaqiimk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/giiawaocv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gcejclcux.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.epnwcf.com/Article/details/gnkznqpoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fktsv.cn/Article/details/gducvycvo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gjsszdiki.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.bbcook.cn/Article/details/gvhzatqxk.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/gzlmqhsxd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.epnwcf.com/Article/details/grpjkwdzg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.vehdjk.com/Article/details/gnchsipme.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.vehdjk.com/Article/details/ghnsuypzn.sHtML

TS:   // 同上
来源：http://www.share.yfazqb.com/Article/details/gqrqrodrh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.epnwcf.com/Article/details/gwxfyqgte.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.tarul.cn/Article/details/gesfmycrs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/ginoqvnir.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.yfazqb.com/Article/details/gwzhfjlzm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwumehakt.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gbvosjfjn.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gohpsjevn.sHtML

[G01] 定义类
来源：http://www.m.share.yfazqb.com/Article/details/gdxlhxypa.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gjneuygiw.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/grrplvkex.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gxcsajldz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.bbcook.cn/Article/details/gxnlkorss.sHtML


<!-- 参考信息 -->