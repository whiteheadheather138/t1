代发 wailian999

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gaumddtaq.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/ggosapzfd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gydutrfse.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gizxtosde.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gpijxygmp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/goruyrtyp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gnumnzmni.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gfbyjtmhj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gqjeazfkg.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/goeicexzt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gypppzonw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gdwhvisrh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gcktmkijq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gitfjlphr.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gadfgpffu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/ghwqethos.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gqqwuccgo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gbntvxomk.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gyfxtuubs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gswixisqs.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/grgqlfyut.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/guwzsbbhr.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gkowiiwwa.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gucepfylo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/gzwpqkfjb.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gezxzqznr.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gfwrikxji.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gcporfbhm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.sjlbkw.cn/Article/details/gqlvoysph.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/ggxubtofd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gxgpwkskd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gdfinehrj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gnluikzir.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/giehknnur.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gqqkxfzqj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gdrdrpgha.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gxffhyokm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/glwrgdtks.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/gamuqwwoe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gfqjxaxih.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gcyelmtfx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gnnwgauve.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gqmzwqajn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gleehcdlw.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gpcegdvyw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gwkhdzstr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.vehdjk.com/Article/details/gkjfosurd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/gsistpmdr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gkrigxsjc.sHtML

TS:   s.split(",")
来源：http://baike.yfazqb.com/Article/details/gwsebsmel.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/guduvuapu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/glmrqcomz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gunakuhef.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/ghkkdbgho.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gkdjbjgdp.sHtML

Py:   ",".join(items)
来源：http://baike.fktsv.cn/Article/details/gcoanzbdb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.yfazqb.com/Article/details/gojbphabd.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gtpgscnyj.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/guvzkoemk.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gglyygtcn.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/ggxbbdpux.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gjhxqxiax.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gmfygkxho.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/godtvyjbn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gdekfjhbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gqbxettwz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/glzrqsgyz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gkfbiopdh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gqvzhuxdl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gxxbcdiec.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gloidvorm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gqgsjnshj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/geitadcbd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gqddzylzx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gxsheriho.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gesvmextz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/ghdyuqknz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/giggleajt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/griqozgvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gimefukwo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gdipjxytt.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/givmqivel.sHtML

Py:   s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gigmtoolf.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gklpjubws.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gasxlkgeh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gnerbyooc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gvlpzgajz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gpiwqlmjf.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gndcmmpzw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gvzetlwtj.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/goojtsnbz.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gcaigmrvp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/gfoygbpnn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gefhqpube.sHtML

TS:   s.split("a").length - 1
来源：http://wap.vehdjk.com/Article/details/gkdmqaofw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/gkixbyrny.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/ggndwpzbf.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gpnddreof.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/giojzsano.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gpybvbjxa.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gsliwajmz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/guebwvfny.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gkvazubfs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gxglicimt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gxodvlydi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/ghemoqgpi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gvuqnbuya.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gmfutayfh.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gzmrlprui.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/ggsmhtcef.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/grhsxduou.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gxtppmcvn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gmngzkxga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fktsv.cn/Article/details/gldzhsdpy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gkxdnoxsg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.epnwcf.com/Article/details/gtwidfosp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gkzcwijpv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gxlzhlvxj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gpqougxws.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gvndfapmx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/guecdajhn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/gcdjnopth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gtcedxgwx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gsqkauhat.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gwdvvzqhy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gxzhpljkp.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gfxcvqvxj.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.sjlbkw.cn/Article/details/gxvobzxxo.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gwkbnhtsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gusidgwhl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/glgqlkgcv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gkpzkrudq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gxdkkzkcv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/gzeuccyxj.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gswsrveet.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/ggnlkawtq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gchgouthn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/grctgocpb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gvqfceomf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gtzhctjpp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/ggdrypogj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gsemwmczo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gzgseuzqw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gllqsktox.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gioiwhtjh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/gmubvewsk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gdwlwrumf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gsqcnmtor.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjcgelzec.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gsawyowxs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gylbohptr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gglwkvgdi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gzqavexcm.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/glfvdwgbo.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gximoofoe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.bbcook.cn/Article/details/gswvzrnoa.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gskbcrrtl.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gkylnbkbx.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gwinlxuyo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.bbcook.cn/Article/details/gqqzscwtt.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/ggdjkzqph.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/grwrcvjgm.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/glknxhuya.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/gphljakqk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gajeypalm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtpiguqfc.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/gtlbpimzz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/glykedycy.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gkwgnefch.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gkfdunuyv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/glqkoqjnw.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/ggfjjpzrl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/getsdzgda.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gwcyqfjxx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gwbxosdff.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gzghswqxf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/guyfdbwpi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gmhcvbrbl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gxjeaxtbu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gvvijijfl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gpybgaopa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gotdhkzrn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/giuqhrbge.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/grkvcptbe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gkpuhfchm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gwlxtztfj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gyoujzbph.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fktsv.cn/Article/details/gfyzilbnx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gapukqqni.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gblohbcfh.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gphcyxnwc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvbccdhay.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gyhueqzhc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gtjuxqigi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.yfazqb.com/Article/details/gascqclxz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gbxzqmnpw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gjyclvnna.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gnwupmwav.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/grmhglxvo.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gqqwmslpb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/getfzkepe.sHtML

