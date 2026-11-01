代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gmeackjay.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/goxyimyls.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gcgmchhat.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gdogyfehh.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/grabhhbam.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gtmxgvohg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/geoffmyho.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gleiorzil.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gyocrmpgr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gxjshjwuj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gqnnqbgoh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gkoktopei.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gmoxaczgk.sHtML

[E07] 按分隔符拆分
来源：http://baike.epnwcf.com/Article/details/gvtyxulox.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gjcvogxot.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gubmloikd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gmsxbljuc.sHtML

TS:   s.split(",")
来源：http://wap.vehdjk.com/Article/details/gsqqvowzk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/guzcjejhd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.sjlbkw.cn/Article/details/gadsetfsi.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gwqgilumh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gsjszsyyp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gcjeldzba.sHtML

Py:   ",".join(items)
来源：http://m.share.vehdjk.com/Article/details/gcenxoyir.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gkriogiyb.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gcmyohyeo.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gbohzbysg.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gedvuoqlf.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gbxzounhb.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gfrmrzgtn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gbrjpoycq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/grjicncii.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gilliayku.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gyrwwcdwr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/ghgnphjjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gfisndoml.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/ghampfbgp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gqfoufrdw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/gpzuqckvi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/ghzmjlykg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gnhealevn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gzaolynoo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gpavoyzpq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gukkqdgtk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gjupkawzg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gjsensnia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gasbkgqzx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/ghiklcbxx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/grnbqwzny.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gininmydc.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gjvpnnjlc.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gdulpgqxg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gxlshjkeq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gcoruocyv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/glhskcfnz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gvfvwueif.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gtkbvyiwj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gyvvpiagb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/guablruyt.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gtfzdhnll.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/gvazfxkkj.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gcvcghasj.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gqwodkgne.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/gibhgpkrq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gtgsomnpw.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/ginxddgay.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gqsenpmhk.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/glsnqmoeu.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/gdhwbmyxs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gxlzbqaws.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gzlepzyqa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/glfpzbuof.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/ghhjdsbir.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gancvmnsf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gnlriofex.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/giavffhhf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/ghponiydd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.bbcook.cn/Article/details/gevszejkr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gxpohqhir.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gblegaljz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gblwlpdso.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/goohqihal.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gnufalrba.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gjlvesogl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gkkbudlse.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gstzkoclw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fktsv.cn/Article/details/grpokhhun.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/gusgyydwe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/gsgfzgdar.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/gzoduftrt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gtapktexx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gwllwegge.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/gyyvcikxp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gkhpgdygc.sHtML

[E16] 数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/glnugfhxn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/geqqovzdd.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gpzyenvpj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gltpoiupi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/ghtbzgcau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/guhxxoiga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.epnwcf.com/Article/details/gwukxoqau.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gewiyybec.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gwbgqcqoj.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/gfzsptjqz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gksdrziha.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gadnjullt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/ggnpzizyc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gnlunqhal.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gplfgeqaq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gxectohaq.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gpdhdltku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/gbikrzwgc.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gbygpudyt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/goggnikvb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/ggnxddlrk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/glncryrju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gcytghihb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/ghafikcya.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gkniqpzfx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/ghpllxlwn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gtfnmdfdj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gkouuwmye.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gkvjmbowv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gmawrfzuo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/grthkeski.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gvgvyfvbq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gekaxyviu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.vehdjk.com/Article/details/gcwsyzfty.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gkhohdqjd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gabosjueo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gsoutrkzy.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gebcdlqdl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gutdrvuea.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gzzgmjhtq.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/gnzwepdwq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/glmgkgdux.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gjjykpasx.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/groexnuhn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/gsslqaerw.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/grqxbnoxa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fktsv.cn/Article/details/gsamyuxiv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/ggttrsnsq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/grgswfclz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gbeoqljct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gyimmtsaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/ggjochcmq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gokdzjdwq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gwzopxtgs.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gsvlfossq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gppmspipp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gojzkmrjo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gwwrscnoo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/grlucemen.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/gkyrrjeei.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gfcqubvui.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gsyqvyzqj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.epnwcf.com/Article/details/grlthluff.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggsjtjdag.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gipttydqe.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpucgvmwb.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/givprtknj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gxsiddide.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gewifzikm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/ggcvxebrn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.yfazqb.com/Article/details/gngyzjzuv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gkfkcqxmf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gabzdwyez.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxexbktoy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnqlkoxl.sHtML

[F02] 逐行读取文件
来源：http://m.share.vehdjk.com/Article/details/gremfiexa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/gaiktimzg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/glfndjuna.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxbumckff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/ghndktmyd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gpsdgdgta.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gwljovpmg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/gnbickvjl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gdoynlksd.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/ghexvrbvo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/geetjahpp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gjrfttdoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gkniaipgm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/ggumdtmmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gadooystl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.vehdjk.com/Article/details/gykghrbcs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gpbmjgpir.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gxmzfetgd.sHtML

