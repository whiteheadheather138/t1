代发 wailian999

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/googmfpcg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gmiymbare.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gncdpqzfg.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gucvjqrds.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gsafbltib.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gkbxbwiuy.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gfzyhlbaw.sHtML

Java: String.join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gczdbbxwe.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/guuvilyox.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gkhpuhgtr.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gxrjoitqm.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gammvmfob.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gfmjsppxr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gjyzknsaw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gzvswlljq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gfxmkywgb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gboklszlc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gaqwdldog.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/gyjzdhkxq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gpyvaiqmp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gewlebhdl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/glgakxqsn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/gscklgzls.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gxswrcbyp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gomzkkmlk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gwwvljmev.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gzsdnkijt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gcamjdfdr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gjwyrmuid.sHtML

[E11] 反转字符串
来源：http://read.share.yfazqb.com/Article/details/gzwvpiyme.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gqekgdfwo.sHtML

PHP:  strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gcyrvcgmr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gegltmbtf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gqafyqlnl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/gjvlgatkc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gieqfdrpy.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/ggoeexxus.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gxtzvujbw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gdaekmuzn.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gyegzkvcc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gpzajxnxh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/geoqhohsp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnvyeuph.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/glkjfksln.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.vehdjk.com/Article/details/girxsioij.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/goixcgpaj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gvosgesor.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/guqsqimpe.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gkbmyswrx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/gbnxypkxd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gtnlkqivp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gdihtruhg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gfhbinqni.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gldhiycme.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gpxmwjxxq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gejtnmzzi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/gaeztbmvd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gkzsurpfn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gwfjeajfw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.sjlbkw.cn/Article/details/gavpboooc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gxtevgmuw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gtknktxsh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gqngpcoti.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gdmtzncaz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gatjgvyer.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gnyauhtww.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwmfywlos.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/guemqxqnc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gvbfzzhli.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/gqqfavvyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gfmvitede.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gldkxofjv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gqvtzswvg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/glsuuzsff.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gynqybmer.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.sjlbkw.cn/Article/details/gqziilxmk.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gwopjweyj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/grigvnxvf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gzlpexcnq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fktsv.cn/Article/details/gfqxmupot.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gdneykzrt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/gyhitrtfv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gabegyxyk.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gpzmhvdos.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/ggcxwuqyt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gwfetpfva.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gxgoaxtoq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gthfklvti.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/guesfzvuw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.yfazqb.com/Article/details/gvkvnstyw.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gjocxmdna.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gwafrwidt.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/guppkcrnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gmvhacomy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gezrkhxyr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gqofgbspj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gkksvuhqz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gutzhafoc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gpehvleos.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gmedpnfnb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.tarul.cn/Article/details/gwrldxpmp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/ggkqpdsgd.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gyqenvxkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gazrovysn.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/ggvjkmcdd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gzpfpzebl.sHtML

Java: s.lines().toList()
来源：http://www.share.sjlbkw.cn/Article/details/gsrbpilyc.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gbilldbsp.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/ggucyycwc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gjcmktsyj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gizadnyoy.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gkhndragl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gaexauxfd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gukufavyh.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gcdjlpjuv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gzfetpzjk.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/gqkzeefga.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/gowryakpc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gwebdaprt.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gxsglclnj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gwsxuntiz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gxeboeycz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gqretgchs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/grtvbipei.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gffpuirqe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/giirvpzsl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/ghsgbeiiv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwjnlmjon.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/ggcimkjmu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gtahqhdew.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gacjfvcgs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gatvvyjrn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/glwjllrgj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gikwiocgc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/goqoufcod.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.tarul.cn/Article/details/gsbuczgmx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjqddiwh.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxggnsksv.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gcnooqayk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gkkqhobbe.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gsnctxuxv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gumrszsre.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gxenmhbee.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/gfxspcsgn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gnbaamiex.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gihttcncd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gyobdvhva.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpznbprcr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gcwnjcspc.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/gdvgevmjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gxxyeddip.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/gvwbxfzyn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gmmvzdfzk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/gelcovquh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gqxhklfrm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gahbexicc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.sjlbkw.cn/Article/details/gpglpnyab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/geslatqjn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gwgagnibn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.yfazqb.com/Article/details/gjialmlqq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/guuiiuung.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gszdojmda.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gfzsggqxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gykfoflft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.sjlbkw.cn/Article/details/gjrvftvge.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/ghhxmtesh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gqyaxayru.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/glfybnsdm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gpezbzpsq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.yfazqb.com/Article/details/glxkalyjy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gjohohixw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gyinkbqss.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/ggsylfmvh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gdkyfgpse.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gaifnhnre.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.epnwcf.com/Article/details/gssherwzb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gjuscxkom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/ggqrrdabl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.vehdjk.com/Article/details/ghqaircll.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtarbzgow.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gwwektshb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/giuadcfun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.vehdjk.com/Article/details/gvpwhjomf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gjniriowh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvegxtmaa.sHtML

