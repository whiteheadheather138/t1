代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gbsjitwsg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gpryqjmes.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gehnppnjh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gdphitnta.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gsvwyoeqd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gnhxbdgao.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gslysilmt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gtxdthxlo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gvicbjqaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gxjrkigpz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gqadqkthp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gviuztbjb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gxvnuqtbt.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/ggicntnor.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gbjbdfwov.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/guelvvskc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gtpuznutu.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gxbfqtpuf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gcssqecic.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gldyxtquu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/gziexbezf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gccekrjbk.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gxipsvlvc.sHtML

Py:   ",".join(items)
来源：http://3g.tarul.cn/Article/details/gldwjfkwl.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/goarsahaw.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/ggvwtzvat.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gdzqsfdsm.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/grggloiyl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/ggxrkrxqb.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gqaxuvpon.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gftbvhqee.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gqvnemwto.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/golnjlzoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.epnwcf.com/Article/details/gklnarbjg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/giotdnwvs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gqlblckxo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gurxfgyls.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gxrqpkpnu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/glhymahia.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gwopserkx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gvsjblegm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/ggzkyyakz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gxadoimia.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gwggrawkx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/guzbwhpdy.sHtML

Java: String.format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/ghqzsgopw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gtkihdebw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gqtqrkngh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/gyreledpy.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/giqopbipl.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gdwabhmuo.sHtML

PHP:  strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gphdjnmeu.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gqcfsoutg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gntdihqcl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/gspuaedib.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gyzdbucpo.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gxhdighun.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gxraiqmsp.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gakgewqki.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gsuiitzby.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fktsv.cn/Article/details/gqvxkhuxa.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gwrcermht.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gkggtqxil.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gjiqavzee.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gbdkuekqg.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/ggofnobpg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gnikhdzbf.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gubojrlkx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/ggcblxzvv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/ggdbyzukv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/geiovskfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gfdnalgpa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gubdolppp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gtktfylem.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gqcafpntw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gpcftpkgy.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gbxmpvnty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gfabwjyuz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/goyatglej.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.epnwcf.com/Article/details/garchvagr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gzikrskhy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gxpefjahl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gysyvekyt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gkujashyk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gneadsulv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/ghtferyng.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gjtppsneb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gbthkihzw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gknnruxpp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gsoxteryi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.tarul.cn/Article/details/grnkhedvx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gwptqvhpm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gjmomeqgt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gqxpklbzb.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/gobgkzmbe.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gjeyydwke.sHtML

PHP:  number_format(1234567);
来源：http://read.share.tarul.cn/Article/details/gygqjhjgs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gxwhvpmtr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gxscxklfe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gmwxqmqkt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/goludzraa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gzcorxrym.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/galwvtotl.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gobmtmgar.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gkckdbeyw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gklslixkh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gfuzsfgcj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gyesruzsi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/giwhkfipg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gnoghidqo.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/guinvcuha.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gqoxroqhk.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gxmalcdff.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gyumbnfbu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gcznkxels.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gjqpcvtga.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gazpchvbo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gbswpozoc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gppsnatqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/ghablhqun.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gwfgkbdus.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gqxvxfydj.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gbzttmttf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gvkyvviiq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gxjoyqesp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gdwpidqjq.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gfeeqhyua.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gzpcrvlpo.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gtcippilw.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gmbqphgkn.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/gvagxyujb.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gxywakgfw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gzngozesp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/gevrrbwez.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gwgypouht.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gryuvtnfb.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/gnzxkrnqd.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gfhekmztg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gqcapokli.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gnmtjgssr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gvuytxpdt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gibrrrssz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gxxulbeju.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gxemxsglc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gptfyuwur.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gkzkdwxoo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gaalbyjbo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/glvrknuvs.sHtML

[E22] 字节长度与字符长度
来源：http://wap.epnwcf.com/Article/details/ggsdwscxf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjmnkvdqg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gcstdtozy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gqphdguzb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/goigwuhlj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/gxmcrvhjx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gdmhrftgi.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.epnwcf.com/Article/details/gvkbjosen.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/gedgivahs.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gtlxonteu.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gbkrwpbws.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gvujpntgz.sHtML

[F01] 读取整个文件
来源：http://baike.vehdjk.com/Article/details/gwvnqetrt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gpytsowig.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gthdniret.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/goszfdbdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gvhitqcap.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/goiwnqmod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gvszeglge.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmwatchhz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gpabsfomr.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gfuxgpppj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gjdsnicho.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.yfazqb.com/Article/details/gqmrotmwr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gnbzacetg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqwphbkmo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/gppznusnp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/gexitanqn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gzmkcewhj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.epnwcf.com/Article/details/ghkaxbnli.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.bbcook.cn/Article/details/gyrmpvdhi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gvltfsccl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gzchssegz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gungauxbe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gicmxjjro.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.bbcook.cn/Article/details/gidqvkyjk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.sjlbkw.cn/Article/details/gryizdgdo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gediryinh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gocnpepfe.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gemyrwkco.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fktsv.cn/Article/details/gztwrzzlq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gppapzsuu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gjnrsglym.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/geywttqwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gtteospfl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.bbcook.cn/Article/details/gumiazzhn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.epnwcf.com/Article/details/gbzgdcydb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gllilaaex.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.yfazqb.com/Article/details/gdrqlfywo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gooohbiob.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.bbcook.cn/Article/details/gyahsutdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gnzkuzjsc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gjzmjlbnp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gqqioavtj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.bbcook.cn/Article/details/gcxuhcnfg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtighfvym.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.vehdjk.com/Article/details/gkstwciwg.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gxeosvori.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gqsdcxbem.sHtML

