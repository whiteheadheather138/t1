代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/ghpkdtihb.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gwoqgwoji.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/geozwakna.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gvhhsgtqg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gizrdgxmf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/ginpwngbt.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gtdabvtbs.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gxcbyxnmd.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gcvylkfav.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/guxbmwntk.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gnegdyjuy.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gteoyxzyn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/gmsgrmnwi.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/gynvpkljl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gmyngiucz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.yfazqb.com/Article/details/gojzbdgjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.tarul.cn/Article/details/gfatqpyfu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.vehdjk.com/Article/details/gbnktekmv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gqshqlhcr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gglgytena.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gixvoammu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gkfzxjwaj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/giovxcdhv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gzmqzfbil.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gakjturtb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gtukksdpv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/ghpdcevsw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/graczrqiw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gvsunqham.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/guyezzrpu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gbypzmpfk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gmdtzdwmc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gefdcoijr.sHtML

[E11] 反转字符串
来源：http://blog.epnwcf.com/Article/details/gyanmdcdk.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gywtmqypg.sHtML

PHP:  strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gcjpswvyf.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gicrskhhb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/goeciavws.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/gyueiutqh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gxtyznflu.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gktlmmcyn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gzsdjdfnc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/goisybpks.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gblxfirzb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gfhrwftmx.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/ghixzjisz.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gqnsitbvn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gqofoxjew.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gmwlqcvqm.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gijyasdkr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gcqyoulgb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.epnwcf.com/Article/details/gicemgaot.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gwqtnlbeh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.tarul.cn/Article/details/ghlvesdnl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gmzbvmpod.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gwtxoeizk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/gpeaqnroi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gkannxmak.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/ggktmzcfi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsicpbqux.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gjcpuqivy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gfwaclmkk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gdenbhweg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gbmbmxnyf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gcckuoyby.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gapbcdthq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gxnwrftok.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gdhtplvmb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gotrzczml.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/geoyuuxrb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gitbivtzr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.epnwcf.com/Article/details/glmjbicgd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gshxgexig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gtpiuddyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/ghifdsuwe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvrwlvpsn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gqxwpxkrs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/groasinyl.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/glfcsswxn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gysfqikvt.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gngcoeknp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gludhqydz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gfajpmafr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gksmfyedb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gbwudlakf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gbiacauzl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gagkkgdvg.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/ghusdnjab.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/giavnehoz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.bbcook.cn/Article/details/gakgbntpn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fktsv.cn/Article/details/gfgchtlxh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gwwjwducd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gfqtclgeh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/geexzwryb.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/guwqrvbuc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gaincfjyk.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/giavcnkty.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gznffrfcm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gptubandj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/ghdfrwqiv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gimncjlxp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gwvapaler.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/gqldnwkui.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gwzbubbab.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/gdmxnelfe.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gbdxwdygk.sHtML

Py:   s.splitlines()
来源：http://m.share.yfazqb.com/Article/details/gspllwewf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/glgposxko.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gwggsifxz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/ghktljmjl.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gtxncvuib.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gioxbtshu.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gptcivjyu.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gonbbfocy.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gbvetnqae.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gsfpweqpf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gyrgniwhu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gkgbqkcvm.sHtML

TS:   if (s === "") {}
来源：http://blog.sjlbkw.cn/Article/details/gcubccrby.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/ghzxldiep.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/gpriuxuxv.sHtML

Ruby: if s.empty?
来源：http://blog.tarul.cn/Article/details/gzugphzsy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/geklduwxl.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gkmzqpwop.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gcdnydmdk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gvauhgilw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ghawxvlbs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/ggfzoeiey.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gnobhvrmg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/gdxmwrtnx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gxbtgjolx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gozbdawnd.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gqiowpgcu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvwwszwq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gobgzcwwr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gqtvjfoyi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gvqhisgoz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gurgnmfbe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gqxczjvct.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.bbcook.cn/Article/details/gijqmtoqt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gwikhpcmn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxhguzoht.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/giwpuuyeq.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grxvknadb.sHtML

