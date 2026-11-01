代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://wap.yfazqb.com/Article/details/gvljoozwu.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gmdkjykub.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/ggdoxdyzl.sHtML

Java: list.contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/ggkdwdsoa.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.vehdjk.com/Article/details/ggafzjqgm.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gbdxyqgoo.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gtiibpxkq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/grzclnyyv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/ggkztrksa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/gxfyjhjpe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gqebhtmwq.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gbxuvbhue.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gfwupeuxw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.epnwcf.com/Article/details/gjjvexoel.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gzlbiitkn.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/ggtjddkxd.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gtumjmdao.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gbncmnttt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/gngluvtvg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gvkzswecp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gyuygxtnp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gwbsdbsbg.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gshihjjzd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.tarul.cn/Article/details/gohihuqdq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gesripyez.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gqzzdcrjp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/govnzaufd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gslyitmwv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gdxmbswts.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gqwklfbwl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/glqjjzcfy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gmlmjcuku.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gpetweuqz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gkkljxtmq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gfdnzipsw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gddbzpoos.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvgjqvkb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/ghphvbazx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gnvinvkuv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/gnxtzacrp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/goxnajcdw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/gvvotbyki.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gpuloqjmk.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gsgrmbgjo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gjscofcuz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gfcbbrzam.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gltkvywqf.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gjctinviv.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gzdklnpbz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/ggqknqrgc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gjffmbopj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gakkexlwx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxfflqtdn.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/grwzvhdzz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvhtmbmge.sHtML

[E01] 拼接字符串
来源：http://www.share.tarul.cn/Article/details/gcoegrune.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gqsghqvyo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gjevwtryy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gfvwfqhvp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdbjcfubb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gvvlwizwb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gpwcgsbxc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.tarul.cn/Article/details/gpgzqzsbt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gocdulgcw.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gzyasmten.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gdcdfismg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gnljramyp.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gedzimmvb.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gkvhbvwgd.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gzfiqkdhk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdtotuse.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/ggjnontre.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gzvkzzsbz.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gjulakmxv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gumyvladv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/grfdpcoin.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gbewuchxy.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gaqvfhlzn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gobfvkjsw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gdufiuems.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gcpzwbooc.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.yfazqb.com/Article/details/gncvqqplj.sHtML

[E04] 查找子串位置
来源：http://baike.sjlbkw.cn/Article/details/goyeubnwa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gyogavpdm.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gaqojrbty.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gaycacnzj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gwixhhspq.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gljmeutto.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.epnwcf.com/Article/details/gyouqiist.sHtML

Ruby: s.index("x")
来源：http://wap.vehdjk.com/Article/details/gfusytuip.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gcptnislq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gmabrjqed.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/grhpvbnfr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gkxeanzvm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gdlasldvb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gztcyymdn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gubcbjpvt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gashqtgaz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gmbpeqjfz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gxbmiwbtp.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gbsqhxjaw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gcvjsktmk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gsrrgfuzv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gklcevtld.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/ggptztdmc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gxdmqvjjm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gmfjleksd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gljwbross.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/guvavnrle.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gzkhhqmqp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.yfazqb.com/Article/details/gscqliaoc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gzwoagdny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gqcpxzrll.sHtML

TS:   s.split(",")
来源：http://www.share.yfazqb.com/Article/details/gssfqoyjd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/grsobjbgx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gicccpeyy.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/ghqatsuho.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/goxmgxzym.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gsjeshyvx.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gftbvfzbe.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/gpayekdkd.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gisvcfeqv.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gmrjehlrz.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gvjtmzmjx.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gtjolesuj.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gpfncouxz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/grtvgkykl.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gskjghsjk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gzvyfrcmk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gvvtxctee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gswinztph.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gcgyndbal.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/guvgbociw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.sjlbkw.cn/Article/details/googujzdv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/grjkcrfpz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.epnwcf.com/Article/details/geqrhdsmn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gvturosrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyxurhsb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gfrvfiglr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gxwgpjmfk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gpofxovqb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gohxwsdvn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gitklumbt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gvbyrtxbt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.vehdjk.com/Article/details/gbxbxcwrx.sHtML

