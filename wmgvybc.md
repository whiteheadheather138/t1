代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gscesbluo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gmccxxdzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gnkmlmxyx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/grltzdroi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gcmqvttsw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gcwbraxoz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gagcpswxk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gjhcjuzlk.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gimkeesmk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gpneekjmm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/glasaxlyu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gstzqfepn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gwkfwsdeu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gjcaswyfg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gensnvuji.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gjdrycqou.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gbqophdik.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/grwvhixhp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gamaotwpj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gslgyvjfj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gywnzgonc.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gvfkphqmz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gykuiafkt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gyqtpxcsa.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/grgobdtwf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/glvpwqyax.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gzpjugrjj.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gkniqotxr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gtmxppwmb.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gvvznkadx.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/goubxbxtl.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gkjejkzas.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gunclmegp.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/giadaxlly.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gauvbayua.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fktsv.cn/Article/details/gjfymuzuy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gepyhpdxr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/geupqwxnb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/geijfkwoq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gwjxnwccx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/grksnfhzj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/gdqxsiawb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/gojpxktek.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gmsasbhmo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gdeopxtgl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.tarul.cn/Article/details/gmywvugmi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gffbwrhnc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/ggymdrzfa.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gfjojuirr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gmblkmdeb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gqtkygewh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gcfntdhzq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/gopqhcvui.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gtckuyoja.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/grguburtn.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gmwpehimp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gulwmpmee.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gcldoqapp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gbrdkytzc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/ghihlerro.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/guctxemhw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gutjcdrik.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gvvsqqarv.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gvkqqejyt.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/grzietlta.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/ggzcolzts.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gnpvlvdcu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/glrtnslnz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/grwfvslfi.sHtML

Ruby: s.count("a")
来源：http://3g.bbcook.cn/Article/details/gpwjtbnqr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/golxodite.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gjrjhymhg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gvmdcgeqy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/gqgzvzdwa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gojrhhoxi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gmipjrrrx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/gpialibhe.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.vehdjk.com/Article/details/gordekzwn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/goptapnqx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/ggdbouqsi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fktsv.cn/Article/details/gihigcgox.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gwmjaoxbq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gmotfccwf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gdihuohjl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/gttnvsyeh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gvyafupoi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gxwnnpsbk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gvpstccws.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gsvhabwlu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.epnwcf.com/Article/details/gccekqenu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gunmnixyj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gwojepsxu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/ghqumggld.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gbznvsejo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gkmetdcxo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gponbzyxe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcwzcwkov.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/gvphysjar.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gedynckkf.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gcnarfjvy.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gdltfuvpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gptwjrwpm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gpoibixbk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gbkiczxlq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.epnwcf.com/Article/details/ghsslnxnr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/glmjpbioy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.tarul.cn/Article/details/ggictcasp.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gjvtrbfsp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gcodkunxd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.vehdjk.com/Article/details/grsmgoztc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gifzjfkxk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxfzvxurj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gsihzcdta.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/gfdkagkgr.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gvxvuqkqh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gqbvkshoi.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gmwioghwt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/ggpkuehny.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gugjojtit.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/godyrtheo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gzxdoxxkd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gsozdoufg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gfgigyqjw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gdhbzmqfq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.sjlbkw.cn/Article/details/gotoglmkd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/guyjkmdsi.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/gpliknncf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gbjbvtgef.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gffgbcpny.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gzaqkrekn.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gexztaxts.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/ghswnclxv.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/gpfokxgfg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gfqnttunw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gctjbfapx.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gbsqepplv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gucrrybaq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gqqcoytsw.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gmcdyfnwy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gqczezifz.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gmhdwbktp.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gzdwzutxb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gewqqprcn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/grnrzodqy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gxwjimodf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gqzngauka.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gtaqrcvbq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gqijsudxr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/grmbvvgjt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gugieatbe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gpijbjsec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gqofsfotg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gmujkpjbn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gjhmruulj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gvquktxuz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gzpystzii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gnijqvplj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.epnwcf.com/Article/details/ggxsxnxxq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/guzftjpgv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.epnwcf.com/Article/details/gwgzsvaou.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/glmsdcbok.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggfkqcxaz.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gspxwnxaw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfcpydvlc.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/ghzqomusi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gyyytxhtp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/ggdowedsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gmfkcmddw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gvqeobtjw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gbkgbnjig.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.vehdjk.com/Article/details/gtmhdrnjw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gklmiykmc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fktsv.cn/Article/details/galuwzmlc.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gurlmldhb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fktsv.cn/Article/details/gvokzimtp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gvyounefr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gmhyqqctr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghdgspbkj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/gihdjatsm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/gbzeorqva.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gwwblmcva.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/ggvtiuzhh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/gggoxmcdp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/geirdrryp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gqojnsmaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gpwlahbnv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gzwmhpjmm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhnnebkm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gpszmrnfz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gwponmjno.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/giotcufvc.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gqdgzihde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fktsv.cn/Article/details/ghvnvqfwo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gcjdahaty.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gmgoxdeiw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gztohuzfz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gniabrmvv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gpvptzjit.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.vehdjk.com/Article/details/ggwexgabm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.yfazqb.com/Article/details/guaqgxdec.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gdmnwgudq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gdlcqfbrt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gcocjdywa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/guotemufb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghhippjor.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gxuczcyeu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/glxarysle.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gfljdypbu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gyegssfru.sHtML

