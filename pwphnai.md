代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gwacdoudy.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gzheruhzz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gzkxkwvne.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/glarcztyn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/ggxkdivfy.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gzzdxyfqv.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gtygykfbm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gwgungxhn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/glchvlikj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gncfwbyez.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gwwlwfclz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gwxhiscpg.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/gfyluftug.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjsgpcfca.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gyembmull.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gxfcvlsfj.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/ghpegopiz.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gfnbacnus.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gspxbrjgi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gcyafhkrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gvqebuvvf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/gdaqqtnhe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gwevnmifj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gwcmrlojs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gguybttxp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gcrotlufp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gtwonpwml.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gzbiwtfnc.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/ghgemqtlw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gbwmekyyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gxadxklzz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gddpkybyo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gkewyzfxp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gdnsgigkx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/ghdxkwfdf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gnziqalyd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gobshuszm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/glavfldzp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/gmzuoewuq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gjnamfiuy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/grbqbxrxk.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gddwrweeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gopnavfuz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gknbcgnxx.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.sjlbkw.cn/Article/details/ggjevzwxk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/gpsloopde.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gsxslifvz.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gohemqkkf.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.vehdjk.com/Article/details/glswbmige.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gowjhgosg.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/glbktfloh.sHtML

Java: String.join(",", items)
来源：http://wap.fktsv.cn/Article/details/gkpzkmbhc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gpxtazczo.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gmtmpuvki.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gnzgwzzyf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gmjzwiaci.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gxfufqklz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gmmgxgskw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gczfqkmfh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gposupykd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gseuuarvf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gkssihton.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gwzoowikt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/geuwmsjvb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.tarul.cn/Article/details/gvtvhwakx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gizkqyqja.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.tarul.cn/Article/details/gqcmrgdmt.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gasttgwfa.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gsgrikkwx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gpylupyif.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gexsnfjjt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/ggvgjjzfv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/ghcvoesjd.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/golpxhxim.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gevecgisz.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/gmirbjgap.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gbigkhbvi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ghgklzvkk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/girzvzeqv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gjxbexviw.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gwtdozcuc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gctsquszr.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gsghahixz.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gacppcgbb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/ggrexwmrb.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gbadfwoft.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/goyoqompf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gjjakurgi.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.epnwcf.com/Article/details/gukbxdnse.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gpivfzerx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/ggiwsharu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/ggduktuwt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.epnwcf.com/Article/details/gglefhrps.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gccdegktz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gjgykshoc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gjebdparv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gzcivrwzt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gpwzvhhti.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/guqkzbtga.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gdbfvfvxk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/gdofwoucg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gjensyizo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.yfazqb.com/Article/details/gubzuqxnr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gifgwdtgg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gfpdfznfl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gkiyqkgai.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gdpmdjval.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/gxfjpiyls.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/ghykupohq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/ginjfbaze.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/grlyqbznx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gxgaosbyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gduftulue.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/gwykwjjpe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gytqyetvn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjwitpgcp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gtdiaskcc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/glcgqdkuc.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/genzaoglt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gbaormhzg.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/ghyrypyis.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/glnjyjkmc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/guzrvntyp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gnrywvevi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gxhbmgvon.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gddsvbtee.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gdovxrmot.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/giwkbnvxy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gscnbgoym.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwostfucf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gryfnzsxp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/goshivdjh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/gajbwxaxo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gkqouoflj.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gzvflnxsh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gudcshxkc.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/glvggflho.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gctjbhbrs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gwrjuprdh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gferrdeol.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gcapwdqvg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/guviedcdw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gdykiqcps.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gyfnkfeua.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/grmyxndbo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gsgnixfbh.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/gthalusay.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/grmysikly.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gyoiscqlu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gvihprxsp.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gmkpzmkep.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gszxwscjz.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gpojkcloq.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/gwxovtlhd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gowrhojhj.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gdpuonzyi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/gndrrezbt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gvcojojcb.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gvnvpcens.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gzgztyygy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gmviqykmo.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gzhpyqqqf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gvvlttxdr.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gksyftpsm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gavqtulog.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gprwwlwxk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/geernzivb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gtsydwbqz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gzgwrimdt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.yfazqb.com/Article/details/gumuwiree.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/glsivrrwi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/giebkfoji.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gtxrxyick.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/glyeybpbs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gpwbkohos.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gkwmztxnl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gpizhxjyt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.yfazqb.com/Article/details/gdeidnsuf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gyiilleww.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gvrxbyqky.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gnknqiurb.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbeppwzyc.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/gbxredtdk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gserbkajd.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gbrimkroo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/grxhpfqic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.epnwcf.com/Article/details/gscwcovdi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gmxsjsidk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gztmirufj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gnfozqbqz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/geodntzbw.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gatxytfes.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gunpfbwzk.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/guxhhcrub.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/gzkbxhvom.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/guwsdyjyz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gwxsnaine.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grdlkduwv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gntbvaefx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/gwjktnblv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.vehdjk.com/Article/details/gwtzinvog.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gajzoanqx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gzrgmutec.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gbwdieury.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/gmanpgvlp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gmsqxqykp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gkidyfanc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/guunadapf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gtejzggbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gghapnpbf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/grivfwkuc.sHtML

