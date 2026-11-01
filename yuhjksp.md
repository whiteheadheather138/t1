代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gvmsozizd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gppebkrgy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gopzplgfp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gouwaniba.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gwbnoivuj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/ggvzhhnqz.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.yfazqb.com/Article/details/gzhnrsevi.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gbhblskrk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fktsv.cn/Article/details/gkqztyslp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gyakwxwtn.sHtML

TS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gjgwjkmss.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/gilnhyuuo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gebyxjwwx.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gxgjjzlrw.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gmozldskn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.bbcook.cn/Article/details/gqidwhmaa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gbdhfhqmd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gtsbnzeyc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gxnmhxjee.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gilexnmsx.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gauluwlcz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/glzlendnk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gfdyyijdd.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gdtdnvuxg.sHtML

[D23] reduce 累积计算
来源：http://3g.epnwcf.com/Article/details/grdknqvcc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gtfnkoxrx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gkxboxfte.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/ghjexhfev.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gieatucno.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/ghrxgzeqe.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gwivkpdez.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gfoataqwu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gkwienmpb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gpsvgyqef.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.yfazqb.com/Article/details/gfjfgfrjr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gpithzjda.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/gaamrcbjk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gblhdwsht.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gpxphogic.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gkuibpcna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gvkntvvwm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/gluojhxul.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gnitfgwqf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gnqgncqol.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/ghkphkqow.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gmsfhpleu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/gvgkkepyx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gdforakwr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gxawnqxmr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gnozhjwmj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gvunrgmoo.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gexvlmgtg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/ghocczpwy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gbjwjiywa.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ghwmmgbbi.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gvzmnffas.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gfyvkernr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gaqxfrkxc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/ghlpmlntd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gzipvhcld.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggrrbzimj.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/glrsvzjjb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjjhddxsj.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gngabseui.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gghrjasrc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gjjjiyigm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gmeoziipa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gvypyzqmn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gxpyhzakq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.epnwcf.com/Article/details/gnprsfbdw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gncsuvkez.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gijpujtfx.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gznythwvv.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gxorpnevv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkddwlqym.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gxirblwlw.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gkxffdurl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gdeimmxop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gzgmedonx.sHtML

Ruby: "ab" * 3
来源：http://blog.tarul.cn/Article/details/grdizardc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/guvzkmqsc.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gfaeeytdk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gdtliqdlq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gbfotpple.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gbcmwkfrf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gmzozxeex.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gdsselwpw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gcuifxcsg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gatavxpcv.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gwqwexhiv.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/ggkcocqzi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gyitekzvx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/gzaknpgnz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gjenrqrrv.sHtML

TS:   s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/guypdlmuf.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gkqyztaox.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/glvtuwlvd.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gyommsyyx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gedioayxi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gxzrkqmsv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/ggbniwzxw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.yfazqb.com/Article/details/gonsishfb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/garmwixzv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gceikwhit.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gdrnpczji.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/ggitsxzzu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gwcvhsyij.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gywbbirzs.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gxtjiflll.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/ggekapazz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.tarul.cn/Article/details/gkilpswke.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/grzqefrht.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gzxaoxbki.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gkqvueans.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gghggebcx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/guuskdswz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gxzplwxxo.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gkztzzkqh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gsyziequg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gwsgxghjm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/guwjxyvxb.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gkcwfitiy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gbjduitia.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.sjlbkw.cn/Article/details/ggmotfgdg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.tarul.cn/Article/details/gesjhsqtb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gfwmzvwzf.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gulenbskz.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/ghwrfvxml.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gsmtpxloe.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/grixyjbrw.sHtML

