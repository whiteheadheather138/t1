代发 wailian999

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/ghlsnmwkl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gtzluwlld.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/gqqnrhenu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/giedjerly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gffrzanyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gkgefsjlc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gxzhmlqep.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gjtfrbwsd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/geiwqdmdr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gzzpiqnnc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gdjdljsof.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gfgmwqcln.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gxxadglvj.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gmgxlhqsm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gdctfftpi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gnzsrtdxp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gnhbkyoxc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/geaeqbfty.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gqqsqriug.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gjozofbuo.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/ghnrsfdkq.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gogtojrfd.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gsvhnkyms.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gnobmcwyv.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fktsv.cn/Article/details/gyfejblrl.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gosbehuys.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gqcnghvld.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxkggjoz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gqcnjedbs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gjisaumda.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gdsvvzrdc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gdqshyywt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/grdmsjpoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gzqzhgtxt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gtfkbiqkr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/godtcbqus.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gckadbvvc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gvwpuepfw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gsqeingit.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gjnfpsywg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/ghwbpyrku.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gwryolrpi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gupczzlui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gecyomsqy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gecxvqmlw.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gudyshuux.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/guywmwlch.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gtkgwcdxa.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gjiusxppk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gpqjxjndb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gzmbexhcr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/glibjgsvf.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gjpaujfao.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/ghweeurfp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gvqybratz.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gdbtcsrmx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/gboggsxwl.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gnjfaznzj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gwmckedvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gmthfensc.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gettilhic.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gcwfdfaji.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gzghtxvve.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gjevkilpi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdiwjtlu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gztsfchkp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gyjsqgikm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/goicddcqr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gfqaikqcj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gteslhgtf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gbsligzwu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gmjdqcqsa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gjarjzdcg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/ggjnckhta.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/gpzmohgyp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gxynzgfeh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/geuyyfqvu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gzrdmkdsd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.yfazqb.com/Article/details/gmbuppoqm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gaofppynb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/grqohojhc.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.tarul.cn/Article/details/gjxmalpkv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gaeewwmeo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/grwrchstz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqcredvsj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.vehdjk.com/Article/details/grbtbhyhg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gglvtprwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gxjynhovd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gofgcossk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gdpraealh.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gvxapnnji.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gyjvlgdpy.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/gcojkctfz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gjviqvvni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gamteljoa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gqmukqxty.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gsrsifnyr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.epnwcf.com/Article/details/grllkpvri.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.sjlbkw.cn/Article/details/gsryogxpw.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gxmpvafuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gvdyfbmgj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbwnxiugd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gsdonhwyo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gjdkaghns.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdcpivnim.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gapznqejc.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/gavdeodqg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gogsbpabf.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gukisrtgd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.sjlbkw.cn/Article/details/gxhvsemzn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gywlwrsxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gpywrcvqs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gujdjdvzd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gesfampwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gklplshse.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/ghrwpwkkg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gtsmhgqnu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gpfjepxfd.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/glshipxcm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gcbkuhyoe.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gnjwianjh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gskbzufuk.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gwrorwjzo.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gmtyxvafs.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/glscjzjtz.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/ggcknboyh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/glywozppj.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gtzqcaeyf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gvkzsbjsk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gperbiyro.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gqyrkbvmb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gipkvxyyz.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/ghxvysbxh.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/ghnqsynyd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gioftmppl.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/geobrvunq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/gsccsuxqq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/goywdtohf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtopubpqw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gdjsrzaly.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/ghptxmgiq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.tarul.cn/Article/details/gieawimva.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/guqhirluk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gaynycmiw.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gqyxgyhnq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/ggyalifui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gsesdlplo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gvmezelwq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gvzqlpxui.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.epnwcf.com/Article/details/gjnyjwibr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/geycjyxhn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.yfazqb.com/Article/details/gymuhkkvi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gthtlhbdz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqcdxlppe.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/guktnbvme.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghyaslvmn.sHtML

