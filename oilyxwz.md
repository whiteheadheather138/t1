代发 wailian999

C#:   s.Replace("a", "b")
来源：http://wap.tarul.cn/Article/details/gtnlmhhaw.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/gbvmdgact.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/geyhkqzqd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gkztuzzfi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/gbadfwjgc.sHtML

TS:   s.split(",")
来源：http://blog.vehdjk.com/Article/details/gnirfmpso.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/glybuiqju.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gmdcxjajg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gnzahjfon.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gbabxuaql.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gcakeprpz.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gpdtycpsx.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/ghbmhepsv.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gozhjktgz.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gzwwwinas.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/ggrrzivjd.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/ghqlijanl.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gvtjivnlv.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gwvlrtsnh.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/gpevghapq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gbevrfruh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.tarul.cn/Article/details/gvevooiqi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gsqgmmtun.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gkrbfgtpz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/ghstkrrsu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gyocrfzex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/ghwoytmyg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gxurivqez.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gqczjizmt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gnyhidfji.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gujgrbedo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gnxeasnji.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gcimhnltc.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gbfpjraft.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/guarnbrhq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gnsuwzlyf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gslkuvpgb.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/gktyokhem.sHtML

Py:   s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/gphdzvevu.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gmyyxhllk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gjdkkiyqa.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gquacitog.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gmaksqzvl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gtqniequt.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gyknfjvsw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gkklfxymu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/glfbufoof.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gfnlmwsoy.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/grevegzfr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gvknrjnyl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/ghnfnsaqk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/giqddvrbw.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gkabafxyi.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gkhmzyhqe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/glfzhtzuw.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/gktmgbqgq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gcetldyip.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.yfazqb.com/Article/details/gjxxnxlxo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/ghikkescw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gkrqlwgkh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gfiwtknax.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gzkujsxcu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gjobveoim.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gxpyvbxfr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gbojtkedi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gplacevej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.epnwcf.com/Article/details/ginnsroxj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gwgiubcrm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.tarul.cn/Article/details/gixzvnpkk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gmxyokejw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gejezckgp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/ggsjmfzfk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gmbcshdil.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpndfsrx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gnyminjzf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gguneumqp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/glbelqbmp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gsrzzajsl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gvdvavqzx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gjwhfkzgp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gniwwsban.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gwaovavdw.sHtML

[E16] 数字千分位
来源：http://mobile.fktsv.cn/Article/details/gckvlyovd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/giadeetji.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gazyxwpmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gkhzysuoa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/ghmtmcjqn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/glaerparg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.bbcook.cn/Article/details/giofdqten.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/goucakrzr.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gxmfokbph.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gwjjiwnre.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/ghqvulkpj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.epnwcf.com/Article/details/gxaeskmlj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhqspnmt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gqmadloba.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/ggvzphyst.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gujvnumli.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gllamofjo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/gszhxwfdd.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/geodnevtw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gfekpugwb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gkzlgrgps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gnzaaggvt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gpdcpbnvw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gxmrxhuzk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gbcfvybvq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gcqykumyn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/ghtorupht.sHtML

[E19] 多行文本按行拆分
来源：http://3g.sjlbkw.cn/Article/details/gljalhqah.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/garaacadg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gbolrdnic.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gcsgxrzzp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gsbyfjybc.sHtML

Java: s.lines().toList()
来源：http://3g.vehdjk.com/Article/details/ghmhusgis.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fktsv.cn/Article/details/ggxyxaqew.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gekzockab.sHtML

C#:   s.Split('\n')
来源：http://www.blog.tarul.cn/Article/details/gznyzdwor.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gbapavzsh.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/gpazymimk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/glpeuovrc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fktsv.cn/Article/details/gzhmmvpme.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gjyxzwgqu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gexlkegjq.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/grynrafmi.sHtML

