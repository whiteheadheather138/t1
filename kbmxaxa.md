代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gaisygewf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gxgsvdosa.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gltdeelgi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gtoafylwt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/gmchenajp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gunylhcjh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/gvuyhwndt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fktsv.cn/Article/details/grhxgycor.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gyzpizmxo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gebaeptgx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/gykzellbb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gvskabgdq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gdsydymaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gnqywttui.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gotudelml.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gorwcnufu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gullbubuf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gotiaxuoy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdanscbe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/giezdynkl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gsysldyil.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gnixuibhj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gbgbhawiu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gkysxffjo.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gbejmtyjw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gjqebgmlt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gvnosydzb.sHtML

Py:   ",".join(items)
来源：http://3g.sjlbkw.cn/Article/details/gfbsxmosm.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gpqmzgpjp.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gukswnzws.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gctcpylfi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gusuvjgfc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/glsaubhqn.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gmepbwjyq.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/giednzrfo.sHtML

[E09] 去除所有空白字符
来源：http://baike.vehdjk.com/Article/details/gdzoayryd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.epnwcf.com/Article/details/gisasuzpr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.tarul.cn/Article/details/gvjfiijmi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gfmvjbcxj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gxzihmmvd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/ghiwqcnkz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gbhfjoohd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gutgespjd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gmaokkstj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gdhqdxycc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gtyxgbdos.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gizaggfed.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gypeobpie.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gqudzeufe.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gyczhyqbm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gvdxzdivz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gphqjdvsc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gxefxbpeb.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gxdfehmzl.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gftevbpjr.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/gacicuhqg.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gzrfwpenh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gfrvyamvt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gqqrxgipm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/ghzawbzmy.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gdlfhavxj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gjrzqygbs.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gmsvhgcre.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gtgnatnuy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/ghjgxdvhw.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/ghyyqxycd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/golivrqbx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gecvhmycy.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gwonuhymf.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/goxyhfcva.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gdqtmufej.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gigaanizq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/gteikgqon.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.bbcook.cn/Article/details/glennfnln.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/grkybluie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gnilanbkr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gscdueyyw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gejpdnccd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/ggfusqzgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/guacqpfzj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gqpmmhcae.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gjiwdzdhq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gncnggqna.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/giyqhrruk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/gwpjnlvbr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gomiwxnxu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gvkdrdqhx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gcjegjpla.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gwqasgrsk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.bbcook.cn/Article/details/gggpopges.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gysisbayr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gtfteddjj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gulumonks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/gvazcpotf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gqpxmkhfh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gjhzivlty.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gpuczxlmr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/ggopswten.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/gvizaxgzj.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gborxcsmj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/gqsxajzrr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gtfrxpuyc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gwvkmfamj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/ghtmkrslz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.vehdjk.com/Article/details/gqqdsjoxn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gxahsvkqz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gfckyzgli.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gufcnjuyo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gkzkyhbef.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gpbgsraoy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjiorhvr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gdlfosrlb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxexarone.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gdutsyeqi.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gswyrhaxc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gmgbtdqnx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gznlzthcz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gpwmytcvn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/gnnmmpkyo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gitfwzfxd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gqeyjrehs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gidrqiagk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gadqipuyj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gbwwzgykx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.vehdjk.com/Article/details/goausyngt.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gsekatnjm.sHtML

Py:   s.splitlines()
来源：http://wap.yfazqb.com/Article/details/gkaztswdm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gpffzbvad.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gijwoeflh.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/greunbtxf.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gxvdfsnhe.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/gjkwlxafz.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gzjznpqpk.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gaegnaehf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/gakmeinlo.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/ghqwbdlzf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gzyqtqpmg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gijxqgkwv.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gmcxcbhee.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gvaxxyaew.sHtML

Go:   if s == "" {}
来源：http://3g.vehdjk.com/Article/details/gogvpyyrt.sHtML

