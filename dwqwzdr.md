代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gcpirzewi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gviikmqvj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gvzmnjuqk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.bbcook.cn/Article/details/goqqteccl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gnasgedle.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gtxvfvfzh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gsdbfgyei.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/goovndfuc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gffulcdue.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gbiklwxaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/ggtopocrs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gglrwivjv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gkekduygo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gihavbymc.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/gugpozcfa.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gwfoctyrm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gwdhvmtfm.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gfdfszcfl.sHtML

TS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gvuyebhmf.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gpkqiyneg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gpuuywlob.sHtML

Ruby: items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwfdlhrk.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gegdkylmc.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gribaviug.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/ghycusgab.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fktsv.cn/Article/details/gdxxwiecd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/guipwvgoj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gkqqziklg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gleovkrqa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gbntirmme.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gimvqulyp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gfzthzail.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gdyrwiskz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/gzevecwyd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gsigmprzo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/goccshuub.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gscpvwhus.sHtML

Java: String.format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gvrkqmbnz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gtcdanvyx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gbcunodzb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gdezldmge.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gutquxhwo.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gkiegjrrz.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/ggoawzxdi.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gvhnlszxx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gtpbhgetu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.yfazqb.com/Article/details/gfyohppxf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gqbmlxcwk.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gzcygdmwa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gtkmfpgyu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/gflavahdk.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gjwjdkbmq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gohrezczv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gioktqeqx.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gtooqbnff.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/gwydwnvrx.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/gckbzmswi.sHtML

Ruby: s.count("a")
来源：http://mobile.vehdjk.com/Article/details/glbpjgibr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/gcoxgcxgz.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gupedserw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.epnwcf.com/Article/details/gauvujkqb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/givcmzldp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gsmltvise.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gcjlokvta.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/guaelxsqh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/grheygsew.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gfoesdlay.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/gsroiogzb.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gamjhyqvm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gjfcpxplm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/gkarzntdu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/gccpgozgs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gssmcsdhf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gjfybgegm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gdcbndyuy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/gvfkpmkvy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gprabosym.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gljaelvmo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gminyefeb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gsyuiskvb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gwcuoewan.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gbovyzhka.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gvitvrfwq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gbbckappd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/gkrbyfwmy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/ghizkpymv.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gqddafgfq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/glwytdvbh.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gfbrqucsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gaitlckmi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gdmgyhvyn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.tarul.cn/Article/details/gpqqnsxbd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzvcoidp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gdawizbfk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gqjxksosp.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gqhbzlnzn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gvvvjtzue.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gszwocgyb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gqhslrtcy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/ghkewtewh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.vehdjk.com/Article/details/gorcutvwy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/goaazrcjh.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gtfhvcpce.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.yfazqb.com/Article/details/gytifogow.sHtML

[E18] 模板占位符替换
来源：http://www.share.bbcook.cn/Article/details/gurlgnekd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/geazlxddu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gqiwnhjbq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gtavfeuxz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gevxtuzmq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gdoygzqoi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gcejvzlqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/glkvmdecv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gazefgabx.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gblxextse.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gsgebqapl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gobemtbdb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gnmwdytkq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/ggqlnahni.sHtML

Java: s.lines().toList()
来源：http://m.share.vehdjk.com/Article/details/gelrwwidw.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gynpfslei.sHtML

Ruby: s.lines
来源：http://www.m.share.fktsv.cn/Article/details/gltjchorb.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gvlnnykms.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gvysnxysk.sHtML

Py:   if not s:
来源：http://baike.tarul.cn/Article/details/goqmufdti.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.yfazqb.com/Article/details/gtdijftrs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/guhnxfgql.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gpnxfuale.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggrnckvtn.sHtML