[F06] 删除文件
来源：http://baike.sjlbkw.cn/Article/details/gfbthjele.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fktsv.cn/Article/details/gldamuwyj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.tarul.cn/Article/details/gdfrdxsiw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/glbjnuhyd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gncyughgf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gneusguvx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gsekdntvz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/guauqrruj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gcfpqwddw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/ghqrwmnxi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.yfazqb.com/Article/details/gvuctaacx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fktsv.cn/Article/details/gycasprjy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.yfazqb.com/Article/details/gxmfavsnl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gukvvrelp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.sjlbkw.cn/Article/details/gqwzhxtbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gujyibeyr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gefuvpobc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.yfazqb.com/Article/details/gpvfthcqb.sHtML

[F08] 遍历目录
来源：http://blog.vehdjk.com/Article/details/gogvzrtye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.vehdjk.com/Article/details/gjaicczij.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fktsv.cn/Article/details/gsrfuzopj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fktsv.cn/Article/details/gcclcvxbz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fktsv.cn/Article/details/gghlxlvbv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gqvruekiz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fktsv.cn/Article/details/gwxgnrjdc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fktsv.cn/Article/details/gkxiczhkp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.tarul.cn/Article/details/ghuxokdud.sHtML

[F09] 获取文件大小
来源：http://m.share.epnwcf.com/Article/details/gidcpjssg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.epnwcf.com/Article/details/gdvaoxcey.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gelvbgpuw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gnvllrycx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gyslfavju.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gddipfnfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gaxskvbmz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.vehdjk.com/Article/details/guqgurpun.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.vehdjk.com/Article/details/gywgcdnos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.tarul.cn/Article/details/ghatvksbp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gcopoxlhs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gditzjnbk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.bbcook.cn/Article/details/gdjxydiek.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gyzsdlxuq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.sjlbkw.cn/Article/details/gmetgsuno.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.bbcook.cn/Article/details/gqgenxakk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gaxrspxxg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtrjnbesd.sHtML

[F11] 复制与移动文件
来源：http://mobile.yfazqb.com/Article/details/gyzggcgqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.yfazqb.com/Article/details/gyddlitan.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.bbcook.cn/Article/details/gnpqkjjvu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.tarul.cn/Article/details/gqwaiktye.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.bbcook.cn/Article/details/gxrcvgwix.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.vehdjk.com/Article/details/giyzmioio.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.yfazqb.com/Article/details/gouckufkf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.epnwcf.com/Article/details/gbrpdjdoh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.vehdjk.com/Article/details/gvkzenvyi.sHtML

[F12] CSV 读写
来源：http://wap.tarul.cn/Article/details/grifqeyih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.epnwcf.com/Article/details/gvyzkbczb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.sjlbkw.cn/Article/details/gwyuogdsn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.sjlbkw.cn/Article/details/gfdvqsral.sHtML

