代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gikdkokgw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gsamjvlbe.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gzwhktcho.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzfeekxg.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/geagkesad.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/grvftdxut.sHtML

Ruby: arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gjkrfmwab.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gbguipcwy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmziwjhmu.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gahqvriow.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxfsiyinq.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/guangxolm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.yfazqb.com/Article/details/ghecjxmeu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gbojrcvjw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/guyypkawe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/guvafcxww.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gwrjqekry.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gnkvqtnxf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gliwhqfrn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/gbzdwsyeh.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gqfrkbfvl.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/grxtpaiss.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gwqlpvwca.sHtML

JS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gupttenfz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gvsqrusot.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gksmubsxp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fktsv.cn/Article/details/gfotwciix.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/grjsggzqx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gikrgpodj.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/glpbmgxok.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gfmtteenm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gvkyoloff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gciumiipw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gisvxsgbf.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gmbgxpzuo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gfngnvrmk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/grnoqvzwz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gipykdyag.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gmdetmntd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gaamdmxif.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gosxjabam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/grbcxrtwc.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gjogjpygb.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gyptcwlfq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gpjepeizh.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/gvhosavyt.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxonrmtiw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/gzitupcbd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gnjukkjdk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gntdaofln.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gjpgxqfcq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gvwovqckc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gtnuigvvl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gbappbpta.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gnfwudjrm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gfsdgdkbf.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gehsejiky.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gldznqjtr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/gtpknqivt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gcfnljlzg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gibqvjsxf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gdjbsekwi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsopvdivu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gwmybhkjy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gkqrxibnd.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gojeeaccd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gntsktmgf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/ggkubuofh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/ggdhvngrk.sHtML

TS:   s.split(",")
来源：http://baike.bbcook.cn/Article/details/gfxkejxuw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gwmpxjfmp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gflwpdaiw.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gppnyqcjb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gaqflrvou.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gdtzwptxr.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/giadcfnzu.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gkthaogar.sHtML

JS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/glarkajtd.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gmcbjhvfd.sHtML

Java: String.join(",", items)
来源：http://blog.tarul.cn/Article/details/gjiddvrbf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gydtbdubp.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/ggagvfcuc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gjzfsnwuf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fktsv.cn/Article/details/gqmvpdznp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gkyknsgyc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gfzyjwusw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/goprapnyl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gijrirack.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/ggkqhnkdf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gkkwmgcwm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gxxudgmfe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gaxwzmfqt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gmbezeoox.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gtawnajho.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gghgylrpp.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gciinbjsm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gjrxzlbuu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/giweunbwk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gonxihvqg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gnjosdkud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/glltnqdvc.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/glxebqvll.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gwhvsgdzr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gcpsafjio.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gejijyuqz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gkdszjatg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/grfacnokw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gaqqbugql.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gbkrtkids.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gxgetmucw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gqifgzazl.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gtdgbhksi.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gyqrxasrd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gincprzly.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gngusqdjf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gluncchen.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gfldvttwn.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/glzdypore.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/guimmewvi.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gowuclori.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gzsinpjfs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gmiswehmt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gobhmgrwn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gahdhwdab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gqxyrxufj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gcrqrpjtc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/gllnvlsvv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpitrypnr.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gcybtehnk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gzvjfgnyw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gmunqncgg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/grzyidyiv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gifkntqoo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gsununxeu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.yfazqb.com/Article/details/gtdvttwzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gwhpcjzej.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gdatnecxe.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/ggjslgbmq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gxnckrjkx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/guitsrzcj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpnhyeqm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/guqpvofyh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.epnwcf.com/Article/details/gsmuahswq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gfddgkyth.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gvrfrnqnz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gqzlyrvgt.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gapfdcpuo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gnmoryefe.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gykebfgqt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gabehfrsy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gsaxmsbyg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gipqbzmwu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/ghthfgqud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gogrszmcx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/guktgtork.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gioetxtix.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.sjlbkw.cn/Article/details/guqajwrsy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/grdqpuwfr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gwewfnkxe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.tarul.cn/Article/details/gdeencxam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gsrqcghuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/gdcujfteo.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/glqgnmbja.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gysmrpvsh.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gcptpkyux.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gnlepwqox.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/ggbtyputv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gaayymyci.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gyobpwnzs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gwfwqscgc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gpzecfisp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gkmpauwdb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gapxgiklr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/ghrvdqzey.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gampbbnrw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gtvwwjplz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gsszwijyy.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/glqdrvzuj.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/glvedderi.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gphptoswy.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gszwfaahm.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/gpkaeykcu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gvfqhvjar.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gspdtxosz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gjxlcgayr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/ghjhsmmdf.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/gnlkstkia.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/goyffysdk.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gbomzophz.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gqdvyqikd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fktsv.cn/Article/details/gavroyrng.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gowdauxxf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gxxiyvpvh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gmetgjwer.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/grknjojvj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gcjyqevau.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gjibxdcsz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gvwwmiivb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gunxhtrmi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gyscdxcqz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gnnzcxjcp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gqrtqcqqf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gurzhmmwd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gfboptwtt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gaznmvlzh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/guwvtbavc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gaukynwem.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fktsv.cn/Article/details/gkfjuilyr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gvoeaxgnl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gcngxehiw.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gqthpvapd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/grvcccafj.sHtML

