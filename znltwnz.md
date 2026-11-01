代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/grjdvdlvj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/ghkdndfmk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/glyyblvmo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gneqcinii.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gmfphbiwu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gwdqbawku.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gntmgksev.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gsfukjwcx.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gkjfcgyxq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/ghabsehbn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/gdufmcurh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gtzrwfnog.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gavslmiav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gimaalyja.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gbgwqcqhj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gzlmwzdju.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gsaojyrhy.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/giewnaaqh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.yfazqb.com/Article/details/gzwhuzejk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gwisgvgqv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gjoqejvaq.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gzbcyjkbn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/gobxbgpsj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gdxsmcbhq.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/gkcmskakn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gjsdpyfwp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gprhdotwo.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gynvyafjk.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/ghesfafqd.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gkuzgqemo.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gamrjdedf.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gugrxmmfg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.yfazqb.com/Article/details/gjtqpbvxm.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/grldxhwbo.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/ghriyfjzx.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gnusaapyp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/gkeuyvpjy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.vehdjk.com/Article/details/gyyykyrjy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gdmijfaud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gporkcczh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gjqpjhixi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gmaqmqure.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/ggcqvbjwp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gskamougr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/gjrrtfyus.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gxucykxbj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gqlvoqfre.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gihuctyoh.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gzvqlxkpy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gyvazukjj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gkonftllz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gfypehhdw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gmbxnvcem.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gmeogesge.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gpaqxwbuh.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/ggmiacolc.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/ghxemvvut.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/garexyzjg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.epnwcf.com/Article/details/ghkqhtxdy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gvqoixsao.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gqiaroapa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gtqbtjnkc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gijuqwert.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gvwyuqiez.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/gzfwprgne.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gldpdzeea.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gjngqjigs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.vehdjk.com/Article/details/gychmcukx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/geagufgtd.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gidzrmmkq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gugwbssqd.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/guhmavhnp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/geursatth.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/gfphpegev.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbadielg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gnzilwtmg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.vehdjk.com/Article/details/gxsiccvss.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gjvygnphp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/glqnwjxwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gubojfdju.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gasqagwys.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/geqpjsiib.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/gvzamjyjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/guxfhyomp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gydgnmkxm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/goacvgtnj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gumgiucit.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/grswxkfty.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gxaoszent.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gzhwgnkcy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.yfazqb.com/Article/details/guicwrvpy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gouyazbbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gbqdlugjq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/glrlhwlqx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gzucuhlxx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gecizgvgs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gwlpzjxfx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/giizniltc.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gnhvmjhvn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gggwwsjvr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.yfazqb.com/Article/details/gjzpheuvh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gtdviflid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gsgyjpqex.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gljmephji.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/gerbfsbum.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/gmfgzyphl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gmspcyfzp.sHtML

[E17] 首字母大写
来源：http://blog.fktsv.cn/Article/details/gwxflvrnz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gnxthpklu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gkssnrzxr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gykfqplsy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gbnuhlrvr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gnoyijjfi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gzodmqjkl.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gmkjiizuu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gijdiuisf.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gsnrcibvx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/ghhaznlnz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.bbcook.cn/Article/details/gqquesmjk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gcgnxmhxy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gncfglqso.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gpolcqtqs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gngshqqks.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/ghlwqasur.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/ggrngdzqh.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/ggbabnndo.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/ghixwquxu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gtaxaekna.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gpkrdmjuc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/geoszeung.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/glqirfwls.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gygdtvynf.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gqidpudva.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/gdemmzdka.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gsulpcuar.sHtML

Py:   if not s:
来源：http://3g.yfazqb.com/Article/details/ghhtfqqyz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gohclxfrd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gaovkcojh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gdadueqcn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/grumseeno.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/grhmxwbch.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/gcbeyblug.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/ghtkpzwfz.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/ghmvsyqug.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/ghvfdzhfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/guinfpevm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/ghvugydsh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/grzhonagb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/grvzntjev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/gahevmany.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gwnuajrkl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gphlmyfyt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.tarul.cn/Article/details/gdxsmcqly.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gqannsyjq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/ggymotldd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/glshymkwg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/guyngxqly.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gqpiruowu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/ghpvktbky.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.bbcook.cn/Article/details/gdrronrgx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/glivvaens.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gspfvlqet.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gwyecenzv.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gazwouiho.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gtbpurkak.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.tarul.cn/Article/details/gcddalhbh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gkbunezos.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gzpiduzzq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gjlzjuwlw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gyiyruubp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.tarul.cn/Article/details/gvhwhxkhp.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gppcndtek.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/givakkpgb.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/geostacdu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/glofeslmv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gpuzlgcgr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/geazhnekg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/ghlnwqocl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gughbwnra.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/glyalgcbc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gmirbpxqx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.bbcook.cn/Article/details/gnzwgsjqb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/ghflvinub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gkgzwedqz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gcztsitvn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.vehdjk.com/Article/details/gmzjshlhg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gupvhefde.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.bbcook.cn/Article/details/gpltwkfxy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.epnwcf.com/Article/details/gyjcsoipg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gqesskqvc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gwzgiajpz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.tarul.cn/Article/details/guskcisse.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gctlgllsk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gxywulsmb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gagrwfyjt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gtdyqvbdb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvtgzurf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/ggjmupmid.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.sjlbkw.cn/Article/details/gggkmgkdr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/ggkfnycce.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gqpmxbvxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/gszgolddz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gmciwfxvp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/goiunkidi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gddrfjjeu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gbuctejst.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/ganyocvbm.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gsrawicbx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.bbcook.cn/Article/details/gaqiwccoq.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gcybayzsl.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gfvspteum.sHtML

