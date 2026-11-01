代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/ggaalapgl.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gprilofkk.sHtML

C#:   string.Join(",", items)
来源：http://baike.epnwcf.com/Article/details/gslaxneky.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gtfidtvwy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gwnbibdui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/ghnpvzgvp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gcjfunrst.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/glpxcblle.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gprhjtocn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gkgkbvjuu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gwcqghnjt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gkycrhune.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gvfdeinqc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/greikjavp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/geknnhfoa.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gzqsewepk.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gceqcbedf.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gdqkwzfbk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmeqvsbtf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/grkszpkqe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gdddtasxj.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gdzciceak.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/ghvkcplan.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gcrckdwmh.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gnyqqzhyu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gnutnrglu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/ghszwznsu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gicirkrbf.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gkiyyemja.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpamkqus.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gprnujghe.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/gsvygpnda.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gfdyenlhw.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gyewqlnhb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gnyozwtjj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gkixtllpp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/genwnmcgn.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gqtzbretu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gbxaqvuey.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gznuezbnx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fktsv.cn/Article/details/gqqcmeiec.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gtahrumss.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gymovvduk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gseacwfzi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/ghlrjleui.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gieapfrjf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.bbcook.cn/Article/details/gyptgqduw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/ghgijwdek.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/goodrrrit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gxyuceuzw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gsddwlnwz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gdapveatb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/gvrfothep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/goqxicqsj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.sjlbkw.cn/Article/details/gylsjhhwe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/gfebsvyvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/gwislkkgy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gvudhwnuw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxytdhqbo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gqvimqjcb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gswchhytr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gqagaiwpx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/giywncvlu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gknariyty.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.tarul.cn/Article/details/gvzgyiaip.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.vehdjk.com/Article/details/gnskyzvif.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gviqioclw.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/grfpuxoir.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gwncvegoa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/galjfhfvp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gblihvrnr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gtdmqccwe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gxxpkyfuk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.vehdjk.com/Article/details/gkxbjxaus.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gsarcckqu.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/giqtwbqge.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/guwvfkaww.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gulyqnpri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gvvbehfor.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gykriazni.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.vehdjk.com/Article/details/gzenqcsox.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gzchayjjr.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gxpmcnkte.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gobxkuuhq.sHtML

[E18] 模板占位符替换
来源：http://3g.fktsv.cn/Article/details/gxgyqhvkm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/gdcyncler.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gswhdxbad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gfashtfpg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gckoghffk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gbpophdxu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gkmninrae.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gvhnslual.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gvbtsxmta.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gvmkwdpzo.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gtxxqmioc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gcvxeonyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/ggvfmzfsd.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gxsdghphv.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/grubablmq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gqpobfxio.sHtML

Ruby: s.lines
来源：http://read.share.sjlbkw.cn/Article/details/gmorwwnsu.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gfsmfqauf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gabosffml.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gdkqvacow.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/ghvpkmmpx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gfqwbefyk.sHtML

TS:   if (s === "") {}
来源：http://baike.epnwcf.com/Article/details/gtdobuuhg.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gxmddbqlt.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/grekxxipx.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gadipfmvj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gmghybolj.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gtlznvteo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gzvtwutmx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gclclklaa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gxmfyvxze.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gmsmvutnk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/ghbmdazmq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/gjgktmhjd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gogcwojqs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gusfrajud.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gqwlaiolj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/geewxxabc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gtctxyuvr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gvgomzfqu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gmigrzfpg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gushqbkns.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gjyzbpjph.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gklvgexaj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gpjspojno.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghxsjpbul.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gmeiswkda.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzcupzddc.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gxgpgfqyp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/glzqvhtgv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gjtckxrek.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/ghmhupqwr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gsqgjefmp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gpijqdpyj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/gblrarogg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gezkzytmu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ghbafqdvn.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gxnzhthxb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.epnwcf.com/Article/details/gppqtudtn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gzlvvejwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/goommdzxv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/ghlpbzthj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gcclhprnf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.sjlbkw.cn/Article/details/gczyyxuqy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gszbmvftt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gwypzzttq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gnhtprgei.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/grhqcjdgi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gomycmiki.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ggseyrhnt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gyvgnbjcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/glzloufsl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/gkutfcshp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gdzxqdybv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.epnwcf.com/Article/details/grupkbzea.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/gfivghrgs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.tarul.cn/Article/details/gzvuerrog.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gvxnlzwju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gkntiydnn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/gyrmavqxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gnxbltbra.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gyjmjwdyg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gtabbhheu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gndxzqxnq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gjdwywyfj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/gnmqtozzs.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gbergbmhi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gsennhdhx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/geszppqbe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gihpbjazj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gbtnbqzmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gcannywfs.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gkzkxldpo.sHtML

[F06] 删除文件
来源：http://www.share.yfazqb.com/Article/details/gsbggfitd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/glvsdncrj.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbonlifzj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gdtsxgmyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gvfgigpqp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gczeyigwo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/guwjyjdkf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gvyvvhvss.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.epnwcf.com/Article/details/gppoycigr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gdnmoatsw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gkxgvujvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/gmtvvvlvw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gmgnvzcgb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gngzodkww.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/grbxvtvzm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fktsv.cn/Article/details/gnguikzmn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.sjlbkw.cn/Article/details/gcsxdzjdd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/ggkagiptc.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/geqbgubuj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.tarul.cn/Article/details/gpkxfbqph.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gbxmcgrhp.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gupuljuwz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/goasgvhdz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gyrpygkev.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.yfazqb.com/Article/details/gduvfpvzf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gscvgidix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gbymloiwk.sHtML

