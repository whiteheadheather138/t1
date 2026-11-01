代发 wailian999

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gwbiqipvw.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gbzdslyzv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/ghxkizeki.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gfcbcxurc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gulpiyrbk.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/goomblouv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gczgahkeb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/ghypyuqtr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.yfazqb.com/Article/details/gejhjjkln.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/guvikrqws.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/grdqrxmry.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gyvhcwdcq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gehhpwxgs.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gfdmjbsbf.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gynkrlcnc.sHtML

Java: String.join(",", items)
来源：http://baike.yfazqb.com/Article/details/gmlzoulpd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gtyrgwxzf.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gwvjkdsvg.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/glvxtlxro.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/gvltfooll.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gwhzmqzra.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gorqljefp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gxnllkrvh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjoppwpl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fktsv.cn/Article/details/gvpztrsmj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gqbqdzpeo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gnjgldtkv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/ginxqompx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/gmlkgomvu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpmglltz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gfwhuavhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gndjxhuis.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gnhdlfvfd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gichkbtgr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/giwinpdbm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzhzkegj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fktsv.cn/Article/details/gtehybspc.sHtML

[E11] 反转字符串
来源：http://m.share.bbcook.cn/Article/details/gvewufzos.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gwjftxxhz.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/gnsmkcssm.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gyklyadyt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gcnchspkm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.tarul.cn/Article/details/gpxmhahwt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gmkydggjg.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/gvqrvtqqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gddovxntf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gyfkuxdep.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/glxvgbqsd.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gnozyuwfy.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/glldyanad.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gatkxtdmo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gszltbuyz.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gcnthgmla.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gxwcujbcn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gyqkpruzf.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gvpmkoaxp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gnwnxfioe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/gzfwecler.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fktsv.cn/Article/details/gnratkonh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gschgntzm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gwdlekjke.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gnbsjvhze.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/giwoiabbn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gcmxzssui.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/grlcgssxs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gxzusjcyy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.yfazqb.com/Article/details/gtxuygvaw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gupfsyfjj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gepvwcrei.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gbeksomkj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/godiwcygx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/ghcghwmrf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/ggnbxkonu.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.epnwcf.com/Article/details/gycepkolh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gsjgmptmj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gqtoarssz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/goximtaul.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/glyokdkpx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/gwctixmdc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gwhpgmbpa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/grnkaoqse.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gwfshgutb.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gxirjghrt.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gwmdwgyql.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/gdparyzab.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gvwhtiklp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gskcboqor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gkauxpxvy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.bbcook.cn/Article/details/glwlykora.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gsdhsdxuv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/ggfxzselm.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/glmdnujcz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.epnwcf.com/Article/details/gblnxpcgf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gvzagrqou.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gwthufvsv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gxzrsexrr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gjnkoonvv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.yfazqb.com/Article/details/ghhpucftc.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gnojsnuwv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.yfazqb.com/Article/details/gdlrfmvju.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gmdlwpoku.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gvdovcqvv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gyvxkyxku.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gauvgarpg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gjjxuhrgf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gwpgiyfqk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gogvqiqkq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gwutgofnw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gwrcszibv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/gniicgzkt.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gqhallici.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gtewkplsz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gqmdivdht.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/ggaemtozo.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gsnkgiikp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.tarul.cn/Article/details/gcuptolyp.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gxcunyzjj.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/grasiobte.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gmvipsxer.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gzcolmqlm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.epnwcf.com/Article/details/gxeiijzvg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/ghstsfjjb.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gqrmynrot.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gytajhrlc.sHtML

Go:   if s == "" {}
来源：http://blog.fktsv.cn/Article/details/gmuvfvixl.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/ghneyjxdq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.tarul.cn/Article/details/gwzjzfgdh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/geiuivzop.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gigqfoxrz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gmuhktrsm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gfrvnhzio.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gpkuzbvby.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gkmhnveed.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gsuaghoqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gcbzmcvpt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/ggcbmcjqj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gexpqzile.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.tarul.cn/Article/details/gudgsgaaf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gppdoymir.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/ggmqofwrl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcwypejg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.bbcook.cn/Article/details/gjbnxwiji.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.bbcook.cn/Article/details/gdxjxwwih.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/gnxbwevln.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/gutgmfgci.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gsydtbkjq.sHtML

