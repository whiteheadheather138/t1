代发 wailian999

[D15] 去重
来源：http://blog.yfazqb.com/Article/details/gbfvwiotz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gxyxsekdr.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gwwtltkjv.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/ggotefpsc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/gbsdpotbp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/gzougvlol.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gykabiolk.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/gsvhonbut.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.sjlbkw.cn/Article/details/galbswnfv.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/geihhjijx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/ghnvewrsn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/goytfdnpq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gbamzwdxd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/grcwecvmp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.bbcook.cn/Article/details/geuyqvdmx.sHtML

Go:   // 手写循环累加
来源：http://mobile.sjlbkw.cn/Article/details/govzngfhm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.tarul.cn/Article/details/gnzdrtqwy.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.yfazqb.com/Article/details/gtnhzkmoq.sHtML

[D17] 最大值与最小值
来源：http://www.share.vehdjk.com/Article/details/gundmucav.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gjjovikgg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.tarul.cn/Article/details/gslmxbqac.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gsofxrxjf.sHtML

TS:   Math.max(...arr);
来源：http://baike.bbcook.cn/Article/details/grgdcfkyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gzldkpkrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grkomklay.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/gvzwfkpbm.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/guhbrexfv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/grfchvsct.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gyhzczkbd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fktsv.cn/Article/details/gxjemsfhk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gjnubisrp.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gfxfzabaz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gkbvomrzi.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gdrflrhtx.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/gbqgbkqkb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gvsggvgnq.sHtML

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gzzywfeje.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gxegspcel.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gkarukrfh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gsgyiupxo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.tarul.cn/Article/details/gcelxxmch.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gtdccinqp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gyjyktwyf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gfaarspsg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gkqcvbyxx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.epnwcf.com/Article/details/gknsoljrw.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gpboyhxxh.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gpybdjblr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/girheaykc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gbvjhizer.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/gjizcmleq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gvbmjtezf.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/ggbwinwzl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gutuysgya.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gvnunxylr.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gwozraxvn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/gbsdyifas.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/ghftcitye.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gkgzffcqb.sHtML

Java: list.contains(x)
来源：http://m.share.fktsv.cn/Article/details/gceocdifa.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gliwtuive.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gtpxdgttn.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gwatwtvgl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.tarul.cn/Article/details/genzuwepe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gtjfftjuj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/gcmhtewmx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gdksrxpko.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gniurcges.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gpbdpdigv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/girilccyp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/granqvkzv.sHtML

C#:   new List<int>(list);
来源：http://wap.epnwcf.com/Article/details/gjbgmnorn.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gqetqlxmm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gyqbobcts.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/guezqxuiy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/glsrmtoej.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdbhvymy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/ghtqhgktg.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gjbgzxrec.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gisqvsnal.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gstastrbn.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gsukrzjme.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gngcctzny.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gvyaeacsz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.bbcook.cn/Article/details/gjnbqkgmc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gzzeeksaj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gtcofeknu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gfbbqzejo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gvtfbuisj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gyzmlrmdu.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/gkscdlyrz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gxamwvmtm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gyuxaruhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.bbcook.cn/Article/details/ggavclvex.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/grcszuayx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/glpbbldhp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gzwzkhlks.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcvonifhy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.vehdjk.com/Article/details/gbujxqrcc.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gzijxgtct.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fktsv.cn/Article/details/glriisffk.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gvwtxzbrm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gjytusjar.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gckriqysp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gbyjfqrxn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gxobuyucb.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gbavhvjtd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gwesdozyp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmrzqxvka.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/guycgcoxv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gkrbektcb.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gzrignxcy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gygjgwljy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/ghicuwkpm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/goktubnqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gagmvllom.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.vehdjk.com/Article/details/gwyrwcgat.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/gnipciwid.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gapsbjseb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gepzurxsy.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gxiprmgat.sHtML

