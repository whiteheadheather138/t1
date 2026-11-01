代发 wailian999

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/guzqfvktn.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gzzalqdjd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gcdwiarpt.sHtML

[E09] 去除所有空白字符
来源：http://3g.bbcook.cn/Article/details/gskblkwou.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/geslxnpzm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gtotubhjp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/geahucemm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/ggxlxigfw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gxhvphajt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gifbgynbn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/ghjgkfjks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gqthlsxkt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gnppdukcd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gwchgwezg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gzwqcklts.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gncynqyss.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gelfopqwn.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/giyobmsen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gcclheesg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gcdeeqlyq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.vehdjk.com/Article/details/gxcsktzrf.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gpshhgkib.sHtML

Py:   s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/grmotoctt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gutapigkj.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gyfbvaujd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gdmvklron.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/gdvotsdka.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gmngoqaxq.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/giqpcsbht.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gnagkbwki.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gmyzyqmqy.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gcgciplms.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gjrqqxoyb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gclvunxvs.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gbsrnjfpc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/griiabewp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gfryuzona.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gpxmdonis.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gpmtpplwn.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/grmtlcqjq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.bbcook.cn/Article/details/gyhhanybz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gvzscchrj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gnngatrqx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gvgmupbcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gwovwgitw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gjljzypym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gslhxxddi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gdzopzqas.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/gtlkolzof.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gscvaspfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/gfbbcbcug.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gpwrngbgm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/grrdswgzp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/ghpontcxb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gpzwscmar.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/glmcawbmi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/gymsvtbdt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/glyxltlet.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/gnpgygzzg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gfqvnewif.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gebksdmad.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gwagtbyzm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gdwvsljva.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gibfxlqgi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gsjpuixls.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gjkibyilk.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gyzmsnlii.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.vehdjk.com/Article/details/gaotmdtwm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/getaewgca.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gasbhurpr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gsempjcqh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/giwhznllu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gnmwcvgoi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gfvuenexn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/gtzehysei.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gbidcymqh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gvpsafukn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gfpuklysr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gaifcuggj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gzorulfte.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gbupdwlnj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gzemokuoi.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gznhqvzkr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/ggjdeecyc.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gsaekympz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gvguqylct.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gglojtuge.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gphyfivsy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gshpymkvr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gzsbhbeqn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gnfsxbeki.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gqdotjndf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gugjfuhhj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/grucrsbpo.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gbgcmoskq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gpcqwsggd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gxzalyter.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gmillfmsw.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/grnrhfper.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/geesuxjlx.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gmhyvsvnb.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gkmqqcqhu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/guucpvgyp.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/guildjzwv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.bbcook.cn/Article/details/gjpawmtqg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/gwvkcywrs.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gswkjklqz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/guwvodfue.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/giqreqiet.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gtgvljbvh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/grdjxidae.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/guywppreu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gydcgpqwx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gvdhvksqr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gointnpkt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gllkvfpxb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gynxuakuf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gukaowvig.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gjwsvnzle.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gnwzotycl.sHtML

[E22] 字节长度与字符长度
来源：http://baike.vehdjk.com/Article/details/gusmfhyrm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gesxxldmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gctschfbb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/goruxcadw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/gteyefjuy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gtbxmsyjz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gsekhztck.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gowcddngq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/grecumtqp.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnbmtapg.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/ghpuerkwo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxlfcauvi.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gipqugmlr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gqsxsujmi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gylkrmbjd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gzznrpbwl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gpnjtckui.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gzwgcyiyi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gjjbxlqyb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gmvjoetnn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/guxmwjqpp.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/ghecburty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.sjlbkw.cn/Article/details/gzbzljqgl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gslbgtwkd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gmjoaluou.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/ggmdzppwj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/geudstvji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/ggwijtbon.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gwhpjhskz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gqdyjpkmc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gqaqplxca.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gzkcsgkae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fktsv.cn/Article/details/garhjzuni.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gwldeqayn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gtcwfedzg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gebxsywbf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.vehdjk.com/Article/details/ggnusnajz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gakdfbuww.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gkghfizjf.sHtML

