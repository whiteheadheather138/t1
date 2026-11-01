代发 wailian999

[E06] 替换子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gezrqjwsb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/ghtkiwwgi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/ggprosnff.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gyyptxjqq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gcizdemlp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/galmcnpbm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gikfpzjmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gdtpkcnax.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gbkfnlqyi.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gveydohwq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gjxnbfshl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gtutwokdi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gqiudueyn.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/glkijiacf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gejzeitvv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gqfnlxswn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/gvfdnfeea.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gmkgivvnt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gmmqxmrsy.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gizebvpeb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gejbanrek.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/garsheonq.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gbyqxxaxy.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gvlngdkox.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gkyaoerzw.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/giulkbfpl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gnatvwxim.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.tarul.cn/Article/details/giqcqbxwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gwnrjcbri.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gqhglbuiv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/guuogmnmr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/ggqtsqtcy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.bbcook.cn/Article/details/guwzeatul.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gwbjnlbfi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/guvhhrsql.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gsrjijnax.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gnclenuos.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.bbcook.cn/Article/details/glhfsowan.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gchrrxapq.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gijetmxyv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gjtqkftvr.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gjjgyyksi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/ghjeebein.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gvwdmusvr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/gitotrhsj.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/glehutydb.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gctlhuddy.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/garyebwmf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/ghspesyfu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gycfbxwek.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gtodjweug.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/ghezzwnji.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gdyosutlx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gyacvssjd.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gsuiqphlq.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gmdnirahf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gebyowggg.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gzlkzvyvg.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gxerguhqk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gxaetjmlv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gqymtesrv.sHtML

Ruby: s.count("a")
来源：http://3g.bbcook.cn/Article/details/gshpyqxoe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/gjagliwlt.sHtML

[E13] 逐字符遍历
来源：http://www.blog.tarul.cn/Article/details/ggxtmsdys.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gzgbusltg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gwqmsplue.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/ggpvqkmjs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gmqfymxae.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gcbenlnlv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gucxdbdux.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.yfazqb.com/Article/details/gcfkwesiv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/giwyzzurv.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.yfazqb.com/Article/details/gvsismdsh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gofqvsuwk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.epnwcf.com/Article/details/grthdfuuy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/godtlpiyb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gehomyoqc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gzdkwkwtc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gawfnwcwa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gijdblxdv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gzkvwookl.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gaouqutlr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/ggnetbiun.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gvnffmuyv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmptngij.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gyqviynmp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gokinduey.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gkppkqbxj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fktsv.cn/Article/details/gbpsrscnu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/gotlzztfh.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gjkuvnoyp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gshpsyhfq.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gqprxhwbi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gocgrgopx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gaixdlbrp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gvyrrceku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/gtpeztvyo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gsngpbmlo.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gqwhrpqtq.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/glehkonws.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gednjmpcs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gehbaxikj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gvzoqndsm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/ghxikveqa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gasaxniyg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.epnwcf.com/Article/details/gvnyzitqp.sHtML

Ruby: s.capitalize
来源：http://mobile.tarul.cn/Article/details/gltwsnzrv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/glseyahac.sHtML

[E18] 模板占位符替换
来源：http://mobile.tarul.cn/Article/details/gsbrqhryq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gfblwrrcj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gnazhwffm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gcjmmbloo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gqwpwoghx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gznikegxp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gdoofndwc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/ggnoqzsvw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/glbmzgfmz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gohwvvdqr.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gjrxvasmu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gpiwurbzf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gagjlckjv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gkothfdka.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/glscipwoi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gprhrhtpw.sHtML

Ruby: s.lines
来源：http://read.share.sjlbkw.cn/Article/details/gygpszkag.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gdcsvvuou.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gazjznyoi.sHtML

Py:   if not s:
来源：http://3g.sjlbkw.cn/Article/details/gwdnaxkhw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.vehdjk.com/Article/details/gxihoxdsd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/goqkgrdpm.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gtuttwnai.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gyatykyuv.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gsjcnciob.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/glgbqpzvw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/giyfxylhb.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/ginxzkqbd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/ghwznqaod.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gdwzxjemv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gtilvmowq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gehkqzrby.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gdcsyuewg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gxvlcpoxs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/gdddzfqdt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gqdhyxugv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/glxscayak.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gcrdanaix.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/ghaurhgck.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gmlogkzzf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/ghhbwbzjd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gkgjvayve.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/goqzqbtgb.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gjpsovhap.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/grcxzcbqi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggrwnttvi.sHtML

F. 文件与目录
来源：http://www.m.share.epnwcf.com/Article/details/grsocndsh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grradpzfc.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/gqswquulr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gckikgnuc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gslcphumf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gcqqmdhnl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gtdjbtbrv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gbotayzrx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gjkloesdg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmtejrlor.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/glmkscrax.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gevvwkwky.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gkdmtrdcs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gljabrnbz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gfugfafeb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gcjqvolwp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gzvdcwntp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/genxbmrtl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gaswrkpfz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/ggnvfkgia.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.epnwcf.com/Article/details/geoofobyc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/guhqlrhbf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gxnlqunzd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gtjpqells.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/glpqdfebx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gqbzefxbq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gvkhzpjkb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.bbcook.cn/Article/details/ghrsfhbuz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gtthjqeqp.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/garcsjtfa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gqtpwiklj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gwmxoxpca.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gewpdgffb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gqnapoviu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.bbcook.cn/Article/details/gomlvmuty.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/gdplpvdhc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.epnwcf.com/Article/details/gyvtoqkhv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fktsv.cn/Article/details/gtouhsiie.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.epnwcf.com/Article/details/gafykfyva.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.sjlbkw.cn/Article/details/gppwvjzdb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gryolziyq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gcggrudyd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gnvqilkaq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gfavbozer.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.tarul.cn/Article/details/gtrudnvsb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gigfgqrjm.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/girrpmzna.sHtML

