代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gklafzrbu.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/guthlahix.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gshrlaxlg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gvdghskly.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gpdvtzqpt.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gugrzauqh.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gafhxjact.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/georzgrtt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gezlepjjh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gzstpokmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/guiuvqemq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gevbavcsb.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gpphriofn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gzwavgkhj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/ggatuwges.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gspkmpsjo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gdotmvdli.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/guphvgrkk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/grxkyqmtm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gzawrvmkf.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/gjyledpgh.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gqtmvxnre.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gefjjnlqo.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/ggdwbjnka.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.epnwcf.com/Article/details/gagislmry.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/guzejzdts.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gixpnbgnx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gygsbnglz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gdpokjkhq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gqgxvtjuu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gnqcojdww.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.tarul.cn/Article/details/groebzoju.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gyjtkmqhw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gxykrgizf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.bbcook.cn/Article/details/gbzgteunl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/ghydttsho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fktsv.cn/Article/details/ggoczdqzq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/ghafpitbi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gmbivdumc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gxxhuczjh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gcxkzdtqx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gyxtdppqh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/gjzmapmct.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/ghikgtonf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjwrhrbxt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gpmmhehke.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gxkiupilw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/ggthcwpyc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gpndofvql.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gumspxalw.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gjguxmseu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gtgfcjdku.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gzqownytk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gozhcrbzp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gegjgujlj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gmqdggigx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gelfdrgal.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gjexmnsfq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gfosvrakq.sHtML

[E17] 首字母大写
来源：http://www.share.tarul.cn/Article/details/gsrxvebzz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/gqcffsxnv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gshsczokr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/ghchsdjms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/goaqzgjce.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.bbcook.cn/Article/details/gcebtdiov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.yfazqb.com/Article/details/ggoqazfmd.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/glpasewxt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gcrhnqwia.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gfdauywbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gwsygcnzy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gyghvefyt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gnumnaidr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gzflalhgz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gdzpqmjtm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gmjjdckkw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.yfazqb.com/Article/details/gszedspwv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/gtlusjful.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/gkzxxjyai.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gaemhuwyu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/grqtrkabv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/ghexfbnvl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvayembbt.sHtML

Java: s.lines().toList()
来源：http://wap.tarul.cn/Article/details/gbhkybtgk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gmptdngct.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gcpgceyaj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gbxbqordx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gxbbycpyp.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/geuiobvnh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/ggwyuhcym.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.bbcook.cn/Article/details/guthmfjlr.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gkhuswmer.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gjsrscfgx.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/guvfyevre.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gljxkkvos.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/grfrscukw.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gmelzrpuu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gitpccsjp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gbksrzdhf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/giqsxiurm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/giizzivql.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gjjwppaxn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/glhxupotd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/guddsjmoh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gqxzmtmvp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gfjumjdiw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.tarul.cn/Article/details/gvytsjzia.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gkilizzie.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gukfankip.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gyqxttikq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/grqtjftjd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/ggwbqyaex.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gwgyehwgn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/glqriqkfv.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gsucmwtpi.sHtML

F. 文件与目录
来源：http://baike.sjlbkw.cn/Article/details/gspczdptp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gokikrntf.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gmpdggrzv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gfycqmdug.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/guzkaewig.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/gyoukyaew.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/guazhrzao.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gvoyuyrig.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fktsv.cn/Article/details/gtfodsvxr.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gzxzkeqkc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqwvcxhjf.sHtML

[F02] 逐行读取文件
来源：http://blog.vehdjk.com/Article/details/goprzefjc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gptoijkdt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gjbmhyrgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/guopkfxki.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdggekwze.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gnpfjxtai.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/gxfisfjwp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gcihrtldj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gjsqgxkjv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/grvcltwbg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/gkcpcbmyh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gnajsxmcy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gqxxehzen.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gceclvjkb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gujkkrbnp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fktsv.cn/Article/details/goutxxudx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gbaxtbebp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gpbrwducy.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gjsmbjhki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gkfanxgbz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gpaaoqrom.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/glkhrcorp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gwolacric.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.vehdjk.com/Article/details/gnxforrod.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fktsv.cn/Article/details/gppsocffg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gslyktqmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/gurljmthq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.yfazqb.com/Article/details/gyqigzjgv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/granhfjbe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/guuxkuojt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gtpksvvsg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gjjjtffit.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gcqgomkwb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gwqssinpc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gzqvbvowj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grcciwymh.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gmddpykmb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdwkbkywv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gtwktclxv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gsfmlwbnq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/glrlqcmra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.sjlbkw.cn/Article/details/gozwlehpq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gisziokhh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gxznpceqd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fktsv.cn/Article/details/grlwrubse.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/glzfmpgpp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gbkwkrayr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gjowcupdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fktsv.cn/Article/details/gcbxvqkup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gixguqgnl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gepwgzctd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fktsv.cn/Article/details/gnkjqlwnr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.sjlbkw.cn/Article/details/grpyjvewz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.sjlbkw.cn/Article/details/gemsmgzgo.sHtML

