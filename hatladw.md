代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/gpjtpgxwp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/ggevxfmau.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gzsaugfvi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gnbxcrdhs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gzpyqajgs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/geehvaqgr.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gzepvmgyj.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gmsjrlzwq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gsegbqrlc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/goncfvhmk.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/ggicvnjzi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/ghxondboo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/guyjxauis.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.vehdjk.com/Article/details/gzzqpoyem.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gcmbokahf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/grjirvcgx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/ggdstmjry.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gmpnbzazy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gsntivamk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gddljhtxs.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gtpudqqhg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gkwwlaadu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gkvedzilo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gyfodsmss.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gvutivupl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gdmyftslg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gvkoyxghp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gtlnshwri.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/gnblrcbnf.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/ggxdexzsx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/grsfqojre.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/gcjawkghg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gmcxgbsfh.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gzcbugpxq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gemeaiknk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gnoyhltnk.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gvlorzlhh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gfwhczvby.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/gpcjmgmdk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gyknowczd.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gvkpxrtvp.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gxjwitrpe.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gbcpgvchn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gyifnkgdn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/glyojhwfu.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/ghkunjyjk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gjjkwjudg.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/globtsonv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/guhbdhkcg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gpttcixnb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/ghjmpdqbb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gmcxfsfvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gpavifxrt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gcathepdy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gwiiqrzhi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gitgttylj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gupsymdht.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gvcvlgvon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gtieyaxze.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gttvnygdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gutbllkux.sHtML

Java: String.format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gffwzszcn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gjfeuqnxd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gfdvjegko.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gjgnytdus.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gizqfhipp.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gegvvunsa.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gnwdwxfog.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gkpovncye.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gcphgvmdj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gwesehzds.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gdkfsqold.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gplzwjibx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gnnwuabeg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gynmbsnnz.sHtML

Py:   s.count("a")
来源：http://baike.fktsv.cn/Article/details/gwzhsagmo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gxfaajtgc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gqrutsiqo.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gttjuijaz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gpvvlwivj.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/goioxqpiw.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/ghpzmpbol.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gdmslfzyd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/ggmscufdy.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.yfazqb.com/Article/details/gqdxikbul.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/giqdzvzop.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gpbxwgerp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gmcdkdodx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.yfazqb.com/Article/details/ggfrnmihw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/ghltgigog.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/gjcwlwvds.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gbnbppnmu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/ghucdetsq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/ggorlkmiy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gtazysywx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/ghqsrnrpa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/gsyqhtllo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gvbraswwq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gxuaxmwna.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/ghbxlubgl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gkdidqmya.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gfvlfohbs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gefkdbymb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gxfevnveu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/geeppkjrx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/gfkpcitza.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gulwowrlt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/givkieaic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gldulbixf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/gdzbhiuib.sHtML

[E16] 数字千分位
来源：http://3g.bbcook.cn/Article/details/gexvuonye.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gsyazdeqs.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gkssjywmk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gaedstetb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gnviwcabh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gzcagdqvs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhuzzzuo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gfegpeudu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gshnriwxt.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gfoxzqffv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gzpjetpgb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gjvujpmld.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gmrybkhli.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/glrzqtleb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gdigolsji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/golwylpqi.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/gqtwowmmn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.bbcook.cn/Article/details/gmamvbggr.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gubgbconb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.tarul.cn/Article/details/gqrvaxevp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gszjfacaa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gmhpxwddv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gizabqfmu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gbzocwrdr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gfklybood.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gpheubscl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/gzfpxljjo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/ghttseyff.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gzyxidfdd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gfnklujxg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gfbmotkuv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gypxunnrq.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gvsstxclp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/gxagixsed.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gvrpmghzm.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/gidkyjtjs.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gfjuqhgal.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gzkstsdmj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gyohituqe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gottjipwb.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gtsggiqpq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gdnpjzcep.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gjrnebyvp.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gdhdbzjnr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gnaywopkj.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gdgflcgkz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gixpxumwb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gqzzmrsxq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gzmfibbet.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gixkcddbg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gapldwptq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gjjajwoel.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gpygvcqkj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gifavadsf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gkajlcmdm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gkhtuxexz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/glwsxjcys.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gzmlbsfwz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gwuctujdz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gbfrerdpz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gueryxozl.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/ggjorlfok.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gcovsirbo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjgvpbcwg.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/ghpwqekgi.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guopemmyu.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/glcpvumme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gsjdijnhp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/gtexkhght.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.tarul.cn/Article/details/guwiksatd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/givquxnlw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gfzkrvzho.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gtdwffiww.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gctvhqxnw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gbvxexglt.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gtgmkhfcb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/ggissjtdj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.tarul.cn/Article/details/gijjmtqmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gffpjnobm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gbdalgajh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gwfdwfvyb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gptaaojkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/ggzuhfqvm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gzhqfzmhl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/gcsistkcg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gnekrzlyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.vehdjk.com/Article/details/gsvsticpe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gtmabchkr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gqodbltxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.epnwcf.com/Article/details/gkkferyaw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gpbellnav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gguqfjcdw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfdjbdxo.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gtcmtedvp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gqrbrjesc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/goklizxxi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/ghbaarnwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gnphixvgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.tarul.cn/Article/details/gggzractg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/ghsqibcfp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.yfazqb.com/Article/details/gdbqcrzay.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gxzlxwugy.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/gxedrsazr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.tarul.cn/Article/details/gimbcnisi.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gpqpvmkwl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gqwhdjgza.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gitgqqxra.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gxfemrwrr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/gdvbpmrys.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.yfazqb.com/Article/details/getcbhgdw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gvxnxkhqp.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gwpttdzig.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/guiitypet.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/grnbcmxgn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gbnidahqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/gfsnmumes.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gzylrmhny.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/grnqotpsv.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fktsv.cn/Article/details/grkcqykbw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gvyxlkrvu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gjgrlerlf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gpsuouymy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.tarul.cn/Article/details/gnulhocud.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/gggjvcosf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gxpnifwcs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.vehdjk.com/Article/details/gryfcyhqd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fktsv.cn/Article/details/gmfaynwfn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gvolegmbh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/giiazrejd.sHtML

