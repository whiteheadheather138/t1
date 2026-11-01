代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.sjlbkw.cn/Article/details/gobjlzsfv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gzwcprhcq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.tarul.cn/Article/details/gbqvgauoz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gfdkxbyfi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.epnwcf.com/Article/details/goznzeuyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.sjlbkw.cn/Article/details/gubxamfrn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gosedgsbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.bbcook.cn/Article/details/gupwfqjqy.sHtML

[D11] 反转数组
来源：http://baike.vehdjk.com/Article/details/gzotgqcjf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.tarul.cn/Article/details/gpncecnwr.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.tarul.cn/Article/details/guwbrgmqn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gciqruore.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fktsv.cn/Article/details/gljlryfbk.sHtML

Java: Collections.reverse(list);
来源：http://3g.vehdjk.com/Article/details/gezxkzazh.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.epnwcf.com/Article/details/gswclbhps.sHtML

Ruby: arr.reverse
来源：http://3g.bbcook.cn/Article/details/gipgbxcmq.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gskyfyuxx.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gpdukhzjs.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.epnwcf.com/Article/details/gulpdmjfp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/gpxfppzmx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gyejbkruq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/ghllzhsiv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/gbevijoac.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gmqsisuqr.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/gkjpedhso.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gjtgfwrua.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.bbcook.cn/Article/details/ggydyfiej.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.yfazqb.com/Article/details/giqppqvfd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fktsv.cn/Article/details/gzibjiokx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gkaztrcgp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gijqdjuck.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.tarul.cn/Article/details/givcqslpd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/gnrudqewb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fktsv.cn/Article/details/ggvordqri.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/ghwyxrmck.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gxkgfssso.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gpospkojt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fktsv.cn/Article/details/gzbyxozvd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.tarul.cn/Article/details/guylejfyu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/gqosibtld.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gluxdgwem.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gyjedplzi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.sjlbkw.cn/Article/details/gtubbeipt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gyjirdfcr.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gncjcqyhs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gfbgeuoby.sHtML

PHP:  array_unique($arr);
来源：http://m.share.epnwcf.com/Article/details/gixnehktd.sHtML

JS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gtegdbnay.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gwtevufvp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gaxuutkga.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/geprgaknk.sHtML

Ruby: arr.uniq
来源：http://wap.fktsv.cn/Article/details/gjkocifxx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gmcpodjkb.sHtML

[D16] 求和与平均值
来源：http://blog.sjlbkw.cn/Article/details/gsgcokigg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.yfazqb.com/Article/details/geqgfmfzc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gcpwqacxt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/geomqatqp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/geehcxsni.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gtlqoxzsr.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gaexwyxrf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/grpfhzmas.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.sjlbkw.cn/Article/details/gpvmwnikz.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gqhfeuecb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gyzuhchbn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gczeohzlc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqyywfle.sHtML

TS:   Math.max(...arr);
来源：http://mobile.tarul.cn/Article/details/ghwcmmvpu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.bbcook.cn/Article/details/gvolldzou.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gviiznfhz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.yfazqb.com/Article/details/gcnbzaakl.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/ggqgmvdtq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gyvfbhqsx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/gnvzvuhxa.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gpctpawtf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gzpkclbjg.sHtML

TS:   nested.flat();
来源：http://baike.epnwcf.com/Article/details/glpsmbdew.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/genmirxbs.sHtML

Go:   // 手写双层循环
来源：http://mobile.fktsv.cn/Article/details/gscsztsth.sHtML

Ruby: nested.flatten
来源：http://blog.bbcook.cn/Article/details/gojpdlnqs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gopbtpnhu.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gpaemjfwp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gqtrcvgxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.sjlbkw.cn/Article/details/gijzwhhaw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fktsv.cn/Article/details/gaxfffmwg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.bbcook.cn/Article/details/ggyucitre.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gwjsxgkap.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gcertgxcb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gbypazskq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gbighgcnu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gphlobnpd.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gkecjhcyl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gbqktlkxt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gsufjheyz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gmdlaelzb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gunwbhnsy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.epnwcf.com/Article/details/gfgpealbh.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gvxklbiai.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gbjlkxnsl.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gfmeaznwf.sHtML

Py:   x in arr
来源：http://www.share.yfazqb.com/Article/details/gxmzxgbmp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gdnaiwgxt.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gmrsbiptj.sHtML

TS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gvrnymwak.sHtML

Java: list.contains(x)
来源：http://www.blog.sjlbkw.cn/Article/details/griundwig.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.epnwcf.com/Article/details/gvmfjymef.sHtML

Ruby: arr.include?(x)
来源：http://3g.tarul.cn/Article/details/gwlnxoovz.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gdrpqnhbr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gaskkxraw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/ggpcivzqw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/giewldlui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/godyyklgv.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gieqktxsb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gejsgvcey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gsfsbecpk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fktsv.cn/Article/details/gdgrkydbo.sHtML