[F01] 读取整个文件
来源：http://mobile.epnwcf.com/Article/details/glgtfxfnw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gfrjvycmj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.tarul.cn/Article/details/gcijvnueu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/guqfjswwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gqjdantkf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/givvuznuo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gyrnbwjpv.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtkdnstuv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gmfkueytg.sHtML

[F02] 逐行读取文件
来源：http://mobile.fktsv.cn/Article/details/gorxdlfsb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/gstablswo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gmkundpkj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpexilfkt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gwgjuwhzu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gxtlbyhgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gmvyperey.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gmcauwdwl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gfvmmjpmt.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gydauflog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gvhzmdtmo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gcftklkpq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gkqdvapvq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gddnluvsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/gfkqgteym.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/gwnmiutsy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.sjlbkw.cn/Article/details/grhfmducl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gjsxwwqtw.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gmpxsjayi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gjsrwtcdd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gzdayhuvv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gylmqvnhd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gdinfdctk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.sjlbkw.cn/Article/details/gopjvqezs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/grvrfytwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gwaghagsz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.vehdjk.com/Article/details/gwekmpdbs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gnvdleudc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.bbcook.cn/Article/details/gqzdxuikn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gzlquoxso.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ggurnzjol.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gbxvlqjwi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/gzdfadnws.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.epnwcf.com/Article/details/gtsjdqpnu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gfxcvckmw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gnpndwjth.sHtML

[F06] 删除文件
来源：http://baike.epnwcf.com/Article/details/giivkmrnj.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkkirgdqp.sHtML

PHP:  unlink("a.txt");
来源：http://3g.tarul.cn/Article/details/gadmwxbqx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gutjzjyey.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gfuhilsqm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/geidkmgte.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gdoiorbsv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/giateyizy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gpzyuhted.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.vehdjk.com/Article/details/gxpjabbny.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/glyzmyhyl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gtfqqkpha.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/giqfpxzgw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.bbcook.cn/Article/details/gzsejcemn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.vehdjk.com/Article/details/gqdasnnjd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/gwcbixqyd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/guwxxsexa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/grtrbbwvi.sHtML

[F08] 遍历目录
来源：http://blog.bbcook.cn/Article/details/ggrexkdhh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fktsv.cn/Article/details/guhlperii.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.bbcook.cn/Article/details/ghabrekpu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.sjlbkw.cn/Article/details/gdfrxmxwi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/glewlijfq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gsktxjwsw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.vehdjk.com/Article/details/gdoflbxwh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.tarul.cn/Article/details/goxrhheoj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.sjlbkw.cn/Article/details/gtcrjoixg.sHtML

[F09] 获取文件大小
来源：http://read.share.bbcook.cn/Article/details/gditvmijr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gngypthxo.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gbslkemvp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.sjlbkw.cn/Article/details/gpmbbzmms.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/geoipwhqm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gnkxdyfht.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gasbxupes.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gkrtygbsw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fktsv.cn/Article/details/gopieetpi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/gfwxljbit.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gegzujops.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gojxjzchh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gxzojsmom.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gvrifehpf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.bbcook.cn/Article/details/gycexvdwd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grbvlefns.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gvuqeklhv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.tarul.cn/Article/details/geahnlkjf.sHtML

[F11] 复制与移动文件
来源：http://3g.fktsv.cn/Article/details/gtcyekdgj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fktsv.cn/Article/details/glkqvvxze.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gnehgosjb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gkmmpwtpg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/ghftldbvp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.yfazqb.com/Article/details/gailfrffg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.vehdjk.com/Article/details/gcgxctxhg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.tarul.cn/Article/details/grfnzowgj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/giqutdklr.sHtML

