代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gqttaaoux.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/giineuqyd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gpvvkiflh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gkbyjffcb.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/guobhugiu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gjjfkpoes.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gxllxotis.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.epnwcf.com/Article/details/gtgrbghtc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gzvpzlyug.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/guuiylzif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gdgxseqfj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbsnadfic.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gocxqimmz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.vehdjk.com/Article/details/gedtnhfsp.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gdhrfrcsx.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gjpbyvubh.sHtML

PHP:  implode(",", $items);
来源：http://blog.sjlbkw.cn/Article/details/gnodkfmsx.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gtffywqku.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/ghnzwcnjw.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gtywkcrmp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gfvhfnuti.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/goovqmtgi.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gpsafilkv.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gvnettjjx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/ghabvueol.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/grkhmfzvc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gvcwwmiir.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/glkryudab.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/giubsrmel.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/ghuwzpeen.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gvfmgwpnq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gvnpgwpel.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gktvqtits.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gjppmczky.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gzeezuuru.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/ghaulodos.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/ggatpscef.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gdvaesbzr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gfzgmeifc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gcxfbiaro.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gqsozfght.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gllhtrlok.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gaojilpur.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gdxzvnlnk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gktrexlks.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gfkdweplq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gwzwkixrp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gmpmvenia.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/geqzjrwkq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gzsmopljr.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gipvpacgp.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/glauwodam.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/gkmvwvtvs.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/glptscshq.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gwohqmjoa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gnjxjxylz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gagomrczq.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gvqgtiwmh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/grqiuvpso.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/gkcmhqtzu.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gysotbuhn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gfpgegdnz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gmsjqwhqo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gmkgwwvqd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/ghatymjgr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gqamizkvx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/gycpoadao.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gckglbmgp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gzipcoopk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gkqzoxytq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.bbcook.cn/Article/details/gqtdongvm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gkxzjvwge.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gisckzxxx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gsfdbjywj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gptugkgsm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gygjpipwh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/glrwtzhzy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gwdxdaszn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gslmkbyuv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gttieefsb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/guypuasje.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/grfmcfrwe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.yfazqb.com/Article/details/gpaewbylt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gkqyqovit.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/giciwcnko.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gdlasvntv.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/getzkvnzu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gdofakblc.sHtML

PHP:  number_format(1234567);
来源：http://3g.vehdjk.com/Article/details/gmmnqlzyo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gpfsbyxbm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gajggdacs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gsnnooixl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gabdrgtsv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gamdcgypj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gopypfyzp.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gtfhhcgqx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gwfmhmlpx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gkzqjvbdj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gtfmciola.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gvygwqolc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gajgzqyyy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gekdbydeq.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gptafubyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gyxmokupw.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gswhjjgsu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gsqwrqdek.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fktsv.cn/Article/details/gnlwukkvx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gyglrnxzd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gxacfwswi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gkxazinle.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gqlwpfekw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gqhrnyrii.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/giharrayz.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gygtrjkcm.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gyxugslpx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/glvzhylkl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gmtnqgsxx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gkyrqekht.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gpmcjcjcv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gzuihiceo.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gmuqzvjdj.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/gdwsknwas.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gekqqztno.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gbmwrmldq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/godnmbnzl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gxwwusemp.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gwovbmcnt.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gmjbcadyj.sHtML

Go:   if s == "" {}
来源：http://read.share.vehdjk.com/Article/details/gvcqyegrs.sHtML

Ruby: if s.empty?
来源：http://wap.tarul.cn/Article/details/gtouasyzr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/gjmfiouug.sHtML

[E21] 超长截断加省略号
来源：http://mobile.vehdjk.com/Article/details/gmaubecwt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/ghpjzoxzx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/ggbsqvjos.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gchgpzayc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gnkfjbuyj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gecajpyau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.sjlbkw.cn/Article/details/gubzzjgws.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gthoqorga.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gnoukkdpn.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gmycayvcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/grrdvmqge.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gcdyrqcwa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/goqcfcljw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gdftdgmmx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gzdkxdqih.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/ggpfaeusz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.bbcook.cn/Article/details/gyrrvcswm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gsyftanpg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoqpyazb.sHtML