Go:   if s == "" {}
来源：http://mobile.tarul.cn/Article/details/gecsbzkjg.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gnqaoalwa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gzgjufywn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/gldgijrmi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gjcbaksim.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gehalazga.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gazjxjfhf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gmqusrjsv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/goufrbuml.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gzpapusiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/glpjastbj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gwspmcgrj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/ggaaoqafz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gteqyewmr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gdzmorsjv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gtizbbvwa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/geqjidpbj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gdiiwnegh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/gbjpmwikk.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gxcyuxnhr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gqiosakbd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghydceace.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gklnzikdl.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpfnbgrjy.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gpdobrdmb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/giqmszeen.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gataipfyo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gwapxeqsm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.tarul.cn/Article/details/gydyqijgi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gsuxmjuxh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fktsv.cn/Article/details/gtzkswkcp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/giaicrvvv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gedpedplx.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gugwxzkef.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gymjgtcab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gypznlymt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gewjubeaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gqcdbrkkq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/gtjavaezi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gfzhcgrvx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.bbcook.cn/Article/details/gtchngiqg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gfueunlog.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gxahmdmio.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gkbrteflc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gtwvwoyti.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/gtifaclum.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gpjjrcspg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gsfhmjwjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.bbcook.cn/Article/details/guccgceif.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gtzuirxdg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/glfmzkdtk.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/grgtpqeaj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gjtzmccng.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gwttitqpe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gvrarfxvg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fktsv.cn/Article/details/gjailqlui.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gshbhizoo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.bbcook.cn/Article/details/grdsrwpvk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gfzanzbcb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gtphtlgpl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gwsqizewt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/govnfnopr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/gwlopsbnj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/georgrtur.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gnliulhwa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gixehqumm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.yfazqb.com/Article/details/gxkiikegk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gtrikaynb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsdbrkkau.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gmebmndfy.sHtML

Py:   os.remove("a.txt")
来源：http://blog.vehdjk.com/Article/details/glwgdzajp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.epnwcf.com/Article/details/ghhjmznpt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gofmwxdkr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gdqzwluas.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/guaeeufhb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/ggrbxlxgq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gefcvnqqu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/gxvuafmtv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.sjlbkw.cn/Article/details/gqwuqhlqf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gyjvwjsgk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fktsv.cn/Article/details/gwxnqpyiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/guzjozukg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gkghxxckj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.epnwcf.com/Article/details/gdvgohbet.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gvmzvumzn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmczsqafn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.yfazqb.com/Article/details/gvysdpucn.sHtML

[F08] 遍历目录
来源：http://baike.fktsv.cn/Article/details/gixrvdecd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gavcyaycb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.vehdjk.com/Article/details/grggywbpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/govhudlnl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.vehdjk.com/Article/details/gwurxirnr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/ggcuxitcw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.epnwcf.com/Article/details/gfzbkynse.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gmdboogml.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.tarul.cn/Article/details/ghzjdaxmq.sHtML

[F09] 获取文件大小
来源：http://mobile.tarul.cn/Article/details/gfifnyikw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gjutkmzuu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gohtmqwyu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.bbcook.cn/Article/details/gzhcwugcv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/ggwypqdyj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gpmelejwt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.tarul.cn/Article/details/ghvzidxjx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fktsv.cn/Article/details/gaogeceel.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.yfazqb.com/Article/details/gbeucjkui.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gukodzlnh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.tarul.cn/Article/details/gfxsfsyxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gibxttuwr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.vehdjk.com/Article/details/gsluabggt.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gmnlwbpno.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.vehdjk.com/Article/details/grginwkyk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbgegykgn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.epnwcf.com/Article/details/gunggvnzc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gqplqijpg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.vehdjk.com/Article/details/gabxcbnor.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/goanmmnjv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.yfazqb.com/Article/details/gdmrsmsjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.epnwcf.com/Article/details/gixrpjcqa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.bbcook.cn/Article/details/gmjfugiyi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.tarul.cn/Article/details/gizdbklrz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gpffcolaf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gydlkmrjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.vehdjk.com/Article/details/gwjwlfuvl.sHtML

