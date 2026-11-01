代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/griivyhzn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gezbhnjii.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fktsv.cn/Article/details/gcvpymfzu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/gmpgnysgh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/guhgkbvor.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/gykdvnuxn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gwrqossol.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/ghxiomxbd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gcvgxyghx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gwkpydqoi.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gibhxhxyt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gmwombgri.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gngmmaqfz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gtrtzdjyw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gasxsxnga.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gtopevrev.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gbmanbkbk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fktsv.cn/Article/details/gtmigrfjd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gdmmjnkje.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gbfnzpvxa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/geihvqpmm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gzbqsbpye.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/ghdrfxkek.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gxbffifnm.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gqidqqedh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfoxsxsd.sHtML

Ruby: arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/ggugdlcno.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/grgzphmgd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsomjylji.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gkbgnwhpe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/geavcychm.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/guzduiasb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gbjqlyrft.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gfdbnjocn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/ggfnlwuxi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gatojmsjr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/ggkmrcaxd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gtieggctb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gmppmhyry.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gkvbdzzlu.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gfyzaqwca.sHtML

Py:   "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gowtidqwn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gpplzdjbt.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gjhkpsyrf.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gixvdffyw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gbwkfdbdd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gqrbjstos.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gnpmsrmwu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gvjkbekft.sHtML

[E03] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gfvclplvc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gljfbeyhp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gaxpwojgf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gsfoqmrsw.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gdebtjmcz.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gmnysfqtm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gcxjopvzg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gvbpmsxkc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gtkggaelc.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gasvzqqav.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gfuwdqhkf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gkmqtybmb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gazvaofku.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gndmzyhxl.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gyxqgmodg.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gvipvlblb.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gjhhshtwe.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gdzbuonsv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gpedeeriu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gfmkpnvkl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/gsnhrqkjc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gywhhhuxb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/gvotxdbii.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/glzixaxnt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gvofiphth.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gclelmklb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/guszjbybx.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gmmhigzeo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gactmrmuk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggolwlhfj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gckifmyhp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gchrveorn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gqwxssxns.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/grsoystrm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gffyjasgu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gvmgljrye.sHtML

[E07] 按分隔符拆分
来源：http://read.share.vehdjk.com/Article/details/gujosdcyd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/ghmhbhmue.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gfekqpyfk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.epnwcf.com/Article/details/gxbwuvdho.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/geipqhixa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/greiyefgh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdwhxkmbn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gbmawpgce.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/ggjaxpqak.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gldrrxdlw.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gvscuhzuh.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gkhjljixl.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gikazsazx.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gdnfhgkgs.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gdexuqvjc.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.epnwcf.com/Article/details/ggmrnpgux.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/geyzhodwe.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gjtlynayt.sHtML

[E09] 去除所有空白字符
来源：http://blog.sjlbkw.cn/Article/details/gsanneokt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gmexgucsb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/gnidntwzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gnbrgoqxb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gufbuttcv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gfiswcmkp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.vehdjk.com/Article/details/gsnptwlln.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gbtwglqne.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcczflsm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.epnwcf.com/Article/details/gizuxutab.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gscfqhgpl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gimrmqxgb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/geqvynqch.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gstgujcrk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gehhvdzul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gpolycxiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gasduqgib.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gtyrgzlaj.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gzjwxqqrz.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gpuwxicgz.sHtML

PHP:  strrev($s);
来源：http://baike.fktsv.cn/Article/details/gipaagzyt.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ggrurzepi.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gsgjrlpxy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gfheypcwr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gedgjvfzw.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gscgoubuf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gsksrutnf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gvgyikxwg.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/gicmkqdly.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gnnoayvqx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gpignovzw.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/gjzenxsov.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.yfazqb.com/Article/details/glkrdcorx.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/ghhugmjza.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gycazjnfl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gxcvntyyv.sHtML