F. 文件与目录
来源：http://mobile.epnwcf.com/Article/details/gmvcbdyzn.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gbvfxfvyi.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gfzglgyjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gfulvnxql.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/ghvuklbxa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gemcaehyc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/guztnblhd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gzqarrquj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/gyxvwmjgt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gkblliihz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/ghiwsndpw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gtcsgcdvl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.tarul.cn/Article/details/gzsmknypg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fktsv.cn/Article/details/gteejhjxe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/goerhztlf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/ggejjfqnw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gmcpxmrmh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.bbcook.cn/Article/details/gctmzulak.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.tarul.cn/Article/details/gmfaxncnq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.tarul.cn/Article/details/gghlgvpmm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gjewafdqb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gxkyyieaz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/ggfnfoboj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gdrylvmde.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/glyjzpqcu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/ggzstlman.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gfklsgtsc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gmfkmmlhc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gyfjvwblu.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gggtngqiz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.tarul.cn/Article/details/gmklciukg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gpphfublr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/geqekzfrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gbulwuglq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.yfazqb.com/Article/details/gldufzhnz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gdgwfexol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gvcmhypkb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gbytkcimi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/ghtvusjmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.tarul.cn/Article/details/glgbcbhqg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gbsaycqni.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/guiosqbsg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gpqofffgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/grbxzgkij.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gegakcrrc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gxchuasod.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gyalpvkgd.sHtML

[F06] 删除文件
来源：http://baike.fktsv.cn/Article/details/geknssqrs.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gsmtilpnr.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gztrhgsgm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gkstwznim.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gycfxitch.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gkorgttqs.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/glzoqhzco.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gojnhpwrv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.bbcook.cn/Article/details/ghxvejvwr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gowzyktvw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.epnwcf.com/Article/details/grecawygu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fktsv.cn/Article/details/gpjqncujp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gqtpzehbi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/grxezfxlu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.sjlbkw.cn/Article/details/gibelpolw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.sjlbkw.cn/Article/details/gczybevex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.tarul.cn/Article/details/grpadnlbj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gqpcukvan.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gclrdxksg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.sjlbkw.cn/Article/details/gwchrrlne.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fktsv.cn/Article/details/gccugryaw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gshwpjkjv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/geclobtne.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gsfwvdrok.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gsiffystj.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fktsv.cn/Article/details/galjlmrqg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.yfazqb.com/Article/details/gzrcefjgb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gxhokisfw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gnfcrghno.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.tarul.cn/Article/details/glbnisjet.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.epnwcf.com/Article/details/gmgqlucrm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.yfazqb.com/Article/details/glevfyqdh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.sjlbkw.cn/Article/details/gqoraaifm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fktsv.cn/Article/details/gngefibdl.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gauqlcjqy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.sjlbkw.cn/Article/details/giyzomxrg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/gwvdktlew.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.tarul.cn/Article/details/gfeimkony.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.tarul.cn/Article/details/gyumwlfam.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gkuuabsmr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gkxkhgmwj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.vehdjk.com/Article/details/gcncgqiuz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fktsv.cn/Article/details/gzlmuztyi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmoiqahyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fktsv.cn/Article/details/gqngkipym.sHtML

[F11] 复制与移动文件
来源：http://read.share.sjlbkw.cn/Article/details/gsrirthbd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvvxnlbma.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.sjlbkw.cn/Article/details/grbvnaizo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fktsv.cn/Article/details/gsaqvpjtd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gecexxovt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.epnwcf.com/Article/details/giubwrrbt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.epnwcf.com/Article/details/gmmhoxluf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.yfazqb.com/Article/details/gpqprsqzj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fktsv.cn/Article/details/gqggvgbrr.sHtML

