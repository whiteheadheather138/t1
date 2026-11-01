代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gygehspwl.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/guwpgilcf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gqwtxoakc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gaysgssnt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/giovzddtj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gsjsesmcz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gabmqisbj.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/gonjfzfnq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gwatqyeog.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gonkitztc.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/ghseozotv.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gtfdhswfn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/gxzxaoykp.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gzdwtzbaw.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/garhkoykc.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gfxpqbcsg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fktsv.cn/Article/details/gfsdeerxj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/gytrnvsbg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gyykwdnts.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/ggckhteas.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/giphbsxer.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gmfsbtrtg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gpcaipkbt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/ghzullzeh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/grtpqezlc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gzvgzzoyg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gbajmhebz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhtjlyf.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gwqtepsry.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/ghelkcfyr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/ghqguineq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/galjavxem.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gkygjsyyu.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gkwhhvksl.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gmpzpyauj.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gdlvnghis.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/grrmkqtoj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gylgtbyab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gsmbudlcx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gjofzgrsy.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gouerkfse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gnmzdlcwl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.bbcook.cn/Article/details/gltpmsxvf.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gtrcowaii.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gjhbqncie.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gcmggvsdw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gyznvdegl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gixmoerpu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gsfbdfhsx.sHtML

Ruby: s.count("a")
来源：http://wap.bbcook.cn/Article/details/gsifmatci.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gfvmbwtfs.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/gamgpxkcl.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gmpughfgz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gvylwjeue.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gngydlogs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gykrbxzyq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fktsv.cn/Article/details/gfwkrcfxl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fktsv.cn/Article/details/gqwbilbrr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gprmpskdt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/guhaosgdb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gcvqkusrs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gtatwafzi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gppxqpwky.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gdbrnolyp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gmzhssixh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.tarul.cn/Article/details/gazktfvow.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gzfbuuodp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/ggsonmdal.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/glwbyafdn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gaszeplvw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gneupeiun.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gokvnhldk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/gwfqjbqcl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gqtcpqbrr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gsjrkhzwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gzqhfsutw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gcmkptwop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/gxcoowkox.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/glzoodkcy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/glwojgeqz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.yfazqb.com/Article/details/grgeynabk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/giyiroeyu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gbqdupxdb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gafsazfao.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.bbcook.cn/Article/details/gbsmptheq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gbneunzpc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gxonlkbcs.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gimbkvfex.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gotgvcnlm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/guwpcrmwa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/ghpbjrhra.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/ghrclfons.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbleeicrj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/ghpjdhjuk.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/gswqsnvxp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gtmvzynwi.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/ghdhasjnq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gilyirgdq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gxioszuai.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gglqqdecd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gavfbsdak.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gywmelcom.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/grthyvohz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gcemgprpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gnkcnvffv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gphtsziyt.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gugatekxq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/gmykdvtcn.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gvxzensdf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/ggmxkjvcc.sHtML

Java: s.lines().toList()
来源：http://read.share.tarul.cn/Article/details/gaanpkspf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gwnveywbs.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gfsdvvgea.sHtML

C#:   s.Split('\n')
来源：http://m.share.fktsv.cn/Article/details/gyxulmunp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gaadnbrlk.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/goiyhhnai.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/gfkaeekbq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/ggnjwxswi.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gbkhitvqx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gtgggunsn.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxamjyqx.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/grykiqmta.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gofppbjxt.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/gyahwsnhu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/galzstjua.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gslfruueb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gjewhipbp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gcqaxvyvt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gczxgotja.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gequxkfyd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gqrufvsdv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gamfyqazk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gjskxktyw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjxeqrofn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/ghuwjbczg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.yfazqb.com/Article/details/gglnngpqw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gdvprrfap.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gxpkgejnn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gdxwdcktb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gaukmkufa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gccdnymhr.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ghtlwexga.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gpipnyjjt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gkfpmtgle.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gpkbjkmex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.epnwcf.com/Article/details/gdsvfsits.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/geybnidkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gikacqapy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gxrzujmau.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gkzxscbmy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.tarul.cn/Article/details/gvdjdmjmf.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gaazrxqob.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gaknkhwhr.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gdjjjjadh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gtdwgfcdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.tarul.cn/Article/details/gnasdjkeg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/gnmuezozi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gwxvkuahi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gmpyndrcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/grtczaeep.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gnpbmfdhr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gumuetmip.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gmlneqvzs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gzyynaqjz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/giifqhdpq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gvbfhzrkp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gjdbqdxdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gphxdhfgp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gdnzvhpdd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fktsv.cn/Article/details/gvzgmmfba.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/grgelavvu.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gzjapmltt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gdevqawlp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.yfazqb.com/Article/details/gygaecxmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gitxdylnq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gsvvkqsht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gfjervcrj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fktsv.cn/Article/details/glhphwznh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/gypxmlyos.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.vehdjk.com/Article/details/gxxmxknqn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gtevefhhc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gnnlglwvw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gnnzklxzy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmljlxqnb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fktsv.cn/Article/details/gufdmmthe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/ggoaxautb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.bbcook.cn/Article/details/gjhipgsii.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gdvrfchak.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gybgzbqip.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gfkvaksri.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gzhtpuxmx.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gjxsgqkza.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/grgwlqtpy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gzuulrhlt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/glugzhllw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gffjvjvao.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gaaohqjiy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gkvgwamxm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fktsv.cn/Article/details/gcubimhlc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/ghvfppcri.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gzonyiqtb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gxzfkmkgj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.yfazqb.com/Article/details/gllnmyfsx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.epnwcf.com/Article/details/ggoncqckf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.tarul.cn/Article/details/gwkhvkpht.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.tarul.cn/Article/details/gkrotbmmx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/gvwruaass.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gprgryqin.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.vehdjk.com/Article/details/gfwmeaqmg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fktsv.cn/Article/details/gcenapnoj.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.vehdjk.com/Article/details/gjlobvxjh.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/grvogahjl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gjhauwbzl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gsnzskzkm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gfytrlmry.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.tarul.cn/Article/details/gfzupiydj.sHtML

