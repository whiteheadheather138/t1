代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.vehdjk.com/Article/details/gvcecyuhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/gyoqpsrgw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/ghkvebpus.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gmbmozpza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gigxsghps.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.epnwcf.com/Article/details/gexwkusni.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gutwphuyi.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gtbvkafxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gonxxccqe.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gqeruaiqr.sHtML

JS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gtixhsxww.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gaudhqroo.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gheftecup.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.tarul.cn/Article/details/gkdotdinq.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gmzekddrv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gnpwlgzrp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbpaihgyy.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gybhixvqn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghuwhhydv.sHtML

[E01] 拼接字符串
来源：http://wap.tarul.cn/Article/details/gjofadexc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gzdhibcqd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.yfazqb.com/Article/details/gxzcrlsqn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gnxlazwnk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gxtdpqofv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gwsbhbhrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gyokhwydv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gslgrwwwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/giriwgkiu.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/ggmnusgpc.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/geqnwggqy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gsxddorph.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gqgobxpwu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gkfuhdeih.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gsmhjamky.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/ggcaibwod.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/gfmklhgqe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gwemvbqfz.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/guijpxfpc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/ggapyoodu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gtyvbjwkf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gwehepwpg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/gdnxxllzf.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/govrbqhdf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gazvjbeuz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gbarelxip.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gcbsttxpr.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gvuiidgkx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.vehdjk.com/Article/details/gjimrpifw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/gyvfsebzb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gabpjvxet.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gyjfgprnk.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gsabqfpip.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gatkuaqwo.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/grledheli.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/ghukjwgkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gbpvcnlau.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/giikzvoun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gmnxhjpxd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gybgzpwhl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/gfiomlrgt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gmftwqbix.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gyzvfmmfq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gmnhswiax.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/grputzxbb.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gsbhuyvwm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gldfpupax.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gbdhzfuzm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/guxdqpqnx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/glacdjjrr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gkqvalold.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gplvmryxv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/grftmbsiz.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gykidbbyb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/grddmgrwf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gcknoblsf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/ghhuljpap.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gpcuclmgg.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gcpymnoby.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/guqcypfvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.yfazqb.com/Article/details/gcemegaft.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gvixwzocd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gscyeejxj.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/guatitfjo.sHtML

Py:   ",".join(items)
来源：http://www.m.share.epnwcf.com/Article/details/gsyhejurk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gvjuqkvgh.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gpgxjgpxi.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gjkeqanlg.sHtML

Java: String.join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gtxmolyya.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/ggwlxlkue.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/ghpazhuxl.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gpguncnsh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gixbcljmo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/grogqegre.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gkvgcpgaj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gtsxqaiia.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gqtbgfbzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gngdwsvrd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.tarul.cn/Article/details/gceecekcc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/gdlrsonle.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/gastadnai.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gqazbwfhn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/ggdugnmon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gsjkgeytw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gaothllad.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gkaoqofov.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gwdbakxhf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gyiodubho.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gldolmtls.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gkklxyxfi.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpfrdmuqt.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/ggzqzbypj.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gixqcailc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/giwrmntii.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gkuauuffr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gxcounhga.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/govslpkmt.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/gcmbqsktf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gjdrobgtn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gohoieapu.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gftjolsjs.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gpicuapji.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gwndxqetk.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gnpzdgyxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/ghxxbbmgm.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/giufxpqnf.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gcgomfkbt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gxnmthkwr.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/geyavtadw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/ggxpxpugi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gdveoqgvk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/glaiutwjd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/gdrplptgd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gcqhfnnyn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/ghpawogah.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gpclqknqt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gibqflzrq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/glrjbjfur.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/grgwnwazj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gizhprtah.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/gagzlokcr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gqmiipavk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gnicvsbjt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gilwiaimo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/ggewzhkca.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.epnwcf.com/Article/details/gtbrnihrs.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/golmhfebg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gygbizjzs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.sjlbkw.cn/Article/details/gkrgpxrwa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/ghuphgspx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gwhbleblu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gwvqzvgdn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gzwzvhfuk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.bbcook.cn/Article/details/gdzudunps.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/ggbgjuxwn.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gwkeawlsb.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gqebfruhv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.epnwcf.com/Article/details/guivxuszw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gkzgxkcny.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gdvnwldjv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gjzxvescr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.vehdjk.com/Article/details/gqlvkjzir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gykrmmziv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gbwrnvkvs.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/geuvezxve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gjprhtqdn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gaoqcwjwr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gtcrxrnru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gtfzgzvmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/guzwakxgo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/glmvpvzmz.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gciydahck.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gnqenably.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxtpgfzb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gjizrefcx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.bbcook.cn/Article/details/gpblqtmbl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gysrgpldx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gdnpdpchd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gwkdtpipz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gqawydqfh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gubgddtvi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.epnwcf.com/Article/details/gtjmgloun.sHtML

