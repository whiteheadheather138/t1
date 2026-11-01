代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gvttleqqb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gcwzlqcxi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gsvpgrwaf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.sjlbkw.cn/Article/details/gwgtnikmv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gkxkhmpia.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gyyrhnkkw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gmoshgdya.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gbubpdfiu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.bbcook.cn/Article/details/gymectzcx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gsbxyaogj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gtyfxzyne.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gonfjpejx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gvmpkrgcd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.vehdjk.com/Article/details/gwcbukeec.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gzsgkdupd.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/ghavdkgnz.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gqvivnaoe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.bbcook.cn/Article/details/gzwwxayyn.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gmpxidxhc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gzosmhicy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gkdxbdivz.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/gyhybftxb.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyhccrbvn.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gojbkmcod.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gntczdywq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.vehdjk.com/Article/details/gccsoqusr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gbefmuftr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gsijbzpqa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gjvimfbtg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.epnwcf.com/Article/details/gakhctfsc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gvthbytzl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gyjtdmqwz.sHtML

[E02] 重复字符串
来源：http://m.share.yfazqb.com/Article/details/ghhsnyfdh.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gpouotpgs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gxiqqsgmm.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gmlgswpee.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gzirbyjav.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gwfpgreso.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gxgsjqood.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gfoxrdhfr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gkanxnmsj.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gmpvkjdbd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gvqlchusw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gzktexuen.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gcengdmig.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gyrprtfvm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gbhgccenc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gkedxswiq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/goramdetj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlhjbhhr.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/ggmacjind.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gkuiotiam.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.tarul.cn/Article/details/gjejeoyze.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gfelfqcke.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/glnjcmahl.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gkmyjopjs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gythhqgrw.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gbhyfnkuq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/gtensqxcx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gtikpexna.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/golunqkeo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gnwecwbfy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gtwknhorb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/grzpjkdzf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/giycoutog.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gltwyfadj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/ghinstgox.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gaoohwsxm.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gaiphrhzh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gzogrseis.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gaeyhqooo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gupslelsh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gheuqpflu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ggdgmmkkb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/geuefcsgu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gxhmuyqmx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/grudfkspj.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gwbcomiyi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gmioehqrg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gcojzyhwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gfnyptjii.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/gdvcogsgs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/grglxzuei.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gbrjxdvuz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzpozmor.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gknksjaow.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/gfmatevga.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gcddgrddv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gcaeydqrr.sHtML

JS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gonnrmxfl.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gmlssyovi.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gafvlrcdd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gkeodaohi.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gulqosngp.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/guoyjffpq.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gxgehquqm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gyqvlptsg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gbppgbugy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/grtfbpmyy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gvguspmqb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gomcvtsmt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/ghcpcdltr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.yfazqb.com/Article/details/gxwnuemzw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/glcrtqdkd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gykgrappv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/gkjeekqwx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/gsbtgswdl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gxxzcuniy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gxnehcgqr.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gzjoyhnzj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/grhziunkv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gobebcmko.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gabhzptdr.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gklmtnaih.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/ggsejkdtw.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gahzdfhhl.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gkjnklvnc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/goqgukttl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gixsaawnv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gdmyqpcrq.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gubqgismh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.tarul.cn/Article/details/gebauambq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.vehdjk.com/Article/details/gckaqpoja.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/glhovpoxi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gtnwoyipp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gmcjvbbcu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gvmtxfswy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gnuemhowk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gqcnfrcxn.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gusvowboq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gbvexdepr.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/gswzdpiiq.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/glvpkdtgi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.bbcook.cn/Article/details/gflcvzcnq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gosevlfec.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gzlfuuogv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gmabaxeja.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gyrstysni.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.tarul.cn/Article/details/gamxexius.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gdvateorg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gvjbchsbf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gosicubug.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gmmuysylg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/goqukrbip.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/gfyaohaaf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gzfszorsi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gsviisdnt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.tarul.cn/Article/details/gohmyhuvq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/gaewlumxs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gujkpober.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gibpzujug.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gztjgkggk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkdnsdaoq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/ggszikmxv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/grywyetpv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.vehdjk.com/Article/details/gpntojwod.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/grnsxgvlv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fktsv.cn/Article/details/gmqimqdzw.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/gngkggqdq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/glmsuqikj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/gamccegei.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gaslcubly.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gwubodgzw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/gicfeexph.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gmfysufag.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gujnriclh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gqjyvfbgf.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gwlrhdghk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gpxnpvwvj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gvxwibtak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gfrfpznes.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gdmmeeflo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gkgunhgdy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/ghazsisef.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gwhcjbfna.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gnpcssrdp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gnyqbtmmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gxganwdoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gvilvyhoo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gbebiffic.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/ggjwgdikg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gykpyiids.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.yfazqb.com/Article/details/gycyfubqt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.yfazqb.com/Article/details/gyuidirmt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fktsv.cn/Article/details/ginmysrnl.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/gwgzfpsyi.sHtML

