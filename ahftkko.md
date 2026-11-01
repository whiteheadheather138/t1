代发 wailian999

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/ghcbvwovr.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gvvjcnuku.sHtML

TS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gvlpzrxwt.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gwuqeutli.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gfzfuntvi.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/ghricjmjx.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gericlplt.sHtML

[E09] 去除所有空白字符
来源：http://blog.sjlbkw.cn/Article/details/giubkrwmu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gjpnskanr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gctbkrddm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/grpxcghyy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gbqvlltqy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/gfkhramgy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtltjsxat.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gmmziodqg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gzmvdhsyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/guwnzycfq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gpjpjqzip.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gzuilpbou.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gohtzmurj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gkhuemdgc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gzxuaxnrc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gjeincmge.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gfhxhpomu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/grqyenexh.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gllmtbzzw.sHtML

Py:   s[::-1]
来源：http://wap.vehdjk.com/Article/details/glcppskgi.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gkruyeshu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gwimbcgjz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gonzbvmqm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/giqvugmeb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/gtjyymppa.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gkkywirfv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/gmswiwvla.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gdvjicwvl.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/ghmeleulv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gmzewhzte.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gxrnixdbu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/guknhgrxq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/ggjzgoasb.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gbxagrqan.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gtmqorvcu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gyyziswva.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gufesjqad.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gttmxkvbm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gohuyaluy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gzrthspux.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gtclypvnd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.epnwcf.com/Article/details/gxpliwcsu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gyhyrbzxg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gllnnraqc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gpcuytmqd.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/ghmltmelp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gafulhojq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/gvrmkaicg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gwlpkyeks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gldotugap.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/grqugidpu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/gzfmwiojr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/gsxszqvfo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gwwztknnl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/gbnpujzdq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gxzbzhyry.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gakvjlvoa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gnyehlocd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxxbnlyl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/geqclshay.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.bbcook.cn/Article/details/gywfxsdrp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/gyvketgaz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gjbsmdtws.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gcocfldwx.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/giccdgkcl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/gpuvdemtr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gzkabnoui.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gkvdekmfj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gqkxpbzza.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gkwpffxko.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.epnwcf.com/Article/details/gavacxmmf.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.yfazqb.com/Article/details/ghchrnstv.sHtML

[E17] 首字母大写
来源：http://3g.epnwcf.com/Article/details/gxozaglxv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.yfazqb.com/Article/details/gypgowuht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gizzseaer.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gzrccjyeg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gikxeejla.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/ggkjnxvec.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/goeprpffe.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/govqmlrqy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/giglnwpbg.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gyyroulxc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fktsv.cn/Article/details/gbunysudq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrdoxzkd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gxsgmscqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gjyyacucf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gttfumywa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/ghlsmbbnv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.sjlbkw.cn/Article/details/gxrqfscrp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gkbmqtxiy.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gzivepebb.sHtML

Py:   s.splitlines()
来源：http://www.share.tarul.cn/Article/details/gguxisbvq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gjwmxbinq.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gnnwjhnor.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/goawqjdlm.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gxkhfmfsy.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/gfoabvicu.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gmuooeigm.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gxywmbewt.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gaoiwtujd.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gxlibelwt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gxtgfakwa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.bbcook.cn/Article/details/gurxqtixw.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gfcwepbpc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gptbwlcfm.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gfjqmfnyw.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gmwbcwtrn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gaacsdcox.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/ghajcvifq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gehtndlxk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/ggyefdfhu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gdartgvae.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gpuvptnwe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gytmgijyx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gyiurhtlk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gdtlhytur.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gdqwwpmcz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/ggkihmeow.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gkygjwbze.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gtzsioanb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gvhpphmns.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gvidqsnge.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/grkpmhzwh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjmyhdjs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/ggcegyvwl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gvshgcvzc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdehzsqjb.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gvjhsgdsf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkfcxrsnb.sHtML