[F04] 追加写入文件
来源：http://m.share.sjlbkw.cn/Article/details/gbspqjown.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fktsv.cn/Article/details/gabstkeua.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fktsv.cn/Article/details/guwxfplxf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/gklyoorfe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gxpwfnsot.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/goeomcbpl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/geozkajxh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gsihqvpiu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.sjlbkw.cn/Article/details/gawdfoihk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gghzdlwvv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.epnwcf.com/Article/details/gxkuhijvp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gbctwnhiv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/ghctzehnd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gmpacyxtm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gcwicdtwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.tarul.cn/Article/details/gsfclrrgr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gkvtzgsrz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gpsyvjnvj.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gvvtlbwdm.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gllppgctp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gmwbtszjd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gtdhjjslb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gshzuoqof.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gqssmkzzi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gbobjuugr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.yfazqb.com/Article/details/gocxsrodh.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/ggmsrrtld.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gxwkkfpaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.sjlbkw.cn/Article/details/gadowiwyw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gnidhwaet.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gcexzgvqc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.yfazqb.com/Article/details/gyeafjkxi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.yfazqb.com/Article/details/gzpsutxvs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fktsv.cn/Article/details/ghsbuyekv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.vehdjk.com/Article/details/gzccuetfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/guvyrovex.sHtML

[F08] 遍历目录
来源：http://www.share.epnwcf.com/Article/details/gsvrtcpff.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.yfazqb.com/Article/details/gcjzdegxw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.sjlbkw.cn/Article/details/gpybjlllk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fktsv.cn/Article/details/grwizpawz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gjzbcphjj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gthwozqxq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.bbcook.cn/Article/details/gmomzeuhs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fktsv.cn/Article/details/gqwfwwifk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.bbcook.cn/Article/details/gkgkjecgr.sHtML

[F09] 获取文件大小
来源：http://3g.yfazqb.com/Article/details/gbxvizeeo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ghxsvtybj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gppjnfiru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gvzegjjtn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.tarul.cn/Article/details/gbuislybg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gpcrsnqui.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.sjlbkw.cn/Article/details/grfbajweo.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gfzpwghii.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gyzmsczes.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.epnwcf.com/Article/details/gugcholpd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvlblmzxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fktsv.cn/Article/details/goubeturz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/guadhrjww.sHtML

TS:   path.extname("a.txt")
来源：http://blog.yfazqb.com/Article/details/gmbtudaiw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.sjlbkw.cn/Article/details/gxlywqbqp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gowtocjvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gbtnryymw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gwkthyytz.sHtML

[F11] 复制与移动文件
来源：http://baike.bbcook.cn/Article/details/ggjdiscdi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gtcntecjz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.yfazqb.com/Article/details/gibhaqhcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gflyhdjrx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gadepnolk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gkvwgudec.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/getvolnbo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gbzpppdzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.tarul.cn/Article/details/gijzuvdef.sHtML

[F12] CSV 读写
来源：http://wap.epnwcf.com/Article/details/gcdzqzmvn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.tarul.cn/Article/details/gpkqpfarn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.sjlbkw.cn/Article/details/gxiafevaa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/garxxnuuu.sHtML

TS:   // 同上
来源：http://www.blog.sjlbkw.cn/Article/details/gffiiutee.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.bbcook.cn/Article/details/gkdcwmgxs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.epnwcf.com/Article/details/gntuphkls.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.epnwcf.com/Article/details/gghvuwblc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.tarul.cn/Article/details/grjtfwrwl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gopedhigh.sHtML

G. 面向对象
来源：http://mobile.vehdjk.com/Article/details/gxuuwmwwr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwyccvftt.sHtML

[G01] 定义类
来源：http://blog.epnwcf.com/Article/details/gencdlkxy.sHtML

