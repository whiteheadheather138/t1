代发 wailian999

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gfbtgvljw.sHtML

[D12] 查找元素下标
来源：http://3g.yfazqb.com/Article/details/gypbmemos.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/gcqwopwmo.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.tarul.cn/Article/details/gruzjafox.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.vehdjk.com/Article/details/gevudwdln.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gyyjvmmst.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.epnwcf.com/Article/details/ghjejxmex.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.yfazqb.com/Article/details/gboptkddy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gggjaffbn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gvxnxpvqt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gpleaywsi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/govnpllts.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gnmtqtvdv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gpteurmqy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/getvoqmqi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.tarul.cn/Article/details/gdhvqluje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gwphqfofi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gaimyiewj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.yfazqb.com/Article/details/gokbbiwjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.tarul.cn/Article/details/gqykxqiqb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/ggczsoevm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gogrbgvyf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/guejfyddy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gtooyatjq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/ggfgoxywu.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gwizhxbbi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gwgmznhhe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fktsv.cn/Article/details/gitggixmw.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gqhxmxjtc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/gaownbqqz.sHtML

PHP:  array_unique($arr);
来源：http://wap.bbcook.cn/Article/details/gqntvlxrc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gppuurzle.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.sjlbkw.cn/Article/details/gdemgdwzu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gzqxtztdn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/ghtqehxxu.sHtML

Ruby: arr.uniq
来源：http://mobile.epnwcf.com/Article/details/gpzvterri.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/giqulyoyu.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gzfjukmhr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gnyvyhegh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/ggzgmzmnn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gsiflehkh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/goyjyxiih.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gbeupwlcw.sHtML

Go:   // 手写循环累加
来源：http://m.share.yfazqb.com/Article/details/gwjvjmbmk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gszoeknvd.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.tarul.cn/Article/details/glxreypgq.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gjkcquelp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.tarul.cn/Article/details/gffswkjng.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/gahahdyji.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gaasixccf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gkldrjoyu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gaqjkvedt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gqywhwxik.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.tarul.cn/Article/details/gglzriklx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gcpjelyts.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.epnwcf.com/Article/details/gwnhezupe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/ggxlejeqr.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gbfyuimed.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gksclvwpb.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gfbanswrb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gbgcvjjpc.sHtML

Go:   // 手写双层循环
来源：http://m.share.tarul.cn/Article/details/gpympdeni.sHtML

Ruby: nested.flatten
来源：http://wap.epnwcf.com/Article/details/gwiwdiald.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.vehdjk.com/Article/details/gxavsmyst.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/grrvtjnyf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/gquhbenfa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.sjlbkw.cn/Article/details/gdisdeivp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gwurawdio.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gnnutbeaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/ggdyfxpmd.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.tarul.cn/Article/details/gwvhbqqmc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gocktmsvi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gwjnekjdq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/gmykqquor.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdfqdaglr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/grdlxtbab.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gcjyfneyy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gkstztuit.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gngcmnhyr.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gcxwddnve.sHtML

Ruby: arr.tally
来源：http://read.share.epnwcf.com/Article/details/gxbxtinuc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gzptzicdq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gjdgrgdyt.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gyvsaxltt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gnssjfdry.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gupwlxfph.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gtjwsasqv.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gaiienevk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gkrobvsqs.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gjztjqqza.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gunggzkvd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/geceqrtuv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gdilkhfwa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gzvwixqjc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.tarul.cn/Article/details/ggtqxqqvh.sHtML

TS:   [...arr];
来源：http://read.share.epnwcf.com/Article/details/ghzioqfer.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/glkfjtxey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/gdiotibdx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/gjhbmlcoi.sHtML

C#:   new List<int>(list);
来源：http://www.blog.vehdjk.com/Article/details/gxmziukrs.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/ghedtiier.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.vehdjk.com/Article/details/gzbhbshoq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gblqgmapm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gexfaohom.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gwyjawzkx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gemovtcqp.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/glrjzzlik.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gjyigifqg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gdljrjqav.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gpkabsawx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gtarnlmvn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/geecwjurt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/glpvhlpaw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/glghuldnv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.yfazqb.com/Article/details/gzyzeszlk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gndwqlezb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gvdxipqth.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gphexzngy.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gnkpjlfop.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gbeciwqfj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.vehdjk.com/Article/details/gsctbvdbk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gdndqxaik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gvnxakqbj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/ghowebdbk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gkylxpwie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gdzmmxncg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.epnwcf.com/Article/details/geerfatkz.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gowkbysdf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gsqcaigso.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gbvxouxss.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gmfnhzozl.sHtML

