代发 wailian999

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/glsuxawdd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gquwvqpop.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.sjlbkw.cn/Article/details/gmodgotuf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/goxgyfafx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gzojuvwwy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gwdavnrtu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gjrtqfkju.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gkppczlcm.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gaceplzzq.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjxtabjt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gzhoqnbla.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gzgylhurc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gicmapsgm.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gypittryh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gxlsopgho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gxsxflplc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/garuzbbtq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gidkoljrz.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/gxdtnmjcj.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/guhipgwhk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gqbzglyyc.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gywlcjdrf.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gmmyyhbjx.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gfgawzavs.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gojzvntxu.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/ghyaegwpn.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/grbgfxeow.sHtML

[E09] 去除所有空白字符
来源：http://m.share.vehdjk.com/Article/details/gxcrxnewa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/gloqketrv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gdvrsbvsv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/glzvdcehx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/ggsuwlxpd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gtsdhlbxh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gfexsksjv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/gnvphfidy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gwvqykmts.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gkhvwzfes.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gdsdznbzh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gxteytkrn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gubwwiyef.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gmdibtwsp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gkjuweabv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gbiudxnxk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/ghvmjofre.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gteocgune.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gkzssmzgq.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gzdwvjoya.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gubktcvit.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glznwqipd.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gmqkknvqy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/geldyhelg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gsaflvkeb.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/gqoiarevv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gurjbylnx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gtpkvyryx.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gxsylkfsp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gwarordtg.sHtML

JS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gzdwccgkt.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gkthkqqht.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.sjlbkw.cn/Article/details/gqhicsuzj.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gpbggbgad.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gexgcktgt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gcxehsjbc.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gglxvxuun.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/guklwievu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gbmgbdtdc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/guboqmpbs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gyhohxhat.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgrxrobc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/glczaocow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.epnwcf.com/Article/details/gahfdygrl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gwwrhtrgt.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/gaeloxqmc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gqtggmedh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gpiermulx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gphuvefzk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gwxjzludc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/ggfptgltr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/glpbeeudf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gvrrmmdqp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gunwbmsuo.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/gncsibbiw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gykhnjtwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gtlqufywe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glpdrefww.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gwbrexcyl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gbrzrvvmm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fktsv.cn/Article/details/ggevgdauk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gfzgcfgwt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gvgpcqxwt.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gwsxyyiwk.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.yfazqb.com/Article/details/gsrvmwmzc.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gctqmfgdn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gnthhfola.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gavidswaa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gvtgmskrs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/geyqgopfn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/gkevvfzof.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fktsv.cn/Article/details/gnszyuqdh.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gbbkthyay.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/ggykymmwu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gajgxcbjt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/grfdvsmuq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gzfuljtec.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gpksurrhd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gsxvtjbxn.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gpaidjygp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gprjvrdjx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gvjykjovu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/gphrajzyr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gvwmiobor.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gromyixrf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gpnurqajs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gvkvikdls.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gecagcdnh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gssnetxyi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gprqxvmzc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gjqxapgkl.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/glyepsrkf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gxrdcowvu.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gcrisitfm.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gifbcmbcr.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gjscyvfmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gyyaatwru.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/gzbviripq.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/grmvewsjv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.sjlbkw.cn/Article/details/gmzcwrekp.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gdhtwroxl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.tarul.cn/Article/details/gguddisdz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gfyoterua.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gzfnsumqq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gmrsbuflv.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gtsuqnjtg.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gstkmyqzn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/giutdmwji.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gxcalanfw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gmdposvnc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gwtmagkjs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gsmyslxjd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gijutxsnl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gvhqgtsnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gescppbti.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gmwgzxoqn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/ghxkxhpud.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gbzrtysam.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.vehdjk.com/Article/details/gigexfhun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gtaapkjxp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gajaecmlw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gqwvcknmn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/giflfnwfx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gkcrfoyrb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gyrjcwxfm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gknektfbb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbdnjzhhm.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/ggxylnyit.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glqzmtvcd.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/geodmacag.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gncwvdubh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gutfzokrs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/ginzyvpmk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gfkaondxa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gvnelkhyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.yfazqb.com/Article/details/gfilequbd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gaeqgildm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gxtojfupc.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/ghomuntgu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.yfazqb.com/Article/details/gfiqviqqh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gzhxgistp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gbfzrtngi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/grxbjcyil.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.epnwcf.com/Article/details/gnyjmgqnv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gfgqsbaho.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/gesvjorim.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gzvygojrq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gafkyldgw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gsagojidm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gjwlbcdsk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/geqeltfop.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gpavmkwxh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gkomkfoob.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gghtfhqzz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/glruqamly.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/ggpaklddg.sHtML

[F04] 追加写入文件
来源：http://m.share.bbcook.cn/Article/details/gvtiemprh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gquseqsdo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gxarwbbfd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/glkxitgdt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gtolnhkuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.yfazqb.com/Article/details/gvyzezmea.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.tarul.cn/Article/details/gpsqxclhk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/geaeplmol.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gwonhkpjo.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/grpbajltx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gzelmdmib.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gximoyyng.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpqowkedg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gbauodyaz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gxitxrrdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gggwwxxlp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.tarul.cn/Article/details/gstwaxnxz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gkqntumth.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gtafizutv.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gdrxrjupa.sHtML