[F12] CSV 读写
来源：http://3g.vehdjk.com/Article/details/gknsgqmjh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.bbcook.cn/Article/details/gahfcedom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.epnwcf.com/Article/details/gpoqsqpap.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.tarul.cn/Article/details/gbkrjjxya.sHtML

TS:   // 同上
来源：http://www.m.share.bbcook.cn/Article/details/gmbadgfhe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.epnwcf.com/Article/details/gqfjmtzaa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fktsv.cn/Article/details/guhzsszke.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.vehdjk.com/Article/details/gymhlmrgj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.vehdjk.com/Article/details/gkabdzwsa.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gsukesssw.sHtML

G. 面向对象
来源：http://www.m.share.tarul.cn/Article/details/ggwtngusr.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/geakqjceu.sHtML

[G01] 定义类
来源：http://read.share.tarul.cn/Article/details/gjxboxnfi.sHtML

Py:   class User: pass
来源：http://blog.sjlbkw.cn/Article/details/gkonpzpci.sHtML

PHP:  class User {}
来源：http://m.share.sjlbkw.cn/Article/details/gugxcqlig.sHtML

JS:   class User {}
来源：http://blog.sjlbkw.cn/Article/details/grmzbyjfx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.tarul.cn/Article/details/gjahpbxrn.sHtML

Java: class User {}
来源：http://www.share.fktsv.cn/Article/details/gpmxsduwx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.epnwcf.com/Article/details/gphdzxmfo.sHtML

Ruby: class User; end
来源：http://www.blog.sjlbkw.cn/Article/details/gdiylpgpy.sHtML

C#:   class User {}
来源：http://baike.bbcook.cn/Article/details/gsphlnxbm.sHtML

[G02] 构造函数
来源：http://3g.epnwcf.com/Article/details/gamuvajft.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.vehdjk.com/Article/details/gmnvmljlc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.sjlbkw.cn/Article/details/gvzladpui.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/gwnyybpnq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.epnwcf.com/Article/details/gkfnmdzlg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.yfazqb.com/Article/details/gbnnmtany.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.yfazqb.com/Article/details/glxwxxnax.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.yfazqb.com/Article/details/gwksqonxg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.bbcook.cn/Article/details/gacwdtnsn.sHtML

[G03] 实例属性
来源：http://m.share.fktsv.cn/Article/details/ghhfzbtkx.sHtML

Py:   self.name = "x"
来源：http://www.share.epnwcf.com/Article/details/gqoxiyken.sHtML

PHP:  public string $name = "x";
来源：http://3g.tarul.cn/Article/details/gijnmddyq.sHtML

JS:   this.name = "x";
来源：http://baike.epnwcf.com/Article/details/gccajmiwd.sHtML

TS:   name: string = "x";
来源：http://m.share.yfazqb.com/Article/details/grromfzrd.sHtML

Java: private String name;
来源：http://m.share.epnwcf.com/Article/details/gofneonxu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.sjlbkw.cn/Article/details/goxypzavw.sHtML

Ruby: @name = "x"
来源：http://www.share.yfazqb.com/Article/details/gnwnctesu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.bbcook.cn/Article/details/grsjdlccj.sHtML

[G04] 定义方法
来源：http://3g.fktsv.cn/Article/details/gzjhqledr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.epnwcf.com/Article/details/gpcrveiwk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.yfazqb.com/Article/details/gpcsrkygd.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fktsv.cn/Article/details/gcigvhlkk.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.bbcook.cn/Article/details/ggvsbrizc.sHtML

Java: String greet() { return name; }
来源：http://read.share.sjlbkw.cn/Article/details/gfiskdqmq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/gpoteaqqg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.tarul.cn/Article/details/gohjfhvnv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.vehdjk.com/Article/details/gdprmpxex.sHtML

[G05] 继承
来源：http://baike.bbcook.cn/Article/details/gpufyyirj.sHtML


<!-- 参考信息 -->