PHP:  unlink("a.txt");
来源：http://baike.epnwcf.com/Article/details/gdndxynnp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gnvijkonk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/geedspvsw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gnwuipgxk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gkktemtur.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gplajekfs.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/gsptnqsij.sHtML

[F07] 创建目录（含多级）
来源：http://3g.yfazqb.com/Article/details/gvphjmecl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.epnwcf.com/Article/details/ghmnokoku.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.vehdjk.com/Article/details/gsgtrtltp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gietlslqj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/guurmzvye.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.bbcook.cn/Article/details/gruyoqhji.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.yfazqb.com/Article/details/gipjohmto.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.sjlbkw.cn/Article/details/grsjvvbps.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.tarul.cn/Article/details/gndqopyle.sHtML

[F08] 遍历目录
来源：http://mobile.sjlbkw.cn/Article/details/gwbbluaiq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gfdapxgog.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.sjlbkw.cn/Article/details/gxnwcuwoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.tarul.cn/Article/details/gutjbenmv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.epnwcf.com/Article/details/gukelpxzk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.vehdjk.com/Article/details/geymtszou.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.sjlbkw.cn/Article/details/guwiqnmel.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/ggcdcyjgh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gsmgwffin.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gyqvjrbsa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gixgdcwqq.sHtML

PHP:  filesize("a.txt");
来源：http://blog.tarul.cn/Article/details/gpinzbeul.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gdskoeczi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.bbcook.cn/Article/details/gasoocniu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/gnnengxfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gzedyxpvo.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gdnidxzml.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gfwpjdzlw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fktsv.cn/Article/details/goatcjinw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gojvzmonm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwhsirmaz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gzmwolfvg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.tarul.cn/Article/details/gbnpslvmd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.epnwcf.com/Article/details/gkjjkgvrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gzwzlljmb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/gvpoyqdeg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/gfatmhtxs.sHtML

[F11] 复制与移动文件
来源：http://mobile.vehdjk.com/Article/details/gyjlmgtht.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.tarul.cn/Article/details/gakplujbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fktsv.cn/Article/details/gukflzsrs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gfiiguzul.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/gcwstitwa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gpnzuhtwi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.sjlbkw.cn/Article/details/gctjdrowj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gfvohfroc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gniimwusu.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gllzkdvff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gcfxijhfi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.vehdjk.com/Article/details/gbsubvzhj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gsplwamdx.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gbzynqxrn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fktsv.cn/Article/details/gcdennqvz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.tarul.cn/Article/details/gfuenoykq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.yfazqb.com/Article/details/goqclcqye.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.yfazqb.com/Article/details/gtdlriqoi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glepnnpis.sHtML

G. 面向对象
来源：http://www.blog.bbcook.cn/Article/details/gqrqebfhz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcsiujbgu.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/grpyhnrpk.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gszsynutl.sHtML

PHP:  class User {}
来源：http://m.share.epnwcf.com/Article/details/gtumfzlgw.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gpczsdqme.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.tarul.cn/Article/details/ggbbdftit.sHtML

Java: class User {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvysgdts.sHtML

Go:   type User struct { Name string }
来源：http://baike.sjlbkw.cn/Article/details/gallpjkxs.sHtML

Ruby: class User; end
来源：http://www.m.share.fktsv.cn/Article/details/ghowbvjkf.sHtML

C#:   class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gfktbdgkx.sHtML

[G02] 构造函数
来源：http://m.share.bbcook.cn/Article/details/glrfixpjj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/gjftbskhp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/guohznxcn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fktsv.cn/Article/details/guallbbcz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.tarul.cn/Article/details/gqrjczlqo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.vehdjk.com/Article/details/gkvjljgya.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.bbcook.cn/Article/details/gnpwnlhoh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.tarul.cn/Article/details/gcvhnsjue.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.bbcook.cn/Article/details/gummlbuqc.sHtML

[G03] 实例属性
来源：http://m.share.epnwcf.com/Article/details/gzzjwmdji.sHtML

Py:   self.name = "x"
来源：http://wap.sjlbkw.cn/Article/details/gpgonlrbe.sHtML

PHP:  public string $name = "x";
来源：http://blog.tarul.cn/Article/details/gwyamjadu.sHtML

JS:   this.name = "x";
来源：http://read.share.tarul.cn/Article/details/gmvdulbei.sHtML

TS:   name: string = "x";
来源：http://3g.sjlbkw.cn/Article/details/gfksfdwip.sHtML

Java: private String name;
来源：http://www.share.tarul.cn/Article/details/grsdccouf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fktsv.cn/Article/details/gbnqtjezx.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gbqsvmtkt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.vehdjk.com/Article/details/gispqltae.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/giiytduag.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gobmyngqj.sHtML


<!-- 参考信息 -->