Ruby: if s.empty?
来源：http://baike.yfazqb.com/Article/details/gjstubtyq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/glctexyxs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/ghkcfmncs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gyaddcwhp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gknmljnbh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/goqvtgigp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gxanveqsx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/ggrtherrm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gbttjvwkg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtffiudvg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gxofrjttr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gmaqohpot.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gzffdcasy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gyaenrswg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gapwkgmgx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gtdqajigz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.bbcook.cn/Article/details/gwvxljkra.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/gwqrwrlqh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gnekqolle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.epnwcf.com/Article/details/gyignpccs.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcwmcawin.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gzuzmldff.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gdxyyunwg.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gmfaxndzl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/grcsrgjdk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fktsv.cn/Article/details/geueeigya.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gtzwvhasx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gtmcibwlm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.epnwcf.com/Article/details/gchfjcxbs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fktsv.cn/Article/details/guoqygpty.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gtblwmgse.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gboyxukjh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gkmbbtlzu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gpqhqhoos.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.epnwcf.com/Article/details/gzjknotrz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gmkvjnsso.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gciwzsqvk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gojdqarem.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.epnwcf.com/Article/details/gycxmbbmd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gbhheqjhe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/glkejiutu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/glszlkvav.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.epnwcf.com/Article/details/gkjwoxvxc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/giizuhcql.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gmaizqury.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/grrypmbmy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gjfmkkcmm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.sjlbkw.cn/Article/details/gbiydypga.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gwzjpccoh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gsoyqafmr.sHtML

[F04] 追加写入文件
来源：http://mobile.vehdjk.com/Article/details/grevbcumh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gqecxykfl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gjbqnnfeb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gvakwvzzs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/ghngzjxna.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.bbcook.cn/Article/details/ggaqgruwc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gqtbzopdm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.sjlbkw.cn/Article/details/goftxbvya.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.yfazqb.com/Article/details/gabnfwdag.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gsfcbdope.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/grkzwfjlp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gzkclewsn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gircimsqz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwrjuvstc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gtavyjzwm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.bbcook.cn/Article/details/gditlxeqk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gbubcvyso.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.yfazqb.com/Article/details/gorousoel.sHtML

[F06] 删除文件
来源：http://blog.sjlbkw.cn/Article/details/gwguszweb.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gbkwhqqib.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gqjofgypl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyedokexo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfpislfjd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gsoseunmx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gfzcfzmwe.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.bbcook.cn/Article/details/ganglvjcv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gtfrxaxfh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fktsv.cn/Article/details/gxsgqysih.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fktsv.cn/Article/details/gyydqotwm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gzyuzwyxv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.tarul.cn/Article/details/gzknwygon.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.epnwcf.com/Article/details/gvffekklw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gfnrsdoam.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fktsv.cn/Article/details/gtgwpmaht.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.vehdjk.com/Article/details/gztzmewkh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/goxxtgtwp.sHtML

[F08] 遍历目录
来源：http://3g.tarul.cn/Article/details/gjdnvfcyb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gmugdmols.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.yfazqb.com/Article/details/gvmvrqpet.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/gmhflarqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.bbcook.cn/Article/details/gsyjemqoe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.vehdjk.com/Article/details/gqilpjflo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.vehdjk.com/Article/details/gdggqyotx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.tarul.cn/Article/details/gxbblsjjf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.yfazqb.com/Article/details/gnrixmflw.sHtML

[F09] 获取文件大小
来源：http://baike.yfazqb.com/Article/details/gvzsquzzx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.vehdjk.com/Article/details/giynbtrds.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.tarul.cn/Article/details/gxnhvebtj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.bbcook.cn/Article/details/gticthvls.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gwlqcshwv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/ghifyosel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.bbcook.cn/Article/details/gapzlpngk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fktsv.cn/Article/details/gkltcuuas.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fktsv.cn/Article/details/gjsskfxhe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.bbcook.cn/Article/details/gdzmldbvo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gekwxxwid.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.epnwcf.com/Article/details/gikpovgvh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gozdarmjo.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gcmcjihjs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gxzmtxeyi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.yfazqb.com/Article/details/gweutqiwl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gcxxnohqu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.epnwcf.com/Article/details/gfqeqffme.sHtML