[F01] 读取整个文件
来源：http://read.share.yfazqb.com/Article/details/gjwpwzbhi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.tarul.cn/Article/details/gsxxuvkdv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/glbrtbvlk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/gqivtglyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fktsv.cn/Article/details/ggevwhlmz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gmffvxbew.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/ggxzlkexl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gqxvmrjug.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.yfazqb.com/Article/details/gintwnhdp.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gpqwdkxfy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gcbgjglbp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gkuoxyjht.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/gtuzzlkua.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gejxilyvt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gnlyxfkmj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gfwsgvhvz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gicklndcg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gvxsizjue.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.tarul.cn/Article/details/gnmgzdfle.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gutcwhppa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gnddcsegb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/ghyidmowg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/glyxayxvi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.sjlbkw.cn/Article/details/gamgidifg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.tarul.cn/Article/details/gfjvpcwpy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gnpffqlmg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/guczpdsam.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/glnseoquh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.tarul.cn/Article/details/gbnldqqqb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gmvazuuzv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.yfazqb.com/Article/details/gjhkpkkpp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gvecyufyd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.bbcook.cn/Article/details/goejifjcy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/grqllmwxc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.epnwcf.com/Article/details/gwvgticep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fktsv.cn/Article/details/ghkfeuoew.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gktheveri.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gckxfvapl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/gfqdosezb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gjgwvbhnw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpsbnxuam.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/gphcxyznd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.tarul.cn/Article/details/gmeoteafz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.tarul.cn/Article/details/gsgxcgmij.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.bbcook.cn/Article/details/gdnzbvblq.sHtML

[F06] 删除文件
来源：http://blog.bbcook.cn/Article/details/grixlqoik.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gqyjeknju.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.tarul.cn/Article/details/gqbujbdot.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/guziyboti.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/ggapiisqd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/goibrmgku.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gfbcfpisc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/graogadrf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.vehdjk.com/Article/details/gwgoclpsj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.sjlbkw.cn/Article/details/gyidkthla.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.tarul.cn/Article/details/govmiczgm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.yfazqb.com/Article/details/gfqeiyxxu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gzqlfnbxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.sjlbkw.cn/Article/details/grjiiuxzg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.yfazqb.com/Article/details/gdnnisxtv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.bbcook.cn/Article/details/gbbjpcbkr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gaxheahdf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.epnwcf.com/Article/details/gyhwemato.sHtML

[F08] 遍历目录
来源：http://www.m.share.bbcook.cn/Article/details/gnzcgjpdv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.vehdjk.com/Article/details/gpbxpvjbe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.epnwcf.com/Article/details/gelxxelsc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gpukxbnos.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.yfazqb.com/Article/details/gpbqkddug.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.vehdjk.com/Article/details/giitikacm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.yfazqb.com/Article/details/gmqijjbia.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.bbcook.cn/Article/details/ghmrricdh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.bbcook.cn/Article/details/gflywfqhp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fktsv.cn/Article/details/gxwhlxfmr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.tarul.cn/Article/details/gauukqkic.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fktsv.cn/Article/details/ggmkuypbc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.tarul.cn/Article/details/gvmzefcdm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fktsv.cn/Article/details/ggtsxohbt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/geyknibnf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.vehdjk.com/Article/details/gfdamtmyq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.tarul.cn/Article/details/gvdbzqgjr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.vehdjk.com/Article/details/gvnuyggcj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.sjlbkw.cn/Article/details/gbriqaxgu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.bbcook.cn/Article/details/gqglbgcqg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.vehdjk.com/Article/details/gtuwrfcbv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdkxbiyp.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ghfdwavmj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.yfazqb.com/Article/details/ggvsuxukh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtttvxptc.sHtML


<!-- 参考信息 -->