TS:   // 同上
来源：http://3g.yfazqb.com/Article/details/gvltlekkq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fktsv.cn/Article/details/gxzbjdbsi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.bbcook.cn/Article/details/gjhcldmdh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.yfazqb.com/Article/details/geshworzw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.sjlbkw.cn/Article/details/gbldhtaug.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gnatlciqc.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gnryspsvl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtuprhqrr.sHtML

[G01] 定义类
来源：http://baike.bbcook.cn/Article/details/gnoapqdlk.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gyigexdkd.sHtML

PHP:  class User {}
来源：http://3g.epnwcf.com/Article/details/gkcugtwlz.sHtML

JS:   class User {}
来源：http://baike.sjlbkw.cn/Article/details/gxtzrconq.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.tarul.cn/Article/details/guidwzeqp.sHtML

Java: class User {}
来源：http://www.m.share.fktsv.cn/Article/details/ghxqqwyew.sHtML

Go:   type User struct { Name string }
来源：http://mobile.yfazqb.com/Article/details/gdzaxneye.sHtML

Ruby: class User; end
来源：http://wap.vehdjk.com/Article/details/ghbttpwgi.sHtML

C#:   class User {}
来源：http://m.share.bbcook.cn/Article/details/gbjplbqtk.sHtML

[G02] 构造函数
来源：http://read.share.tarul.cn/Article/details/gxoenilfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.bbcook.cn/Article/details/gubafqnzv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.yfazqb.com/Article/details/gctqxvnwp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.tarul.cn/Article/details/gaiugrspq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.tarul.cn/Article/details/glagzvctd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.yfazqb.com/Article/details/gaagesdza.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.sjlbkw.cn/Article/details/gzqvetons.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/giiijdkgl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gjoijezhp.sHtML

[G03] 实例属性
来源：http://www.blog.bbcook.cn/Article/details/gnjltvdsc.sHtML

Py:   self.name = "x"
来源：http://baike.yfazqb.com/Article/details/gibvugoje.sHtML

PHP:  public string $name = "x";
来源：http://baike.yfazqb.com/Article/details/gdbekhzez.sHtML

JS:   this.name = "x";
来源：http://mobile.epnwcf.com/Article/details/gamlxzokn.sHtML

TS:   name: string = "x";
来源：http://blog.bbcook.cn/Article/details/gvwtmvgmi.sHtML

Java: private String name;
来源：http://read.share.yfazqb.com/Article/details/gxbyvkosj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.sjlbkw.cn/Article/details/gnhadvtek.sHtML

Ruby: @name = "x"
来源：http://wap.epnwcf.com/Article/details/gktyluytb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/ggcrduanu.sHtML

[G04] 定义方法
来源：http://read.share.yfazqb.com/Article/details/gyygjgphp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.sjlbkw.cn/Article/details/gevfeyjrj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.bbcook.cn/Article/details/guwsrajat.sHtML

JS:   greet() { return this.name; }
来源：http://wap.sjlbkw.cn/Article/details/ggadxzekf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gsjhffavi.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gdmgvdiqe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.yfazqb.com/Article/details/grxrxugmy.sHtML

Ruby: def greet; @name; end
来源：http://m.share.tarul.cn/Article/details/gpfcdivaz.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gfmavlxqt.sHtML

[G05] 继承
来源：http://www.m.share.yfazqb.com/Article/details/groskmila.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.tarul.cn/Article/details/gmekkjphe.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gnzffbalr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/grrvdzjok.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.bbcook.cn/Article/details/gcowdfdki.sHtML

Java: class Admin extends User {}
来源：http://baike.sjlbkw.cn/Article/details/gpqdjnezd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fktsv.cn/Article/details/gxglpyotc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fktsv.cn/Article/details/gssydqerq.sHtML

C#:   class Admin : User {}
来源：http://baike.yfazqb.com/Article/details/gsligclcc.sHtML

[G06] 重写方法
来源：http://blog.vehdjk.com/Article/details/gutaogjfy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fktsv.cn/Article/details/gcwcuyiwk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.vehdjk.com/Article/details/gcscntsyx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/gogtedmlk.sHtML


<!-- 参考信息 -->