[F11] 复制与移动文件
来源：http://www.share.bbcook.cn/Article/details/gwvnznhlu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gyuppfwnq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.tarul.cn/Article/details/gilnbaflp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gjkgyokrh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gytbhnlpk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.yfazqb.com/Article/details/gozucvcwp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.bbcook.cn/Article/details/gtnpltupo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gevgwooot.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gihbfdous.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gnymsqqfa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.vehdjk.com/Article/details/guxzfxhat.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fktsv.cn/Article/details/grqgrhjiq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.yfazqb.com/Article/details/gtflkzfrd.sHtML

TS:   // 同上
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxjckmni.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.sjlbkw.cn/Article/details/gwoxtvaax.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.tarul.cn/Article/details/gehkypycs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fktsv.cn/Article/details/gxshgvzaa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/gxzkfopyh.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdusgtbjz.sHtML

G. 面向对象
来源：http://baike.sjlbkw.cn/Article/details/gmnaijhea.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/glqrqyzxp.sHtML

[G01] 定义类
来源：http://blog.fktsv.cn/Article/details/gwrffpxte.sHtML

Py:   class User: pass
来源：http://www.m.share.fktsv.cn/Article/details/gsvnosvjp.sHtML

PHP:  class User {}
来源：http://read.share.fktsv.cn/Article/details/gnqqwtaya.sHtML

JS:   class User {}
来源：http://blog.fktsv.cn/Article/details/gxvjanphz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/gqyqdrecu.sHtML

Java: class User {}
来源：http://www.share.epnwcf.com/Article/details/gdsxvgsie.sHtML

Go:   type User struct { Name string }
来源：http://mobile.epnwcf.com/Article/details/gwsdebmei.sHtML

Ruby: class User; end
来源：http://wap.yfazqb.com/Article/details/grdxvbjwg.sHtML

C#:   class User {}
来源：http://m.share.yfazqb.com/Article/details/gylemqgce.sHtML

[G02] 构造函数
来源：http://3g.sjlbkw.cn/Article/details/grrdefsns.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fktsv.cn/Article/details/gjmnvvtlx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.bbcook.cn/Article/details/gafzszugk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.yfazqb.com/Article/details/gviibuixu.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/ghlvdmvij.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.yfazqb.com/Article/details/gjlzibrod.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.bbcook.cn/Article/details/gagdeuwhk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.vehdjk.com/Article/details/glrprjcyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.vehdjk.com/Article/details/gsgujumru.sHtML

[G03] 实例属性
来源：http://3g.sjlbkw.cn/Article/details/gggkxpbkg.sHtML

Py:   self.name = "x"
来源：http://www.share.tarul.cn/Article/details/gsxlminol.sHtML

PHP:  public string $name = "x";
来源：http://baike.epnwcf.com/Article/details/guczinenh.sHtML

JS:   this.name = "x";
来源：http://blog.epnwcf.com/Article/details/gulpqnlcn.sHtML

TS:   name: string = "x";
来源：http://3g.yfazqb.com/Article/details/gvixgmssd.sHtML

Java: private String name;
来源：http://baike.sjlbkw.cn/Article/details/ggstobqrh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fktsv.cn/Article/details/gapagbwte.sHtML

Ruby: @name = "x"
来源：http://blog.tarul.cn/Article/details/ghszmbvst.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fktsv.cn/Article/details/gfrxfvucg.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/gvutavhjz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.epnwcf.com/Article/details/gnoisnnld.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fktsv.cn/Article/details/gohdnndwj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.yfazqb.com/Article/details/gzgmqhrux.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.vehdjk.com/Article/details/glrrhldxl.sHtML

Java: String greet() { return name; }
来源：http://baike.bbcook.cn/Article/details/gzefzhuto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.epnwcf.com/Article/details/glzafmvrg.sHtML

Ruby: def greet; @name; end
来源：http://blog.epnwcf.com/Article/details/gvkexesoy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.vehdjk.com/Article/details/ggjyzngbo.sHtML

[G05] 继承
来源：http://www.m.share.epnwcf.com/Article/details/gechvutus.sHtML

Py:   class Admin(User): pass
来源：http://baike.vehdjk.com/Article/details/gzgfuobzd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.yfazqb.com/Article/details/gjemlbjtu.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gvqueipah.sHtML

TS:   class Admin extends User {}
来源：http://www.share.vehdjk.com/Article/details/gdbtsyoka.sHtML


<!-- 参考信息 -->