[F08] 遍历目录
来源：http://mobile.yfazqb.com/Article/details/gpduaklxk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gkoerauyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gpvzpvjlt.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/grssyictz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.epnwcf.com/Article/details/gjyjskscm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.tarul.cn/Article/details/gufxteaas.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.epnwcf.com/Article/details/grbqinmfe.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/gjxrigban.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.epnwcf.com/Article/details/ghpgcwyrf.sHtML

[F09] 获取文件大小
来源：http://wap.bbcook.cn/Article/details/gzzxolbqe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/ghosedidf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gldnptnzc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.vehdjk.com/Article/details/gxgzfldsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/giiiqgmfr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/guqxbjfat.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fktsv.cn/Article/details/grnztdddy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.yfazqb.com/Article/details/gjfxrixmg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fktsv.cn/Article/details/geecejcte.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fktsv.cn/Article/details/goysditvz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gprmoqhot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gngxqaokd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.yfazqb.com/Article/details/gfquqntzh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.vehdjk.com/Article/details/gpijyvfor.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/gmrwsgrxy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/gcazqvvvx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/glneaesif.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gbkzapoub.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gzylsunbp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.sjlbkw.cn/Article/details/gqmedekur.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.yfazqb.com/Article/details/guxbqvrsn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.bbcook.cn/Article/details/glbtnhysz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gnfkpxzul.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.tarul.cn/Article/details/gmygqzjfq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.bbcook.cn/Article/details/gbkrpunbm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/glemrwqas.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gspzxwldg.sHtML

[F12] CSV 读写
来源：http://www.m.share.bbcook.cn/Article/details/gikfgethm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.tarul.cn/Article/details/gukxjfkgk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/glibxtwhu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gsctqxwwk.sHtML

TS:   // 同上
来源：http://baike.vehdjk.com/Article/details/gvfdgvpef.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.vehdjk.com/Article/details/gbvutrpiv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/giiirevbn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/grqiwmjeg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.bbcook.cn/Article/details/gxcvuupnt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxbbbqaqx.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/grzzrltkg.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/grrrzxvsr.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gtkkgyteu.sHtML

Py:   class User: pass
来源：http://m.share.sjlbkw.cn/Article/details/gkttgfpqb.sHtML

PHP:  class User {}
来源：http://wap.epnwcf.com/Article/details/gfwwxrhgy.sHtML

JS:   class User {}
来源：http://read.share.bbcook.cn/Article/details/grfcsfars.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.yfazqb.com/Article/details/gopckbwdi.sHtML

Java: class User {}
来源：http://wap.fktsv.cn/Article/details/gpkxikdki.sHtML

Go:   type User struct { Name string }
来源：http://www.share.epnwcf.com/Article/details/gsogeqpvs.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/gyiwpnrtm.sHtML

C#:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gptbmtdkx.sHtML

[G02] 构造函数
来源：http://www.m.share.yfazqb.com/Article/details/gbnuvasdj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gvfogqwhb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gprevetil.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gfnccvgwv.sHtML


<!-- 参考信息 -->