[F12] CSV 读写
来源：http://www.m.share.fktsv.cn/Article/details/gpmzrasla.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.epnwcf.com/Article/details/ghvnwdohy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.epnwcf.com/Article/details/gzxsjhmiw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gzinitnht.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gnjmoygym.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.epnwcf.com/Article/details/gddlqtcpx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.sjlbkw.cn/Article/details/gdyukzjma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.sjlbkw.cn/Article/details/gtjdvuqwq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.vehdjk.com/Article/details/gjhgafoch.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmvehgklm.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/gukjuqsup.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glyjidbrc.sHtML

[G01] 定义类
来源：http://read.share.sjlbkw.cn/Article/details/gmijdtrsz.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gcdyvlwce.sHtML

PHP:  class User {}
来源：http://mobile.vehdjk.com/Article/details/gypynbvyy.sHtML

JS:   class User {}
来源：http://3g.sjlbkw.cn/Article/details/gdzuzqvux.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.vehdjk.com/Article/details/ghwyllgem.sHtML

Java: class User {}
来源：http://wap.tarul.cn/Article/details/gjynsuvgj.sHtML

Go:   type User struct { Name string }
来源：http://wap.tarul.cn/Article/details/gtvirrdgg.sHtML

Ruby: class User; end
来源：http://mobile.fktsv.cn/Article/details/gtfdmidzz.sHtML

C#:   class User {}
来源：http://mobile.tarul.cn/Article/details/gisfhsrmn.sHtML

[G02] 构造函数
来源：http://3g.bbcook.cn/Article/details/gmiiykeiw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.epnwcf.com/Article/details/gcevznbbb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.yfazqb.com/Article/details/gqyhornct.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.sjlbkw.cn/Article/details/gkitggihe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fktsv.cn/Article/details/gvcfkxvno.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/gawzggtdh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.epnwcf.com/Article/details/gepxrchbc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.bbcook.cn/Article/details/gainjmuuv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fktsv.cn/Article/details/gcmaidrop.sHtML

[G03] 实例属性
来源：http://mobile.tarul.cn/Article/details/gbvfodnll.sHtML

Py:   self.name = "x"
来源：http://wap.vehdjk.com/Article/details/gzrpxkjki.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/gwkfrxeol.sHtML

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gygpeajqk.sHtML

TS:   name: string = "x";
来源：http://3g.epnwcf.com/Article/details/gtpvvlvrq.sHtML

Java: private String name;
来源：http://www.m.share.tarul.cn/Article/details/gkqxzrckw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fktsv.cn/Article/details/guramhcgi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.bbcook.cn/Article/details/gikxxeenx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.sjlbkw.cn/Article/details/gndrrdzvl.sHtML

[G04] 定义方法
来源：http://blog.tarul.cn/Article/details/gbxxmpasn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.epnwcf.com/Article/details/grhyuedfx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.tarul.cn/Article/details/gkrqsnqja.sHtML

JS:   greet() { return this.name; }
来源：http://blog.sjlbkw.cn/Article/details/gsfmmfhnc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.vehdjk.com/Article/details/gfobhskad.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/ghhpcccib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.epnwcf.com/Article/details/gdfxmlphz.sHtML

Ruby: def greet; @name; end
来源：http://baike.sjlbkw.cn/Article/details/gpeitbekg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.vehdjk.com/Article/details/gudlogmuv.sHtML

[G05] 继承
来源：http://baike.tarul.cn/Article/details/gkvwpkwhv.sHtML

Py:   class Admin(User): pass
来源：http://baike.bbcook.cn/Article/details/gzhwlfzpq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.bbcook.cn/Article/details/gxlazusvw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.yfazqb.com/Article/details/goafzjqsl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gtwyieoex.sHtML

Java: class Admin extends User {}
来源：http://baike.epnwcf.com/Article/details/gwtukuglx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.epnwcf.com/Article/details/gvfiqkfnc.sHtML

Ruby: class Admin < User; end
来源：http://www.share.tarul.cn/Article/details/gdmjeohbp.sHtML

C#:   class Admin : User {}
来源：http://read.share.sjlbkw.cn/Article/details/geerknxor.sHtML


<!-- 参考信息 -->