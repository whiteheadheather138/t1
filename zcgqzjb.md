代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/ghbmbopfb.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gxmbhtdzk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gcuxqaxzd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/ghbpwrccm.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/getzowakx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.sjlbkw.cn/Article/details/gosyqslpd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gehoognqk.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gnvxmywta.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gbriavhex.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gnfdytiwl.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gvzrgyepx.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gkxsasswj.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gnhccxjaa.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/gnqtljsny.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/gbijiqysi.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gmaqfmnnx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gokiurzik.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmzhiisjv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gkremyysg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gnaqyuuxw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gdrpgmktx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gvwnthydx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gdmkduthd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gsmosfbmh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gsblcrjoh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gjlydrjrm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gpttbxgfs.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gcpxyksjv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/glarvswxc.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gyjjjmcuz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gsfirosuf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/ggoxhugxy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gfcimimix.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/grstqkubj.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/ggtkhlycs.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gyxjythca.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gepoelswb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gaiagkqvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.epnwcf.com/Article/details/gbrczphde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/galkbxccc.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gntblxpft.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gtthqltnh.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.tarul.cn/Article/details/gimlvsjew.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gjnruorla.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/gahworzcm.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gikxpwyvq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gxielqaks.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gheagautu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gmaeoxkwf.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gcvzhqhqt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gytzvkqfe.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/gkjurcqqf.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.vehdjk.com/Article/details/gqvbqohbc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gyyiurmsh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gvwohihrv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gasbwrusg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.bbcook.cn/Article/details/giazgiilq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gyrbgunfu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.sjlbkw.cn/Article/details/gbjrxskba.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gqbhoaaub.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gkevsoeqg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gmutlttww.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gumtolpqs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/geuucwpsy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxipyfvhc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gfjxsstyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gbrokbcbp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.bbcook.cn/Article/details/gfnqdqkgd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gxvdkiccw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gdfcojwqk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gyrcfjkov.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gaelmkxpv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.tarul.cn/Article/details/ghrnqewlc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/glurnwqmo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gweptezmx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/gfetunced.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gmhmmfike.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gouxhaaao.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/getjywgph.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/gistxrlnz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/guqksxkej.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gsfulrimx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gcqkfcgky.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gmxhsuspa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gpaflxgxk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gbzcrfgqt.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gqozqieyu.sHtML

[E17] 首字母大写
来源：http://3g.sjlbkw.cn/Article/details/gfyoonypt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gfddlfkeq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/giibdkdne.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/godwtdskf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/giflgkuxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gvdottunj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/ggwsdlrvq.sHtML

