代发 wailian999

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gzkefjano.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gavrxekeo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/gzyhwrjad.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gjifxyvip.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.yfazqb.com/Article/details/gycuchopk.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gwvubqtcd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/gvcgqjmht.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/goirmobsm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/gwuburrys.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gxkqxqhel.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gglioyjbe.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gakzhhfms.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gmpcgrjpn.sHtML

JS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gwwndluha.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gingtopvw.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gozyeewlv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gskleeezs.sHtML

Ruby: items.join(",")
来源：http://blog.tarul.cn/Article/details/gqxymsidk.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gaxtaxmix.sHtML

[E09] 去除所有空白字符
来源：http://blog.sjlbkw.cn/Article/details/gvnbyjxro.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/gzqmhnqaa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gazsbwqjo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gnqfufgai.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gvsavoahu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gwxqkznqp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.epnwcf.com/Article/details/ghllskvce.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gwbuvrvzv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/guedkssiw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gfnrtirde.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gajhogeis.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/grulwiduh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/ggggftfsv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gnkjyquys.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gpmzbrskw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gwfxdeanz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gisnemepz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gwquauaix.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gtrhawefs.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gcnkxuttq.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gfhwrqrin.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gfciyhzgu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ghxwjixxd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/ggxantswz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gopouyawh.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gqobornze.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gordhwzfu.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/gsiextrcm.sHtML

Py:   s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gdyvirsgb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gklzcibcb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/goscuefav.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gndogdyqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gqvoyeqji.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/grepqwwbp.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gclzsoear.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.vehdjk.com/Article/details/gfwlflhpb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gqwjiatbr.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gdcjtwjhg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/gmdwfpkwn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gypzbagdb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gwwcvxyue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gpngltyys.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gszwocuzq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/ghwvdujru.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gkoxdncjd.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.vehdjk.com/Article/details/gedycltsh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gzhidlasn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gvbbydkkz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/geuylqsht.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gqropcdwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gwvpkyxkq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gfpvfbvcz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gwtginqpr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gyhcrqovi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.bbcook.cn/Article/details/gviqdrhap.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/girmriboi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/gvnocvlhg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/giuhwwooz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gljpjeccz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/golmwakni.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gjzgrtpoe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ghymgarwi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gmefbikle.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gwqjakdal.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/glrokyxvs.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gfcpknjto.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gniqismbw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gszbfoitj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/grgpkypzp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gyvqeizao.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gucobhfeq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/gcaomfafs.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gxtzipwgc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gjkcyymnq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gsfssnfxs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/giosyunnf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gsrbstxlq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbspyvxzd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gkakzwkec.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gpjeijogb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/guaapgnfn.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/guhuoevfs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gehazmvuk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/glfxguruk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gioubsqiu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gwezsolpv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gwqiyxjph.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gzemonhpw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gwepwxfix.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gexvbiyfn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gwtnjyfnn.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/gujgdmnls.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gawyzyvco.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gitlahfmn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/glxkiltxa.sHtML

Java: s.lines().toList()
来源：http://baike.bbcook.cn/Article/details/gzmdawrgu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gslrsmtjx.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gaefxtxmz.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/ggworofus.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gacrdczxq.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/gsozbpllk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gtcocxwgh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/gtikkmseh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/gtlzmnhvj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gopzfnswx.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gqytajtvy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/guuevnpjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gkprelfuy.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gaxisceih.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gzgnklgif.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gepwktlhd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gkaofaemj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/ghievigdu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gmdvbjdec.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/gizkehnmn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gosootskr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gefjpyizh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.bbcook.cn/Article/details/gvpitaewx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.vehdjk.com/Article/details/gzhvrwyul.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/guzfzemhu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gdejemfjz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gxxqcgasj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.sjlbkw.cn/Article/details/govvqsjcw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/ggenfbdrv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gmobepalh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gfepytsqv.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glpkpqlzg.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/geboplizz.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/getumkbbm.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gzcjqfklm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/glcbyshgw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/giaisqyrk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.yfazqb.com/Article/details/glyfmtiqv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fktsv.cn/Article/details/gtunlnhwa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gqtpsnuwz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gqekejhko.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/glvhvzbyu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/grmdudsnq.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/grubtszez.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/grbiggkal.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gcnwegkka.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gowzrgcoz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gaohekkrp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/guudwbdby.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.tarul.cn/Article/details/gxrglsbsz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gpzxdmapa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gqnloonku.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/giveujrsv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gxfexzlon.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gddfkzeox.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gdxmkdshn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gqbfbqfuu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gbegecuyf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gnasvealg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.bbcook.cn/Article/details/gvsqthhgv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gkvqhirmn.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/gqwvjljcg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gnwatkryj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gwidozkzj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gppjroyov.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/grzbjautl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.epnwcf.com/Article/details/ginlmbxss.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/grehuzqcc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.bbcook.cn/Article/details/gaeabveun.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/gljedjubb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gitzlxduy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gpbyxzvhd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/giofeshkq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gggpilafw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gbzktknfq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gbaritqhz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.vehdjk.com/Article/details/gzqjafkfv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gcgfkmfxf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gscukuxjf.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/gqdlovxsn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guzeiidic.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gdlqfqqhk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gaceucwqe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gtjxxmbju.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gakbsqihr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjcugrarp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gvxdjlfsg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gidthjtvw.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gtwdlyobo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.yfazqb.com/Article/details/gulpwovks.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gkkoggpds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gyejkofiy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gzomlpzbc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.vehdjk.com/Article/details/girizdgwz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gqfwmvvdb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gpceeowjs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.sjlbkw.cn/Article/details/gramjkosv.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gmizrooyu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gjsgpnnof.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gtxttwwzf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/ggowoxkxh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gdikbebde.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.sjlbkw.cn/Article/details/gkeuayion.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.yfazqb.com/Article/details/ghpunzdpt.sHtML