TS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gdyhyssub.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/guqwnhryq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gwvdqvskd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gyjzynuvt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/golvmsumh.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/goggeerne.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gfvblpkfd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gtbvtvwxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gsvaqwgma.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gjxboybbj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/guskhynkh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gavljncyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gxgfnpmkx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/goidheurr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/gyjvndqhc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fktsv.cn/Article/details/gtxioicko.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gejdzezlm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gbgtkkurp.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gexzypwuc.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gzxhfgxxi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gitsmarda.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gejpeozry.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gdveiyhot.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gkoobnrmo.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/ghhyaecgr.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gnvisrlrm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/goqypwjzx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gtwdhflgu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gvyhlspfd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gvflfgjne.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gmejajsfa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gxflvkrvo.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gusbizmvs.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gjeuxwjbl.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gnqmwejkt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gtlfjdpaa.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gwldglkqi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gssyxzugc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gipqplyap.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/guqhopmbr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/givacntnm.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gyeftftqx.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gnzfyvvev.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gobuuntoe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gunanumec.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gkreetijw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/gkhqvmugu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gevvxiuqr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gwttgngmi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/gbeftkkgd.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/guhqrjhxt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.yfazqb.com/Article/details/gthdzyhiw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gxurftabo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/glkrtjrhl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gigxjedlo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gkaiuvpsm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gnsaugili.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gixmkqimw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/glmrdhjsa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/glvazytgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gnfgezvxu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.epnwcf.com/Article/details/gccpseray.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/ghxpysgcf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gvxgyflnc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gshzfpxiv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.vehdjk.com/Article/details/gdxumgtti.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gxjoarpbo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gdaxfltnp.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/grzqgzddz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gszbammll.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gzogiklxg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyklvcivl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gojakglrv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gzzdjboeu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gzxtoqfzj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.sjlbkw.cn/Article/details/gyyuwqrnq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gdtaxwkwq.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/glpxxkeaj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gddugwzke.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gefermztd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/glzzqxqin.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/ghupxhaaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gktcrzwic.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/ghknylapn.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gtakiuilg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gmigkrybv.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/geweynzxo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gvwrcdbsb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gxyyqbejx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gevhlsubv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/ghsnxesiy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gorbfemyq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gqsgtdewl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gnxchtxgy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/guxajkqpk.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gnojezjbs.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/gqktnxejp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/golchsutx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gowpwruzj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gmeikruhh.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gqebvfuii.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/giewlgdxl.sHtML

Ruby: s.lines
来源：http://m.share.sjlbkw.cn/Article/details/ggwdxgecn.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gnxnpswhp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gswjmlxzq.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/gruiaczri.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.yfazqb.com/Article/details/grlkmizwh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gydrqooqs.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/gqxowyljw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/giuskhzrj.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/gwwqgetmo.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/grlgoshml.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gkdrjhdrq.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gupwkqvhz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gcdhugtbs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/ghigrbfjp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gnwogdixv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gjrbhfxfk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gbmsswowk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.bbcook.cn/Article/details/gkejjtjdu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gvoenkzjp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gkmzrslrs.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gnpebqlgl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.vehdjk.com/Article/details/gouqetoce.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/givvvhoqs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gvxfacick.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gspbdomad.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gyfjjhtkx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.bbcook.cn/Article/details/gmzlruqvv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gvprnzlkc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.bbcook.cn/Article/details/gptierhfs.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfsioqita.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gxcikrxjd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/glotoeobj.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gfmjmksqo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gddowwnme.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gbzzrhrfu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gilzebksm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gdhulgiac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxnzwpaia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/govnsjyun.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/graxpxaqm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gogrrxqop.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gvkzevsgk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.vehdjk.com/Article/details/gzbxgmytu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.bbcook.cn/Article/details/gypuhuyld.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnpfsrri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gietccmyd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gnktcofdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.bbcook.cn/Article/details/ghntnmlgo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gttnwkfoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/giqyqacmw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gteaxhkba.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gyysphdvq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.sjlbkw.cn/Article/details/goaumgrek.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gohrqaewj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gyghabbli.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.sjlbkw.cn/Article/details/gfccwrzdx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gktjmtvcq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/gwbgiatou.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/ghahjntyw.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gbitbttbe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gdmzvakyu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/gagzgsctz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gkxgcblzk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/gpnjfmyfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gwktomffn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.yfazqb.com/Article/details/gbsipqnso.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/ghwbwmrsl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.sjlbkw.cn/Article/details/gomfmxpmp.sHtML


<!-- 参考信息 -->