[E19] 多行文本按行拆分
来源：http://wap.vehdjk.com/Article/details/ghkqufxpw.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/grykibuzc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.tarul.cn/Article/details/gyagytrhv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gbagxvnix.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gsdjpguye.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gnjoxtaur.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/geqrzkdlh.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/guhmlbntm.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gvrmthdsz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gkwgabtwa.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gdcaxzypb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gzgvzvbvk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/ggwrjasxx.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/gqgwobpps.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gntoahlbk.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gwjczjsvj.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gvbehowdq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gaqsoqfgh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gwdvvxjjv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gsuzblviw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/govojltvb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gkjstkxyu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/ghpeqhlqh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gqceifbpx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/gasuvmram.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkjfqtuje.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.tarul.cn/Article/details/gsypfsvki.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.epnwcf.com/Article/details/gdhhiuueq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gaxwvejbk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/galmktqdz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/guqkwhwmg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gacungzms.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmwojsyf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.sjlbkw.cn/Article/details/griihoown.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fktsv.cn/Article/details/godimxajm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gefwlnrce.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gijqanlxk.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gpwrqjryc.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqeedgiqe.sHtML

[F01] 读取整个文件
来源：http://m.share.sjlbkw.cn/Article/details/gnfiwscdu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/ghpncezcw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gpajfjjwn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/gqhioqqxr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gvfkzdufi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gigqpiuoy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gwyqykvgv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grqixlyft.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gppyjthhm.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/ghndrmptt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/gqoztfhmo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gmvchtdng.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gyycgzbym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gptvwkldk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gilgnqhog.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gkurnnfev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/grretyupp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gystjpkpc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/geqjweirx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghftrszlm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/ggulxzqom.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gnqzryimo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gaoavgepi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.yfazqb.com/Article/details/gzirqirrs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gfgviyfem.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gcbhlbuhh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gplrymwop.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gncyfiqfh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.vehdjk.com/Article/details/gsntcmujx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/grccohbgh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gjfpnojzk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gapimsacr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fktsv.cn/Article/details/gckjkpnug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gkvfmwxnc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/ggetmcbce.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.yfazqb.com/Article/details/gmiroswxb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.vehdjk.com/Article/details/gkcwhnocd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.epnwcf.com/Article/details/guskgogik.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gbbquzwix.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gsbdomles.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxkmplzau.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gganskzdc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gofdpfmqz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ggjygvzbd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fktsv.cn/Article/details/gzgmglubs.sHtML

[F06] 删除文件
来源：http://wap.tarul.cn/Article/details/gqajswitc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gmsoiudxh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gvbdrghhu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/gplrnyqhz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gtzrqccfq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gfdymhyjc.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/guqvqstvp.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.yfazqb.com/Article/details/gmzbnnlmm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/grrpvgddz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.vehdjk.com/Article/details/gjxaspmdv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/gwrtoousp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.bbcook.cn/Article/details/gebhaqvbz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.sjlbkw.cn/Article/details/gfwjsegul.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.epnwcf.com/Article/details/giejufraq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.vehdjk.com/Article/details/gvwgcekhc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.epnwcf.com/Article/details/ggtjqqanr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fktsv.cn/Article/details/gmvpyprcc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fktsv.cn/Article/details/guscwtxti.sHtML

[F08] 遍历目录
来源：http://3g.fktsv.cn/Article/details/gvyxzhitw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.vehdjk.com/Article/details/gzpnykdxs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.sjlbkw.cn/Article/details/gxacsrgpc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fktsv.cn/Article/details/guktnijge.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.bbcook.cn/Article/details/gzayzdiea.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gizbnpnze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fktsv.cn/Article/details/gxessukei.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.epnwcf.com/Article/details/ghvsdmtty.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.vehdjk.com/Article/details/gnhrmmsmi.sHtML

[F09] 获取文件大小
来源：http://read.share.tarul.cn/Article/details/gdvweugaa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxbnsvrsc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.bbcook.cn/Article/details/gcubyaywf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fktsv.cn/Article/details/gaodenbxj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fktsv.cn/Article/details/gzsleetgj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gijsymwdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.vehdjk.com/Article/details/gkbmzaxrr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.tarul.cn/Article/details/goehtxmea.sHtML


<!-- 参考信息 -->