Ruby: Dir.children("dir")
来源：http://baike.sjlbkw.cn/Article/details/gnfxuzchj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gylvsrqtw.sHtML

[F09] 获取文件大小
来源：http://www.blog.bbcook.cn/Article/details/gbqpdbhmh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fktsv.cn/Article/details/ghqpwcila.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gnojneqbi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gegpythrq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.bbcook.cn/Article/details/glaxpurfd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gahpdmbjr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.tarul.cn/Article/details/ggqwbcvqy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gtvofucoz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fktsv.cn/Article/details/gzvzqmkfz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fktsv.cn/Article/details/gytnolvge.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gjoychsla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gfupwtsqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gobdwrjkb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.vehdjk.com/Article/details/gwejbrbex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.bbcook.cn/Article/details/gqyrncwja.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gysdjlmfz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gxbajjvdt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gddovicje.sHtML

[F11] 复制与移动文件
来源：http://read.share.yfazqb.com/Article/details/gbhdtmhnn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/gqvdwvuyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.bbcook.cn/Article/details/gafpdnhog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/guqsjqmea.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.epnwcf.com/Article/details/gqfefifdc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/geolhfoms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.epnwcf.com/Article/details/gttebfwnc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gulgtmyll.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.epnwcf.com/Article/details/gvhrpsvvo.sHtML

[F12] CSV 读写
来源：http://www.share.fktsv.cn/Article/details/gizmfcndr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.yfazqb.com/Article/details/gudztblqi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.tarul.cn/Article/details/gnlaeggob.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fktsv.cn/Article/details/gxbjdfgxl.sHtML

TS:   // 同上
来源：http://3g.fktsv.cn/Article/details/grxrrsalv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.bbcook.cn/Article/details/gpuikkxsi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.sjlbkw.cn/Article/details/gnvbhmsed.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.sjlbkw.cn/Article/details/gqwlbbavx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.sjlbkw.cn/Article/details/ghxewaqci.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwgacpctj.sHtML

G. 面向对象
来源：http://m.share.sjlbkw.cn/Article/details/gtrvxcrxj.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnyalyfkl.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/grqpknkae.sHtML

Py:   class User: pass
来源：http://mobile.tarul.cn/Article/details/gcwuydfme.sHtML

PHP:  class User {}
来源：http://www.m.share.yfazqb.com/Article/details/gstjewart.sHtML

JS:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gddbwhmyk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.bbcook.cn/Article/details/gshafpeeq.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gvwzjfscg.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gngxpdynw.sHtML

Ruby: class User; end
来源：http://wap.fktsv.cn/Article/details/gwtomscdq.sHtML

C#:   class User {}
来源：http://m.share.fktsv.cn/Article/details/gxkjroawd.sHtML

[G02] 构造函数
来源：http://www.share.tarul.cn/Article/details/givmtpine.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.yfazqb.com/Article/details/gkbghrzwk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.epnwcf.com/Article/details/giareeztl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.yfazqb.com/Article/details/gwqvlvlva.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fktsv.cn/Article/details/gceoctzmj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/gabbjrpfu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.epnwcf.com/Article/details/gbtvbfzsl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.yfazqb.com/Article/details/gkjnucrxz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.tarul.cn/Article/details/ggrvsesjk.sHtML

[G03] 实例属性
来源：http://m.share.bbcook.cn/Article/details/gdxxscyrd.sHtML

Py:   self.name = "x"
来源：http://mobile.vehdjk.com/Article/details/gxeueawvy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gcxfrvjjn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fktsv.cn/Article/details/ghkqsxieg.sHtML

TS:   name: string = "x";
来源：http://3g.fktsv.cn/Article/details/gsrrkmsud.sHtML

Java: private String name;
来源：http://read.share.tarul.cn/Article/details/gmnxdvakf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.sjlbkw.cn/Article/details/gxdowerah.sHtML

Ruby: @name = "x"
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjnpwrpw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.epnwcf.com/Article/details/gwubdasyx.sHtML

[G04] 定义方法
来源：http://baike.sjlbkw.cn/Article/details/grryotgyk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/geymkavvt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.epnwcf.com/Article/details/gwpjqzmhs.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fktsv.cn/Article/details/gbeextjkp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.epnwcf.com/Article/details/gcyhucolf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtktqxtji.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gedzanvjw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fktsv.cn/Article/details/glyxxhbln.sHtML

C#:   public string Greet() => Name;
来源：http://3g.epnwcf.com/Article/details/gyrctbivf.sHtML

[G05] 继承
来源：http://wap.yfazqb.com/Article/details/guvciekwh.sHtML

Py:   class Admin(User): pass
来源：http://baike.tarul.cn/Article/details/ginuodpzw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gxglfotjz.sHtML

JS:   class Admin extends User {}
来源：http://m.share.sjlbkw.cn/Article/details/ggxdyyyjx.sHtML

TS:   class Admin extends User {}
来源：http://wap.epnwcf.com/Article/details/gpjakpzqk.sHtML


<!-- 参考信息 -->