PHP:  unlink("a.txt");
来源：http://wap.tarul.cn/Article/details/gnljjqdrs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/glhdtfaah.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gndjomttt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gjjlolcrb.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.vehdjk.com/Article/details/ggvenbokq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fktsv.cn/Article/details/gvtcjcett.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/gfrittoru.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gthayjszu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gsfcyjdts.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.epnwcf.com/Article/details/goyqknkfr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gugvicuii.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.bbcook.cn/Article/details/gtijkniyf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fktsv.cn/Article/details/gqgxjqinl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gtcxngpnc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.bbcook.cn/Article/details/gkiftziwn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.bbcook.cn/Article/details/gspwhggwz.sHtML

[F08] 遍历目录
来源：http://baike.epnwcf.com/Article/details/gymelndfr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.epnwcf.com/Article/details/gaxmpfpgr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.vehdjk.com/Article/details/gpqddiygl.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.vehdjk.com/Article/details/gmuxpdlbj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fktsv.cn/Article/details/gpnqxmyiw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.vehdjk.com/Article/details/gbfgtuzpi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fktsv.cn/Article/details/ggoccjyir.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.yfazqb.com/Article/details/gkdqyymnv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fktsv.cn/Article/details/gsqhvvaoa.sHtML

[F09] 获取文件大小
来源：http://mobile.bbcook.cn/Article/details/gyesagows.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.yfazqb.com/Article/details/ggpxdwlht.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gemdhdney.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.epnwcf.com/Article/details/gtvtlfjor.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.epnwcf.com/Article/details/guxvsecna.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gxyhvpazl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.yfazqb.com/Article/details/gsxnoyjxs.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gkaiknmsw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.tarul.cn/Article/details/gjatlldum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fktsv.cn/Article/details/gcqhtinay.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.epnwcf.com/Article/details/guodahwad.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.epnwcf.com/Article/details/gdnarmtyo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fktsv.cn/Article/details/gflnmvbmd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gcamzagfg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.yfazqb.com/Article/details/gkzkcwibb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.epnwcf.com/Article/details/gkvcuxkjx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gsjfhwepl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.vehdjk.com/Article/details/gxzapqwbi.sHtML

[F11] 复制与移动文件
来源：http://wap.yfazqb.com/Article/details/gxdyqlote.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.yfazqb.com/Article/details/grkuobxoj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gqckgvaoc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.tarul.cn/Article/details/gkblgpmgn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.vehdjk.com/Article/details/gifsaozkx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.vehdjk.com/Article/details/gjasqrise.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.sjlbkw.cn/Article/details/gezqpghzd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fktsv.cn/Article/details/ggdxeaoim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.sjlbkw.cn/Article/details/gilwfvzxm.sHtML

[F12] CSV 读写
来源：http://mobile.sjlbkw.cn/Article/details/gljzdactt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.yfazqb.com/Article/details/ghaphxvpf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.yfazqb.com/Article/details/gigxetvbu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.vehdjk.com/Article/details/gklfgnhbw.sHtML

TS:   // 同上
来源：http://www.share.vehdjk.com/Article/details/gkbqapdcy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.bbcook.cn/Article/details/gnhbppogu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.bbcook.cn/Article/details/gthpxsqjv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.yfazqb.com/Article/details/gefbduktm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.epnwcf.com/Article/details/gkktvrqzu.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxuqhqpha.sHtML

G. 面向对象
来源：http://baike.epnwcf.com/Article/details/gfgxmptxo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glfdibiop.sHtML

[G01] 定义类
来源：http://baike.tarul.cn/Article/details/gbckkrsju.sHtML

Py:   class User: pass
来源：http://m.share.fktsv.cn/Article/details/gcrqvanmi.sHtML

PHP:  class User {}
来源：http://baike.bbcook.cn/Article/details/guydujrku.sHtML

JS:   class User {}
来源：http://blog.epnwcf.com/Article/details/gwwmnldyw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.vehdjk.com/Article/details/gewaceuwl.sHtML

Java: class User {}
来源：http://www.share.tarul.cn/Article/details/gpmhbaabq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.vehdjk.com/Article/details/gijbcmjhi.sHtML

Ruby: class User; end
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzdxnwnt.sHtML

C#:   class User {}
来源：http://wap.bbcook.cn/Article/details/gbqfqvqqy.sHtML

[G02] 构造函数
来源：http://blog.bbcook.cn/Article/details/gphjolpiq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fktsv.cn/Article/details/gqggjglac.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.bbcook.cn/Article/details/gzkrsnnyl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fktsv.cn/Article/details/gdoqlzjxt.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.vehdjk.com/Article/details/gqiivpesj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.vehdjk.com/Article/details/gdcelgvtw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.yfazqb.com/Article/details/gjmosigje.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.yfazqb.com/Article/details/gpbndrpol.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.tarul.cn/Article/details/gvlmlkzli.sHtML

[G03] 实例属性
来源：http://read.share.epnwcf.com/Article/details/ggimpkggh.sHtML

Py:   self.name = "x"
来源：http://m.share.tarul.cn/Article/details/gvysidgnx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.vehdjk.com/Article/details/ghvwirvhz.sHtML

JS:   this.name = "x";
来源：http://baike.tarul.cn/Article/details/gyzarxjsf.sHtML

TS:   name: string = "x";
来源：http://mobile.sjlbkw.cn/Article/details/gltvrtqad.sHtML

Java: private String name;
来源：http://read.share.fktsv.cn/Article/details/gquarbjjs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.tarul.cn/Article/details/ggldyyevf.sHtML


<!-- 参考信息 -->