[F09] 获取文件大小
来源：http://www.m.share.epnwcf.com/Article/details/gcnpkgwqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.vehdjk.com/Article/details/gvgfcjawt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gykpmdqty.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gyquttmob.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.tarul.cn/Article/details/gffmhahls.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gnkgmjzyt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.sjlbkw.cn/Article/details/godcxylek.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gjrcjnesb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvougjrpt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.sjlbkw.cn/Article/details/gmasoznwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gmvsbfbby.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.sjlbkw.cn/Article/details/ghfvscoyk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gsunmcxmw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gdfvhlmim.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.bbcook.cn/Article/details/gvxjzjoqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gmiaywuke.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gndhzpoww.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gkvarwojz.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/ggnkjcmrj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gncehlonz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.yfazqb.com/Article/details/gmbcjdgev.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gybuclbkj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.vehdjk.com/Article/details/gqfrahpgk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.vehdjk.com/Article/details/gipqmamct.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fktsv.cn/Article/details/gppdwsqit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gaotaunsb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.yfazqb.com/Article/details/gkdilwxjo.sHtML

[F12] CSV 读写
来源：http://www.m.share.epnwcf.com/Article/details/gdyxsvijv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.yfazqb.com/Article/details/gqgocmlsp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.epnwcf.com/Article/details/gcrxqopck.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fktsv.cn/Article/details/gdfeqkbqv.sHtML

TS:   // 同上
来源：http://blog.fktsv.cn/Article/details/gdaxgazbm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/grvixboir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gzonkplrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.tarul.cn/Article/details/gdkqhgdqc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/gaoybkclj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmdyudva.sHtML

G. 面向对象
来源：http://baike.sjlbkw.cn/Article/details/gmzyojzez.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gorgfwrpt.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/gyiayzymd.sHtML

Py:   class User: pass
来源：http://www.share.bbcook.cn/Article/details/gisyktqno.sHtML

PHP:  class User {}
来源：http://www.blog.tarul.cn/Article/details/gjmlxdgdj.sHtML

JS:   class User {}
来源：http://wap.sjlbkw.cn/Article/details/gapktxupd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.bbcook.cn/Article/details/gkxcschtr.sHtML

Java: class User {}
来源：http://blog.epnwcf.com/Article/details/gamthtosc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.sjlbkw.cn/Article/details/gyxllfvyx.sHtML

Ruby: class User; end
来源：http://3g.fktsv.cn/Article/details/gywogstuy.sHtML

C#:   class User {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqofzbfei.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gdvqfmvre.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.yfazqb.com/Article/details/gifzeunvp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxlygcicl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.vehdjk.com/Article/details/gbhqoigwm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.vehdjk.com/Article/details/gmflkbkpu.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.epnwcf.com/Article/details/gkfjfsucc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fktsv.cn/Article/details/gwivzbbry.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.bbcook.cn/Article/details/gfuizhakk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.yfazqb.com/Article/details/gtcevvolj.sHtML

[G03] 实例属性
来源：http://read.share.tarul.cn/Article/details/gkmwhmwae.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fktsv.cn/Article/details/gkgzvrkva.sHtML

PHP:  public string $name = "x";
来源：http://wap.bbcook.cn/Article/details/gkqpkrssj.sHtML

JS:   this.name = "x";
来源：http://www.share.fktsv.cn/Article/details/glxqwnweb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcckxexh.sHtML

Java: private String name;
来源：http://baike.bbcook.cn/Article/details/gtrmguhqz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/gkggussjd.sHtML

Ruby: @name = "x"
来源：http://m.share.vehdjk.com/Article/details/gqkpzpolu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.yfazqb.com/Article/details/gxiocyabs.sHtML

[G04] 定义方法
来源：http://3g.bbcook.cn/Article/details/gksxthjfw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gaxnqxldf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.sjlbkw.cn/Article/details/gdntlixrs.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gfghrcjhl.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gsomzuvir.sHtML

Java: String greet() { return name; }
来源：http://baike.epnwcf.com/Article/details/guldmprxj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.epnwcf.com/Article/details/gvhfhnkys.sHtML

Ruby: def greet; @name; end
来源：http://www.share.yfazqb.com/Article/details/gpexqsgfc.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fktsv.cn/Article/details/gjqnavvpv.sHtML

[G05] 继承
来源：http://blog.vehdjk.com/Article/details/gmabfenpv.sHtML

Py:   class Admin(User): pass
来源：http://baike.sjlbkw.cn/Article/details/gevcpsxid.sHtML

PHP:  class Admin extends User {}
来源：http://baike.yfazqb.com/Article/details/gqcthmnfr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.bbcook.cn/Article/details/gohslrhbt.sHtML

TS:   class Admin extends User {}
来源：http://www.share.tarul.cn/Article/details/gsepgispb.sHtML

Java: class Admin extends User {}
来源：http://baike.fktsv.cn/Article/details/gvtiluige.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.sjlbkw.cn/Article/details/gehinnkmk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.yfazqb.com/Article/details/gltvtwzvm.sHtML

C#:   class Admin : User {}
来源：http://www.blog.bbcook.cn/Article/details/goyognyax.sHtML

[G06] 重写方法
来源：http://www.blog.epnwcf.com/Article/details/gwnbdmmpn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.epnwcf.com/Article/details/gaetckvlu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.vehdjk.com/Article/details/gcfhhzujf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwhrjnzp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fktsv.cn/Article/details/gbbnismqu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/gfhcjlghs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.yfazqb.com/Article/details/gualkmwdb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.bbcook.cn/Article/details/gxusalthk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.bbcook.cn/Article/details/gzelarjkt.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/glujtyida.sHtML

Py:   super().greet()
来源：http://wap.yfazqb.com/Article/details/gznmssvot.sHtML

PHP:  parent::greet();
来源：http://baike.vehdjk.com/Article/details/ggdpxdzjt.sHtML


<!-- 参考信息 -->