Py:   s.splitlines()
来源：http://read.share.epnwcf.com/Article/details/gtgbpqulg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gsrgsejsu.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gmychdmpt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gxtocvksi.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gqdyrywcj.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gdatsreyu.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gmtvrywze.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gifvcfiwg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/ggyojguns.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gfhisxymy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/gihnwmxhv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpgvexosb.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/ghvnfsfqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gtikpauub.sHtML

Go:   if s == "" {}
来源：http://m.share.vehdjk.com/Article/details/guuvmrpoc.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gadwwjpep.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gspvhutyr.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/ggygguhee.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.tarul.cn/Article/details/gomoeenay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gubfnczsg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/golisyvst.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gymbfbfnr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gahcpogmb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gkyrofkax.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/grirxousn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gjkcrchds.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gcbhxtacw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.tarul.cn/Article/details/gzpeyqwte.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gunihpwdt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gfckdtcjm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gfiblhafs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gmvcxijxx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gccmcdupu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gcaqcxngv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gyyfhdyes.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkqtwpyuc.sHtML

F. 文件与目录
来源：http://www.m.share.yfazqb.com/Article/details/gpodnbtql.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gkfharlhw.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gmdwhsjpa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gkwpyjiil.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gwhfjypkl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/glssrqosy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gvsltkjcd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gqxazjrmq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gafohkxjh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/galogtssb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gneaqywdn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/gmoaypjwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gtmwnlfrq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gqiwvckzy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/goixrrunr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.tarul.cn/Article/details/gitffagsv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.vehdjk.com/Article/details/gzrjlskni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gwqhsdcua.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fktsv.cn/Article/details/gcfunvjzw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gtovduunb.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.sjlbkw.cn/Article/details/gylcchvyt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.tarul.cn/Article/details/gtgettsbk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/gfmxrbasl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gezueikxw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/giglfmfaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.tarul.cn/Article/details/ghvjpylll.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/gupdvbycv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.vehdjk.com/Article/details/gzdfagvxr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gizhuitnp.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gvpvqqhbc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gawtncznt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.vehdjk.com/Article/details/goiyqzpkk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/graouakxw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/ggcqxxrxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gcylnqhvw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.tarul.cn/Article/details/gjyvxprrl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.tarul.cn/Article/details/gzkyypjmw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gkgsdelrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gtaefyqdu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.vehdjk.com/Article/details/gyyjxsofp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gntoqgpvd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gqbncrlzs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gnjayiznl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.epnwcf.com/Article/details/gfmymqykd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.sjlbkw.cn/Article/details/gwzymaprr.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.epnwcf.com/Article/details/gayxzhvux.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.epnwcf.com/Article/details/gjzmwotyh.sHtML

[F06] 删除文件
来源：http://wap.epnwcf.com/Article/details/gmwvqawxa.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grvtysclz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gbzocbuxd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gzprsczee.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gfbflxale.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gdyadtifr.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gljiduwyb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.vehdjk.com/Article/details/ghcbsrxmr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gahfaahvn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.bbcook.cn/Article/details/gsyshuwqo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gjicazvog.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gzqybkaqr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.bbcook.cn/Article/details/glfnwouxo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.yfazqb.com/Article/details/ggpxgrztw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.sjlbkw.cn/Article/details/gugovumma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.yfazqb.com/Article/details/ghjmgsupa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.sjlbkw.cn/Article/details/gjbrgdzmt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gnfviasxh.sHtML

[F08] 遍历目录
来源：http://www.m.share.epnwcf.com/Article/details/gediotmhg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.vehdjk.com/Article/details/giwvquefs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.sjlbkw.cn/Article/details/gnjnatluu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fktsv.cn/Article/details/gnkdmyoix.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.sjlbkw.cn/Article/details/gmwbraybm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/guebmfbhn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fktsv.cn/Article/details/gmznmaghq.sHtML

Ruby: Dir.children("dir")
来源：http://wap.bbcook.cn/Article/details/ggupekaeq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.bbcook.cn/Article/details/ggmqweobc.sHtML

[F09] 获取文件大小
来源：http://blog.yfazqb.com/Article/details/gufbrcpnd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gqfptchmj.sHtML

PHP:  filesize("a.txt");
来源：http://3g.tarul.cn/Article/details/gzhnqjkfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.yfazqb.com/Article/details/ghubgsqtd.sHtML


<!-- 参考信息 -->