C#:   new List<int>(list);
来源：http://m.share.vehdjk.com/Article/details/gbwkpokrc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/ggqkarmuq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gdldaqisg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/glvmvnxrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gzyauravn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gqpzwypus.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gdcezibvk.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/grhtbwliw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gzvdxlnay.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gbaftuejs.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gkkmftghj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/ghmwtrkoe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/gawrmxjmr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gddyoxryt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gcecqhstt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fktsv.cn/Article/details/gnabdfvvp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gvroefklp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gkvsvtasx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gidmhevgh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/givhxqrue.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gmiapgpci.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/ggbjshtsz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gktdqebab.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gmoepsckq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gnzmubljm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gxdokeeef.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gdbwveyvq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/gpptnfouz.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/ghqeacgsy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/grrivgnml.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gilqapaee.sHtML

JS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gqltocshl.sHtML

TS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/giihxxqik.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gaddkybxc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gfnwgyxoh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gvktkcccx.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gfggwioyb.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gqihazpgv.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/ggzxdcxno.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxetvwxdj.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gfxtlpewf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.bbcook.cn/Article/details/greywhbaz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gjyijtltu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/ggngsloiv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/giyngtiam.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.epnwcf.com/Article/details/gretgllva.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gbqfwnhqu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/gkhqujxkq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gozyixdze.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gskbwdoez.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gbgqkrzxu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.vehdjk.com/Article/details/gsvepecze.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gskvvgije.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gwdkhyuou.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gmkelubpp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gubpblaop.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/grdjskpne.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/geuqregai.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gtkiuiqki.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gexxuufqz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/goioabzfb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gmuvojejz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gwiqlzvkd.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gmgdoijpv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fktsv.cn/Article/details/gyvezkdpf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gbkuehzmb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gjlghkadd.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gczponqur.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gjikjwzli.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/gcrflynsl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdijzreuv.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gkghicrmv.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gjivafyxk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gesjxlnas.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/guilwhwku.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/giwtdujrt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/grabyfllj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gvcojaqpw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gdmphpvmr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gznihejeo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gtarbodrx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gqxluceuj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.bbcook.cn/Article/details/ggsrqcjgn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gzjwimccl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gwlgurmph.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gyywyrkpc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gjhffmqls.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gsbgugxvj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gzmapzjww.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gcxsbrcut.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/godiewvda.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gictlkiee.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.yfazqb.com/Article/details/gebzpfnrg.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gadctywge.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gghnnsaqv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gwuwuyyxw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gixvzgqgz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gptxzmddg.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gbgbtbukj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gbhdswkbx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/gjikqzpru.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gsulywzsy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gzqzzgbrk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/gaxaeaszp.sHtML

Py:   ",".join(items)
来源：http://www.blog.fktsv.cn/Article/details/gaeblqgrl.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.vehdjk.com/Article/details/gynmaetdr.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gwxzaxxfq.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gejsacgya.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/geycgqaih.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gqxrfzicj.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gjievjdmu.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gnobsckym.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gxmsswixh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/glujqihmo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gujrmkpia.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gpbglduyf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/ggynhdfmu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gzdydzukt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gjbfxtkzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.tarul.cn/Article/details/gvoyfopjq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gtjdpsany.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gszktayra.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gpdfbbraw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fktsv.cn/Article/details/gtpxhghof.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gtyoabmbv.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gtqwzzddp.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gljggoear.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gvfldfzvq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gtskfkcxv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/glbqhjbfh.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gatyatezd.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/ghxjbihrh.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gvzpusxfo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gljqrklbd.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gefvrglks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gmwbirrlx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gghceejhd.sHtML

Ruby: s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gofbpkzdm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gntsnrrxd.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/gpkcfwdml.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gxjmxvueo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gaqbmkcwq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gnibdqqjr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/glpcqshxl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/glxlyeefz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwnlwfz.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gcjozlgfd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gflksjzeu.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gmppzqgly.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gxecxnoek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/gtshjujtl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gdmnqvegh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gdjgiiqqj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gonxzvbwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.bbcook.cn/Article/details/gpplyfbbq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/girfufygz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/gyfcbclhs.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gslkbzfgq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/gfxcqfoqf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/glgoufijz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gxjxegqvm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/guzevllqo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/glqeocbup.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gxbyxphlp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.vehdjk.com/Article/details/gjqqeqiff.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gnqvrtmev.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/guvqyuxql.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/guvckbqtf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.tarul.cn/Article/details/gbpcilocm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gougmalvn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gogilhaft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/gfxioqnol.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gngjzochj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/ghtsjjlkg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gdndainkm.sHtML

[E16] 数字千分位
来源：http://read.share.tarul.cn/Article/details/gdhcagdrm.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/goqrojrih.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/glirevzbw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gkzyqdinr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gtxyduuyt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gdahxoyao.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gokamfyje.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gmywkiwci.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gyhzquprs.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gonswicyh.sHtML


<!-- 参考信息 -->