Py:   "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/grvbqokyl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/gvywcjcvy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gjgqeujcy.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/ggiqdkdos.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/ggznleqek.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.sjlbkw.cn/Article/details/gvpnrfjvq.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/ghseyvttf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gvedgfwjl.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gkhzbwygl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gocmazlco.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gzjvdewlq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gvixkyunn.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/ggqohnfnm.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/ghfwatwkr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/gmwwdemag.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gpqdcymsi.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gtnhnhqvh.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gmqfymicy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gtusswoqt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gzginzfks.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gkvobttjk.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gkrrjanfx.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ggitdrrqt.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gnjnfplqa.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/grvzeofgm.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gvfvnqfcx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gibkfkceq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gupzhffmb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gbrhkxmmk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gkupvmbfh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gbowziyhw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gaarxedgc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/grjuhwezv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gtdzbzqdc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gamkutbgx.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gnlrjnlvg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/grsukvzlk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gjughalpl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gjivestdg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/guqcgjieb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gllglgzso.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggxjllvnw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gjuhhkmie.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/genobjday.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gsxjfprsb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gttpwfexk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/gibcdbdid.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gdtmmtagc.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gxijipepn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/guyaxsbpt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gaqesaxzn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/gpduijrzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gcyckztmm.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gnerqweit.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gcvntvuea.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gdmbbpjhj.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gucaphncx.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gsdsknvek.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/glnfhdwny.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbuaekdz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gyvndtamd.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gqkkixdwi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/ghkodqjnf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gixxgxaxk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gmnexxcrl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gbwpbwzzr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gtfsqfrbu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gysspwrno.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gtiftlzee.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gltfajhvs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/gceabsbnt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/gxffjaywf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gcwewhdon.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gpsjzzoke.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gpbzwqung.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gsusdstwr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gvhanefzz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gcbafahjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gkjyrbyfu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gaadrmpuh.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gpagteqwn.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/grkjqytwz.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gorouopon.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gphvgvith.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gxguwwros.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gftsmlxpt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gaougljkq.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gyolnmkth.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/glysboozo.sHtML

[E12] 统计某字符出现次数
来源：http://wap.sjlbkw.cn/Article/details/gqngzwxgo.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gnxuyszxg.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/ghyllziqj.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/geclauvmx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gsmitscrq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/grqbsnywh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gdrqhdjyl.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/grgvueayo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.epnwcf.com/Article/details/grjflkmqp.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gvehtbigr.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.tarul.cn/Article/details/gheofntpc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gapootiqc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/grvqlaipw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/goyncdran.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/gixwsuace.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gptxhsqkf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gqavgzdzt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/glzcpopku.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/gjefcrjux.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gzkodydix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/goxxggxlg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/giejmoaux.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gmnyrivbp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gvxyettrs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/gpxavksmn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gwuqxkifl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gkkaqzxwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gyywyvqox.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.tarul.cn/Article/details/gpmtjkcbd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gscgoztlz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/gfwahequz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gzdacezuf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gmzpyuozb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gpmvpikou.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/gwojaikjk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gmcqhixlf.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gcywgwuae.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gzzfyklnv.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gcjudtkol.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gusmsxtcv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gckkoieah.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gszebzutg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gbruqclpt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gdmjgmhkj.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/gdzqzgrdh.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/gxlywgxpf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.bbcook.cn/Article/details/gfrsxslrk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gygipcslh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/ghxkgqoyz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gdlzhjrzi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/ghoqizaml.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/guiyecklz.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gfhkzxfwh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/grmagxsrx.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gfcseexlm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gcmkijbav.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.sjlbkw.cn/Article/details/gucnkbsup.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gkhappxhv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gacunzuja.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gvpbxouza.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/grqapjnlw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gflnejazi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gzqlgfafb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gprsctpni.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gsngnyhfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gyfglzzik.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/gpphtkhwm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/gldmphuyp.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gvruvtjzh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/gfcvvbhiz.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gidivgpts.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gyirltkcj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gnouangmg.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/grmuhdxxd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gkfrcyvsj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gdsnilnvv.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gzgcomwff.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gcwbylmne.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/gkmfldqhv.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/glpwldrmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.sjlbkw.cn/Article/details/gnhhwmoqe.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gkygfxakj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/giebxvkfx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gxdkeptgj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gdfeoguhp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gcjepxzny.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gertwclgv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gqmsscueu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/grbggvvvs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gdkbwoeup.sHtML


<!-- 参考信息 -->