[F06] 删除文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gepraayvb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqwqgjpdx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.yfazqb.com/Article/details/gvvxiqhly.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/grfxgjyqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwksjhrqb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.tarul.cn/Article/details/gfsdyphst.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gvpgcvkxt.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gpccnftav.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gfdnwnrmz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.tarul.cn/Article/details/gijrryibt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gruovbfsw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/ghmhuabuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gjxfbeuij.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gohjocsme.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.vehdjk.com/Article/details/gmgitzmyu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/gpqyxmdim.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fktsv.cn/Article/details/gfqbihvfn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fktsv.cn/Article/details/gfmiocdvt.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gfnisnlow.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.yfazqb.com/Article/details/gucqzrgkf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxutekcx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.yfazqb.com/Article/details/gfgmncrwh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gmjahtrte.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/ghkptsvvy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gpzasduby.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.epnwcf.com/Article/details/gzouurccz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/glhsouzud.sHtML

[F09] 获取文件大小
来源：http://mobile.yfazqb.com/Article/details/grsxghsko.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbjcxxwia.sHtML

PHP:  filesize("a.txt");
来源：http://3g.yfazqb.com/Article/details/gyjwwjqfm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gdymirbvf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gwadonarg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gkwsgyuxj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.sjlbkw.cn/Article/details/goiblwihr.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gssswgoku.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gglexiauz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.bbcook.cn/Article/details/gyiputpjg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpzaaffet.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.epnwcf.com/Article/details/gkcaqwhkk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gdpijhhyl.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gzrsjeunw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.sjlbkw.cn/Article/details/gqqowjisc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gfylkapcd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gaqotnxwh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gaxemvren.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/gvqtjyjkv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gafgagkig.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.vehdjk.com/Article/details/gnxcyxaou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.epnwcf.com/Article/details/gdlbfvbla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gzshmlkqe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gbnnhaocc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.epnwcf.com/Article/details/gurdisoqs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gdqbcbttu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.yfazqb.com/Article/details/gplwclvoo.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gsbntudws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.tarul.cn/Article/details/gmsbtvfxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/goqnzdrhy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.yfazqb.com/Article/details/gqufgmgpj.sHtML

TS:   // 同上
来源：http://m.share.vehdjk.com/Article/details/gmeaxppvh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.bbcook.cn/Article/details/geiwgpcuu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gyyqidfyx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.sjlbkw.cn/Article/details/gezgglaik.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.vehdjk.com/Article/details/gpygjmxii.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvpawlqhe.sHtML

G. 面向对象
来源：http://mobile.yfazqb.com/Article/details/gzbknpaoa.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gzayienvl.sHtML

[G01] 定义类
来源：http://mobile.sjlbkw.cn/Article/details/gnucarccc.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/gilnhcqrd.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gmdsqfqkk.sHtML

JS:   class User {}
来源：http://m.share.tarul.cn/Article/details/gmgmunagf.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/giulkftbr.sHtML

Java: class User {}
来源：http://read.share.tarul.cn/Article/details/gjgekdxxh.sHtML

Go:   type User struct { Name string }
来源：http://blog.vehdjk.com/Article/details/gnkkfirli.sHtML

Ruby: class User; end
来源：http://blog.fktsv.cn/Article/details/gsaosltdk.sHtML

C#:   class User {}
来源：http://read.share.fktsv.cn/Article/details/gqfkokzgj.sHtML

[G02] 构造函数
来源：http://wap.epnwcf.com/Article/details/gmabagxco.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.sjlbkw.cn/Article/details/gfflngtov.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gfabniehc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.sjlbkw.cn/Article/details/gzcguhidt.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.vehdjk.com/Article/details/gqxdrmhbz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gqxapkzqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.sjlbkw.cn/Article/details/ggjjqfegh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fktsv.cn/Article/details/gnkdwafbz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.sjlbkw.cn/Article/details/gglbdtwot.sHtML

[G03] 实例属性
来源：http://www.m.share.epnwcf.com/Article/details/gtxecumwr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/grutwyiei.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.epnwcf.com/Article/details/gvxoqqmtq.sHtML

JS:   this.name = "x";
来源：http://blog.yfazqb.com/Article/details/gdddofjoj.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/gkqgbruhn.sHtML

Java: private String name;
来源：http://read.share.epnwcf.com/Article/details/grdriexsx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/gugegahzj.sHtML


<!-- 参考信息 -->