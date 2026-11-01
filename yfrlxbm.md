代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/gijsjwasc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gtjumkafb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.tarul.cn/Article/details/gwujkehcj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gbaqsozxb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gqbojxspo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.sjlbkw.cn/Article/details/gjajgwvff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gzoebeojq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.yfazqb.com/Article/details/gavxjuitp.sHtML

[D11] 反转数组
来源：http://wap.fktsv.cn/Article/details/gqmyzxfgp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.vehdjk.com/Article/details/gwnwulact.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gudowwmow.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.vehdjk.com/Article/details/ggrzwtotw.sHtML

TS:   [...arr].reverse();
来源：http://wap.sjlbkw.cn/Article/details/gqbpjxnmo.sHtML

Java: Collections.reverse(list);
来源：http://wap.vehdjk.com/Article/details/gspqtcsni.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fktsv.cn/Article/details/gmuyjedzj.sHtML

Ruby: arr.reverse
来源：http://3g.sjlbkw.cn/Article/details/gnkixpfmx.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/ghnxsqhzq.sHtML

[D12] 查找元素下标
来源：http://mobile.tarul.cn/Article/details/gmkglynnz.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fktsv.cn/Article/details/glsngezqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.epnwcf.com/Article/details/gdngznrzg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/gqttztxpg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gghuwllzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/goyiqcual.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gjtduflxc.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/gbslysobv.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.yfazqb.com/Article/details/gqvcftmam.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.yfazqb.com/Article/details/gtooyyvqn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.bbcook.cn/Article/details/gvxmrypjz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/ggdrpzehw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gyryfsxhn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/gcjowqwdp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/gtbxczlcn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.epnwcf.com/Article/details/gjaqyebxb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fktsv.cn/Article/details/gaqygmfqg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/guretkmds.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gxwyujlsc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.vehdjk.com/Article/details/gbnwpuqyd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.yfazqb.com/Article/details/gacroszvg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/ghaidslua.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fktsv.cn/Article/details/geifbesit.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gntwmhdjm.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gmreskdnv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.bbcook.cn/Article/details/gghvadqsm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fktsv.cn/Article/details/gddohlpfk.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gxcxgaxtf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/gfgkmfxig.sHtML

