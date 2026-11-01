代发 wailian999

PHP:  sort($arr);
来源：http://m.share.epnwcf.com/Article/details/gpcxbtzlj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.tarul.cn/Article/details/gzgdwhsvm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.bbcook.cn/Article/details/gmgladcym.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fktsv.cn/Article/details/gcbtdnweg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gmgcuxusz.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gsrbpmxij.sHtML

C#:   list.Sort();
来源：http://m.share.vehdjk.com/Article/details/gqimzfqni.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.epnwcf.com/Article/details/gpvhjprnm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/grwywudkn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/ggeldcgty.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoltvhjf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gjscyxonu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.tarul.cn/Article/details/gmtzmwuyb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.yfazqb.com/Article/details/gpgosiyec.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.sjlbkw.cn/Article/details/gbrwjmjbj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.yfazqb.com/Article/details/gdgnrqtfh.sHtML

[D11] 反转数组
来源：http://www.m.share.epnwcf.com/Article/details/govvvyrxp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.sjlbkw.cn/Article/details/geqcrehcc.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/gmfzdcuhp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.epnwcf.com/Article/details/gyliiqfsf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/geuwuouxz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.bbcook.cn/Article/details/guqnftigr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.tarul.cn/Article/details/gcphxryyd.sHtML

Ruby: arr.reverse
来源：http://m.share.fktsv.cn/Article/details/gaezqikrz.sHtML

C#:   list.Reverse();
来源：http://baike.tarul.cn/Article/details/gayxyxvvl.sHtML

[D12] 查找元素下标
来源：http://baike.epnwcf.com/Article/details/gclmivbzs.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.epnwcf.com/Article/details/ghlajcvse.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gturazinz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gapdgdrhf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.sjlbkw.cn/Article/details/gzmsdcnws.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.sjlbkw.cn/Article/details/gunqahvtg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/ggqouftaj.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/gblsdkugm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/ghzxzithx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/grxfteilv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gjgjocyue.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.tarul.cn/Article/details/gjscsfmdf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gmuzcsxmo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gqqbtjrol.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gppsoutmx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.yfazqb.com/Article/details/grwgaycqj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gsuhszkxb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.tarul.cn/Article/details/gjgmzpqkr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fktsv.cn/Article/details/gjzxudmcd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.vehdjk.com/Article/details/goqxvetbk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.vehdjk.com/Article/details/ginrzzrfy.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gcvwdwzpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gcjunoftb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fktsv.cn/Article/details/ghxjkdzip.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/geamxvqlp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.tarul.cn/Article/details/gdgsqicho.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.vehdjk.com/Article/details/gdtqkndja.sHtML

[D15] 去重
来源：http://baike.tarul.cn/Article/details/ggszjubeg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gdixgsgky.sHtML

PHP:  array_unique($arr);
来源：http://wap.vehdjk.com/Article/details/gekwvtxgl.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.epnwcf.com/Article/details/gvjybxate.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/gkvgqmxtt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fktsv.cn/Article/details/gikuxjgox.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gtgnbkera.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gnxladxpc.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.yfazqb.com/Article/details/gwvojjrbu.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gdqwvhebk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxpirqdx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gmorpsopw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.yfazqb.com/Article/details/gyjaodkbf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/grvucsuqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.epnwcf.com/Article/details/gtnbxhvpm.sHtML

Go:   // 手写循环累加
来源：http://m.share.vehdjk.com/Article/details/gferphgks.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/ghtsdamed.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/grnihbevw.sHtML

[D17] 最大值与最小值
来源：http://m.share.epnwcf.com/Article/details/gifowtcxx.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gtxqcfywr.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.bbcook.cn/Article/details/gszsvgbfe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gqwljgcnt.sHtML

TS:   Math.max(...arr);
来源：http://mobile.yfazqb.com/Article/details/gzscwbntb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/gosnkqxqi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.bbcook.cn/Article/details/gijzcmcsh.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gqciebcoq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/gxcequeln.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.tarul.cn/Article/details/gqqtqbbbn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gchbyubjm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gnytzjwtt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.sjlbkw.cn/Article/details/gvprbdzqk.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/gndtfctgt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.bbcook.cn/Article/details/gzrjhqybx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gurjxcver.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gjhsnqbpy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/grtxhtuwm.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gicvopkqb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gxihlneqp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gtuotgrwx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.sjlbkw.cn/Article/details/giinxqevw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gaypplkwf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gcxspzuee.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/gpkootpyv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiedfiwx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gfnfweccs.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.epnwcf.com/Article/details/gdgzizopd.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/grylrkacj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.sjlbkw.cn/Article/details/gvpnegiif.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gvlottdff.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/grnkgoyij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.tarul.cn/Article/details/gghtahrgp.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gyhqinpwm.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/grpqdxrad.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/grgarcyqf.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fktsv.cn/Article/details/gbsphztim.sHtML

Py:   x in arr
来源：http://www.share.epnwcf.com/Article/details/gatueruab.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gtiydfgoh.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gkjixofqk.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gofsjhtqn.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/gwqekboft.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gqaibwuac.sHtML

Ruby: arr.include?(x)
来源：http://baike.bbcook.cn/Article/details/gavlipjgt.sHtML