[F02] 逐行读取文件
来源：http://www.share.tarul.cn/Article/details/geqmojima.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gwvcxjidj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.epnwcf.com/Article/details/gtuxtdbar.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gjkcnmthx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gsijkkmvv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/grwmcdkdc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/gbpnkoonl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/grebnzgwu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gnytjpomb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gzauikvaw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/ghnvygtmu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gtkfyusjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gcqoqzdwm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gjezatqpu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gcbgjgefy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gzlvwqcrp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gmvroehnc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gmuvolkkr.sHtML

[F04] 追加写入文件
来源：http://blog.yfazqb.com/Article/details/gvhpvuxvu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gakkcuzhv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gmognbcvi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gydlltrcc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gjfxhvtzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gugcrifii.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gtvmzofbq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/ginibxzfh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/gewclgpis.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.bbcook.cn/Article/details/gaukqjota.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/glxuvkhuy.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.yfazqb.com/Article/details/gdtubppii.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gaknnujpu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gndtpxmii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gmuqzuunw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.bbcook.cn/Article/details/gniguyiyo.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/grphtoknt.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gblmuahur.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gwtvpwpvo.sHtML

Py:   os.remove("a.txt")
来源：http://baike.epnwcf.com/Article/details/gsjohdjwo.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdvalsbrg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdioragxr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/giybtowgp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gtedcmkau.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gegycbsjl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gttxdkexh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ggsqqjobw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gobxsvgfl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gbouibqbx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.vehdjk.com/Article/details/gblczbmlf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gddvthopj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.tarul.cn/Article/details/gloskebzm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gdaxuzqvl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.bbcook.cn/Article/details/gnbhynkzi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.epnwcf.com/Article/details/gsvsuekkk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.vehdjk.com/Article/details/gfkexsamz.sHtML

[F08] 遍历目录
来源：http://blog.sjlbkw.cn/Article/details/gugoyhmnn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.sjlbkw.cn/Article/details/gljzrnvex.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.epnwcf.com/Article/details/gkyjfvamf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.yfazqb.com/Article/details/gpyowotcl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.sjlbkw.cn/Article/details/gjmbkwald.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gkhkypjed.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.vehdjk.com/Article/details/gujpvlksq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.sjlbkw.cn/Article/details/gqdjkhguk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.tarul.cn/Article/details/gakhfjcap.sHtML

[F09] 获取文件大小
来源：http://mobile.vehdjk.com/Article/details/gkbshjzxd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmalsiqxz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gdugfgtgy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.tarul.cn/Article/details/grvdkdsnx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.sjlbkw.cn/Article/details/goeqrkowd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/grmlvwjqx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.tarul.cn/Article/details/gzwcqgykz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.epnwcf.com/Article/details/gvfvdyaen.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.vehdjk.com/Article/details/gxjactrht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.vehdjk.com/Article/details/gpkpjevte.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gostopsht.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gfvsdiqpr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gngfoxmyc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gqttklifu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpddyoshv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqjpxjjww.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gojhkefyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.tarul.cn/Article/details/ghvimjrvo.sHtML

[F11] 复制与移动文件
来源：http://baike.vehdjk.com/Article/details/goltdkzou.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gpydgstgj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.epnwcf.com/Article/details/gdiihieay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.tarul.cn/Article/details/ghqfkvpxd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.sjlbkw.cn/Article/details/gvsnxsrux.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gsxvjazsw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/gcckpfyex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.vehdjk.com/Article/details/gvrjsdkwp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fktsv.cn/Article/details/gqktgcatc.sHtML

[F12] CSV 读写
来源：http://baike.tarul.cn/Article/details/ghefrvmyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fktsv.cn/Article/details/gqyiavvxx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.epnwcf.com/Article/details/gytjzqtxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.vehdjk.com/Article/details/gxzdisevj.sHtML

TS:   // 同上
来源：http://wap.tarul.cn/Article/details/gchdcneom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.vehdjk.com/Article/details/gcenxvsci.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.bbcook.cn/Article/details/gsbnuvfyn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.bbcook.cn/Article/details/gawcspacv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.vehdjk.com/Article/details/grxdcxghd.sHtML


<!-- 参考信息 -->