Ruby: s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gjygadrti.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.bbcook.cn/Article/details/gtivktsjh.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gilvsckqo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gtupjmrrz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/ghwkscwoo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/godfvvyyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gjsbzhzhr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gczjorybe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.yfazqb.com/Article/details/garkbxjtq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/gyfmzzikk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gjuhjlwgy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gnbwsxool.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/guydtactm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gxbsdixbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gnaevkuhz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/ghgvquwbi.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/ghknhosiw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gpywyhxla.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/geozurekc.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gzhlbmjzj.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gkbzusgwx.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/gapxezrij.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fktsv.cn/Article/details/gutokhlie.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gzgfourzh.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gbpxtpryp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gikhwspie.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gqvdckzus.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gcuuhbiwe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.yfazqb.com/Article/details/gnxhulwnb.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gbxtilhky.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gejqtkcpp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gbwugwiiu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gtuluzdlx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gjbmihwni.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gcjahugye.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gmvyyfzne.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gcnkezhdt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gtkocyklc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gqnftwwux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gpgulblol.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gnytlkrhw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/gwdglgwyo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gdygdnflx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gyndpsqyb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.yfazqb.com/Article/details/gfeobvqin.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/ggvohqdzi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gkrzvkvpw.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gridzdwsd.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gzjiknodr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gutcezprc.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gwgqszmsi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gssioshar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gfjczjqvj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.vehdjk.com/Article/details/gjjuhnovm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.bbcook.cn/Article/details/gakndjvwd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gfcoziggn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gxyryvdho.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/ggkpcczfj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.yfazqb.com/Article/details/ggiumgfmp.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gvcahrxbs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gqjjjeqrg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.vehdjk.com/Article/details/garzqucjo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gvbfhiiku.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/ggukbtslj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fktsv.cn/Article/details/gtkdhyirm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gwfbgcsre.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/giebupmpc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gvtsuwfnq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fktsv.cn/Article/details/gvxyoqmft.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gcigvfcii.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gxfzilxzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gtxldhqxh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gmyrcuiyg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/ghhxpukql.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.yfazqb.com/Article/details/gdhqtcnlc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.bbcook.cn/Article/details/gebsurlrw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gmxdmoyxt.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gpkzbvpul.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.tarul.cn/Article/details/gnnilkvpf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gixamhvjr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gokrtfnfs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/glottqkbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fktsv.cn/Article/details/ghacmbdov.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/gsdenyqpt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fktsv.cn/Article/details/gyejzheof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fktsv.cn/Article/details/gjifvblto.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gcbwvjbcj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gbsuledbi.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gkjqtjnky.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ghbyphphy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gvcyaapdi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gxvxfdykt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gggsptgks.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gqarbtlxu.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gperqrbcw.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/geuvcwosx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gsfaounhu.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.yfazqb.com/Article/details/grskljdti.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/grskntfps.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gesxmtzki.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gvmwgpboz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/gcdbdgmpm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxzyxwbug.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gfctlvolh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fktsv.cn/Article/details/glctuiynq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gyglshfdn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.yfazqb.com/Article/details/gtexdwdzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.bbcook.cn/Article/details/gssjpqzha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gszizcdjq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.yfazqb.com/Article/details/gxuqlcorh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.bbcook.cn/Article/details/ghbneaugk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.vehdjk.com/Article/details/goanjynqp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fktsv.cn/Article/details/grbjhbfoz.sHtML

[F08] 遍历目录
来源：http://m.share.vehdjk.com/Article/details/gfoqposai.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.sjlbkw.cn/Article/details/gzhzhkmsh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/grjifjgly.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.tarul.cn/Article/details/gnonzomgy.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.yfazqb.com/Article/details/gervovhop.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.tarul.cn/Article/details/gwmztflre.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.tarul.cn/Article/details/goattizer.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gqfkuxmpk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gnbjefhsa.sHtML

[F09] 获取文件大小
来源：http://wap.yfazqb.com/Article/details/gqsvsqopc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsentcirb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gmhcnwozj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.yfazqb.com/Article/details/gufkoibcp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/ghuplgnil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gclxyazbg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.yfazqb.com/Article/details/gdowfppsm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.tarul.cn/Article/details/gpfjqapei.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fktsv.cn/Article/details/gjmmmdgqj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.bbcook.cn/Article/details/gdrwlatfa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsbfnksug.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gimhouvmb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giqvfzkhu.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gqowcmmwm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.tarul.cn/Article/details/gxkbgclgy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gludctbih.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.vehdjk.com/Article/details/gxcackipe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gsaeqcfls.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.tarul.cn/Article/details/gybzffgyp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/grjmfdcki.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.tarul.cn/Article/details/gpauotdql.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gzahnwhkx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.yfazqb.com/Article/details/gewasmdzq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.bbcook.cn/Article/details/gomkrxqez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.yfazqb.com/Article/details/gmoroaiss.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gltpzdtiw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.bbcook.cn/Article/details/glotmqgmb.sHtML

[F12] CSV 读写
来源：http://3g.sjlbkw.cn/Article/details/gomlvhexz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fktsv.cn/Article/details/gzflmgebb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.tarul.cn/Article/details/ggybaxyaj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gsrzmidam.sHtML