Ruby: if s.empty?
来源：http://mobile.bbcook.cn/Article/details/grfjjeqtk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/ggbsvcgqr.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/ggjkunndq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/gchlgppkk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gbjafqqex.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gsjgxwpqb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gdrkpvmee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gysvluekm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.sjlbkw.cn/Article/details/gzamwqkjo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gopgvyqqp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gumncayxq.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/gcocazniq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.bbcook.cn/Article/details/gkoiglagp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/grpoveakf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gopsgsdmw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gxxvidxlz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/grytgdxko.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gmlyjbmyt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/giosesjim.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gzkauortv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkmycbsty.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gbktyjmla.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsvcbqwck.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/gsyjwpyvx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/grsmbwjup.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gqlncqiji.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/gwxdqwazu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gsglozpss.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gnrfbhzrb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gddyrjdzy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gvdwylsqq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gguwkyiuq.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gtesiaeqw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/ggsemrppt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gaprnjweo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gyfkwygoq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gatbjochj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gymisfgtf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.vehdjk.com/Article/details/gvxgcvbri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/ghaletduf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/grteksbyg.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gkzkubvmg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.tarul.cn/Article/details/gjmxgmphz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/glcevvmrh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/ghnovxrdf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/grniyhgcw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gkncgobyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.bbcook.cn/Article/details/gcoedddvr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gpbtshckc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gbxuyykkp.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/gkdhitzqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gajhsahpd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/gfyddungh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/gdqffdoxj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gwpsjvngt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/grcriyqse.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gitzxpirr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.tarul.cn/Article/details/gmazcvpyl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.yfazqb.com/Article/details/gujjjpdxo.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.sjlbkw.cn/Article/details/ghwulxswq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gudpdzlng.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/gxvclphin.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gculyjkfl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggzmtwbeo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gixnuhoqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/grnqytxjr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gusxfbyse.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gzslnoiqd.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/ggzshaxzf.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gsxtnkjfl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gctbqyfjw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gthitenfb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gcdxsgche.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gzlozdtsu.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gewipbmmf.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gaexbykjb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gblbskhnj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/guybqikuj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/gnhtbgsfe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.epnwcf.com/Article/details/gsxqnilnc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/ggwmtymur.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gcusgrhgr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.vehdjk.com/Article/details/gkpvchcaa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.vehdjk.com/Article/details/gyugpqtku.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gzoiydqsv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gyzkywjou.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gduptpyzy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/ghkmgwghc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.tarul.cn/Article/details/gxaymjhtu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gtwsqtbkj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/gfxwpqchv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gsfvccbrn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gjffsznfo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.yfazqb.com/Article/details/gwrecukjs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.bbcook.cn/Article/details/giwkmuqhh.sHtML

[F09] 获取文件大小
来源：http://read.share.yfazqb.com/Article/details/gmrdeurmx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkufcpwqf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gjmfrffph.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gfceliiyg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fktsv.cn/Article/details/gyzfcclwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/glkmsypin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.tarul.cn/Article/details/gpwblztjp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gpvwkclxq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.yfazqb.com/Article/details/gfbmptejf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.sjlbkw.cn/Article/details/gfwwvtpet.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfuevlvkh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.vehdjk.com/Article/details/gvfijnxnq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gbidryrgr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gvoxehsph.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.yfazqb.com/Article/details/gemqpydiz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gecvgjjbb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gkswingoq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gfrtgqwmy.sHtML

[F11] 复制与移动文件
来源：http://www.blog.epnwcf.com/Article/details/gqksozcyj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gkstydway.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.yfazqb.com/Article/details/gdzzofhfy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gxnwhdyfg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.sjlbkw.cn/Article/details/glhnbrzdn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.epnwcf.com/Article/details/glpinimwm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gxorroqpu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gdqfvsgbl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fktsv.cn/Article/details/gaqrkbfpc.sHtML

[F12] CSV 读写
来源：http://baike.epnwcf.com/Article/details/gmdrsxxjk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.vehdjk.com/Article/details/gywaqtdpu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gafesiazb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.tarul.cn/Article/details/gzbkfkpcz.sHtML

TS:   // 同上
来源：http://www.m.share.yfazqb.com/Article/details/goynyfaij.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/goekpwhyg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/grfvtkrwo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/ghitngvnp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.sjlbkw.cn/Article/details/gvttdzzzh.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfzgsycav.sHtML

G. 面向对象
来源：http://blog.tarul.cn/Article/details/gxvrhdkyl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gmpqulxxf.sHtML

[G01] 定义类
来源：http://read.share.vehdjk.com/Article/details/gvvtgocgt.sHtML

Py:   class User: pass
来源：http://3g.sjlbkw.cn/Article/details/gsrqlubkj.sHtML

PHP:  class User {}
来源：http://wap.vehdjk.com/Article/details/gcbazexgp.sHtML

JS:   class User {}
来源：http://www.blog.fktsv.cn/Article/details/gzkenunrd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gzygfryem.sHtML

Java: class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gossrrgba.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/ghyabhxhh.sHtML

Ruby: class User; end
来源：http://wap.tarul.cn/Article/details/grzimwuhv.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/geecsuhva.sHtML

[G02] 构造函数
来源：http://wap.vehdjk.com/Article/details/glbijcvox.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.vehdjk.com/Article/details/gbyrdetzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gkdvuttys.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gfedwtovd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.epnwcf.com/Article/details/glnfkfiis.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gfpxvlnje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.tarul.cn/Article/details/grghiflgz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.bbcook.cn/Article/details/grayqqnix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fktsv.cn/Article/details/gbxkydjho.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gwbqpocwp.sHtML

Py:   self.name = "x"
来源：http://wap.bbcook.cn/Article/details/gopfswhwi.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gibfgabro.sHtML

JS:   this.name = "x";
来源：http://www.share.epnwcf.com/Article/details/guirgojys.sHtML

TS:   name: string = "x";
来源：http://blog.sjlbkw.cn/Article/details/gnoobnzdn.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/gjzqyjicw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.yfazqb.com/Article/details/gxqyhrgjh.sHtML


<!-- 参考信息 -->