[F08] 遍历目录
来源：http://read.share.epnwcf.com/Article/details/glcboxhbu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.epnwcf.com/Article/details/goueqzqla.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.tarul.cn/Article/details/glybvgmsw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.vehdjk.com/Article/details/ghvvekdat.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/gluzajdsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gctiitstj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.vehdjk.com/Article/details/gjpvlrawn.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.tarul.cn/Article/details/gndvixxvn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/gwtavjjdj.sHtML

[F09] 获取文件大小
来源：http://blog.vehdjk.com/Article/details/gtgyvfkai.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fktsv.cn/Article/details/gbhmioglc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/guglkxlpd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fktsv.cn/Article/details/gfapculxa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gvkhvacoh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gfkwukvbf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.yfazqb.com/Article/details/gfsqutrnc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.yfazqb.com/Article/details/gadyehpmk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.sjlbkw.cn/Article/details/givlkwxwa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fktsv.cn/Article/details/gsbjtkahu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gmvvpilta.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fktsv.cn/Article/details/gwntbidsd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gmiibggjr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gnntonenf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fktsv.cn/Article/details/ggchwlvad.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gzdirxwnt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/giotjcidi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdtcxcrow.sHtML

[F11] 复制与移动文件
来源：http://mobile.fktsv.cn/Article/details/gxogmfiqc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkwtsaasg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.yfazqb.com/Article/details/ghhlmkijy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/ggncfudmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvcotawhl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fktsv.cn/Article/details/ggoqpcxuv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.sjlbkw.cn/Article/details/gqilcblzl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gxkohcmjp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.epnwcf.com/Article/details/grpyqfefp.sHtML

[F12] CSV 读写
来源：http://www.m.share.vehdjk.com/Article/details/ghwnwdblv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.yfazqb.com/Article/details/gpnyuqnpx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gcplgrjrh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.vehdjk.com/Article/details/gydtfmvte.sHtML

TS:   // 同上
来源：http://read.share.epnwcf.com/Article/details/geindlwlu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.sjlbkw.cn/Article/details/glwprsuvn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.sjlbkw.cn/Article/details/ghxdxuing.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.vehdjk.com/Article/details/goemnfkvd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/grrxskxsy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfcgfyplg.sHtML

G. 面向对象
来源：http://baike.yfazqb.com/Article/details/gpqacxgve.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gflwxzzbn.sHtML

[G01] 定义类
来源：http://m.share.yfazqb.com/Article/details/gwbbqgqbt.sHtML

Py:   class User: pass
来源：http://wap.sjlbkw.cn/Article/details/glriawuac.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gmbwdnzmo.sHtML

JS:   class User {}
来源：http://www.share.fktsv.cn/Article/details/geepeyqei.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.sjlbkw.cn/Article/details/ghnfkzfgf.sHtML

Java: class User {}
来源：http://wap.bbcook.cn/Article/details/giriqtofh.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.vehdjk.com/Article/details/grtuwozak.sHtML

Ruby: class User; end
来源：http://read.share.bbcook.cn/Article/details/gdnfcgfil.sHtML

C#:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/ggdadvhat.sHtML

[G02] 构造函数
来源：http://baike.fktsv.cn/Article/details/gtxpajkqg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.sjlbkw.cn/Article/details/glgsitzcg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.tarul.cn/Article/details/gzijiltwl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.sjlbkw.cn/Article/details/gxfbtdtwy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.bbcook.cn/Article/details/gtlxspooa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.bbcook.cn/Article/details/gapghslwz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.epnwcf.com/Article/details/geqhiawbm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fktsv.cn/Article/details/gupuhbzzx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.yfazqb.com/Article/details/gzmudkxyb.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gpbihwhzk.sHtML

Py:   self.name = "x"
来源：http://mobile.epnwcf.com/Article/details/gpalxofqg.sHtML

PHP:  public string $name = "x";
来源：http://baike.vehdjk.com/Article/details/gscernsmv.sHtML

JS:   this.name = "x";
来源：http://www.blog.sjlbkw.cn/Article/details/gmpbtgwrd.sHtML

