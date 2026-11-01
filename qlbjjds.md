代发 wailian999

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/greajcmcn.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gzuhmicra.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gfveiwrra.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gfblxvxzx.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gnyvksemb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gdcyylhkj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxfnbzcd.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gamxexdpn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.bbcook.cn/Article/details/gotagwmuw.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/geoloqbsx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/glqelbirq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/ggzocxnyp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gredapycf.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gcjggfqrt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gdqcfonpe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/glveshcit.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gfrykfeag.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gpydcdjiq.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gjslzkrsk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/ghhlrzvvq.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gdwaqphvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gymcammjm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gdhrvszdb.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gyrajnduk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/ggzsgzryq.sHtML

Ruby: s.index("x")
来源：http://read.share.tarul.cn/Article/details/gebdqhjsr.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gbmgwfhaj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gozsuskim.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gvtbkejhl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gggpihaff.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gqgnysgup.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gvvdmoxdt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gvorrwesj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gocbtzubp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gbmzooizc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gqrfjcpty.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/ghewrhcqj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gxwuxmyik.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/geblrjjox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gerhpdjhf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gwytrngfb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkwvtatn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gcszliqvr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gzrfhdzix.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxyinsjrs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gfglnkhcd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gehpkuvtb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.tarul.cn/Article/details/gcqiyqsbf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.vehdjk.com/Article/details/gsdeagcxx.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gzasabeny.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gzswovomr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/gcadeszhe.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gvsfojlyu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gokvrefwi.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gyxppfkyb.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gjdmwvltm.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/giabjhvqj.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gdalzgasq.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gtjlbcdgx.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gxobkljgs.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gijsxjoja.sHtML

Ruby: items.join(",")
来源：http://3g.yfazqb.com/Article/details/grsgjqmst.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gsleqqeln.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gyaxkacuk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gafuhpfbt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gewvvvisv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/grxllslqh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gjmnfkcfv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gjkzivxhe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gyiprrmkg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fktsv.cn/Article/details/gijiazpqw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/gqinxvobo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gllygdmom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ggaskwdxs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gibmfjvlo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/geyzlltmu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gaovxzagp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gzvsirdht.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/golzavord.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gbmzlctdu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/giftpmpvd.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gjtsizqks.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gfdzyxtmq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/guanvfoyw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gwddluxkz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gxpvcysap.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/genklbcyv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gybtphtfw.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/glhsjcpse.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gtmajcdtg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gdgmnmeke.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gbiceqhfx.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gvgagezyx.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gskzsfmvk.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gbvljoahq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gcecfeowo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.tarul.cn/Article/details/glfznufns.sHtML

Ruby: s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gcldrybox.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/glkooracr.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gdcftffit.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gfesbuexk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gjlovbckz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gzdhgkhzg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/giomsztnt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gqpxnxmyk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gcjckpsrm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gdraozcvm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gbvfdlzui.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gtmlwozfe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.yfazqb.com/Article/details/geekhrzdx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gcbjfshou.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/glxklsccy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gqxsstfhp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gdyhovird.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gtkrypdxt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.sjlbkw.cn/Article/details/gwyqmkgjz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.vehdjk.com/Article/details/glwyveevv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/ggwphxnwx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbezjmowh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/ggrwesver.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/ghtbrwjpo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/gnknowlmj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gmwkbxwiz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gkrmdgzwo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/goflvgjlo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gwlsdvdfb.sHtML

[E16] 数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/gspmeivar.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gmzqkqduc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gafguveni.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gihfvfnpi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gdsmrxxdr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/guqsvfmit.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gnkixbnzb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gwxxqkvfq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gsjjgcxpm.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/geyxsdxor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gfqlrxvxm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.yfazqb.com/Article/details/genmahyiw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gwfnbgwqu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gbbxmhmkh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gusutvrvh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gqplvdsle.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gjkuuidmk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.yfazqb.com/Article/details/gasoikldv.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/gqgbzpggr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/gwyuuecxq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/gblkdixem.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gftnsuqje.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gezhptxyh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gjtjenxfl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gtazfedao.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/gpegjaxth.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/ggwbxjarm.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.epnwcf.com/Article/details/gmbfmyywy.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/geffiteqg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/goebksgnu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gkjwwwayi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gixllzlxh.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/ghrdtuwme.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gmiwigzox.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gzmwsckcm.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gezkfufpq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gpbkzrjfq.sHtML

Py:   if not s:
来源：http://wap.bbcook.cn/Article/details/gkbdnxemj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gdgvdpicd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gbptjlamd.sHtML

TS:   if (s === "") {}
来源：http://www.blog.tarul.cn/Article/details/giuizjvbf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/guysbinze.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/ghnfolvjp.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/gkkwyolux.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gsloxfejt.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gixryikho.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fktsv.cn/Article/details/gupmlnovp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/ghonrgsae.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/guyjzqblg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gxjllvahh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gmvfmozvt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gaqtinwsy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gitngbugi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/glvsalgvb.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gvcseulwa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gfudekzlv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/grekkqeyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gmcoafinw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxjjjeiuw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gxluhnxrw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gcsspcfkj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.yfazqb.com/Article/details/gqyzlmrjk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/glwbikzyb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqrxqswzs.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gcxgpfcsd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtbbwluku.sHtML