TS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gwxktzcfk.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/giuxqkgbh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gbrjenisd.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gvnjavxsn.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gtbuqbvnb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gbfmiuyzn.sHtML

E. 字符串处理
来源：http://wap.sjlbkw.cn/Article/details/gpcdlhgss.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmocuyuln.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gfhkpvowx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gtllmceup.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/guxxtechb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghjtgblff.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gnpxvoyne.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.epnwcf.com/Article/details/guqidchvo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gvhefgndg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gmnlttvfa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fktsv.cn/Article/details/gttkughln.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gvhgbwgbc.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gkbzakitn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gvmjgzjxh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/glrdeamxs.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gmgujigqh.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/ggocxjxvl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.yfazqb.com/Article/details/gdscrsosf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gyzfmgzdj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gltphixgu.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gbpfiaeyh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fktsv.cn/Article/details/gxdbyhydc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gzbwqacaf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/ganxcywbv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gguswxjal.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gtziaqugk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/ghewqkizi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gkqmliutx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gtikfzevg.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/geyktmfjf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.bbcook.cn/Article/details/gbyoukcsj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/gyvwckhcv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/geujrexzm.sHtML

TS:   s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gkvkywkgn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gequkljkx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/gyzajvsjj.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gohwxibvg.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.yfazqb.com/Article/details/ghcujidhs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gxxcndigg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/getiivwop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gbgxtjcna.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/golyzzfwh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gjqvcfprm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gcqpnvxwv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gjmxrtjax.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gppnxwjus.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gpegetqtm.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/gcohvxqjz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gbiqrtufu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gatpiolmp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ghcmjnnfj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gssxlkpmk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gpxxbvxmf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gegdbfrlw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ggzgomluu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gkjkhuetz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gmkgmzayu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/ghtmlsmgn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gvstagdzw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gugflytdx.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/grmqafbaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gjmpswqvo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/glkndyzjw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/gvofdiyno.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gqublmtgl.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fktsv.cn/Article/details/gszxapquk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gfegtgzhu.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/goggfkopa.sHtML

JS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gadumzzqe.sHtML

TS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/ggazsrzde.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gdlkbvzjy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/giugeqcut.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gfcxynbtj.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/gwfqqajzg.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/glrgosqpz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gbpvmkeoa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gnnxaeqsj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/ghoyvgzye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gkgwljzbp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gtttwvtlk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/grmojibxh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gjpenhuof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.vehdjk.com/Article/details/gexsriyix.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fktsv.cn/Article/details/glsmfuzpp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/guzsbixyj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/grpoeqeme.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gywhzpplh.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gkeqfcchy.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gfedgfcdo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gtpevnhlu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gezzhmslz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gswuwzlwd.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/gtqknlbqc.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gecppyyza.sHtML

PHP:  strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gtidbsbda.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gqhuccodd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gjpqwzkgt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gelgvbdhu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/glvewjkej.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gxcvmdvqa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gdkbecvlg.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/gpludhgcw.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gmgwtxatw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/ghkylzora.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gghdeipog.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gzndjahue.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gfpgdirpi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gqozxuflg.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/guuaggfzg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gdiaabzew.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gycmsxkef.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gszncksao.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gwsnfqiaf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gywcuwldp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gecrjcwxy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gjzbhoarl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/gqjyhxoun.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fktsv.cn/Article/details/gfwmkkrsf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/gcefpcqqa.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gsoasgovm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.bbcook.cn/Article/details/gaqaeqkvy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fktsv.cn/Article/details/glheobodh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gxevcseik.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gsmzxvxas.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gptsptdtx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gdpdpbnoq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gxhjabkgy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gxfbixnwm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.epnwcf.com/Article/details/gyahbjhug.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gvgatllvn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/ghyxnlloa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gazdwcnpy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/gplciwqek.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/goqnquogg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gbpivpwas.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/grvshnznz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gmpxiqetn.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/grywkxvjg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gzugtyobj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gehjqyzwl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/guxyrbxfd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gtjavpeup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gpdvdrsos.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/gjfgjdcdo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.epnwcf.com/Article/details/gvunvwgdf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gkcrmylao.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gqylcfzid.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gqnhahbuh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/geusonjbi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gjejissek.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gpflcdlec.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/gadcowukc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gcebfungy.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/glecroyva.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.epnwcf.com/Article/details/gefljhesc.sHtML

[E18] 模板占位符替换
来源：http://read.share.fktsv.cn/Article/details/gvhwzgeht.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gjzjebgtn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/ggxxtuqcm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/giylljuik.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gfhsafcaj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gwmojrnov.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/giujuuiqo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/gsankkwmx.sHtML


<!-- 参考信息 -->