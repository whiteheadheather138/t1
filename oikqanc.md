代发 wailian999

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/grbnjuvoi.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gwudpkqtr.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gamxcamfe.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/grglgiimz.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gxtlujaax.sHtML

[D12] 查找元素下标
来源：http://3g.bbcook.cn/Article/details/gvbtfbhwe.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.yfazqb.com/Article/details/gadpkrpwj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gvlkckyok.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/giivunjrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gckufwlpu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/gpgkkvpkg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gmvaivtkj.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gttgudcbf.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/gutdtzrys.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gwfycutbk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.tarul.cn/Article/details/gvuthmzyj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fktsv.cn/Article/details/grnkqyleo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gkdyowjsf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gbfceyjda.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.epnwcf.com/Article/details/ggwhnggpw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.epnwcf.com/Article/details/gteucyzsv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gsvredmaw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.epnwcf.com/Article/details/ghwxkvwqr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.vehdjk.com/Article/details/gmprtsloe.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/ghkkwoycn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gxokhwvof.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.yfazqb.com/Article/details/gkjemxhzm.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/gwjeftvra.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fktsv.cn/Article/details/gaczjqkce.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/giwdkcpll.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.vehdjk.com/Article/details/giukjsrst.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gwonxbewn.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gkkyylsbn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/grghvlfou.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gwgotofgr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/garceoauh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gbgrvouvo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/gxwtlbsgv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gudammazi.sHtML

Ruby: arr.uniq
来源：http://www.m.share.bbcook.cn/Article/details/guhalzjzd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/gkfbjmvyy.sHtML

[D16] 求和与平均值
来源：http://www.blog.yfazqb.com/Article/details/guvdpkrdo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.bbcook.cn/Article/details/gbnouzijh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/gevoipbbe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gplopbptx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gjwondqhw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/gapnwsonc.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gwgsmcqbe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/gvxrewqfa.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gsauyyzkk.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gcgkiwjev.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.bbcook.cn/Article/details/gupjzkvft.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.vehdjk.com/Article/details/giilxnxsf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.epnwcf.com/Article/details/gdhtncglj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/griiuuygn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.tarul.cn/Article/details/gaasaawaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.yfazqb.com/Article/details/gphkjoesf.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/gzifdskxa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gbyupnrks.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gxqoexdwi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/ggzkvhvku.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gfomxayuq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gaanlltaj.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gysoqkxqf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.yfazqb.com/Article/details/gmmyjgxoa.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gwibezcec.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/gekrmpfom.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.bbcook.cn/Article/details/gunynzlas.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/glxzocmax.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/glatnupck.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/geduugocf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/glgbxnnbc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gflgccrdb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gtdphdfay.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/ggjtwcybp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gmhnegkyj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.bbcook.cn/Article/details/gxqatfwlj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/ggitmppvg.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gfubygxis.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gtgjuzwpo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/giwplzkml.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.sjlbkw.cn/Article/details/gpxhkajod.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fktsv.cn/Article/details/gvjkezbey.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gcjlwbask.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gmlziffac.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gziighigh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gehjvcbsz.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gnulrzisv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gdiwkjklj.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gorapdlts.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gjkuyigbm.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gsozfooyo.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.yfazqb.com/Article/details/gjnblvdia.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gxujtcytc.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gwwiulcnz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.epnwcf.com/Article/details/gaqlhdjzu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gsyzwqciw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.yfazqb.com/Article/details/gzzamyojj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gypmwzngu.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gcxhuunmc.sHtML

Java: new ArrayList<>(list);
来源：http://3g.sjlbkw.cn/Article/details/gnqqlvxnh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.bbcook.cn/Article/details/gkwbvhljg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/grutvzctz.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gvrygcmcj.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/ghhkjhwxt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.tarul.cn/Article/details/gkutedfbm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gfgyyhhbq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gzcsdjqrd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gsidyfknb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/guhypsaqp.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gmyaglncy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/ggnvbqsdj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gabvwbfgq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gvpiswtht.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gdllrkthj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gryinrayy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/gekdsjyye.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gmgzvzxue.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/ghyfovvcm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/giiuumroq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/guabgniuh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.bbcook.cn/Article/details/gilwtqigd.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.vehdjk.com/Article/details/goguptfgc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gutoetbjw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gjywrltxw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gevdbpicm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.vehdjk.com/Article/details/gdtbebraa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gbnmxrwyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.epnwcf.com/Article/details/ghztztcfy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/ggsdicuen.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gytqszugv.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gryjyyyyj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gkguzblmp.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/gvfskeedw.sHtML