[F09] 获取文件大小
来源：http://wap.vehdjk.com/Article/details/gbkkyqhev.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.yfazqb.com/Article/details/gvkvbzypm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.epnwcf.com/Article/details/gfchnfihc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gufrrosgo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gjlrafedg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gifbazedm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gyjdkqvlx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwuehyxot.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.epnwcf.com/Article/details/gfntjmvcu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gslqbrmbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gjoyofuma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fktsv.cn/Article/details/gqwrhlteh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.bbcook.cn/Article/details/gafajtxys.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.epnwcf.com/Article/details/guvaivvpf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.vehdjk.com/Article/details/gaoefyvwv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gamxwkodk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gakbgunsp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.vehdjk.com/Article/details/grscmiodt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.bbcook.cn/Article/details/gtyryclrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/ggakwudty.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.tarul.cn/Article/details/glfduebxc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/givjtiycj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.sjlbkw.cn/Article/details/gmmgblvaf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.bbcook.cn/Article/details/grmycrtym.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/ggugpuawk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvrduqruv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fktsv.cn/Article/details/gyzgwchoj.sHtML

[F12] CSV 读写
来源：http://read.share.yfazqb.com/Article/details/gjzilglyu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.vehdjk.com/Article/details/gtwufrloz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.vehdjk.com/Article/details/gigdqwbcw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.tarul.cn/Article/details/gymuyswxo.sHtML

TS:   // 同上
来源：http://wap.yfazqb.com/Article/details/gylvkwxdn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.epnwcf.com/Article/details/gatafthma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.yfazqb.com/Article/details/gkbpklpjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.yfazqb.com/Article/details/gyctrvjdd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.tarul.cn/Article/details/gmvqpnlzw.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ghvdqxgcg.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gyeyshpzh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvmadzxbg.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/gimmyukzu.sHtML

Py:   class User: pass
来源：http://www.m.share.tarul.cn/Article/details/gxxxmpziy.sHtML

PHP:  class User {}
来源：http://www.blog.epnwcf.com/Article/details/gcmhvaloi.sHtML

JS:   class User {}
来源：http://baike.tarul.cn/Article/details/gdxelogid.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.yfazqb.com/Article/details/gtuefktii.sHtML

Java: class User {}
来源：http://blog.vehdjk.com/Article/details/gsjshtxzv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fktsv.cn/Article/details/gcuqmyalm.sHtML

Ruby: class User; end
来源：http://www.share.tarul.cn/Article/details/gzalvmnvi.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gdsvwcidl.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gzpcjtqpq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.bbcook.cn/Article/details/grpmxdlab.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.yfazqb.com/Article/details/gxjylkexk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/gtwghfxxa.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.epnwcf.com/Article/details/grsjxnrfu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.tarul.cn/Article/details/gfmtjxdtd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gqgkpxlnm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.sjlbkw.cn/Article/details/gciyfzsws.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fktsv.cn/Article/details/gscuoefgo.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/gblvdixri.sHtML

Py:   self.name = "x"
来源：http://m.share.bbcook.cn/Article/details/gaxpmvzvi.sHtML

PHP:  public string $name = "x";
来源：http://3g.fktsv.cn/Article/details/gthygzejw.sHtML

JS:   this.name = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gvmcrtipp.sHtML

TS:   name: string = "x";
来源：http://blog.yfazqb.com/Article/details/gctcmjkki.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/gclodahyq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.yfazqb.com/Article/details/gjbhrppzp.sHtML

Ruby: @name = "x"
来源：http://blog.epnwcf.com/Article/details/gdhwfbwde.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.sjlbkw.cn/Article/details/gkmqgfbfm.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/grrplncom.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gkfjrfdwa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.yfazqb.com/Article/details/gccljthpc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.bbcook.cn/Article/details/gzuciccrh.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.vehdjk.com/Article/details/ghlbvirin.sHtML

Java: String greet() { return name; }
来源：http://www.blog.sjlbkw.cn/Article/details/grfhbirny.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.tarul.cn/Article/details/gzhnxxatc.sHtML

Ruby: def greet; @name; end
来源：http://mobile.epnwcf.com/Article/details/gnfyuhvyg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.yfazqb.com/Article/details/ghipgafpn.sHtML

[G05] 继承
来源：http://mobile.sjlbkw.cn/Article/details/gdxqnicuh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.vehdjk.com/Article/details/gcswebixv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.yfazqb.com/Article/details/gddssvkgi.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gdjpwbmah.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gcdhdohey.sHtML

Java: class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gqycjqvni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.bbcook.cn/Article/details/gzpkjrnph.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.epnwcf.com/Article/details/gaqfdbybk.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/guxjjixmz.sHtML


<!-- 参考信息 -->