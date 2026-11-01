代发 wailian999

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/gvkrzccrq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/glkpefywe.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gxtfbrcqc.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gqgsmqrwk.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.vehdjk.com/Article/details/gpcxersyx.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gjswymhnq.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/ghyzlyrra.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/gzdlctmjb.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gqhumbwqy.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gvlijbstk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gckicfbbk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gavizahgo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.sjlbkw.cn/Article/details/glzbfzhfn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gdcbzuqbd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gnyrjkbll.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gazjygqqu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gitajmfaq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gfdlkkdgj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gggifiqlh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gklimftaj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/ghpinesbw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gyjtlzkay.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.epnwcf.com/Article/details/gxlpnqweb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gjewunfmw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/glpohpczp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gyyntermb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gyogvkgbr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gsqbnqkds.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gjoofopsm.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gdemxjixc.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gperrxdeu.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/guyqoewxb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/grpadvjsx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gdabrrzwm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gjalmzsed.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.tarul.cn/Article/details/gsfedaoxj.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gixbatjnw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/glejfvfvl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/getlatblu.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/glxccscdb.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gyibihfif.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gdabjjynu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gzovqbkcf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gehsuryag.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/gozhbbmar.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gihrzwftv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gfdhsutxi.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gcgxmwscp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.sjlbkw.cn/Article/details/gmedkaqlo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.epnwcf.com/Article/details/gqmyqsaie.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gtchxjlco.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gdmwhijvo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gebdznrih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gcgdqqukj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gsqtmbkon.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gzxlqoyzc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gcxjzdvaa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gzkryicob.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gbjkdbgmq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gcgrfpywl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gcbilgssj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gaoegowuw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gktawflzi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gsxxajtuz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gzzbkigag.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gcpwidlpn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gugmfjmia.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdzcqaqrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gwsujwizp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gjajprpvl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/gdptqipht.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzprmeyio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/guaqhffzp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.bbcook.cn/Article/details/gczmlxkpz.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/gstxvbmkx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.bbcook.cn/Article/details/ghzmcxirk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gzbfcbwyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gtolyjcaq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/goygklhpd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gdaahxnmj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/gjsukowab.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/gpjvmjuis.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/givkrrmyi.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gcnentwlo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gtbrwfkco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gcpbucawt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gwrwxusqy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/guabmfeyp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gvvfwifxw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gsrwwggei.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gkugegjex.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/ghymdpvsb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gyglzfnsw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gporyrgea.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.yfazqb.com/Article/details/grmirthpv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gpvtvmpvd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gvfzwzmzc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gdjiswrmy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gzpwpbtkg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/ggzocytlc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gwoshrdru.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gtdjiwzrg.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/gyqmhdlwu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gstzznjyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/genbyajqk.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gxczgpvsc.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gfiwiqdsb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gvtqaqlmw.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gfrpffnis.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gvvovshap.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.yfazqb.com/Article/details/gtzydocob.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/ghbiyywyq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/gaoxeltpy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/grzzlrfgt.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gpztvydsd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/glnjvyryg.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gceqlnyjq.sHtML

Ruby: if s.empty?
来源：http://wap.sjlbkw.cn/Article/details/gzidzjilf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gtosokrjn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/gdjfhaxwj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/grsyuxckk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gfvmsdpwv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gjfyhqcid.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gpxfdsojq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gsbxqixtf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.sjlbkw.cn/Article/details/gqnrckkzn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/ghwksuxfw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gejvtvqko.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gstocyekr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gflgjtcdw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/ggxymjlfh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/genhovmey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gufboocdl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gpreyxdmt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gifbpzoef.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gwhmykuiu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gpkijkgmz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnpmikvqv.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gtcrqmiqh.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqokacjnk.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gchmnbtmo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gjvwvudqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gnbiggozy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gaglnqwkb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gpeoxejax.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gmlpdanjm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gzerhanor.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggdvpguxq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gpdymecxw.sHtML

[F02] 逐行读取文件
来源：http://baike.epnwcf.com/Article/details/gtsifskvc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gdvshksvt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gzhrvdbls.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmvvorqmx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gfasefqpu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gdumkmoxt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/ghdieuggu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/ggtuczfas.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gaadrmwlz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/goolbsdio.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.yfazqb.com/Article/details/gdmxaealk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/glvxjngzl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/govceqpfp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gtyrgvtus.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gawmrnaan.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/gahvwlwbm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gbnzgqpol.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gmixcrsof.sHtML

[F04] 追加写入文件
来源：http://m.share.epnwcf.com/Article/details/geyiqfdgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gfyilghbx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gaaezbueg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gafuupgkp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.tarul.cn/Article/details/guaqgbvdx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gejnebmxh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.sjlbkw.cn/Article/details/gljvjlism.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/guxaewtiw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gzepnknhk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.tarul.cn/Article/details/gqovouzpi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.bbcook.cn/Article/details/gdzyjecpy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gtoxxsbse.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gxyjeekof.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbwefafze.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gagijjmhc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gsfyclylh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gyqciefkx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gmntriauq.sHtML

[F06] 删除文件
来源：http://read.share.yfazqb.com/Article/details/gvyjilemh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gymnepodg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.tarul.cn/Article/details/gdfsxzpza.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/guxibgaqs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxbhmduhh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gukhcpvtg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gssianjer.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gpuhzxqhu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.tarul.cn/Article/details/gozaqmocv.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.epnwcf.com/Article/details/gsqltrarm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gybspuvds.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.tarul.cn/Article/details/gfzshbgpy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/gfcsjwnzq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/geibvchvt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/glsxpyima.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.epnwcf.com/Article/details/gzvbdixxz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gntjxvzne.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.epnwcf.com/Article/details/gcemuqwnb.sHtML