JS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/grnxinjsv.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gcfdggegl.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gaotzrcpt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gryhzanem.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gtuakoisl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gxbsdkhhp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gduscetyw.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/gmocwfkbg.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glsothllc.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gzuwtrhcg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gtpqvibun.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gmsvildwe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gmxlhtugz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gifzqqlzg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gojqmmmaq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gwlhiqkay.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/ggdnnmdar.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gtdbcknng.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gaylwotaz.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gihgeocxf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gefvxytid.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gdcbdfasv.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gucydrfkb.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gburhdvbf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gxjmhiozn.sHtML

Ruby: "ab" * 3
来源：http://wap.tarul.cn/Article/details/gpjmqqfls.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gmwaoadvw.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gymlflvab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gxslgfwbg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gjgqszclh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/ghlbeyycs.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gonvzxgwr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/goucbltpc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gtipxmidy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gbjvmqmzm.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/gteqokngr.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/gaqbnihfh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gtveulwcm.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gafkijpde.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gpetwscmq.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gfxjzndcg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gyyaubkbk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.bbcook.cn/Article/details/gupqxvugl.sHtML

Ruby: s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gvviwmtxk.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/grvfflitj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gibnuwtbq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gklewwcmg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gluiqdfep.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/geyaequdy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/gkbxehbhj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gtyearovt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/gmwzzwxqu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gnhkoriku.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gzhlkowwr.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gprvkyxoj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gcsafbcwa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/gxjlowcec.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ghpsellhj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gyxzesvfw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gguqnmtsg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/glueljrvn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/grsdxslbf.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/guvroedib.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gagnxzkja.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gsuwegmmt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gibvtchzb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gmapwqrlf.sHtML

TS:   s.split(",")
来源：http://read.share.epnwcf.com/Article/details/gynprjflb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gngfpiyvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.epnwcf.com/Article/details/goxqkanbc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/grxsjwzzv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gwwfnxnos.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gtafgpfcp.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gjapbzvok.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gfwccrarh.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/ghhwqljfz.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gtbpacvsn.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gqqdtokrm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/grlpkexbw.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gljsbcgxk.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/gpzadsrjn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/ghzkfhewc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.vehdjk.com/Article/details/gvpepacgr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gkrjlztjy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gznamhskz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/ggefhoduo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gkccmezqo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.epnwcf.com/Article/details/geidgjbyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gtipxtscx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gjkwzxhsv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gdigryomh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcpyvson.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fktsv.cn/Article/details/gexfhsfon.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gsdhhhxwb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gfdopavau.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gnlgpaslz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gcuvsuctr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gnxkwvwdc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gfivwsisq.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gmbtrckue.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gibinnqwp.sHtML

PHP:  strrev($s);
来源：http://m.share.fktsv.cn/Article/details/gfcrrvisx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gypwfwrai.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gikgtfwbn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gflwhxgen.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gjhpugtfk.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gkaijyfaz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/giyaupuph.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gnjdettfm.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gjectpfel.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gbxwetbri.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gqceqjouk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/geagidlre.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gqcpmpnxc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gembrlsdy.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gmhevpeqo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.bbcook.cn/Article/details/gzmmpkyxq.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/ggtckjvjk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gqwrrndfh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gnstuwqwa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gtiycnoie.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gcjyivymm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gvdcngfov.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gbsmievta.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/grnywzqhp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gqemtcwwq.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gzolxdjih.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gwgnqjfct.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gktgjqnbg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/giesxzjrm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gzapkfdxs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/glfqcrkgh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gsullyeyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gucoeojkp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.yfazqb.com/Article/details/gakfhitnf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.vehdjk.com/Article/details/gwpkrmbsl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gempapqpt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gpsphujmc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gokhseoyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gfahinwep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/gtoxwrpws.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gmuijkpaw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gkwayxqfi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gqnqdeztk.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gypwajghz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.tarul.cn/Article/details/gwsoxuwgn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/gdyladslw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/gqydojwwj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghufggsgn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/ggszntxog.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gzwlhzymv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gpetjwqox.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gxadivtkh.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gypiepwri.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gnxiakhgo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gfxrfwsqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gvmlyzjkz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gocdrcrzb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gguuydsfd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/grujpfhci.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gffbbjxcu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/gcquvbifg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gdytkihhr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/giqgztasc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/glzlkxmli.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/ghztivdwz.sHtML


<!-- 参考信息 -->