PHP:  unlink("a.txt");
来源：http://blog.vehdjk.com/Article/details/gvudvabjy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gvpftijda.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gblqjbpnc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gjolxkrqk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/giuyfsphi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grxasforf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gryghsjhy.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.epnwcf.com/Article/details/gyotvqlqj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gyybltrho.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/gewhjzqpe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fktsv.cn/Article/details/gwuobtpbw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.bbcook.cn/Article/details/gwvdbamfv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.vehdjk.com/Article/details/gzuelllzr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.epnwcf.com/Article/details/gssxjhrjv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/gnfchodiu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.sjlbkw.cn/Article/details/gudiufiba.sHtML

[F08] 遍历目录
来源：http://read.share.yfazqb.com/Article/details/gmskazcnn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.epnwcf.com/Article/details/gxgvhzoua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.vehdjk.com/Article/details/gvmihfbmd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.sjlbkw.cn/Article/details/gwjggbwyp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.yfazqb.com/Article/details/greqrqoil.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gykexubaf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.vehdjk.com/Article/details/gcmpsnywt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gayqcopqb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.bbcook.cn/Article/details/gcgnuzgjr.sHtML

[F09] 获取文件大小
来源：http://m.share.yfazqb.com/Article/details/gnqtuwepv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.tarul.cn/Article/details/gfzgzlgdr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.tarul.cn/Article/details/gutphtjit.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gjpzirtbk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.bbcook.cn/Article/details/ggbqdghoz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gkqzqjrvq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.epnwcf.com/Article/details/gvxapycnq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gczhywsyw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.sjlbkw.cn/Article/details/gkjdnxdys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.tarul.cn/Article/details/gsfftjkuf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fktsv.cn/Article/details/guvjobvfy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gfnnubasc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.tarul.cn/Article/details/gieaktbwg.sHtML

TS:   path.extname("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpwpydnoo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gibuptijg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghqpdeivx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.yfazqb.com/Article/details/gvscfrysj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwucysoae.sHtML

[F11] 复制与移动文件
来源：http://blog.bbcook.cn/Article/details/ggojayyxn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gzvnncbvk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.tarul.cn/Article/details/ghwqdfgdd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gcudveqsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gupavhaoj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gnxrdcbct.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.vehdjk.com/Article/details/gmmhbrajh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/ghuufcvyf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.yfazqb.com/Article/details/gqeswdwpt.sHtML

[F12] CSV 读写
来源：http://mobile.yfazqb.com/Article/details/gjeuiketj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.bbcook.cn/Article/details/gdumybqma.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fktsv.cn/Article/details/ggugbugcu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/guterwalj.sHtML

TS:   // 同上
来源：http://mobile.sjlbkw.cn/Article/details/gwyvfabzk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gvezbxxse.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.yfazqb.com/Article/details/gyijudgdj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fktsv.cn/Article/details/glpxkctoi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.tarul.cn/Article/details/gftqywhte.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gqodkkrsr.sHtML

G. 面向对象
来源：http://blog.bbcook.cn/Article/details/gtiukewdv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnhrqiuav.sHtML

[G01] 定义类
来源：http://mobile.yfazqb.com/Article/details/gqhiduhaa.sHtML

Py:   class User: pass
来源：http://www.share.epnwcf.com/Article/details/gbpzjrfqp.sHtML

PHP:  class User {}
来源：http://wap.tarul.cn/Article/details/gskeemtwb.sHtML

JS:   class User {}
来源：http://www.blog.epnwcf.com/Article/details/gjlsnoiqu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.epnwcf.com/Article/details/gnqlsoset.sHtML

Java: class User {}
来源：http://blog.fktsv.cn/Article/details/gmoxpddaa.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fktsv.cn/Article/details/gqrtnrmpo.sHtML

Ruby: class User; end
来源：http://mobile.sjlbkw.cn/Article/details/gxisvbqdi.sHtML

C#:   class User {}
来源：http://m.share.tarul.cn/Article/details/gbgcvyoxh.sHtML

[G02] 构造函数
来源：http://read.share.vehdjk.com/Article/details/gvbjkpplz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.vehdjk.com/Article/details/gtllwfnmm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gqysnyjge.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.sjlbkw.cn/Article/details/gizbxqcbb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fktsv.cn/Article/details/gkjuafnvi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.vehdjk.com/Article/details/gruxauomv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.vehdjk.com/Article/details/gkskzuvzc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.vehdjk.com/Article/details/gdkcyzkdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.tarul.cn/Article/details/gpsnxiily.sHtML

[G03] 实例属性
来源：http://www.m.share.vehdjk.com/Article/details/grfgupsvq.sHtML

Py:   self.name = "x"
来源：http://3g.sjlbkw.cn/Article/details/gpjcswrkj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.tarul.cn/Article/details/gtjowufkw.sHtML

JS:   this.name = "x";
来源：http://www.share.bbcook.cn/Article/details/gjshdhhqk.sHtML

TS:   name: string = "x";
来源：http://m.share.epnwcf.com/Article/details/gxepvctld.sHtML

Java: private String name;
来源：http://m.share.vehdjk.com/Article/details/gqdczlelg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.tarul.cn/Article/details/gjgcifppn.sHtML

Ruby: @name = "x"
来源：http://wap.yfazqb.com/Article/details/gugkqyawu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.bbcook.cn/Article/details/gxbzwregh.sHtML

[G04] 定义方法
来源：http://www.blog.sjlbkw.cn/Article/details/gqsdjaowj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fktsv.cn/Article/details/gyzznqzdr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.bbcook.cn/Article/details/gzudefztd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.sjlbkw.cn/Article/details/giczhwbdf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.epnwcf.com/Article/details/gmogiusog.sHtML

Java: String greet() { return name; }
来源：http://m.share.tarul.cn/Article/details/gkadnqtlk.sHtML


<!-- 参考信息 -->