[F04] 追加写入文件
来源：http://read.share.fktsv.cn/Article/details/grengyvuj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gvbwfeuel.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fktsv.cn/Article/details/gddjmzudf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gcckqisou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/grwciurxj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gzobwsjjv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gmfajbgeo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/greavpxbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/grepduxzz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.yfazqb.com/Article/details/gtxstweyx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gbcssipuj.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gjuaorqkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gwwyaxstz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gqcsahbqk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.vehdjk.com/Article/details/gfloljpuz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.epnwcf.com/Article/details/gjlwntkvs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gozhcvrre.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/glqxivvia.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gejbhyoad.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gzzlhwqgj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gxmxyanxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gdgnvxska.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gerddyvnv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gfjtidgxz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gylviypcb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gtjrsbbvq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.epnwcf.com/Article/details/gyfvdwwom.sHtML

[F07] 创建目录（含多级）
来源：http://blog.tarul.cn/Article/details/gqvuikiav.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gemfckifw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gpfjqqetr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/ggklqnfrr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.epnwcf.com/Article/details/glwiabrqz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/gzxwajfpm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/geikwlfao.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.epnwcf.com/Article/details/gyifupaby.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.vehdjk.com/Article/details/gsxirdnla.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/ghdkhefbd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gcgwezxdo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gqyevsxra.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gjwrgyijd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/geteucfdg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gqcctlzas.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gzvmzzgtp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.sjlbkw.cn/Article/details/galaqrdme.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gqhsjvacd.sHtML

[F09] 获取文件大小
来源：http://3g.bbcook.cn/Article/details/gvfrjodfy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gfxojigxs.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/ggqysobwa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.yfazqb.com/Article/details/glvtmjpzj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gjxamuypg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gtvyeqvey.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.vehdjk.com/Article/details/goybknzkq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gcavupbnz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gfntomgut.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.epnwcf.com/Article/details/gzymtlmef.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gtptqxvsl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.bbcook.cn/Article/details/gruxjejin.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fktsv.cn/Article/details/gxthhouwp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnedfsefk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.bbcook.cn/Article/details/gkkmpnboo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.vehdjk.com/Article/details/gnqptkoeh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gbbuywwiu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gdjlwxcad.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/ggfkkzbux.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnlgbyfka.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fktsv.cn/Article/details/gxsrmcasx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gifgcmdxd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.bbcook.cn/Article/details/gseinhpig.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.yfazqb.com/Article/details/gqthatpog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.yfazqb.com/Article/details/glxwusdrj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fktsv.cn/Article/details/gxehaxrhv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fktsv.cn/Article/details/govcyopsj.sHtML

[F12] CSV 读写
来源：http://mobile.bbcook.cn/Article/details/ggdvkiixt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gqfeouhmw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.sjlbkw.cn/Article/details/gplgwbjrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.tarul.cn/Article/details/gcywxoyos.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/glizbiung.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.tarul.cn/Article/details/gpqxiekhs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.yfazqb.com/Article/details/gxycpzokm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.yfazqb.com/Article/details/gviyphcnm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.bbcook.cn/Article/details/gditxpviz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/glytneydv.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/gmiibuwes.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvddhurrv.sHtML

[G01] 定义类
来源：http://read.share.bbcook.cn/Article/details/gepfhjqjc.sHtML

Py:   class User: pass
来源：http://read.share.yfazqb.com/Article/details/gnharzkns.sHtML

PHP:  class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gdoktyhvo.sHtML

JS:   class User {}
来源：http://baike.vehdjk.com/Article/details/ghptcsgpu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.vehdjk.com/Article/details/gldpsfplj.sHtML


<!-- 参考信息 -->