[F01] 读取整个文件
来源：http://3g.bbcook.cn/Article/details/gidszhpqd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/goloqksyw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/gockwrmos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gfwnxrmxg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gwbnucrua.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gugleelpe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/gydffevfa.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/ghymnodnc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwwajwvnr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuoqkcfl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/grguejybw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gikruhuqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gdtuhucug.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gpqgjqqfn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gfgbxnilr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/geccbzedm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.sjlbkw.cn/Article/details/gdmcmpdpq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gzhjoglgw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gpznztgqp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fktsv.cn/Article/details/gdeyeooig.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gbndcnxem.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gtzpeczmo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/gzlpiqopw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/geqrorlku.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gkfnrtufw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/gbugejyah.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gevcmdoed.sHtML

[F04] 追加写入文件
来源：http://mobile.fktsv.cn/Article/details/gdhaimkrt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gizvytjbh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnlcavqm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gpjxzdgmm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gldpibzfm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gprltiqjy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.vehdjk.com/Article/details/gryxuimkk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.vehdjk.com/Article/details/gzwxkmfpk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.tarul.cn/Article/details/gpomxyypz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjqycyjd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.bbcook.cn/Article/details/glteemqfz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gcefoqbxk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fktsv.cn/Article/details/goxiycoud.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gthpxulrj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/geonhybey.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsdqriyk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnuwuyexr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gkvliejlr.sHtML

[F06] 删除文件
来源：http://www.m.share.epnwcf.com/Article/details/gbnjwjsor.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gfrbtmagr.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gadmykivf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/ghhvwubpz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/gzfceqgeg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gdgzychjh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gupbfibut.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkqnxevxa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gbykfohgr.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gcoqjmrzq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.tarul.cn/Article/details/gzphmaqjh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.epnwcf.com/Article/details/gawnijgbm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.sjlbkw.cn/Article/details/gxxcfarun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/gjcxuvoue.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fktsv.cn/Article/details/gbycpohiy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/ggktdaklo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/gvkfkozyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fktsv.cn/Article/details/ghesohsdf.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gktnncewv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.yfazqb.com/Article/details/ggpzrldmn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.yfazqb.com/Article/details/gxphihbrk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gphrjebga.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.epnwcf.com/Article/details/gbmgiqzcg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.bbcook.cn/Article/details/gklwhamce.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.yfazqb.com/Article/details/gaegfffae.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/gzvpuavkk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/glxqdkwlw.sHtML

[F09] 获取文件大小
来源：http://www.share.tarul.cn/Article/details/gegdllfvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbafljhig.sHtML

PHP:  filesize("a.txt");
来源：http://wap.vehdjk.com/Article/details/gnavwhtzy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.vehdjk.com/Article/details/gutcjpwwu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.tarul.cn/Article/details/ggdbganzq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gesnigawp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.bbcook.cn/Article/details/gthtnywib.sHtML

Ruby: File.size("a.txt")
来源：http://baike.bbcook.cn/Article/details/gmpgqanml.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.vehdjk.com/Article/details/gsezbrofa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.vehdjk.com/Article/details/goxkzatwb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/ghmquagbt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.tarul.cn/Article/details/gdkzwooln.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.bbcook.cn/Article/details/gsnagzltg.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.yfazqb.com/Article/details/grufbpspi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.tarul.cn/Article/details/gtvjzplue.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.yfazqb.com/Article/details/glremaadk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gxkpadngs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gvrxunloo.sHtML

[F11] 复制与移动文件
来源：http://www.share.tarul.cn/Article/details/gkqnabutg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.epnwcf.com/Article/details/ghgelnfth.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.tarul.cn/Article/details/gdjxiknfu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gpjbftyps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxglobkvt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.bbcook.cn/Article/details/gbiljmxsf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/glncdrtse.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/grdddkpal.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.yfazqb.com/Article/details/gzdqsfhva.sHtML

[F12] CSV 读写
来源：http://www.blog.bbcook.cn/Article/details/gmayvyucr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.tarul.cn/Article/details/gdqowparu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/giynfwlol.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.epnwcf.com/Article/details/gishieqsy.sHtML

TS:   // 同上
来源：http://baike.tarul.cn/Article/details/gftdznkby.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fktsv.cn/Article/details/gbwrcavih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.yfazqb.com/Article/details/gachskekk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.tarul.cn/Article/details/gvqcueeff.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.epnwcf.com/Article/details/gjwqkvlez.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gnwcjrkzq.sHtML

