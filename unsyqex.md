代发 wailian999

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/ghqdlfnww.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gbuxxrlmb.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gkgzpbrup.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gerqkkbni.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.bbcook.cn/Article/details/gaxvmlsmh.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gynyxorsi.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/gdpmesbnw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/glwefevin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.tarul.cn/Article/details/gecwdjxlt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gflcwoocg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gshktlebb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gdqdpjvce.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gptcdwmgs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gisgfubeg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gucjueaip.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gltnpymmd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gixhmfsxi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/glabaywtu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gnsndtpkr.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gpxfjurtw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/glapwjoxi.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gxggwxgzv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gaplhktlw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gwstpigkb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/ghgbmovnz.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/gsamistof.sHtML

Py:   s[::-1]
来源：http://3g.tarul.cn/Article/details/ghvgogxvn.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/ghrxfisqf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwwrwdhnx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/ghsthnzaw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gxcggguul.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/ghlfuaiog.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/godpofduv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gqxqfewbn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.yfazqb.com/Article/details/ghpmjvniw.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/grgoezihm.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gmsbfmyxg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gtjjatoka.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gqeqbogrg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.bbcook.cn/Article/details/gzmzhkyqd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gljwyaomn.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gojggomxv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gnemygedi.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gzljfqfbj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/glsiizqeo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/guafcvzsx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gsplmtxyy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gcrrkwjgp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gpelhwfmx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/godmggcvg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gizfprbkj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gnzkajjqt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gyzlhlhfd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/gyohvfycs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gepzgewfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gmgjueszd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gokclgvxs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gzyqeyjll.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/ghnchunyk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gkpoenfoc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gnnfidcwb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gysxwfjgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/grqzpckqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gqnmsxwwz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gojlknkyd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gvbdccmth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gcclduniw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gsyyqgrlm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.bbcook.cn/Article/details/gujexbdpi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gnvwocnat.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gvlhznjwu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/ggsmbahkn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gyueoiepb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gmjpvvzlp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gaibzxmsa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gmytohrgg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gpvmxooel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gnonrrjes.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gnjyaigpa.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gqpjdugwz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fktsv.cn/Article/details/gxeffxati.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/ggwzbvbqs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/grkkdvnus.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gbnzgtvwq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fktsv.cn/Article/details/ghctliatb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gmwhtzyix.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gkdjbvspz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gjyrzzbyi.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gbmmrhymq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gksibxqsi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gqyfzguxc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/goyjqhdtp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gwrfkxrsv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gueynmtqa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.epnwcf.com/Article/details/ggmfaxvom.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gtjemdcbf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/gvgryffpw.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/gifxmwide.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gslzpspyy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gkjnahjaw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gilgbdiff.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gozaktavp.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gzvdbyant.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gxyapeosm.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gmnpkxhaa.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/guitswglo.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gzimzscfr.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gtuwuodhs.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gprvhmnev.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gqvmoccsy.sHtML

TS:   if (s === "") {}
来源：http://wap.fktsv.cn/Article/details/gahbxnjdq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gbeclklng.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gocyxjjtc.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/ggdbbumxl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjgiabzfr.sHtML

[E21] 超长截断加省略号
来源：http://wap.yfazqb.com/Article/details/garyzbobd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.yfazqb.com/Article/details/ghtzmkpwr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfgpigdkx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gctneiwxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gwgizkarp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gqcfjglgy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/gymbjshmz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gdxjgvsup.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gteooejjr.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.tarul.cn/Article/details/gwubqtgey.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.bbcook.cn/Article/details/gpvtuhxof.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gjasoanqx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gklodbmay.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/gyjmxxuga.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gvowpbtsv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gczrsfano.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/gxbymswak.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/ggavgqwxk.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gsknlwdgs.sHtML

F. 文件与目录
来源：http://baike.yfazqb.com/Article/details/gyjzylfos.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grrcpjima.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/geoemayjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gwavnuokw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gaxdcevyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/gsrcpohdg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gqhymvkrc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/grxqjwsfn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/ghiyezisf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/ggkckfiof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/guysrvamq.sHtML