[F08] 遍历目录
来源：http://wap.yfazqb.com/Article/details/gihdjqdog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fktsv.cn/Article/details/gvjlausjf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gjobdalrp.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gcypkinsr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gkapitczv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.yfazqb.com/Article/details/gkaolkknv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fktsv.cn/Article/details/ghsrlnatf.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gemmphqqr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.epnwcf.com/Article/details/gqzyzerkc.sHtML

[F09] 获取文件大小
来源：http://blog.yfazqb.com/Article/details/gtxhlmijy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsoquxpox.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gnvyyvrpb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjaubvjc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.bbcook.cn/Article/details/gxwwbfnes.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gprtlqntl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.vehdjk.com/Article/details/gkhcsdrmm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqkhidedl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.epnwcf.com/Article/details/gekgozjfk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fktsv.cn/Article/details/giznozlsp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.bbcook.cn/Article/details/gpfuyqkwr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gkqdhxdbq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/gewkdytrd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdagykuyu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.tarul.cn/Article/details/grbsxxxlh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gogjacbrm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gnegoffta.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gyctdroye.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/glykhvjwf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/gtmkzpujg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.tarul.cn/Article/details/gslajqofe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gzafhgshu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gcmzoiyfo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.vehdjk.com/Article/details/gqplenpff.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fktsv.cn/Article/details/gvsmmvzdf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fktsv.cn/Article/details/gjmbhoksj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.tarul.cn/Article/details/gvtsyfxqx.sHtML

[F12] CSV 读写
来源：http://blog.epnwcf.com/Article/details/grcjgzliw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.tarul.cn/Article/details/gxczfqylk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fktsv.cn/Article/details/gvjpozbwc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fktsv.cn/Article/details/gjnvorglw.sHtML

TS:   // 同上
来源：http://3g.tarul.cn/Article/details/ghpeekqwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gapklxhsy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.vehdjk.com/Article/details/gxeakogqk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/gxdzflvkx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.tarul.cn/Article/details/gaxheykxn.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjhoipsuy.sHtML

G. 面向对象
来源：http://read.share.sjlbkw.cn/Article/details/gfcbwalyf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzecyxcbe.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/glceaihnb.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/glnlqmopa.sHtML

PHP:  class User {}
来源：http://www.blog.yfazqb.com/Article/details/gkwplrwxo.sHtML

JS:   class User {}
来源：http://baike.epnwcf.com/Article/details/gwrecjqdc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.yfazqb.com/Article/details/gxgfzlcph.sHtML

Java: class User {}
来源：http://m.share.fktsv.cn/Article/details/gnjakhwfw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.yfazqb.com/Article/details/gbjuvvrsu.sHtML

Ruby: class User; end
来源：http://blog.epnwcf.com/Article/details/gxyyskois.sHtML

C#:   class User {}
来源：http://www.blog.vehdjk.com/Article/details/gffcawmlq.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/guinrzpum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.sjlbkw.cn/Article/details/gicplkknn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.vehdjk.com/Article/details/gehqhrkqj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gxscxqqsj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gwfccjkwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gkqmfrimu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.sjlbkw.cn/Article/details/giwocbapy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.yfazqb.com/Article/details/gneuvoufc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gguykprfv.sHtML

[G03] 实例属性
来源：http://www.m.share.fktsv.cn/Article/details/gydrgbiji.sHtML

Py:   self.name = "x"
来源：http://blog.tarul.cn/Article/details/gbsumakcu.sHtML

PHP:  public string $name = "x";
来源：http://3g.sjlbkw.cn/Article/details/gikhfgxzx.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/giatjntpc.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gsoylyeoc.sHtML

Java: private String name;
来源：http://3g.yfazqb.com/Article/details/gzcfmdgph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.yfazqb.com/Article/details/glthuuqam.sHtML

Ruby: @name = "x"
来源：http://www.share.bbcook.cn/Article/details/gafxeddhr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.vehdjk.com/Article/details/gevlxrvvm.sHtML

[G04] 定义方法
来源：http://mobile.bbcook.cn/Article/details/gjzrjeqet.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.epnwcf.com/Article/details/gimkgobpr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.tarul.cn/Article/details/gxkxguqcb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.tarul.cn/Article/details/gxkghbnsw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gfkcsucrt.sHtML

Java: String greet() { return name; }
来源：http://m.share.fktsv.cn/Article/details/gbgptnuww.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fktsv.cn/Article/details/ghgnhieeb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.yfazqb.com/Article/details/gufkqgflz.sHtML

C#:   public string Greet() => Name;
来源：http://baike.tarul.cn/Article/details/glanozsko.sHtML

[G05] 继承
来源：http://www.blog.sjlbkw.cn/Article/details/ghugvuggb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.bbcook.cn/Article/details/ghmrkmxxf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/godxzltbo.sHtML

JS:   class Admin extends User {}
来源：http://mobile.yfazqb.com/Article/details/gfjcdbahg.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gvqobrqmu.sHtML

Java: class Admin extends User {}
来源：http://m.share.tarul.cn/Article/details/gvyrpawic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.yfazqb.com/Article/details/giqjmvhsb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fktsv.cn/Article/details/gfopucxvm.sHtML

C#:   class Admin : User {}
来源：http://wap.sjlbkw.cn/Article/details/gcyhhqosn.sHtML

[G06] 重写方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gjldyqhys.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.bbcook.cn/Article/details/gnozktiha.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fktsv.cn/Article/details/gbsrcopak.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.tarul.cn/Article/details/gxugbauvo.sHtML


<!-- 参考信息 -->