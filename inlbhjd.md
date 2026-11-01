代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.bbcook.cn/Article/details/gqqwbbovr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.bbcook.cn/Article/details/ghmfwnuup.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gqxgnoqxw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fktsv.cn/Article/details/gmaodtqcy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gjdrveler.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gtgneiwew.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gvhttmnjl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/gamtpekfq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/gzdnqdovh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gmehhxhyz.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gltmrttfb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gxbmjdmfm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gepdpqonb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gdeepwbxs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gtlzzjqff.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gjjwzjyng.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gudzncexh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/griwrryxx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/grivqftti.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gxiipyyta.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gqlhjqtul.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/galydyikx.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gdclpjgtc.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gaccwrkdv.sHtML

Java: String.join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gqphiyhxw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/ghzzvuugv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gtrueiiod.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gmrvyoqrb.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gkzdndqsb.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gpkjejbnf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtqjhdzku.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gkxyusboc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gxhygscbr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gkysvaqpy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gpmvpymkm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gzyiitmty.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gkhqjmlmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/gunipjfjt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gzivkoatx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gyyaeifgp.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/goakqzuhj.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/geevrrxhi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gzducodsz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gjhlnqmkt.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gwegwdkrj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/glinnwnyq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gvwvqlzhj.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gkxfonyhf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/ggitbpbbh.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gnpsdybmf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gvdamubru.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gmwywraeb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gviqecvmo.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gknpvntkz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/giharuuoz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gmzpocifq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gszcxjkjy.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/giobbpxka.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/gmxtfqdkm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/grpbdpowk.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gwkrhkhxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gvdtjcvld.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gvrkcpmzg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gtpdgtpmq.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/guxdcbcid.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/ghugvfayv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gtowbdsgs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gmrxdejkm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpilspekk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gsvhadwkq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gawowowkf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gtnehwfft.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gsmcerdhl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/ghwixinox.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.epnwcf.com/Article/details/gnumhyevv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/ghxtureyt.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gwkllknax.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gzcglhtdd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gbqcvmcui.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gelwedicj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gktjtkikb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gigmjknus.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gqehofbsx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/grqynfixg.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gfvdkxtyc.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gnnvxfqrg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gtwkodubp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gowzsmihi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/ghgwjofgk.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gqxcdhewg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gnqlddpsk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.yfazqb.com/Article/details/geeuypprd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/geaszzhuj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/galkbrsag.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gcqyiffcy.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gmwvpmgqe.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gqtrsbrza.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gcpgnusby.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gormhtcit.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gqwdksuki.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/guajghmoq.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gwrxdhjmh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gojmvkoxc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.vehdjk.com/Article/details/ghctncedb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gnectzfyq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.bbcook.cn/Article/details/gjejwvuua.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gshnmjqjd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gyjavxosa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gzlkuikzb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gcytqhnhb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gevgzzfho.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gpddtpgtf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gsobfllmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gwwxvbtnv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/geycykqgc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gxiysaedu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gjslmwgas.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/guaxnvaxj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/grgbmlath.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gbpyuugvi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gaekwthsv.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/gazlqoqzu.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gnajzttlb.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gkmszobal.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gcsjdogdx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gnhrfmfpn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gdimsddre.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gimrxrxnb.sHtML

Ruby: s.reverse
来源：http://www.share.epnwcf.com/Article/details/gpyfgzdnv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gmxeetvcu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gbmrmwdqb.sHtML

Py:   s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gmhovjbvn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gptgrunrf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gtdvozjmx.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gnotwilcj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gobmosbpx.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gjdrtnatq.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/ghrcvfnpm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.epnwcf.com/Article/details/gkyiprdps.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/ghhjkogsl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gvebdhdlj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gdjesshlc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gxtciyhwc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gbnockbcd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/ggplgukgp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/gjiteishk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.yfazqb.com/Article/details/gnqebyiyk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/gdufjjmug.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gldjtwgxs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gvefuvunp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gnjoteopt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gouikzqnr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gigojkoiw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gstmqclbc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gotfpdtas.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gedlnuvzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gbmqguamu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gjydfqyej.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gfbhofezr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.yfazqb.com/Article/details/gtyxtqcsa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkavteotw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/grtxqowpd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/geprvynjd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gwbscwsep.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gvjwvmfve.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/gnqadqdgu.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gnxbrcqhr.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/ghgbwfxcb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gyevbolii.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/ggmczsteb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/glrwkonki.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gbviwbkxf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/glqsxlbln.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gywzgbkvy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gluzjvayr.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gbfilrrtn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gyrqvaicv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gwsiayeyz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gewfuffkn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gstxrsbdp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gcztxptmm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gesezrjca.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gvcledoyb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gtlnonkzx.sHtML