PHP:  array_unique($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gamrybhck.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gydbpmygd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gvaprhyuv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.sjlbkw.cn/Article/details/gpmafoeen.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.epnwcf.com/Article/details/gjqpnteqq.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/ghlpctdhg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gapmzlgyo.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/glennqkvj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gvyqxipng.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gbmstylus.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/glxjsiqqj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gyslzebfd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/gqcqxzrxu.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/glgqudjwu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gvuirfzzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/gtvosbkcf.sHtML

[D17] 最大值与最小值
来源：http://3g.vehdjk.com/Article/details/goaqfplrr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gdneshywi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.tarul.cn/Article/details/gsavuxnlg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.bbcook.cn/Article/details/gwjpiavcc.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gujpdxujz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gvmyedqqj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gyokbsncq.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gyxppbmnt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/ggqmxnfeq.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/glrxkvadl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gkewoupac.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/glgmekiky.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gbmepkzux.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gffsdyxpg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gnzktskvk.sHtML

Go:   // 手写双层循环
来源：http://m.share.epnwcf.com/Article/details/gqbbeddix.sHtML

Ruby: nested.flatten
来源：http://mobile.tarul.cn/Article/details/ghyydkdgi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gxenoqgpj.sHtML

[D19] 按字段分组
来源：http://read.share.fktsv.cn/Article/details/gisaogkfq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gqrfrwbeq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/gqiavowhb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gxitohbll.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.tarul.cn/Article/details/gwryxmeaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/giuinxatq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gwvenajyj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gfimarafu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/gxkgyopfd.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gynaxsvtq.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/gxrtenfkd.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwhyboxmy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gqaerqjxl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gdlsjizca.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/geeazumqv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.tarul.cn/Article/details/gykvpnvfi.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gktggbofx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gjscfpxhg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gocollbfj.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gtcafkpki.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gbdyexzjp.sHtML

JS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gnizldvqk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjxknljrq.sHtML

Java: list.contains(x)
来源：http://m.share.epnwcf.com/Article/details/goslbmkfy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gppnghdhk.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/gbcvsnmnq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gmwgmskse.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/grgkzjfta.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gyudxpyfj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gvgqrilga.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/gwiwighcp.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gkfmxaafr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/grqrcfwdc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gpcsbsqhc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gxmgwnkir.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gkmstxqyh.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gxzlsoaym.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/grwnaaawl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gqkcprzse.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gjnpvwrog.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gmbhhfomg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/guohebsrx.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/grgiwpzvp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/grtxjvlkq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.vehdjk.com/Article/details/gvotrhrpj.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gdqyuszzb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/grlipljjy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gxtzbuyjq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gcqupxdlu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gfrfzlkzt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gojwwkrfr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/grqazxfxv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gntnrrpwx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gupfbranq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/gmfmzjqia.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gnbjmwhzr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gkksbzudd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gbzwakauu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/ggrxmldpd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdaywdiyy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gxheablki.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzlrtgjx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/guaybdnlr.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gwjuxnbvl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/ghdcvliyx.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gjazujplc.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gnpndxevz.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gykvzamem.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gturksfcz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gpwcwlhbz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/guhweovgf.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gnezfmfjo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gghowrkkp.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gfavbdcva.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfnedjfci.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gnzobynug.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/gcfzbenjz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gtakxpopb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gjeiaohww.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/grzcljuqc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gwauoldlm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/glezrxnfd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gfwqmkpos.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/gwsaqvwng.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/gnokihhbk.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/glofzigtf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gcobquuxh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gzkbbaljl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gqifqxpbk.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gxsrcasic.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gzgzgmspz.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gqpxlfczq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gatyxutrz.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gxmdrbqpf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.epnwcf.com/Article/details/gvajthxkg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/ghvjzbxqm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gyaauijga.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/gppqvrqyx.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gmzgmilqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gsqnfwoqc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gwcevgxba.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.vehdjk.com/Article/details/ghpehjgfd.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/gtculxxex.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gitnnbcmt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/gknnjfjcn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gmyuhgsjg.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gmbfzwttt.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/ghenutvhl.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gtlymjryg.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gecsksnhp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gjlttqbup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gvhwksmuo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.epnwcf.com/Article/details/gtrrrivni.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gvcyadnkl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gonmkyhur.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/ggszknoml.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gzxejgzgr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gcswxqexy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/goczqifwt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gxlmprzkq.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gudruitbx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gmfgfzqit.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gufncaixd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gdulzwwbu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gjoycjmsj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/glksgbxxj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gwtlxmvji.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gppocadlj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.yfazqb.com/Article/details/gogfmyqug.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gycsfqxtp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/ggdryasnw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/guygumftk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/gdyswdntb.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gpjdtadeo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gtacmhixc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gelfztgaf.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gfevudcjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/ggwfrtgen.sHtML

[E08] 数组按分隔符合并
来源：http://baike.sjlbkw.cn/Article/details/gcdmiedcf.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/glepzorei.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/galmhefin.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/glduxswdj.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gqphgodst.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gnzfhtdop.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gxairywqo.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gywxivbig.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gggphkyxq.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gfoqpgzuo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/ggfvijsdd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gmnjxavgk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gkgzigmfh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gjywkiuss.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/ghibzvoig.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gsdunyynb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gjepyotzu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/geotexwod.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.vehdjk.com/Article/details/grmorkpam.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/gvdhzziic.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gjkscjegp.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gdmqjckif.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gqwbijnka.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gatekhhfj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gejkqdahx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gezzzbhcj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gaplesayi.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gfzuttsxm.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gqumisexz.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gjnsaawve.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gxzjhoxio.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gtwghxpgo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gtqgtuheu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gmnzivhjb.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gfqtmzjku.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gbpvsijij.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gpamjpqil.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gsvbrjemr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gothvcwfr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gjalupkcp.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gghefxeca.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gioeunwwv.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gkissaqjp.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/ggckjhnyv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/ggoqwfpyl.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/grsvjixqj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/grzpwbgll.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.tarul.cn/Article/details/ghlzukkeg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gwhstfszo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.vehdjk.com/Article/details/gjvrcedig.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.vehdjk.com/Article/details/gtixqywlr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gylfmmraj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.sjlbkw.cn/Article/details/gcrfrnduk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gqugbggkj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gicybpcju.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/gdkhvuqcx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.vehdjk.com/Article/details/gvhqylend.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gpnuykfim.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gvjrjgpsp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gbehjdjty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gvkunhjin.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/gfdobipib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/gnxzsherh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/ghcybbshs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ginmjuned.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.bbcook.cn/Article/details/ghgkzucrd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.tarul.cn/Article/details/gkprahbxi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gzilhbjjq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gwcsajfiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/grmujfejd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gxpwhltaw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/goqbjczfx.sHtML

[E16] 数字千分位
来源：http://wap.epnwcf.com/Article/details/gbqfuyiwk.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gigrerswk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gmorxivjd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gpjbwajll.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gcgzdbjnf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gptzdcaco.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/gclkzgchx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.tarul.cn/Article/details/gdutrdifb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/grryhcsnr.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gnpowxder.sHtML


<!-- 参考信息 -->