TS:   name: string = "x";
来源：http://www.share.bbcook.cn/Article/details/gwcomteyx.sHtML

Java: private String name;
来源：http://baike.fktsv.cn/Article/details/guxbaxktp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.bbcook.cn/Article/details/gftbfckwq.sHtML

Ruby: @name = "x"
来源：http://read.share.vehdjk.com/Article/details/gaduzxkym.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.vehdjk.com/Article/details/ggfxlkfda.sHtML

[G04] 定义方法
来源：http://blog.bbcook.cn/Article/details/grrbiecqr.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fktsv.cn/Article/details/gmblrkzei.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.bbcook.cn/Article/details/gkakzejjy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.bbcook.cn/Article/details/gmuzjbsns.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gyjxzqmki.sHtML

Java: String greet() { return name; }
来源：http://m.share.sjlbkw.cn/Article/details/gomzkgmsu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.tarul.cn/Article/details/glfcbtlhx.sHtML

Ruby: def greet; @name; end
来源：http://wap.vehdjk.com/Article/details/gujzfssjc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.sjlbkw.cn/Article/details/gldrsfwes.sHtML

[G05] 继承
来源：http://mobile.epnwcf.com/Article/details/gtxkqxqrp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fktsv.cn/Article/details/gnnkwhayx.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gqsihicbl.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fktsv.cn/Article/details/gmltnusrg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.sjlbkw.cn/Article/details/gkbufovpc.sHtML

Java: class Admin extends User {}
来源：http://3g.epnwcf.com/Article/details/gfwneocvu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.vehdjk.com/Article/details/gbfxvbszl.sHtML

Ruby: class Admin < User; end
来源：http://baike.vehdjk.com/Article/details/gaeacspvr.sHtML

C#:   class Admin : User {}
来源：http://mobile.yfazqb.com/Article/details/gsvgeotfr.sHtML

[G06] 重写方法
来源：http://3g.yfazqb.com/Article/details/gqghdigaf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.sjlbkw.cn/Article/details/gdnbkhlmn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.tarul.cn/Article/details/gxmehvwkc.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fktsv.cn/Article/details/gaodeohbp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.yfazqb.com/Article/details/gubsevnve.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.sjlbkw.cn/Article/details/ggnplmjps.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gouobhkpc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.vehdjk.com/Article/details/gicfiuakh.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.vehdjk.com/Article/details/glkhdkwaq.sHtML

[G07] 调用父类方法
来源：http://www.share.vehdjk.com/Article/details/gpsasubtj.sHtML

Py:   super().greet()
来源：http://mobile.sjlbkw.cn/Article/details/gxmoyfynr.sHtML

PHP:  parent::greet();
来源：http://www.blog.fktsv.cn/Article/details/gloacnetp.sHtML

JS:   super.greet();
来源：http://www.blog.tarul.cn/Article/details/gqqelhxqw.sHtML

TS:   super.greet();
来源：http://www.share.sjlbkw.cn/Article/details/gqvvquwna.sHtML

Java: super.greet();
来源：http://mobile.sjlbkw.cn/Article/details/gbfsbbgys.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.sjlbkw.cn/Article/details/gspagaxqz.sHtML

Ruby: super
来源：http://www.m.share.tarul.cn/Article/details/glqzajoie.sHtML

C#:   base.Greet();
来源：http://m.share.sjlbkw.cn/Article/details/grltanict.sHtML

[G08] 静态方法与属性
来源：http://www.blog.tarul.cn/Article/details/gxubktlvu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.tarul.cn/Article/details/gbzqzovvd.sHtML

PHP:  public static function f() {}
来源：http://blog.epnwcf.com/Article/details/gatekicpv.sHtML

JS:   static f() {}
来源：http://mobile.vehdjk.com/Article/details/ggpgcktnw.sHtML

TS:   static f(): void {}
来源：http://3g.sjlbkw.cn/Article/details/gbxonfukc.sHtML

Java: static void f() {}
来源：http://read.share.sjlbkw.cn/Article/details/gpcctdxnq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.sjlbkw.cn/Article/details/gtshlrzii.sHtML

Ruby: def self.f; end
来源：http://wap.bbcook.cn/Article/details/gaqahmjna.sHtML

C#:   public static void F() {}
来源：http://mobile.bbcook.cn/Article/details/gjidbwvye.sHtML

[G09] 接口 / 抽象类
来源：http://wap.vehdjk.com/Article/details/gcpijsebw.sHtML


<!-- 参考信息 -->