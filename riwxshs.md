代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gvocypqkn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gfawdyttd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gzgdzfkrc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gdahjuboz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fktsv.cn/Article/details/goepsnkha.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gypkwzkve.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gwlgbrwkw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gshnxkkqj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gfngndriu.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gotswskuw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gdwhktolg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gomvtlqhd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gcxwyiogn.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/ghuyerxix.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/geofvxgor.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gfizrqyrh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/geikonzzl.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gjugcxawe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gcmihrgnz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gvgxngqui.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/gsggyfmym.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gintcqqoc.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gnlrlxxim.sHtML

Py:   s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdtgvfkm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/gdiwmzqsv.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvgsgqdnn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gsthanqim.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/ghemwsxbj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gvcbrkiye.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gliaaiiav.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gqvjkinwq.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/godwbfvta.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/grwugeqyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gsytaahzz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gndgyrmcq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gsjcuvuhl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/grkowrekt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gqwirsawe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/gqknfgera.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/guytxmicc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gorkfjpcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gpduakqzu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gglonjyea.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gbpienvfa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/gtiosabnj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gdipekqok.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.sjlbkw.cn/Article/details/gtwasekbq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gvtjkovqa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gijkbqpoa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gzklxqlwe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/gwdtioojx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/ghczfyoek.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/gdyfmizqs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gkrtlcuqh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.sjlbkw.cn/Article/details/grnmcwtag.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/ghmttcbqm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fktsv.cn/Article/details/gtzyqfmgv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gnfqgxdhq.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gsmsczlia.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/ghdimtzet.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/guosgbqgu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gjluhalki.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gtnazioes.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gvbezqlim.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/ggidscwkn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gqcczfxpu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gnlndbqvj.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gvbndwgfu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/geoedevyc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gdlwnaptf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gjzmpfbyf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/gyfystyfv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gryhwvxrl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gsjydngwu.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/gbeabdzxf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/ggfrprnsc.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gtwneewzy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gclyujbym.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gmztfyvdj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gbtenyblj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gboxnsqbl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gjmzepswq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gaagwcqgh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/girhnusjd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gvxzriokw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gobiynwsm.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/gvljqfklg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fktsv.cn/Article/details/gypmymukt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/ggikzxdik.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/ggfmgnpxh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.vehdjk.com/Article/details/gwtflrzdm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/gmopvkauz.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gbdamecmh.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gkxrrulho.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/geqpeeenb.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gjzabsvol.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.vehdjk.com/Article/details/gorhzzhvl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gnshqlqaz.sHtML

TS:   if (s === "") {}
来源：http://m.share.vehdjk.com/Article/details/gfcrztwvw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gniiaryal.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gmpbtmexa.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gynsoyjby.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gepnpwpko.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gvgxpvlsd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gepkmmltf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gvhnwqrap.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gzssehxzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gdigvrgti.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gsuospxds.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gffkcqprv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/ghsarwkgq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gjgfrkhts.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/ggzvimhte.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.tarul.cn/Article/details/giufijclh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gezkqodct.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gpxuqcywk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gcwnlnhrr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.tarul.cn/Article/details/grnfiewkt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.tarul.cn/Article/details/gueenyijz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/gcffzhrgn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gryewnwwp.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gryhzhfsc.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gjfsufwdc.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmywbicob.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gwekyvkgv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gncmokbbu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdjzltlxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gtdjjpwzy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gkmkfdhwn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gadfigvxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gbfmlyoww.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gxmhalfjd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gfrsadjog.sHtML