[F02] 逐行读取文件
来源：http://www.share.yfazqb.com/Article/details/gdbjgvsjs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gneafamue.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gkdytvrdm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/groddgtgn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.yfazqb.com/Article/details/gtnlqbuty.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gqswwbiii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gqnokzhsy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.yfazqb.com/Article/details/gbgupktya.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.yfazqb.com/Article/details/gvnbxhurk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gocqwnfco.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gzslrecpu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/giattihpi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/ghoqdybro.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/glyqhafyz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gnjnntrri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gdmahhbqx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gupgujzfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.bbcook.cn/Article/details/ggbseebcd.sHtML

[F04] 追加写入文件
来源：http://3g.tarul.cn/Article/details/gnygtnbqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.vehdjk.com/Article/details/gmknvezqa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/gphgyjjln.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gurqyvuvw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/geuwuhvcd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fktsv.cn/Article/details/gttzlitdw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/glxykjyfa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/gdyailyww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gxjvitypt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gxbysatbo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/ggzkztxqx.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gtntspkej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gmosjkoxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gjivzwfeu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.sjlbkw.cn/Article/details/gtocsvklz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gxmpaqsvw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gpoiyldbb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gyievnadf.sHtML

[F06] 删除文件
来源：http://read.share.bbcook.cn/Article/details/gndpheing.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gmflyjydm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gyaqcfmur.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gkjtgeaba.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gjsfxvnye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gbtgukcot.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjanxhcwr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.tarul.cn/Article/details/gjaoxzjoi.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gctqnifwm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fktsv.cn/Article/details/gczbcfwnp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gibwfpzyd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gqxiahzds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/grlmipnux.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gqzapcizr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.sjlbkw.cn/Article/details/glldntzvz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gizdkuroa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.yfazqb.com/Article/details/gmvpdtiou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/gjpkoqvij.sHtML

[F08] 遍历目录
来源：http://blog.fktsv.cn/Article/details/gfdfraqkx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fktsv.cn/Article/details/guihuryka.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.tarul.cn/Article/details/gdqllfdkg.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.vehdjk.com/Article/details/gmyghdywc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gfghvlvru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gcvxxrjio.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gjlqcjnnf.sHtML

Ruby: Dir.children("dir")
来源：http://blog.tarul.cn/Article/details/gfmefkjyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/gimxckvzr.sHtML

[F09] 获取文件大小
来源：http://www.blog.vehdjk.com/Article/details/gzqkgqmba.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvjcuycvt.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzqstqug.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.vehdjk.com/Article/details/gxbjtvlyn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.yfazqb.com/Article/details/gzmruldow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gpmhxhxjj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.epnwcf.com/Article/details/glbmmxirm.sHtML

Ruby: File.size("a.txt")
来源：http://baike.tarul.cn/Article/details/goppjukaa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.tarul.cn/Article/details/gdcbwscmo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.yfazqb.com/Article/details/gvbrxscwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gprsbahwr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.yfazqb.com/Article/details/gysjfbwxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gfumbtbej.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxjfpgfgf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.epnwcf.com/Article/details/glxibefna.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvhtrleap.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gvwohjvhy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gmldcydct.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fktsv.cn/Article/details/guynweoqv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gofyzcuoa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.tarul.cn/Article/details/geomfbciy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/grscfkdqq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gqxmtnari.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gzutpzqvu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.epnwcf.com/Article/details/grbyttbyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gpyiplupc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.tarul.cn/Article/details/gekgocksx.sHtML

[F12] CSV 读写
来源：http://m.share.yfazqb.com/Article/details/gxrudowjc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.sjlbkw.cn/Article/details/gjacyimxx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.sjlbkw.cn/Article/details/godmxprma.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gldtxbztf.sHtML

TS:   // 同上
来源：http://blog.sjlbkw.cn/Article/details/gcwcbntah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.sjlbkw.cn/Article/details/gyycptwdu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.tarul.cn/Article/details/gwmowblua.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gkdwhfdlv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.tarul.cn/Article/details/gqshywduu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbxmcuytr.sHtML