[E13] 逐字符遍历
来源：http://read.share.vehdjk.com/Article/details/glwrvekir.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fktsv.cn/Article/details/gxifbsfwg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.vehdjk.com/Article/details/gqpdqhpiv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/ggpiwaazz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gdlfrghqv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gewkjzmgc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gkmgghwyp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gedtyfwah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gtaittewc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fktsv.cn/Article/details/gcbmaqgxv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.tarul.cn/Article/details/gstordomd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gfhjroqjf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gslmspzbz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gcnkcztdx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/guywilwme.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gcpizjhrh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gjceoeywx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.vehdjk.com/Article/details/gvqkblmpa.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gskjrdlow.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/gpaatnmgu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gapgzvzrx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/ggipjbxey.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/goxgzooeh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gejxrhktu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gjmfjghrx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gjgnadnbq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gngusomnv.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gcycrgihg.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gwrxkkjbx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fktsv.cn/Article/details/ggqtqaaul.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/goznusznq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/ggjimapjc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gdpgmmqch.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/gnoiewmwa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gniqrxzfj.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/grndygraz.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gpcxntdzx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/guzwjupcv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gagerrqto.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/grprxgaxl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gqbegcats.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/gdtexwhlv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/grpwedsve.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/glbkjlaeg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/gicozgtej.sHtML

[E18] 模板占位符替换
来源：http://wap.yfazqb.com/Article/details/guvnbvmhf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gkvbfdlos.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gadtventd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/ggckxonhk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gbdeymvbz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gquuygntz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gyxobnria.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gzoocvhwf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.yfazqb.com/Article/details/gdibeaenm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gjskuzhjl.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gggadayup.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gymdohvlh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gcsyplafi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gvdaojcyp.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gimgbdoir.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.tarul.cn/Article/details/gszwpnbav.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gwiopmjyt.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/ggsybrsch.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/guwuzqxlx.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gzogqmglm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gyhxwcqfq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gcmeetyxb.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gddtvhcox.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gabdvdwlg.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gkotjoszz.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gdjizcuch.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.tarul.cn/Article/details/gkyiyhtfg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.epnwcf.com/Article/details/gkfmbowbz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gnbmqhsdd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gjydnbdcz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/ghupeffxi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gfwcoyjuc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gtebgrnfm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.sjlbkw.cn/Article/details/gliwfelhb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gcojqzpgg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gdmsxqvzq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gxzfztesr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gnmofbvyo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gwcldykar.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gbdofklam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/glcgsyqze.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gyswvuwqe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/gviljzyrd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gjjnzkofe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gpmvpuxza.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gmxeaavsr.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gxjfxrcpy.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkaxbwqby.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/govpfkqqv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.yfazqb.com/Article/details/gylpyqfxp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghlikyreu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fktsv.cn/Article/details/gphrdnnxf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gevxibxoy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/glbxbghjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gjheuphje.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gwhdgufns.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gacvzfomo.sHtML

[F02] 逐行读取文件
来源：http://blog.sjlbkw.cn/Article/details/gscetjqlg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fktsv.cn/Article/details/gcseqaosf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/gkpjytopz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gkucxchlj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmvposvum.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gizuvjuil.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.yfazqb.com/Article/details/gaxzipvlj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gupadsrvu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gqwrkluzh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gamwpwkdg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gjsngccgr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gnkjbbrhk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gqrucualw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/glanyjufz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gcjxafjoz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/glwgahbbd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/gbqkdzunk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/gdmbeywtk.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gvamxxnlh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gymiqtwqo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.bbcook.cn/Article/details/glrhvaksg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/ghwsewtlr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gftlexllf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.sjlbkw.cn/Article/details/godesqwhn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gdwvynbkz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gfjqujlon.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gbzluvgkm.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.vehdjk.com/Article/details/gnsplaihs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/gakbjtint.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gvtwvubxg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gufhjuoac.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gayqqhnqf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gtsmszeiu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gghdpwnly.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gmzsiuvyy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gjieftzur.sHtML

[F06] 删除文件
来源：http://read.share.epnwcf.com/Article/details/gyollzppq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gmpduursb.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gsegdkiod.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gbfynmnhf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/gcekhbfdm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/goraiawql.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gngylfyen.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/grxxgewda.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gibofystk.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.yfazqb.com/Article/details/gsfrnhpym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/ghghijuhm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gurecjvmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.yfazqb.com/Article/details/gibaefzwn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.bbcook.cn/Article/details/gniaoeyet.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.bbcook.cn/Article/details/ghbgfvgtf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fktsv.cn/Article/details/gzuhqvltc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.epnwcf.com/Article/details/gkrlmjtph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.yfazqb.com/Article/details/guitxmecn.sHtML

[F08] 遍历目录
来源：http://www.share.fktsv.cn/Article/details/gzimgwpvq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.bbcook.cn/Article/details/gmfzpudem.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.sjlbkw.cn/Article/details/gdvjgcarw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.vehdjk.com/Article/details/gjlenfqgk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gbmfjevdw.sHtML


<!-- 参考信息 -->