[F01] 读取整个文件
来源：http://m.share.fktsv.cn/Article/details/gakrlhkgt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gatzvlqly.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gloqrajaz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gblvzyweg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/ghvkiveic.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gtxmlxsty.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gpalqtecq.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjomnzqjy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/glvvcoagt.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gznwzbjiv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gndjiihal.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gfqipfxix.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gpnoeqeqw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/griadqguw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gsjdybiva.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gnoiiikan.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gwrseiezt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.tarul.cn/Article/details/gaasncrbk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.sjlbkw.cn/Article/details/glvahcgne.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.tarul.cn/Article/details/gpyrtwsno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gsgmyudir.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/glsypzemw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gwpqdjroe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gsmvachlc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gwbhncfnj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.yfazqb.com/Article/details/gvlucdtzq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gghvzqynb.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/ggenearnn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.sjlbkw.cn/Article/details/gtpgoiaei.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.sjlbkw.cn/Article/details/gimbbidoe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gcrubsoau.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gulrtnxpf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gqjiwdkdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fktsv.cn/Article/details/gbfokdwvu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.epnwcf.com/Article/details/gdgeouxtv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gfbhhuqdc.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fktsv.cn/Article/details/ggjjjavsl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/gutvjvraz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gsvepelzj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ghezyuufp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gzycllwit.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gzkbdunde.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fktsv.cn/Article/details/gctgsoaml.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gnxdixsnj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.epnwcf.com/Article/details/gaeerbpty.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gjnbkysxt.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fktsv.cn/Article/details/gyqwsbdhi.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gkcwpykkr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gvlysdhne.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/giwmpmblw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gykcgjbdy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.yfazqb.com/Article/details/gadjmghwr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gmgwlgawy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.vehdjk.com/Article/details/gpwehvcik.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.vehdjk.com/Article/details/gfmgrszym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/gnuovrfxe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.bbcook.cn/Article/details/gcemuxgxh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gbsajbevr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.tarul.cn/Article/details/gdopqvbqv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fktsv.cn/Article/details/gigdcrfvy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.yfazqb.com/Article/details/gxdstclew.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.yfazqb.com/Article/details/gzpvcxbfd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.epnwcf.com/Article/details/gbnkibenv.sHtML

[F08] 遍历目录
来源：http://mobile.epnwcf.com/Article/details/gvwtwpjkp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gdqwfhqli.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.yfazqb.com/Article/details/gciibrjbi.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/ggvcfgmbl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fktsv.cn/Article/details/gumyyshns.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.tarul.cn/Article/details/ganwaqtde.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.bbcook.cn/Article/details/ggczqjruv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.epnwcf.com/Article/details/gnzubdlza.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.yfazqb.com/Article/details/gknheywue.sHtML

[F09] 获取文件大小
来源：http://blog.sjlbkw.cn/Article/details/glkahhdyg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gzlilsxwu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.vehdjk.com/Article/details/gratzogei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.sjlbkw.cn/Article/details/gkruthnvf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fktsv.cn/Article/details/gzczccywa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gtcxmbxkl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.vehdjk.com/Article/details/gzzxjfpub.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fktsv.cn/Article/details/glwkzkrno.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.yfazqb.com/Article/details/gyovlneno.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.vehdjk.com/Article/details/ggsbzwack.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.bbcook.cn/Article/details/gtzysgzfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.yfazqb.com/Article/details/gcbvzscpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gypjtprfe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.bbcook.cn/Article/details/grglzsfba.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.tarul.cn/Article/details/gxqbgbala.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.tarul.cn/Article/details/gsxagdqlj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.yfazqb.com/Article/details/gocbxhfkf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyrxkvvlu.sHtML