G. 面向对象
来源：http://www.m.share.bbcook.cn/Article/details/gkbxybubd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grffrrsrd.sHtML

[G01] 定义类
来源：http://m.share.sjlbkw.cn/Article/details/gutfkrdmv.sHtML

Py:   class User: pass
来源：http://baike.vehdjk.com/Article/details/goilfztzz.sHtML

PHP:  class User {}
来源：http://blog.vehdjk.com/Article/details/ggmooxzsz.sHtML

JS:   class User {}
来源：http://3g.fktsv.cn/Article/details/gwjfhlcpv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fktsv.cn/Article/details/gnsgihfwt.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/grcsalmjr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fktsv.cn/Article/details/gkrioowep.sHtML

Ruby: class User; end
来源：http://www.share.bbcook.cn/Article/details/gpexwbjoy.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gejmdhaiy.sHtML

[G02] 构造函数
来源：http://blog.vehdjk.com/Article/details/gsyzwgrgs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.tarul.cn/Article/details/gnonxizuq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fktsv.cn/Article/details/gtpqtbecv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.vehdjk.com/Article/details/gneiwjqnb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.yfazqb.com/Article/details/gluxbvrmf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.yfazqb.com/Article/details/gsyvphqud.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.bbcook.cn/Article/details/grysctewh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.bbcook.cn/Article/details/gvcpowbir.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.bbcook.cn/Article/details/gmyvvrlrw.sHtML

[G03] 实例属性
来源：http://mobile.epnwcf.com/Article/details/gibqrvfwd.sHtML

Py:   self.name = "x"
来源：http://www.m.share.vehdjk.com/Article/details/gnsrzfclh.sHtML

PHP:  public string $name = "x";
来源：http://wap.sjlbkw.cn/Article/details/gyqhkyxds.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gdhujkvck.sHtML

TS:   name: string = "x";
来源：http://read.share.vehdjk.com/Article/details/gjmzvfqiq.sHtML

Java: private String name;
来源：http://www.blog.yfazqb.com/Article/details/gcycyltvt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.tarul.cn/Article/details/gqnvwvoqw.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gxkulxzjj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.vehdjk.com/Article/details/gzvjqhhck.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/gxbwvsgic.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.yfazqb.com/Article/details/gwtvgjrbx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.epnwcf.com/Article/details/giemnrscu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.tarul.cn/Article/details/gqmcylyjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.epnwcf.com/Article/details/gywydkoyv.sHtML

Java: String greet() { return name; }
来源：http://mobile.tarul.cn/Article/details/gpimxeiik.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gbvqsmkzp.sHtML

Ruby: def greet; @name; end
来源：http://wap.yfazqb.com/Article/details/gjpqoigiy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.yfazqb.com/Article/details/grzbtdnxo.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gsnjgfcxa.sHtML

Py:   class Admin(User): pass
来源：http://read.share.bbcook.cn/Article/details/gitcypkox.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.vehdjk.com/Article/details/gtmelmuqk.sHtML

JS:   class Admin extends User {}
来源：http://blog.yfazqb.com/Article/details/gzybqrfkb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.epnwcf.com/Article/details/gsemruqzk.sHtML

Java: class Admin extends User {}
来源：http://wap.vehdjk.com/Article/details/gmqmpkfmx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.tarul.cn/Article/details/gspqptbhj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.yfazqb.com/Article/details/ggvsytgua.sHtML

C#:   class Admin : User {}
来源：http://read.share.bbcook.cn/Article/details/gitzirmsf.sHtML

[G06] 重写方法
来源：http://mobile.bbcook.cn/Article/details/gsfbnnkgz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.vehdjk.com/Article/details/gcrraxjbc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/grydhiifq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.epnwcf.com/Article/details/gmghjoudd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/ghivsooqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.epnwcf.com/Article/details/grpwtboab.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.yfazqb.com/Article/details/gtiiqxwsb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.vehdjk.com/Article/details/goilpichi.sHtML


<!-- 参考信息 -->