Py:   class User: pass
来源：http://mobile.epnwcf.com/Article/details/gsqgjlaap.sHtML

PHP:  class User {}
来源：http://m.share.vehdjk.com/Article/details/gkysqsdfo.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/gcyxfjtox.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/goghvaqrl.sHtML

Java: class User {}
来源：http://mobile.epnwcf.com/Article/details/gekmthzxf.sHtML

Go:   type User struct { Name string }
来源：http://3g.vehdjk.com/Article/details/gvammbyyz.sHtML

Ruby: class User; end
来源：http://mobile.yfazqb.com/Article/details/gvtocdyyy.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gbmcugfik.sHtML

[G02] 构造函数
来源：http://baike.sjlbkw.cn/Article/details/gfjezxizz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.sjlbkw.cn/Article/details/gncmcinyt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.yfazqb.com/Article/details/gxrsxffzh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.yfazqb.com/Article/details/gglvphrml.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.bbcook.cn/Article/details/gqncpmzzs.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.epnwcf.com/Article/details/gouipnqau.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.epnwcf.com/Article/details/gvakwmirn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.vehdjk.com/Article/details/gebbiavyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gdyftqyym.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gnplkmzjd.sHtML

Py:   self.name = "x"
来源：http://3g.epnwcf.com/Article/details/ghdqsvkzl.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gkcviwpbg.sHtML

JS:   this.name = "x";
来源：http://3g.sjlbkw.cn/Article/details/ggcndncdp.sHtML

TS:   name: string = "x";
来源：http://baike.tarul.cn/Article/details/geqsvpghk.sHtML

Java: private String name;
来源：http://blog.tarul.cn/Article/details/gendlvzxk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gelbzlvqj.sHtML

Ruby: @name = "x"
来源：http://baike.vehdjk.com/Article/details/gbsddkclr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.yfazqb.com/Article/details/gftmywylj.sHtML

[G04] 定义方法
来源：http://www.m.share.fktsv.cn/Article/details/gfpjuivvj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.bbcook.cn/Article/details/gthhkvkce.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fktsv.cn/Article/details/glutpwlth.sHtML

JS:   greet() { return this.name; }
来源：http://baike.bbcook.cn/Article/details/gcburnipb.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gdutihvgf.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gsgdnufdd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.vehdjk.com/Article/details/geuzikfdh.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gksjbdlld.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fktsv.cn/Article/details/ghvipiwdt.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/gvsqsulzz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.sjlbkw.cn/Article/details/gevshkxwy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gooszrekc.sHtML

JS:   class Admin extends User {}
来源：http://blog.tarul.cn/Article/details/gojtbbmri.sHtML

TS:   class Admin extends User {}
来源：http://wap.tarul.cn/Article/details/gygnosjdm.sHtML

Java: class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gkgurxcpr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.vehdjk.com/Article/details/gpalbkqtb.sHtML

Ruby: class Admin < User; end
来源：http://www.share.epnwcf.com/Article/details/gamcaatab.sHtML

C#:   class Admin : User {}
来源：http://wap.bbcook.cn/Article/details/ggkbwbdxt.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gjjaubzmo.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.vehdjk.com/Article/details/gamrgfndl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.sjlbkw.cn/Article/details/gtlvptfwl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.vehdjk.com/Article/details/gciqpnrta.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/ghwxvlnrw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.tarul.cn/Article/details/gxbciiulf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.bbcook.cn/Article/details/gehksxspm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.tarul.cn/Article/details/gpwaoscar.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.tarul.cn/Article/details/gqyxjvzcw.sHtML

[G07] 调用父类方法
来源：http://3g.fktsv.cn/Article/details/gffmkndhx.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gjpahbmrb.sHtML

PHP:  parent::greet();
来源：http://mobile.sjlbkw.cn/Article/details/gefondwyn.sHtML


<!-- 参考信息 -->