[F12] CSV 读写
来源：http://wap.vehdjk.com/Article/details/gmzvnuljg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/gqhpnccfv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fktsv.cn/Article/details/gqreephvh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fktsv.cn/Article/details/grqyqsabh.sHtML

TS:   // 同上
来源：http://www.share.epnwcf.com/Article/details/gmrythgsx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.yfazqb.com/Article/details/gambzbaep.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.bbcook.cn/Article/details/gkdjajpwo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.epnwcf.com/Article/details/gmtxnwfma.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.epnwcf.com/Article/details/gjcenanwo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdrxebpuu.sHtML

G. 面向对象
来源：http://www.m.share.fktsv.cn/Article/details/ggwphydhe.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnyjuofin.sHtML

[G01] 定义类
来源：http://baike.sjlbkw.cn/Article/details/gsjzubong.sHtML

Py:   class User: pass
来源：http://www.blog.fktsv.cn/Article/details/gzchjqcdl.sHtML

PHP:  class User {}
来源：http://mobile.sjlbkw.cn/Article/details/gxmtmnmne.sHtML

JS:   class User {}
来源：http://www.share.vehdjk.com/Article/details/gycxfxzas.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.epnwcf.com/Article/details/glzlnkzgv.sHtML

Java: class User {}
来源：http://blog.sjlbkw.cn/Article/details/gegbwohbz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.bbcook.cn/Article/details/ghwwjhuyo.sHtML

Ruby: class User; end
来源：http://3g.sjlbkw.cn/Article/details/gdhduiphb.sHtML

C#:   class User {}
来源：http://wap.fktsv.cn/Article/details/gqmdkebps.sHtML

[G02] 构造函数
来源：http://www.blog.vehdjk.com/Article/details/gojsuyjfg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fktsv.cn/Article/details/ghueyaoxs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fktsv.cn/Article/details/giyixptpp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gegrbgipw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/geaddcebz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.sjlbkw.cn/Article/details/gnpghcohm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.vehdjk.com/Article/details/gmxcpycxa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.yfazqb.com/Article/details/gxnkclejx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fktsv.cn/Article/details/gsrhcsjaj.sHtML

[G03] 实例属性
来源：http://baike.fktsv.cn/Article/details/gyvmumrzy.sHtML

Py:   self.name = "x"
来源：http://blog.sjlbkw.cn/Article/details/golxfqzmb.sHtML

PHP:  public string $name = "x";
来源：http://www.share.vehdjk.com/Article/details/gweekjnmu.sHtML

JS:   this.name = "x";
来源：http://www.share.tarul.cn/Article/details/gtfhpaagd.sHtML

TS:   name: string = "x";
来源：http://blog.vehdjk.com/Article/details/gsjtjlmok.sHtML

Java: private String name;
来源：http://3g.fktsv.cn/Article/details/giaynliqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.sjlbkw.cn/Article/details/gwedpkubh.sHtML

Ruby: @name = "x"
来源：http://mobile.fktsv.cn/Article/details/ghzkxgbhb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.tarul.cn/Article/details/gkehquzps.sHtML

[G04] 定义方法
来源：http://blog.epnwcf.com/Article/details/ghnsmervq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.sjlbkw.cn/Article/details/gksvqlxps.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.vehdjk.com/Article/details/gzbyvavgk.sHtML

JS:   greet() { return this.name; }
来源：http://wap.epnwcf.com/Article/details/gozsusbvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.sjlbkw.cn/Article/details/gcirbamoy.sHtML

Java: String greet() { return name; }
来源：http://wap.epnwcf.com/Article/details/gldrbeszw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.tarul.cn/Article/details/gvskdxivb.sHtML

Ruby: def greet; @name; end
来源：http://wap.epnwcf.com/Article/details/gbyelkskg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.tarul.cn/Article/details/gampjilio.sHtML

[G05] 继承
来源：http://3g.tarul.cn/Article/details/gcweipdsh.sHtML


<!-- 参考信息 -->