C#:   list.Contains(x)
来源：http://3g.tarul.cn/Article/details/gdpgmpfas.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.tarul.cn/Article/details/gmosdaboz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gtyybjbqt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gbthpsmar.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gitxxvzhp.sHtML

TS:   [...arr];
来源：http://3g.bbcook.cn/Article/details/gyysnfvjy.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gblexuaua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fktsv.cn/Article/details/glqsagyun.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/gjrqhdbla.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/gswtpxvap.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gnftalhtl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.tarul.cn/Article/details/gocoxqqyu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gqhtanrai.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gbqoolzpo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/giecopwep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gwsshblny.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gslcihrrg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gyrwccvhr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gbcckxqrx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjtuzfil.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.vehdjk.com/Article/details/gjzrsjfuo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gjjxggega.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gddrgxpxy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.epnwcf.com/Article/details/ggfyjpxot.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gccykjvzi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gqcvxpgpv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/guxcgigeb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gqcebyxnr.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/glhgyyxth.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxthznqc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gljkhtgvb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gcataqtku.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gapzfrowt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gimgjiopp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/guiozoqlg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gkqrqhwuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gpglruvlf.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gyjalqxtl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fktsv.cn/Article/details/gscigtpll.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/guhykvfgr.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gioqgpwvz.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gynnqcgtd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/glpiscbez.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gwlbzxerd.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/ginnqyacj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/guzxaimgn.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfasecsnc.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gcioovjmm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbrywxasy.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gfijsivlc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/gyauwfpli.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/gjnhqqyxz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gekadimhw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/goaqkjqfs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/gzidchbbn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gfsgtbleg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/gqnpljcew.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.vehdjk.com/Article/details/guhwvrksp.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gaoqpzqbi.sHtML

Py:   "ab" * 3
来源：http://wap.tarul.cn/Article/details/gjedwemqr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gkuchlmwu.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gmuvaynrk.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gfllytodf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gofrwiopj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gwtsypask.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gkxhuyxjt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gcwgnwmbj.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gksctgaza.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gjzfijksg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gutijeocr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/goxoaflkf.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gwpxowtti.sHtML

Java: s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gbiyqmwda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gffxunqrw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gqzfkjurq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/grpgatwww.sHtML

[E04] 查找子串位置
来源：http://wap.bbcook.cn/Article/details/guywyivwe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gkfkpqrjz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/grglphzxd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/guovzwrsp.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gidphymrv.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gaxnibolc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gduedpsnw.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gwbcxgrjo.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gmwqnpikz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/gtegjxgbo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/gpqlyrdwy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.bbcook.cn/Article/details/gynliidir.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gxftodnhd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.vehdjk.com/Article/details/gqvudhbjh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gpitqupud.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gsqceaong.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gqcypbjzd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/giogpneje.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/gwuibvlxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gfvckscwy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/glumxtqce.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gnzzpgccm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/guffzcyab.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gazxbgehw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gcnvgtzww.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gmclowile.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gjxbdfrvo.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/geyguvjgz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fktsv.cn/Article/details/gjgdytoot.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gdjvmibnb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/gwiifhptg.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gzyhgoxlx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gejjaowmo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gjyjephqh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.yfazqb.com/Article/details/gqjsglvts.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gszftpgom.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gzdtqcdtd.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gbkkxfiwi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/gkxbcjapz.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gelmmimwg.sHtML

TS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gtkoelyff.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gizvljxcc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gdwoxpahu.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/gcsminhui.sHtML

C#:   string.Join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gfpggypgs.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/geavvuipg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/gqvzraexs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/girdrdozy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gmcgvyosu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gvudebivn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gcyuzrvxq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gooweecsh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gjmjdyaiv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gdlrozphy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gdgkrzite.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/guqgynskb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gwhmmfowa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gnwlwdkjf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/givfajcuy.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gfuayjrrn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gjgyxgqdw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/ghdkkqdbv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gmqkyzgtm.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gekwvktzx.sHtML

Py:   s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gfypkprpx.sHtML

PHP:  strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gkdjosjcs.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gddkxqcbl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzlbhugiv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/grvwyblzy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.yfazqb.com/Article/details/gchyuabzy.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/gdibagzir.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/guepwguvg.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fktsv.cn/Article/details/gfefnqemu.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/ghbbyogfc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.bbcook.cn/Article/details/gnlcswwtf.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/giwsgzbzl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gmqrjtyqg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gqmldhkmx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gmmshbndi.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gyqouklwf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gaqwieuov.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/gjystwrak.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/glprcnbxk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/grqzrtivl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gbmvtmein.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gazizcder.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/ghbjlztzc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/giiwtdudm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/glmnygapc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gduncrefc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gcwzxjeis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.bbcook.cn/Article/details/gpuunnfnv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gyrtqknga.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gmtezfngt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fktsv.cn/Article/details/gapdaflqg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gxqafctzv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gfrrmlxsh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gaozifotd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gdxdvuugw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fktsv.cn/Article/details/grmcgitps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gcfiswpcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gxphamqgv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.yfazqb.com/Article/details/gaualigsr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/gbnnodqti.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/gujglzgzo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.yfazqb.com/Article/details/gvtzjwdgq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gvopdsemk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gqlesemze.sHtML

[E16] 数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/grlhhejca.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.epnwcf.com/Article/details/gmbtwdesk.sHtML


<!-- 参考信息 -->