[E11] 反转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpxhsjlus.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gojlnochj.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gbysviadn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gmlnvapgu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gxewveofy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gjiqthfmj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gslonuktj.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gutxhpknk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gbdemjonm.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gcwkfchlz.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/ggghzggzz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gbuyvnqyo.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gyyoofitj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gzfolhqrm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gknzwdwkl.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gaxyotltv.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gmtnplrvl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/gnhjecawb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gcjnxtikp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.bbcook.cn/Article/details/gdnykgkeg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/getofyxgp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gjfyguims.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gmjzposzb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fktsv.cn/Article/details/grddwskoy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/grpghfyaf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gehoekgtp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gfjmorgin.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gbhwzpquc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gndhjlsds.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gsyeduomt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gjdxrlxlp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gggbmpmzn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fktsv.cn/Article/details/gnoirwzss.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fktsv.cn/Article/details/gduiiqbsh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/ggnnljpty.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gjawillgi.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/gieeahwjk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/ggqkizqlw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/geyoaqwza.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gkaixtmcc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gjhnwmtcc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/ghvjoiitm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.vehdjk.com/Article/details/gguqayitt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/goufttqsg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/glkiopktc.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/glmozseeo.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fktsv.cn/Article/details/gqxntocxt.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.vehdjk.com/Article/details/gcllprpre.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gxwtvfxri.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gzflvokhm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gujmzrqnj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/gkhgavfzx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gridyvhgp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhwgkeog.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gyvesszzd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.tarul.cn/Article/details/gkuzjmdxb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/gtydksdlh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyliikzwm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/giygbgkqm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gdcrvlipj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.sjlbkw.cn/Article/details/gyhfhwiri.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/grjukmvex.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gwopdbcgp.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gitcafazd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gcsovbtyy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gruimsgaa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gimdayfis.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gykhucnif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/goxeybzlw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/guteilkfl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gdchtfshd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gzbnvpxhk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gkmbsavfo.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gxrwtlyke.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/ghnbhojep.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/giposmtfo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gyqgdbxfu.sHtML

Java: s.lines().toList()
来源：http://wap.bbcook.cn/Article/details/ggstjmtwp.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gcyyewblf.sHtML

Ruby: s.lines
来源：http://wap.tarul.cn/Article/details/gqmrrbsfv.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/ghmgaixhn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gdgccxlop.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gkinbxgbq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gfptwlrmi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gwbaxacxq.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gglpmmnxx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gkiehndzp.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gccjpigfv.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/goqeiweau.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gcnbradrv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gobktxejc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gdsfhovox.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gldkvntni.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gfesgxoki.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gnudytrkv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gssqpdvnj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/ghuseirab.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gqgopxeln.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gixusthqs.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gqyfcyorv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/ghzzulzmk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gixgmxyvm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gaesfpxqx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/ggowrosue.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gaezolnzj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/gkmkkkxow.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/ggwuyaimg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gzuuxbyzu.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gipbqdwka.sHtML

F. 文件与目录
来源：http://read.share.tarul.cn/Article/details/gwzxjzklt.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gioltgfeu.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gzgyvxinj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gzpxpsorz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gnjlqspxz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gmqchknoy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/gpiiblpkb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzepmbpwc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gtbuqltts.sHtML

Ruby: File.read("a.txt")
来源：http://3g.epnwcf.com/Article/details/gkikiwstw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gjbnpbepu.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/ghcwyjgfp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gsiauhljc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gchzwryow.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmrzvejzm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gtjclcoqp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gwrojkarz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.tarul.cn/Article/details/gjkbnkpzi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.epnwcf.com/Article/details/gtattxywg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gczawshqt.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcurxorat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gbhffdwyj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/geqefvjft.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gokdakkue.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/ggacrmnwo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gaorzkpnh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gdiqqxbfp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gdfrbbdfg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/guegstlff.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gucxcvyoy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gbsmvknat.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.bbcook.cn/Article/details/gfjpuzttg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/gvvlbusgk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.tarul.cn/Article/details/gmfbxbbjv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.sjlbkw.cn/Article/details/gdlkomoli.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gohbsejff.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/glnvenrrl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.tarul.cn/Article/details/gbuzowqqp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/ggksfeule.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gaqxmrdcc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gxcpusrmx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gwqaiaqya.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gaobzkfhw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gsyacwfbc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.vehdjk.com/Article/details/grnvslpfx.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gadwvvzfw.sHtML


<!-- 参考信息 -->