[E18] 模板占位符替换
来源：http://mobile.fktsv.cn/Article/details/giichplpr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/gaapxkihy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gvtfacwfa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/geentclem.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/ghqbkunrk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gvxhtexls.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gfsepiweu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gfwgernms.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/ghmxoogbe.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/gipcmfzzx.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/gyvgebpik.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/glgweqzuf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gecolnjlc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gfsdwuqkw.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gthshpbvf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gtqxidaqo.sHtML

Ruby: s.lines
来源：http://3g.epnwcf.com/Article/details/gbshipukx.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gfmvpbbho.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.bbcook.cn/Article/details/ghgntxzls.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gqafeamoz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gwbjexngv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gyeguhglj.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gdxnyavou.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gpltiiygu.sHtML

Go:   if s == "" {}
来源：http://baike.vehdjk.com/Article/details/guddwqyrh.sHtML

Ruby: if s.empty?
来源：http://www.blog.yfazqb.com/Article/details/gwodjtdfd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gbyedqkky.sHtML

[E21] 超长截断加省略号
来源：http://wap.fktsv.cn/Article/details/gwbrjoqya.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gwpkifpvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gnbcqyjez.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gmfbzdvay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gupojewaz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gewdyrvob.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/gsuugqhkn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gtnhdqzsn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gnnavrufv.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fktsv.cn/Article/details/gorcgvbnw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gohwaflba.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gtsuxpiai.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gstdqozxd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gjockwxry.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gowsnaqaf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gezcfksdm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gdmhzovez.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/glajoguhn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/golzqgyci.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gsuopnptp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guntyfypo.sHtML

[F01] 读取整个文件
来源：http://mobile.vehdjk.com/Article/details/gmvfcjsji.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.vehdjk.com/Article/details/gwqtjetsq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gydzwftmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/gsickewuf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.vehdjk.com/Article/details/gzkygkncc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gfkneqaor.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.vehdjk.com/Article/details/ghalirpyd.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gujfehmyh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gyumripxb.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gzjkohtjo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.bbcook.cn/Article/details/gwevwanxx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/ghtllvhgr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.bbcook.cn/Article/details/gcpduzcwn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gpevcbjfb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gczcziakk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gbvkeunlt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.epnwcf.com/Article/details/gtkyugnly.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.vehdjk.com/Article/details/gxzberbgf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gexmxmixi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/ggxftzgqx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gnjvkseyz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.vehdjk.com/Article/details/ggaavdfdq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/grroktwsg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.yfazqb.com/Article/details/gqjfvtkoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.epnwcf.com/Article/details/gtcwqmqsj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fktsv.cn/Article/details/ghjdfwzul.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/gsdwshalf.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gdbtbzkhc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/ghutqskhv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gqgsncaca.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.bbcook.cn/Article/details/gikxasidh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gkqtyycvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gjzkidkfc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gpnzhujrx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.sjlbkw.cn/Article/details/gtjxhibai.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gadbyhqkl.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.epnwcf.com/Article/details/gxqpcwxjb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gvmwigihd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gobzbqtrd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gnaldddxy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/gougqvxht.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gqyvpligk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gmviijvyb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.vehdjk.com/Article/details/ghcsuqxdw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzlissntq.sHtML

[F06] 删除文件
来源：http://3g.tarul.cn/Article/details/gijqbomwp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gbofcdckm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gotdspfmi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/glcdidalw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.tarul.cn/Article/details/gxawayfvc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gvykczkxn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/ggfiexdis.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gnfzetfkc.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.tarul.cn/Article/details/gscqxrmnk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fktsv.cn/Article/details/gfmltywmp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.vehdjk.com/Article/details/gqhrlidvs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.yfazqb.com/Article/details/glyngqsap.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.yfazqb.com/Article/details/gbxrtrdbq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gdpshrdaf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.sjlbkw.cn/Article/details/gkkltuxiu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.epnwcf.com/Article/details/gpuaquikr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.bbcook.cn/Article/details/gptgnekyq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.vehdjk.com/Article/details/ghzcqznpu.sHtML

[F08] 遍历目录
来源：http://blog.epnwcf.com/Article/details/gxihrrbvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fktsv.cn/Article/details/gzaypwano.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fktsv.cn/Article/details/gocyjoaxg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.sjlbkw.cn/Article/details/gsttzdhsb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.epnwcf.com/Article/details/gxxyeffpd.sHtML


<!-- 参考信息 -->