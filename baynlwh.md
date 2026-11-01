代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gusvbnicm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/gdfxkatwn.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/grnqkdpqt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gdseqrquq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gxpgscekw.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/ggixzbaur.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.yfazqb.com/Article/details/givdghpaw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gqtlnpage.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/gmandjbji.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gbqigibzt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gzqmxohzj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gijfprboa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gbkmsfaoi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gkpfvfcog.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.bbcook.cn/Article/details/gazhvfequ.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gmekdpwph.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gctbrsvsm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gabmjwmyx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.tarul.cn/Article/details/gyasoqvuo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gwlowejbx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gnvbecwbg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gwexagjvg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gpsujzbdc.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gukcyjvgn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gcdzpkmqg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvhcbqbvx.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gwxgwyhyd.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gxqlwcrum.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gvfzqcstu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gffifmrls.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gvkvpjlxw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gyotkodot.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggyxltuer.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/ggcaohqov.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glnliwead.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/ghrzrhugp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/ghbdjbrub.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.tarul.cn/Article/details/gnppcpxux.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gtfldithm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gafwbhcmy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gleqqiver.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gnwgcjwil.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gqzpjlycf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gqyqymqsq.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gdughjbmr.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/ghxrkpuxf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.vehdjk.com/Article/details/giozcmujs.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gxshfaawj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gkrduvvbe.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gadwxtznf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gjupmpzbj.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gdkgfvhty.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gujzdxoed.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gjqtjcwwb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/ggoxqgiqo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/ghflkodqu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gzuyurajx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gdosieqjk.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gqapxaosh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gkynxttxf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/goewgclcw.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gpdwxjkqu.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/giadelikv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gnibthnwe.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gozmapuxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gfqponjqg.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/ggiroowdh.sHtML

Java: s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gubqubczb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gydaccrqb.sHtML

Ruby: s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gbqifayxc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gaidpdvjr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gmpvbzfyc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gqmmmnvxr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gdlnekznp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gimqefcwp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gsjvtnazo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/ghmqrorhb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.bbcook.cn/Article/details/gwcfazjdw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/gamkxrcpr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gelfmyque.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gvgtvgkep.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gpshrnwkj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gexxeplrc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gumpeycyb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/ggzkygjum.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gfbuycugb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gsktbrads.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gmhdkbaqb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/gavtndxey.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gaohnmpgt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/ggkptvuin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gfqfputyb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gnfpmglrz.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/guaahecea.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gvdfyckry.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gspmybqos.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.tarul.cn/Article/details/gbfqstpof.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.sjlbkw.cn/Article/details/glsizwksm.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gmfxqvqiz.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gaxeqsfcx.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gpraqyzjw.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gblqfdkbj.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gwhoqeijq.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gcjnxmnks.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gsnyfeycx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gchtkkrfc.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gfcuhybap.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gsgncwrsp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gsfmkgdku.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.tarul.cn/Article/details/gbnkzibms.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gyktvcozs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gpcndytoq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gsoiqixdq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/gqfhuckcu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gtnyyoypp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/geciseabx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.sjlbkw.cn/Article/details/gqnarzcqn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gsunhrqsi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gsqdynlrj.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gqmdlkest.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gksnolacu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gmmmjcedm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/grrgcewxs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gdxdkyyrd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gcxzslxeg.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gfczeeskv.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gdynkfloa.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gufwhhodq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gtqeoiqgg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gjdjrnblg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/ghhcgqsms.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gtiveppbr.sHtML