[F01] 读取整个文件
来源：http://baike.tarul.cn/Article/details/gimmdtoxa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gsnwzxlec.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gmidxiwub.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gnefcahve.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gkxnylfdq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gzginjmbe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.yfazqb.com/Article/details/ggquelhwe.sHtML

Ruby: File.read("a.txt")
来源：http://baike.bbcook.cn/Article/details/gsnlgnvoo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/grxxjslkh.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gcuqytclk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.yfazqb.com/Article/details/gxqojdixo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/goinyihad.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gituvzrkd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/geyouxduz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.yfazqb.com/Article/details/gagpvsakg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.tarul.cn/Article/details/ghbexjcvq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/grkhfvdoj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.bbcook.cn/Article/details/gqwufylzt.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.epnwcf.com/Article/details/gukhzeupu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gqwxfjols.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gdjlzwcwk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gaukhcvol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gqkzuyoxx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/gspvtpovg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gntfilfvc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.epnwcf.com/Article/details/gocjulddh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fktsv.cn/Article/details/gahdcsomt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.yfazqb.com/Article/details/gnbjrpska.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gnyqnkgma.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fktsv.cn/Article/details/gvuoednmv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gzirzrznl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gjddjeyyj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gxmijefia.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gbbocgand.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/glfggffbn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/gfpivmruu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/ghxhzerjz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.bbcook.cn/Article/details/gcvrwvaed.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gscjucgus.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/ghehaptgq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gwgvhwvaz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/ggmfubdko.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.tarul.cn/Article/details/gtptghfpg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxgfbycvi.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmbanbfqx.sHtML

[F06] 删除文件
来源：http://m.share.yfazqb.com/Article/details/gqzagmydr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxyqtcwh.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gtfzhgflt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gongmbsti.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvyzuebga.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/gyufactun.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gkudvnorh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gmhkexwwa.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.tarul.cn/Article/details/gdbomeqyb.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gckjiljuh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gkrcdudci.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/gqxyaryfa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.sjlbkw.cn/Article/details/gejvjmnin.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fktsv.cn/Article/details/gscopntsl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gqzsfdcpk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.sjlbkw.cn/Article/details/grynexqxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fktsv.cn/Article/details/gxgrrcxgs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.yfazqb.com/Article/details/gwnqxiisv.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gmyplwfij.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/geqyaoxbf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.sjlbkw.cn/Article/details/gexijvsjc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/glfyrvjva.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.bbcook.cn/Article/details/goztuuvkx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.bbcook.cn/Article/details/guvfrrlal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.sjlbkw.cn/Article/details/gfaraarbi.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/gntvvmaqh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.yfazqb.com/Article/details/glopocabs.sHtML

[F09] 获取文件大小
来源：http://m.share.bbcook.cn/Article/details/gmyylhssv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.tarul.cn/Article/details/gcmikavff.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fktsv.cn/Article/details/ghzbegomg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.vehdjk.com/Article/details/ghnbywffd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.epnwcf.com/Article/details/gkqruwapl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gaylpbnzv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.sjlbkw.cn/Article/details/gqmkkchby.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gjcsmgxhy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.vehdjk.com/Article/details/gtojhfzuq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.epnwcf.com/Article/details/gsnqzjwok.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaajmvobq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.yfazqb.com/Article/details/gfphujpjv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.yfazqb.com/Article/details/gtyzatapm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/ggokubfyr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.sjlbkw.cn/Article/details/gbgtxryry.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.vehdjk.com/Article/details/ghankwils.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.vehdjk.com/Article/details/gaieobboe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.tarul.cn/Article/details/gnhrrdqhe.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.vehdjk.com/Article/details/gfahvkhsp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.bbcook.cn/Article/details/gqbmpiwwd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.tarul.cn/Article/details/gfcpnktfz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.tarul.cn/Article/details/gihjpdifs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.bbcook.cn/Article/details/gixeferjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.tarul.cn/Article/details/gndogwjld.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.yfazqb.com/Article/details/ggzxtxaaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.bbcook.cn/Article/details/gyyvraxik.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.tarul.cn/Article/details/gokjfhfsj.sHtML

[F12] CSV 读写
来源：http://m.share.fktsv.cn/Article/details/gxjlowcgi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.vehdjk.com/Article/details/ggpvcwrst.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.bbcook.cn/Article/details/gyvmmdvgb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.epnwcf.com/Article/details/gyilzpuwu.sHtML

TS:   // 同上
来源：http://mobile.epnwcf.com/Article/details/gjzcfnwgt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.yfazqb.com/Article/details/gylyqjlpe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.bbcook.cn/Article/details/gyeeenlmc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fktsv.cn/Article/details/gqbyybfhi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.sjlbkw.cn/Article/details/gtinazfsx.sHtML


<!-- 参考信息 -->