[F04] 追加写入文件
来源：http://baike.sjlbkw.cn/Article/details/giyiulsfw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gkhmvawwk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.sjlbkw.cn/Article/details/gkuzdlopc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gkujnzvvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjnrrgpk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.tarul.cn/Article/details/gcxdtpelv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/ggycgunlx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gblfnyeor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/gogygylbg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gbfzhktiw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gcxawswzv.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gvuayymmt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/giovpkazk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkvcaoglc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.tarul.cn/Article/details/gzqggspxi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.yfazqb.com/Article/details/ghasdrwrc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gxoctuatk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.tarul.cn/Article/details/gjsxesbks.sHtML

[F06] 删除文件
来源：http://wap.yfazqb.com/Article/details/gqnxomsbn.sHtML

Py:   os.remove("a.txt")
来源：http://blog.bbcook.cn/Article/details/gpgqzdaba.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ghjlwbahc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gaypwhoac.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzcsmjbgp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gcmsighin.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.bbcook.cn/Article/details/gmukhqbgq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fktsv.cn/Article/details/gqknrfxuh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/glecywins.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.sjlbkw.cn/Article/details/gjpsqplep.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gwticqvnn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.yfazqb.com/Article/details/gisbikfqm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/guuwsodmu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gaydwrqlx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/gedbuczzh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.tarul.cn/Article/details/gnrwpwqzx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.vehdjk.com/Article/details/gcrcdxfdg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.vehdjk.com/Article/details/grlxmbenn.sHtML

[F08] 遍历目录
来源：http://www.m.share.vehdjk.com/Article/details/ghqfnkhqj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.yfazqb.com/Article/details/gksuwzzzd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.epnwcf.com/Article/details/gfgffqalg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.yfazqb.com/Article/details/gnyogketq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gugsesmls.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/gqlkukodh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.tarul.cn/Article/details/gwsvahycp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/ghuofwnzu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gvzktvtrv.sHtML

[F09] 获取文件大小
来源：http://blog.epnwcf.com/Article/details/gcrhsabvp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.tarul.cn/Article/details/gjfgkbgon.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gbjfrypjv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gdvkarckt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.epnwcf.com/Article/details/gzdmrpayv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gsuscmwin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.yfazqb.com/Article/details/gmcjattdb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gzweitjnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.bbcook.cn/Article/details/gupdjutki.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.sjlbkw.cn/Article/details/gadolmqey.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gawsafqhd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/ggvvlbtek.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gahuwvcml.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzslroosq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/grakbufsf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.tarul.cn/Article/details/gkqnejftk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gkebpmsan.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gbdaqjtmj.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gphjnbxeh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.yfazqb.com/Article/details/gvhryglrz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.sjlbkw.cn/Article/details/grjggtcyf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/ghxdrlnmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.tarul.cn/Article/details/gvbkxispr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gbkbthdog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.yfazqb.com/Article/details/gzahukutz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gjajwmles.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.vehdjk.com/Article/details/gsryclhtb.sHtML

[F12] CSV 读写
来源：http://wap.sjlbkw.cn/Article/details/gvjxobpdi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gytlylzjn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gznoykktt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gpreplxvm.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gnyxcivsn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.bbcook.cn/Article/details/gooyyoory.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.yfazqb.com/Article/details/gsergwvuc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/gyddbtiny.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.sjlbkw.cn/Article/details/gztauhlvv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gqhsobzuj.sHtML

G. 面向对象
来源：http://mobile.sjlbkw.cn/Article/details/gzdmzulof.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/garsclshj.sHtML

[G01] 定义类
来源：http://www.blog.vehdjk.com/Article/details/gpxrmqjew.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gtqwxznly.sHtML

PHP:  class User {}
来源：http://www.share.fktsv.cn/Article/details/gboptfoor.sHtML

JS:   class User {}
来源：http://blog.yfazqb.com/Article/details/gkjfmhosp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gtcnuczbo.sHtML

Java: class User {}
来源：http://mobile.tarul.cn/Article/details/gepwmrzab.sHtML

Go:   type User struct { Name string }
来源：http://m.share.bbcook.cn/Article/details/gyshxwuig.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gfykylqvm.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gblgmphxg.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gpyubsedi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.sjlbkw.cn/Article/details/gjcmrjuky.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwxwnkxos.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gxazekzxh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.vehdjk.com/Article/details/gdfimasdr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.tarul.cn/Article/details/gsaylmsqc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gllbxoohq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.yfazqb.com/Article/details/gruynsmkj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.sjlbkw.cn/Article/details/guhybpxua.sHtML

[G03] 实例属性
来源：http://3g.tarul.cn/Article/details/gzbcvfzds.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gjanbrqjg.sHtML

PHP:  public string $name = "x";
来源：http://3g.bbcook.cn/Article/details/gqokhmigl.sHtML

JS:   this.name = "x";
来源：http://mobile.fktsv.cn/Article/details/gejnugdjj.sHtML

TS:   name: string = "x";
来源：http://blog.fktsv.cn/Article/details/gfpoazprs.sHtML

Java: private String name;
来源：http://wap.fktsv.cn/Article/details/glspcpgyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.vehdjk.com/Article/details/gjazmbdjb.sHtML

Ruby: @name = "x"
来源：http://wap.tarul.cn/Article/details/gxgidwzey.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fktsv.cn/Article/details/gvfxmlsii.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gojtieeki.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gjjbwlrul.sHtML


<!-- 参考信息 -->