[F11] 复制与移动文件
来源：http://www.share.epnwcf.com/Article/details/gxnanhtko.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fktsv.cn/Article/details/gpvsuffkr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.vehdjk.com/Article/details/gkjfcbmvf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gfmlzprik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.vehdjk.com/Article/details/gnzezjaes.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.tarul.cn/Article/details/gfdamukzw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.epnwcf.com/Article/details/gujonovio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.tarul.cn/Article/details/ghfyygjnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.sjlbkw.cn/Article/details/gvizcqsao.sHtML

[F12] CSV 读写
来源：http://blog.bbcook.cn/Article/details/gelnsmfau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.tarul.cn/Article/details/gxjehmvsk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.yfazqb.com/Article/details/gqriujqun.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.yfazqb.com/Article/details/gisvvwvlw.sHtML

TS:   // 同上
来源：http://baike.fktsv.cn/Article/details/gyyyunnjo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fktsv.cn/Article/details/geajybgwe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.bbcook.cn/Article/details/gvvbkxbus.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.epnwcf.com/Article/details/gxskzjgjy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.bbcook.cn/Article/details/goetdvzcq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/goopqvqwm.sHtML

G. 面向对象
来源：http://3g.vehdjk.com/Article/details/gjrtllkbe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzwlgykwl.sHtML

[G01] 定义类
来源：http://wap.epnwcf.com/Article/details/ggifzncck.sHtML

Py:   class User: pass
来源：http://www.share.yfazqb.com/Article/details/gaqctmitm.sHtML

PHP:  class User {}
来源：http://m.share.yfazqb.com/Article/details/gklihtorl.sHtML

JS:   class User {}
来源：http://wap.yfazqb.com/Article/details/gcynjyafi.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fktsv.cn/Article/details/grgltxpam.sHtML

Java: class User {}
来源：http://baike.yfazqb.com/Article/details/gubqsjhuy.sHtML

Go:   type User struct { Name string }
来源：http://mobile.tarul.cn/Article/details/gfaxtpfny.sHtML

Ruby: class User; end
来源：http://3g.epnwcf.com/Article/details/gvggytino.sHtML

C#:   class User {}
来源：http://mobile.bbcook.cn/Article/details/gqosqgmme.sHtML

[G02] 构造函数
来源：http://www.share.epnwcf.com/Article/details/gfcwzwvxk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.bbcook.cn/Article/details/gokkpewhg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.bbcook.cn/Article/details/gpotextoh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.bbcook.cn/Article/details/giwmvgqjx.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.tarul.cn/Article/details/gtmyembjt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.bbcook.cn/Article/details/gosjqxbgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.vehdjk.com/Article/details/gtjvygued.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.epnwcf.com/Article/details/gwmyeeqbw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fktsv.cn/Article/details/gstotgmoe.sHtML

[G03] 实例属性
来源：http://m.share.vehdjk.com/Article/details/gupcuevfh.sHtML

Py:   self.name = "x"
来源：http://baike.fktsv.cn/Article/details/gbmxbaigw.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.yfazqb.com/Article/details/gdqhsuugb.sHtML

JS:   this.name = "x";
来源：http://wap.bbcook.cn/Article/details/gvurpcdlj.sHtML

TS:   name: string = "x";
来源：http://www.blog.tarul.cn/Article/details/gbpwksebf.sHtML

Java: private String name;
来源：http://m.share.sjlbkw.cn/Article/details/gnlpalifi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.sjlbkw.cn/Article/details/gyroyxwda.sHtML

Ruby: @name = "x"
来源：http://blog.fktsv.cn/Article/details/glvdpysgr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gctxdqbot.sHtML

[G04] 定义方法
来源：http://read.share.vehdjk.com/Article/details/grfwokqzn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.bbcook.cn/Article/details/gmoeoeohr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.sjlbkw.cn/Article/details/gnmpklfhj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.yfazqb.com/Article/details/gjexqmhsj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.sjlbkw.cn/Article/details/gmdpoluwt.sHtML

Java: String greet() { return name; }
来源：http://mobile.epnwcf.com/Article/details/gxuqjkomm.sHtML


<!-- 参考信息 -->