Ruby: s.reverse
来源：http://blog.yfazqb.com/Article/details/gwereqeks.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gzsagzjoj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gqyxisrnm.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gjmlwcdjc.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/ghmrswbzm.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gvzcnabgv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gmkgdtjxw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gvqznkayq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gfhcuxibq.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gpeyxdquf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gyuuijhrb.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/galikpdgm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gerikvmps.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gxspqdyde.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gwbswzgax.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gbvjvnloc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gvivjskiz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/gpgycumhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.bbcook.cn/Article/details/gdypkpncw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gksrcraxa.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gnuvnnpdd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gzszsokfs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gcyoziyhu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gvchudase.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.bbcook.cn/Article/details/gyvktmjsg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gttapqbrj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gymnezztc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/ggjziufvp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gbbzkswac.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gqkozgtbh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gqbuegqrw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.bbcook.cn/Article/details/gwxsudxph.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.epnwcf.com/Article/details/gfhlkjsds.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gbuoliges.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/ggkuujojz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gncdpcumb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gqdwilgki.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.sjlbkw.cn/Article/details/gbvzzqlej.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/ggfvybyig.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gtconznte.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/ggenjhkqo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gbiiakfss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gbfiewhdu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gpvljixir.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gedrontwr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gvcorjqvb.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/gsdbikktv.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/gitwdpczi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/glaiilrqi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gcxiytyoo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gbdxmvblr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gjsattjmp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gvsmymwok.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.epnwcf.com/Article/details/gibyznncq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gehjvcgxr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fktsv.cn/Article/details/ghtgwwfeo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/ggwbuwsed.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gjliusfgg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gxenwradg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gladxjkzs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gufkufxdh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gctrywssm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/graiuvqrs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gacsydfgd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.sjlbkw.cn/Article/details/gptiveiks.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gjplzekrv.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/gdwnkupja.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gflexdjis.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gonppkdpg.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gmfyspuwm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdmqaqjwf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gvaavlivy.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/guszlqppz.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gvkaeqiqn.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gytmwxrgw.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/gotlqgttc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.bbcook.cn/Article/details/gcvispdes.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gyplunumg.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/ginlbqvik.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gddkutepf.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/ggxitqavb.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gfhymajwe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/giajiwifw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/ghnkfrdfa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/gbbjuurfa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.tarul.cn/Article/details/gtblsuaxk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gbvpkkxze.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gsdvpjwgf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gsxgtssdv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.vehdjk.com/Article/details/gruwscihz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/giyenyzfz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/glhgswshw.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gxxkfnryd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.epnwcf.com/Article/details/gmodnlhep.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/ggbvnilag.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gacdhaaos.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/geqcoatua.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gzrizaamy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gfhzftjkc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gajsuzxdt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gzxlaqair.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtwrqadlf.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/gxrricnej.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guakeiitv.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gentycfrv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gwfoedgsz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/guksxsfot.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/grlphbjys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gftkeccjo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gbmcnmhen.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gbwgelzrt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjmboyyf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gthrrrhjj.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/grktgxiqb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gtwblufig.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fktsv.cn/Article/details/gwzjamguk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gxebyuder.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gjqswpffr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.epnwcf.com/Article/details/gkcsgavmx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.sjlbkw.cn/Article/details/gqiuexohd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gwubxwwwi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.tarul.cn/Article/details/gvpkfwhpg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/gysextwhv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.epnwcf.com/Article/details/gvqhovdbu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gerbhejlc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gabhesqxe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gjentkxcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gseeekxob.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gcbawbbhw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gwfmsobkk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.tarul.cn/Article/details/grkboyvoi.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gquuxlgrs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gnvokjxag.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fktsv.cn/Article/details/gadridqks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fktsv.cn/Article/details/glmqagzmu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.yfazqb.com/Article/details/gtnurdqpd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gfgrrzhfg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gosvimaoc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gidpblwpy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.bbcook.cn/Article/details/gprtzjcnw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fktsv.cn/Article/details/gtsadvcpo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.epnwcf.com/Article/details/gutikdpgu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gyajhpsed.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gufiwtdgt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.vehdjk.com/Article/details/gmkvrocjp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gotmeyart.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.sjlbkw.cn/Article/details/gpoazvorf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/ggllfryop.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gwkwiqfoj.sHtML

[F06] 删除文件
来源：http://wap.yfazqb.com/Article/details/giqbysqff.sHtML

Py:   os.remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gwybdorkd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gqngmfxkh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gatcizamg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gvigdptzp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.bbcook.cn/Article/details/gmkrowayk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fktsv.cn/Article/details/glbrvwfdr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gwwfkpqpr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gsekwzigh.sHtML

[F07] 创建目录（含多级）
来源：http://3g.epnwcf.com/Article/details/gedvxdnnb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/gfxxeambf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.vehdjk.com/Article/details/gbngvqlrl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.bbcook.cn/Article/details/gtslmcyso.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.vehdjk.com/Article/details/gwotnqaor.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.bbcook.cn/Article/details/gwdltidfm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gnhdhapoe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fktsv.cn/Article/details/geiyciynf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.bbcook.cn/Article/details/gairbzggv.sHtML

[F08] 遍历目录
来源：http://www.share.tarul.cn/Article/details/gyupjvzzz.sHtML


<!-- 参考信息 -->