F. 文件与目录
来源：http://m.share.fktsv.cn/Article/details/gimuxjaqd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gdkosbxko.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gtnwcynyw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/goivdszbj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.tarul.cn/Article/details/gugpfptrm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/ghnakbxoa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gvcazsuhu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/grnljnhjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gtdnragxw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.vehdjk.com/Article/details/gjoihrafm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gyctmqlst.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gfxqhayzr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/glzvqsatr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/gkidnhkzk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gfesppfox.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gqzojojss.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gezcuwvhg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gbwatials.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.yfazqb.com/Article/details/gmdqomcuc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.sjlbkw.cn/Article/details/gheecoker.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gcfklrktq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gflapodij.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/gjdfmwxmy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gdfdgnvmd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gludptdiv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gzoljqkwd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gcepfvykw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gupdeegqe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gtxskfbyn.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gupahnhnh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/gwchxmcxh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gqxheczay.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gspylbhdn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gjervzknf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.bbcook.cn/Article/details/guwijddnh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.epnwcf.com/Article/details/gxcegefus.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.yfazqb.com/Article/details/grzkfszaq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/ghvocvnpz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.tarul.cn/Article/details/ghhflmqwy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.sjlbkw.cn/Article/details/ghgdyikpu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.tarul.cn/Article/details/giwpzpaxe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/grfpgbqgn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.tarul.cn/Article/details/gesjfrfxr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/ggvlicgrh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.vehdjk.com/Article/details/gsabzemmf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/gsahzsxle.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/genplylmn.sHtML

[F06] 删除文件
来源：http://www.share.bbcook.cn/Article/details/gzqoultzm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gdirqbhxg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gaqtjuohq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gvoytyojb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gdlyskark.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gqovwcuqk.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gohvmwblu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gwarvjsws.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.yfazqb.com/Article/details/ggwlwixqe.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.yfazqb.com/Article/details/gnfstreuk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/golspzjvn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.vehdjk.com/Article/details/gndgzjfnn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.tarul.cn/Article/details/ggzhxrmrs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fktsv.cn/Article/details/grtxebvfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.epnwcf.com/Article/details/gdjpieidn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.bbcook.cn/Article/details/gyxqcokzl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.bbcook.cn/Article/details/gxhhrzwhx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.sjlbkw.cn/Article/details/guuutewui.sHtML

[F08] 遍历目录
来源：http://www.blog.fktsv.cn/Article/details/gkpxfsuen.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.tarul.cn/Article/details/gcpjyqbep.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.bbcook.cn/Article/details/gotxxxizo.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.vehdjk.com/Article/details/gooaunrkg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.epnwcf.com/Article/details/geijnacio.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gjdmuqmiz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.epnwcf.com/Article/details/gsltspaov.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fktsv.cn/Article/details/gluiukjse.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fktsv.cn/Article/details/gtexpwtvz.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gowmhexes.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.bbcook.cn/Article/details/ggxayrwxx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.bbcook.cn/Article/details/govahlkuk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.epnwcf.com/Article/details/gudcotlwo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.sjlbkw.cn/Article/details/gegvoansa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gdinhqygd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.tarul.cn/Article/details/gamaalgzi.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gzalzyufa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/glsvuwpwu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.vehdjk.com/Article/details/gyffuffrt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzgidmnlc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fktsv.cn/Article/details/ggxutxzne.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.epnwcf.com/Article/details/gqwaweoja.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gwxcdrwdo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.tarul.cn/Article/details/gafcxubmk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gsrjlykjn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.epnwcf.com/Article/details/gflapabzo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gwiigkfax.sHtML

[F11] 复制与移动文件
来源：http://baike.sjlbkw.cn/Article/details/gzcqcumql.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.epnwcf.com/Article/details/ggbngflga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.tarul.cn/Article/details/gelniwwcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.sjlbkw.cn/Article/details/gomibsufh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.vehdjk.com/Article/details/gonegximp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fktsv.cn/Article/details/gqqvokpxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fktsv.cn/Article/details/grcosmziq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gmcjxqejn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fktsv.cn/Article/details/givmfegvi.sHtML