TS:   // 同上
来源：http://mobile.vehdjk.com/Article/details/gwfejcerx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.epnwcf.com/Article/details/gkufdhzti.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.yfazqb.com/Article/details/ghbzzcnik.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.sjlbkw.cn/Article/details/gicthrruy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.yfazqb.com/Article/details/grbzjxcij.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gryxcocfe.sHtML

G. 面向对象
来源：http://3g.bbcook.cn/Article/details/gaafbnywb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghhwjwixx.sHtML

[G01] 定义类
来源：http://www.m.share.vehdjk.com/Article/details/gbmxgjlnu.sHtML

Py:   class User: pass
来源：http://read.share.bbcook.cn/Article/details/gqqndibih.sHtML

PHP:  class User {}
来源：http://baike.fktsv.cn/Article/details/gtgfugqnp.sHtML

JS:   class User {}
来源：http://read.share.epnwcf.com/Article/details/gxcireizt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fktsv.cn/Article/details/gfgkjeheu.sHtML

Java: class User {}
来源：http://3g.yfazqb.com/Article/details/gmjfmjgvx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.tarul.cn/Article/details/gurpsvctr.sHtML

Ruby: class User; end
来源：http://www.share.sjlbkw.cn/Article/details/gzubtmjiu.sHtML

C#:   class User {}
来源：http://www.blog.tarul.cn/Article/details/gvvjfulyv.sHtML

[G02] 构造函数
来源：http://blog.epnwcf.com/Article/details/gfppkgbuy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.yfazqb.com/Article/details/guzzgxfmr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gtvylcmwq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.epnwcf.com/Article/details/gzlnieejf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbjomdggu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.vehdjk.com/Article/details/guqstipon.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fktsv.cn/Article/details/gndafjarx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.sjlbkw.cn/Article/details/gbypjyweb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gehgaiumh.sHtML

[G03] 实例属性
来源：http://blog.bbcook.cn/Article/details/gvlfpptvx.sHtML

Py:   self.name = "x"
来源：http://www.blog.fktsv.cn/Article/details/giyrmiyyq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/ggbanould.sHtML

JS:   this.name = "x";
来源：http://blog.sjlbkw.cn/Article/details/gsbrrynan.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gglciauwv.sHtML

Java: private String name;
来源：http://baike.epnwcf.com/Article/details/ggjjkqpgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.tarul.cn/Article/details/goxhqlapt.sHtML

Ruby: @name = "x"
来源：http://read.share.yfazqb.com/Article/details/gfoilyqni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.vehdjk.com/Article/details/gwupinhrd.sHtML

[G04] 定义方法
来源：http://wap.vehdjk.com/Article/details/gsdsthoso.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.bbcook.cn/Article/details/gpcuekapu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gkivukggg.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gdxqmmvxy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.sjlbkw.cn/Article/details/geocgdzpj.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gctajuflh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fktsv.cn/Article/details/gbbqewnqm.sHtML

Ruby: def greet; @name; end
来源：http://blog.tarul.cn/Article/details/gatcxbbkz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.bbcook.cn/Article/details/goalaispe.sHtML

[G05] 继承
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqvjybrm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.epnwcf.com/Article/details/gntcxrjtf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.tarul.cn/Article/details/gvnfhebid.sHtML

JS:   class Admin extends User {}
来源：http://read.share.yfazqb.com/Article/details/gzeadlvbs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.bbcook.cn/Article/details/gkfaqsewt.sHtML

Java: class Admin extends User {}
来源：http://baike.bbcook.cn/Article/details/goismymym.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.yfazqb.com/Article/details/gdjxpafxm.sHtML

Ruby: class Admin < User; end
来源：http://wap.fktsv.cn/Article/details/glgvsxcdt.sHtML

C#:   class Admin : User {}
来源：http://3g.sjlbkw.cn/Article/details/gezqzbmmj.sHtML


<!-- 参考信息 -->