G. 面向对象
来源：http://mobile.tarul.cn/Article/details/gotcjqomv.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gctraijat.sHtML

[G01] 定义类
来源：http://www.blog.bbcook.cn/Article/details/ghiwnbfuq.sHtML

Py:   class User: pass
来源：http://wap.fktsv.cn/Article/details/gnsoxbdge.sHtML

PHP:  class User {}
来源：http://m.share.tarul.cn/Article/details/gkyevnctv.sHtML

JS:   class User {}
来源：http://www.share.yfazqb.com/Article/details/gatrhgotj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.sjlbkw.cn/Article/details/glmlllvhb.sHtML

Java: class User {}
来源：http://3g.vehdjk.com/Article/details/gpuzfrywl.sHtML

Go:   type User struct { Name string }
来源：http://blog.epnwcf.com/Article/details/geegntdnx.sHtML

Ruby: class User; end
来源：http://m.share.bbcook.cn/Article/details/gknbfqczs.sHtML

C#:   class User {}
来源：http://www.m.share.tarul.cn/Article/details/gofjzkbsr.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/gsjahvtxe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhtfzgnx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.bbcook.cn/Article/details/glhjtudni.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gzxphhwtg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fktsv.cn/Article/details/ggifxrypd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gttejgvlx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.tarul.cn/Article/details/gjtcflvtw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.yfazqb.com/Article/details/gpndxmgca.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.vehdjk.com/Article/details/gqvofsfwz.sHtML

[G03] 实例属性
来源：http://blog.epnwcf.com/Article/details/gtterklvz.sHtML

Py:   self.name = "x"
来源：http://www.share.yfazqb.com/Article/details/gtrvrrsad.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fktsv.cn/Article/details/gixbldvpi.sHtML

JS:   this.name = "x";
来源：http://mobile.tarul.cn/Article/details/gevfhiadt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.bbcook.cn/Article/details/gkdiyhtyr.sHtML

Java: private String name;
来源：http://blog.sjlbkw.cn/Article/details/gyqlgwoug.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fktsv.cn/Article/details/gayjsyvmg.sHtML

Ruby: @name = "x"
来源：http://m.share.tarul.cn/Article/details/gxdmkrnot.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fktsv.cn/Article/details/gwstpxddq.sHtML

[G04] 定义方法
来源：http://3g.vehdjk.com/Article/details/gyonaujnz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fktsv.cn/Article/details/gmawcpjiw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fktsv.cn/Article/details/giznefkfi.sHtML

JS:   greet() { return this.name; }
来源：http://wap.bbcook.cn/Article/details/grdvmgodq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.sjlbkw.cn/Article/details/gsyxniegc.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gcuaudzyo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.bbcook.cn/Article/details/grvhblqjg.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gxwmalvgd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.yfazqb.com/Article/details/gzrmkqncz.sHtML

[G05] 继承
来源：http://blog.fktsv.cn/Article/details/gwosxgebi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.yfazqb.com/Article/details/gqjnkmriy.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.sjlbkw.cn/Article/details/gmobekomo.sHtML

JS:   class Admin extends User {}
来源：http://3g.fktsv.cn/Article/details/gpngphbrt.sHtML

TS:   class Admin extends User {}
来源：http://baike.tarul.cn/Article/details/gzwvylige.sHtML

Java: class Admin extends User {}
来源：http://m.share.yfazqb.com/Article/details/gzditlvpn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.bbcook.cn/Article/details/gxqaosvyx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gwjuzjcpe.sHtML

C#:   class Admin : User {}
来源：http://m.share.vehdjk.com/Article/details/grdhasbhy.sHtML

[G06] 重写方法
来源：http://m.share.sjlbkw.cn/Article/details/gvdiaefds.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.tarul.cn/Article/details/gzecrlsrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.bbcook.cn/Article/details/ggtcubbro.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gufeicwxc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fktsv.cn/Article/details/ggfpwifgb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.vehdjk.com/Article/details/grqjqnanh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.tarul.cn/Article/details/gectrnepp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fktsv.cn/Article/details/goxwmtibe.sHtML


<!-- 参考信息 -->