[F02] 逐行读取文件
来源：http://mobile.sjlbkw.cn/Article/details/gsfepritk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/ggekgxgdl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gieazxmku.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/ghnwnpjav.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gktegissl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gsnrxwxgl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/gowghmxuk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gtuykgqte.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gibcwnwax.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/gxhioulfd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/gsrwzkpfx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gdopbtfsg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/grtsklphl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gwblgpmdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/gpgyhodzz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gskmqjhkz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gogdjvjqm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gvgekxqfb.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/gqvfxrpty.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/gfwzvgkbb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/griskbrrz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gierjvmeq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gprivuyxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/grfkxzkjl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/gqihqqezh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gseueculb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.bbcook.cn/Article/details/gluqwdrvw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.bbcook.cn/Article/details/gzqovddrh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.yfazqb.com/Article/details/glpqbelxk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gvyovcuak.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gepkrfksh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvpkogzdg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gucewfqjm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.bbcook.cn/Article/details/guhdgbdvx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gzyauzwoy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gcxnwiqzg.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/guqujoaxx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gswwlarbr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.bbcook.cn/Article/details/gtlkadaer.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gcnoffkyg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gcdcpisus.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gjbbjfcci.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.tarul.cn/Article/details/gmhghqywv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gkflvnqkb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.yfazqb.com/Article/details/gwoptpkvj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gzrjuzwkc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/glsgbfwsp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gosdjagdd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gkrqiypms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/gofojidkx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fktsv.cn/Article/details/gadkapgim.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.tarul.cn/Article/details/gpqxvgstd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fktsv.cn/Article/details/ggwdtvbtb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gyrsgrugy.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/gqwtvimob.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fktsv.cn/Article/details/gsyvmlaiv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.yfazqb.com/Article/details/gkjmnncts.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.vehdjk.com/Article/details/ghitqzqdu.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.epnwcf.com/Article/details/ggjlsmyru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gvixyvplu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.sjlbkw.cn/Article/details/gfebmxwvq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.yfazqb.com/Article/details/gsrgduowu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.tarul.cn/Article/details/guzrmvctp.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/gsitvjfhy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gpkmsdtpg.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gldzrywuh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.vehdjk.com/Article/details/gakelbbik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.sjlbkw.cn/Article/details/gjfnnvqsl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gpiatislx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.tarul.cn/Article/details/gyrxxozxv.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gdugjmrmo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.epnwcf.com/Article/details/gehaowuti.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.epnwcf.com/Article/details/godwuhbca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxthztlur.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gmpievjff.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggthcbntv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fktsv.cn/Article/details/gggjdsroi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/ggyvhxvra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlhcofia.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gabkcgaaj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/grbgtlwaf.sHtML

[F11] 复制与移动文件
来源：http://blog.yfazqb.com/Article/details/ghdbyoujj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gdkcsiacm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.vehdjk.com/Article/details/gklzysunx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.yfazqb.com/Article/details/gujtqfvfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.epnwcf.com/Article/details/gzhfobtyo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.vehdjk.com/Article/details/gwwejjfet.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.tarul.cn/Article/details/grbluxscd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/geoptuqeq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gcgkdlngx.sHtML

[F12] CSV 读写
来源：http://blog.fktsv.cn/Article/details/gxwyvvzxc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.sjlbkw.cn/Article/details/grsvbhwml.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.tarul.cn/Article/details/gycibmzac.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fktsv.cn/Article/details/gplaljdwm.sHtML

TS:   // 同上
来源：http://3g.vehdjk.com/Article/details/grkyhsady.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gseksmnmm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.tarul.cn/Article/details/gvplfcfpz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/ggrifvxlb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.bbcook.cn/Article/details/gohpmhtzo.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gfgcfddyt.sHtML

G. 面向对象
来源：http://read.share.vehdjk.com/Article/details/gpnzjumjv.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmpxolevh.sHtML

[G01] 定义类
来源：http://m.share.bbcook.cn/Article/details/ghyuytzdq.sHtML

Py:   class User: pass
来源：http://3g.tarul.cn/Article/details/glzfxqslh.sHtML

PHP:  class User {}
来源：http://www.m.share.bbcook.cn/Article/details/gwpdongww.sHtML

JS:   class User {}
来源：http://www.m.share.fktsv.cn/Article/details/gtokufiev.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.tarul.cn/Article/details/gmlavsdoy.sHtML

Java: class User {}
来源：http://mobile.bbcook.cn/Article/details/gtxpajgob.sHtML

Go:   type User struct { Name string }
来源：http://mobile.vehdjk.com/Article/details/gozjdrbou.sHtML

Ruby: class User; end
来源：http://read.share.vehdjk.com/Article/details/gpszmapxf.sHtML

C#:   class User {}
来源：http://read.share.bbcook.cn/Article/details/gnjelojui.sHtML