[F12] CSV 读写
来源：http://www.blog.tarul.cn/Article/details/gotsjtrou.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.vehdjk.com/Article/details/gmevnnlcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.bbcook.cn/Article/details/gnihlgyhs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.sjlbkw.cn/Article/details/gbhenxnja.sHtML

TS:   // 同上
来源：http://read.share.yfazqb.com/Article/details/gpysqeqeu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.tarul.cn/Article/details/gnpzkckqv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.vehdjk.com/Article/details/grycadgpp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.tarul.cn/Article/details/gsabjvjeq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fktsv.cn/Article/details/guxirmxlz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gzemqpbfk.sHtML

G. 面向对象
来源：http://3g.yfazqb.com/Article/details/gberbnpxn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/guvfwrfab.sHtML

[G01] 定义类
来源：http://wap.sjlbkw.cn/Article/details/glkpfbobj.sHtML

Py:   class User: pass
来源：http://www.share.fktsv.cn/Article/details/giyaordqb.sHtML

PHP:  class User {}
来源：http://www.blog.vehdjk.com/Article/details/gotpkshhp.sHtML

JS:   class User {}
来源：http://m.share.vehdjk.com/Article/details/gmnzsevek.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.bbcook.cn/Article/details/ggrdmpwpd.sHtML

Java: class User {}
来源：http://www.m.share.tarul.cn/Article/details/gkskquyly.sHtML

Go:   type User struct { Name string }
来源：http://m.share.vehdjk.com/Article/details/grwuemfea.sHtML

Ruby: class User; end
来源：http://baike.yfazqb.com/Article/details/gzqazucty.sHtML

C#:   class User {}
来源：http://www.blog.yfazqb.com/Article/details/goqydjddj.sHtML

[G02] 构造函数
来源：http://www.m.share.epnwcf.com/Article/details/gtzjkqdgy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.epnwcf.com/Article/details/gvcjtxihn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.tarul.cn/Article/details/gnmhavjea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.bbcook.cn/Article/details/goqolrjdy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gnrrwucby.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.bbcook.cn/Article/details/ggqysakum.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fktsv.cn/Article/details/ghsplaygn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.bbcook.cn/Article/details/genvjjhwj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.yfazqb.com/Article/details/ghvilmxes.sHtML

[G03] 实例属性
来源：http://read.share.sjlbkw.cn/Article/details/gdzlyzziv.sHtML

Py:   self.name = "x"
来源：http://www.blog.yfazqb.com/Article/details/grrnjuxyq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gklgfixwi.sHtML

JS:   this.name = "x";
来源：http://www.m.share.tarul.cn/Article/details/gzgazepgx.sHtML

TS:   name: string = "x";
来源：http://baike.sjlbkw.cn/Article/details/gbdwlowiw.sHtML

Java: private String name;
来源：http://wap.vehdjk.com/Article/details/gthwnzdxg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.epnwcf.com/Article/details/gvjdgknvh.sHtML

Ruby: @name = "x"
来源：http://www.share.tarul.cn/Article/details/gzfsdxwqb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.epnwcf.com/Article/details/gefolmvry.sHtML

[G04] 定义方法
来源：http://blog.fktsv.cn/Article/details/guznyjmvq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.yfazqb.com/Article/details/gkfnymwji.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.bbcook.cn/Article/details/gflisqrld.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.bbcook.cn/Article/details/gzvjqqqii.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhlnrthd.sHtML

Java: String greet() { return name; }
来源：http://3g.yfazqb.com/Article/details/gstkdrnhf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fktsv.cn/Article/details/ghvkwmxsc.sHtML

Ruby: def greet; @name; end
来源：http://3g.fktsv.cn/Article/details/gtkpuqvsg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.tarul.cn/Article/details/gzjhxavti.sHtML

[G05] 继承
来源：http://www.share.fktsv.cn/Article/details/gjokaiwwn.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gtftyzvep.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.epnwcf.com/Article/details/gdtgmfsff.sHtML

JS:   class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gkgqcoykv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.vehdjk.com/Article/details/gfvmmduvo.sHtML


<!-- 参考信息 -->