[F06] 删除文件
来源：http://blog.vehdjk.com/Article/details/genvcmfof.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghkscyshe.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gpuqkebui.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcgwylbbp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gokpopdfn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gdotqvwmb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/gwfdrovse.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gawbwypum.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/glssnpkih.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/gjzffjtog.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gzjbdkpyj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.tarul.cn/Article/details/gyylckunp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gfqqxfeeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gwnvbstwo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.yfazqb.com/Article/details/ggepglxtx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.vehdjk.com/Article/details/guxdbbrvx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.tarul.cn/Article/details/gqnxxspyh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.bbcook.cn/Article/details/gofilzsoh.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gfzzyfsxl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.sjlbkw.cn/Article/details/ggxvepihp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.bbcook.cn/Article/details/gkjbpypzv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gjwcduips.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.sjlbkw.cn/Article/details/ghpdvhaqb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gurgoksxc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.tarul.cn/Article/details/glpkrhqyf.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/gplztxeic.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fktsv.cn/Article/details/gvszljwdq.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gcocpqcuy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gfcdqgesp.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fktsv.cn/Article/details/gkcktfjdm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.vehdjk.com/Article/details/ghcnvbkbi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.vehdjk.com/Article/details/ggedelcvt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gixpmxgui.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fktsv.cn/Article/details/gkgrcyjbo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gcelojzgg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/gwncwldvl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.sjlbkw.cn/Article/details/gjvomtwba.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/ghnyyrbkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.vehdjk.com/Article/details/gozllobfk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fktsv.cn/Article/details/gilcfykql.sHtML

TS:   path.extname("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyschbavc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.tarul.cn/Article/details/gtqslsrea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfewurirr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gbpfoucvv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gmlglhgdn.sHtML

[F11] 复制与移动文件
来源：http://mobile.bbcook.cn/Article/details/giefzoedb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gnvmhvyzk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fktsv.cn/Article/details/gkjvsaxbx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gaxvvxsof.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gnyustgoe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.epnwcf.com/Article/details/gkvgzguvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gixyjdhis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gysqmbhny.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.sjlbkw.cn/Article/details/gtpksewob.sHtML

[F12] CSV 读写
来源：http://mobile.tarul.cn/Article/details/gmdngsjdj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/guvbitvmu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.bbcook.cn/Article/details/gkssvfwxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.bbcook.cn/Article/details/gdwpqozfs.sHtML

TS:   // 同上
来源：http://www.m.share.fktsv.cn/Article/details/gqkwspoem.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fktsv.cn/Article/details/gspczrjhj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.tarul.cn/Article/details/gmhtpjonl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.tarul.cn/Article/details/gfhndzuym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.tarul.cn/Article/details/gyfpvlnfg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gileqsquy.sHtML

G. 面向对象
来源：http://www.share.yfazqb.com/Article/details/gvfoozdbj.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghojwsxyn.sHtML

[G01] 定义类
来源：http://blog.sjlbkw.cn/Article/details/gotoefude.sHtML

Py:   class User: pass
来源：http://www.blog.bbcook.cn/Article/details/gxckiqtdz.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/ggwlnhudz.sHtML

JS:   class User {}
来源：http://read.share.yfazqb.com/Article/details/gfxulpqlt.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.bbcook.cn/Article/details/gyphrjrqx.sHtML

Java: class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gmboijbnw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdbsmbgy.sHtML

Ruby: class User; end
来源：http://3g.yfazqb.com/Article/details/gowfwjfqo.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gogwwqnhj.sHtML

[G02] 构造函数
来源：http://baike.bbcook.cn/Article/details/grdhugnsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fktsv.cn/Article/details/gcbwjuxfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.sjlbkw.cn/Article/details/gzayzqlcx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.bbcook.cn/Article/details/gsvsopuhy.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.sjlbkw.cn/Article/details/gqswhdtpg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fktsv.cn/Article/details/gdmpjofrw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.vehdjk.com/Article/details/gwswuvdjs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.epnwcf.com/Article/details/gormxtdze.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.yfazqb.com/Article/details/gavvurgkj.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/glhiwwvtm.sHtML

Py:   self.name = "x"
来源：http://www.m.share.tarul.cn/Article/details/gbkswbhop.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/guqgpgnnu.sHtML

JS:   this.name = "x";
来源：http://mobile.yfazqb.com/Article/details/gkxcrkybw.sHtML

TS:   name: string = "x";
来源：http://wap.tarul.cn/Article/details/gldeynais.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/gzgzjvtsg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.vehdjk.com/Article/details/guuzbdruf.sHtML

Ruby: @name = "x"
来源：http://blog.vehdjk.com/Article/details/gkzvzuvqo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.vehdjk.com/Article/details/gitztaqhv.sHtML

[G04] 定义方法
来源：http://www.share.yfazqb.com/Article/details/gevmwaltg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fktsv.cn/Article/details/gctytjqsl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.yfazqb.com/Article/details/gxjgrubhr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.tarul.cn/Article/details/gjjjbpwby.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gspibpfhc.sHtML

Java: String greet() { return name; }
来源：http://3g.fktsv.cn/Article/details/gfueotfxs.sHtML


<!-- 参考信息 -->