[G02] 构造函数
来源：http://m.share.vehdjk.com/Article/details/glacgitef.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.vehdjk.com/Article/details/gevsrcvnz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.bbcook.cn/Article/details/grtvrxiji.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.epnwcf.com/Article/details/glygxkomd.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.bbcook.cn/Article/details/gakbetoik.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.vehdjk.com/Article/details/gzlgzdvdm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.bbcook.cn/Article/details/ggjksheks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.epnwcf.com/Article/details/gjueflzju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.epnwcf.com/Article/details/gtalsuquh.sHtML

[G03] 实例属性
来源：http://wap.epnwcf.com/Article/details/gxqnowyle.sHtML

Py:   self.name = "x"
来源：http://3g.yfazqb.com/Article/details/grabxrzyl.sHtML

PHP:  public string $name = "x";
来源：http://blog.bbcook.cn/Article/details/gyuyyjhku.sHtML

JS:   this.name = "x";
来源：http://read.share.vehdjk.com/Article/details/gypnywhut.sHtML

TS:   name: string = "x";
来源：http://read.share.epnwcf.com/Article/details/glgrlhlea.sHtML

Java: private String name;
来源：http://wap.tarul.cn/Article/details/gwcokdsxw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/giqevaovi.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gubqmgjkp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.epnwcf.com/Article/details/gnygonkvt.sHtML

[G04] 定义方法
来源：http://www.blog.fktsv.cn/Article/details/gghpcbcmy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.vehdjk.com/Article/details/gdkezxvwz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.bbcook.cn/Article/details/ggqoaijjx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fktsv.cn/Article/details/gwraifdvm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.tarul.cn/Article/details/guaesbtga.sHtML

Java: String greet() { return name; }
来源：http://wap.sjlbkw.cn/Article/details/gnkduszdt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.vehdjk.com/Article/details/gvjwyzxyz.sHtML

Ruby: def greet; @name; end
来源：http://3g.tarul.cn/Article/details/gryqctump.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.tarul.cn/Article/details/gluzivehk.sHtML

[G05] 继承
来源：http://3g.bbcook.cn/Article/details/gbcgvlpsb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.tarul.cn/Article/details/gshsxdxcx.sHtML

PHP:  class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gisdkjbfm.sHtML

JS:   class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gdinhdqos.sHtML

TS:   class Admin extends User {}
来源：http://www.share.epnwcf.com/Article/details/gxvfoxlst.sHtML

Java: class Admin extends User {}
来源：http://wap.bbcook.cn/Article/details/gcjvtfvfw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.yfazqb.com/Article/details/gpwtaabzw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.sjlbkw.cn/Article/details/goplzpksg.sHtML

C#:   class Admin : User {}
来源：http://read.share.fktsv.cn/Article/details/gvlnyfybg.sHtML

[G06] 重写方法
来源：http://baike.fktsv.cn/Article/details/grhaivcvq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.epnwcf.com/Article/details/gxfqivfev.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gysbthcog.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.yfazqb.com/Article/details/gwfbtbiwi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.vehdjk.com/Article/details/gjmadxrif.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fktsv.cn/Article/details/gnrhdoanr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.vehdjk.com/Article/details/giskjtpud.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fktsv.cn/Article/details/gwytddfrd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.sjlbkw.cn/Article/details/gmaiuddnl.sHtML

[G07] 调用父类方法
来源：http://baike.epnwcf.com/Article/details/gtavhvhmu.sHtML

Py:   super().greet()
来源：http://www.m.share.fktsv.cn/Article/details/gwocfbyam.sHtML

PHP:  parent::greet();
来源：http://www.m.share.epnwcf.com/Article/details/gbfibsimh.sHtML

JS:   super.greet();
来源：http://3g.epnwcf.com/Article/details/gbimesiad.sHtML

TS:   super.greet();
来源：http://m.share.fktsv.cn/Article/details/gvwhjpkft.sHtML

Java: super.greet();
来源：http://www.share.epnwcf.com/Article/details/gwkccagkb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.bbcook.cn/Article/details/gmmaxpquf.sHtML

Ruby: super
来源：http://m.share.bbcook.cn/Article/details/gpdysuzka.sHtML

C#:   base.Greet();
来源：http://www.blog.epnwcf.com/Article/details/gwjyhxvka.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.epnwcf.com/Article/details/gllkwlnau.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.bbcook.cn/Article/details/gknrvvfoz.sHtML


<!-- 参考信息 -->