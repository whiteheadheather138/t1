代发 wailian999

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/ggjitenlz.sHtML

PHP:  count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/goxmmmeog.sHtML

JS:   arr.length
来源：http://read.share.yfazqb.com/Article/details/gqunpqwlr.sHtML

TS:   arr.length
来源：http://baike.tarul.cn/Article/details/gnrpvnees.sHtML

Java: list.size();
来源：http://wap.tarul.cn/Article/details/gvajvbmub.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gkllsygjx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gpjjtgrui.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gcamjpfrb.sHtML

[D07] 切片 / 取子数组
来源：http://blog.yfazqb.com/Article/details/gaoduibjf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gytxxxjlv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gokolxfwk.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gfnfuvqyh.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gmbltqjhi.sHtML

Java: list.subList(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gfgpjabie.sHtML

Go:   arr[1:4]
来源：http://blog.sjlbkw.cn/Article/details/gfxwlgooh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.epnwcf.com/Article/details/gdqziwnov.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.tarul.cn/Article/details/gmucvckvy.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/ggbklcchb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.tarul.cn/Article/details/gykivtcps.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gkpkegkfi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.sjlbkw.cn/Article/details/gwhdhbrmb.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gygilqvgf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/geeheggfx.sHtML

Go:   append(a, b...)
来源：http://wap.vehdjk.com/Article/details/gmccxwlml.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gsrwugxrw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.tarul.cn/Article/details/gjbxqwzrv.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gxkqaxlyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gvdniqqbt.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gsvjtoynt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.yfazqb.com/Article/details/gefgpekbu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.sjlbkw.cn/Article/details/gvkfsvwkg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.bbcook.cn/Article/details/giqepwubn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gyfkuthle.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gukoermld.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/glqptdcbv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/godetwppl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/gdpffbitt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.sjlbkw.cn/Article/details/gvztheapo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/grwlxydvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.yfazqb.com/Article/details/gbwtifqmi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.yfazqb.com/Article/details/gkferucma.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.yfazqb.com/Article/details/gyggwnvlz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gflcndwao.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/goiswpssd.sHtML

[D11] 反转数组
来源：http://baike.bbcook.cn/Article/details/gazemblsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.vehdjk.com/Article/details/gjjaebuya.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrfqkaey.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.epnwcf.com/Article/details/gxsmjyrqj.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.sjlbkw.cn/Article/details/gjcbuqnpo.sHtML

Java: Collections.reverse(list);
来源：http://blog.tarul.cn/Article/details/geiaypvkx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gctdburno.sHtML

Ruby: arr.reverse
来源：http://baike.bbcook.cn/Article/details/gwzrajtgv.sHtML

C#:   list.Reverse();
来源：http://wap.yfazqb.com/Article/details/gcvmyfpnw.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/goczvhrfc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.bbcook.cn/Article/details/gsncctpda.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gbbrqijjh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.epnwcf.com/Article/details/geieivyaw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fktsv.cn/Article/details/gwdohiges.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gubojiahj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gmlslusha.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gxaohfpgi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.bbcook.cn/Article/details/gvlwdibsf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.tarul.cn/Article/details/gxllvpyiz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.epnwcf.com/Article/details/giessurke.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.yfazqb.com/Article/details/gbcbxehyd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gjfcixpbm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gcgjiotqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.tarul.cn/Article/details/gpbcfcesa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gzwvighck.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gfusydfjm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gzzuieumc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gwupcxckz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.tarul.cn/Article/details/gyljpbutd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/glnvckeka.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gqmlvlltq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gvkviiroi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gvghkodmp.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gxbhbgewx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gojpcejhs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gckwkphrb.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gyywmcekt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.yfazqb.com/Article/details/gjzoenfzt.sHtML

PHP:  array_unique($arr);
来源：http://baike.bbcook.cn/Article/details/gputijkde.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/goinnfnkh.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gxutipyhb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gajsdgfgz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/guelbmuuv.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gvfsdgxrl.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gevqawite.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gczvbabiy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.bbcook.cn/Article/details/gbyoblgte.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gkpizsydh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/glenlyzpb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gzjtacaah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gbstqylqz.sHtML

Go:   // 手写循环累加
来源：http://www.share.epnwcf.com/Article/details/gyfdbnwro.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gctmmvayn.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gmitskqaf.sHtML

[D17] 最大值与最小值
来源：http://www.share.yfazqb.com/Article/details/gwikyiihp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gmcvqnzqm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gkwubmcxc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/ggkrhfyyc.sHtML

TS:   Math.max(...arr);
来源：http://mobile.bbcook.cn/Article/details/ggrmygvis.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gevhhwmlj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gqzcxhlzg.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gijydzvcx.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gnpsxodsn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/guxqphikf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.sjlbkw.cn/Article/details/giufcsmmk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrfternw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.yfazqb.com/Article/details/gdaggbslr.sHtML

TS:   nested.flat();
来源：http://www.m.share.tarul.cn/Article/details/gieuwbwop.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gpmrqyjzk.sHtML

Go:   // 手写双层循环
来源：http://www.share.epnwcf.com/Article/details/gcqvkjtjm.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gfknamptf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gwshtrutg.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gbqailjjp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gncdxmkuz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fktsv.cn/Article/details/ggxlaljas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.vehdjk.com/Article/details/gwncywlsr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gljmmausj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gdgeqsvnn.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gjxfryuwu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gsyfnoiug.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.tarul.cn/Article/details/ghlnopxpn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.bbcook.cn/Article/details/goqfgzfnp.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gxayrmtlw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/guokggdom.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gthxrwyej.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gwiuyymrl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.epnwcf.com/Article/details/glfimsrpc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gslbqxxni.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gnrtdlpjc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/glhtswfmc.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/gqadhxfpf.sHtML

Py:   x in arr
来源：http://m.share.sjlbkw.cn/Article/details/gjhimxbvg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/golwskied.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gizitfctm.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwmutwddr.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/grpegvbtp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gxfxdxzgq.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gdfsfgqqi.sHtML

C#:   list.Contains(x)
来源：http://baike.epnwcf.com/Article/details/gvngfxmos.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gnxqfcjrs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gcantaqfj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/gsbfojqkn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gwopffjjb.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/ghghbnaua.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/gyuyqgtes.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fktsv.cn/Article/details/gugfwltwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gmdddkban.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gawedtkfu.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gjiekjuzs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/grytqohrm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/ghhqiikhh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gshojwgky.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gorxwbrlx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gkicmmqri.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/guqveftwa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/gxhncdzsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gwwxprugp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gqsynemnq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gsjlekbca.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gjkcfifht.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/glrlalwth.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/grhmsirow.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gmsodyciy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gbhzhsjut.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gjgbnbclf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gceftzmgi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gfuzrufuo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.tarul.cn/Article/details/gtjguspkv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gwabtashp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gvklysgzm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gfkefkeyo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/gbahqiakp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gceyklvbw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.yfazqb.com/Article/details/gsspmsuxj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gacsrqyni.sHtML

[D26] 数组转字符串
来源：http://www.share.yfazqb.com/Article/details/gdqkihxir.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/guwxlzaii.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gbdypaxaz.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/ggaflzlbd.sHtML

TS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gbnboemep.sHtML

Java: String.join(", ", list)
来源：http://wap.epnwcf.com/Article/details/geaydcbgw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/ghvxpyxdj.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gaqirraod.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/gqezbxzqk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsopnrjse.sHtML

E. 字符串处理
来源：http://www.share.yfazqb.com/Article/details/gdgkeqqmv.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gjzikfbgi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gcmakmkyb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gunwpodzz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/giiqkjwwf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/giyxsppip.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gjzbxsfbn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gbqxrnwoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gbdyahbte.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gnksojzbs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/gladwehct.sHtML

[E02] 重复字符串
来源：http://www.m.share.epnwcf.com/Article/details/ggjytxkuf.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/ginkvgclo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/guxntxqtk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gityspfkh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gwyhawcju.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gnvpjwssh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.sjlbkw.cn/Article/details/gfugkuzco.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gpdzhngvs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/garntoeow.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gdwcqruer.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gtzhbzxsj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gyuafrniz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gjkisnfim.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gdncikamh.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/grnisrfnr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.tarul.cn/Article/details/giodcfipi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/grvmjzwih.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gfotoewmv.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/gdgpoisxi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gzvlyflmv.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gqegvtrgl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gyrndqkna.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gdzhcarhx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/guxpaiigf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gbomhdbsv.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gclrlfnkd.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gnylcluyb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.tarul.cn/Article/details/gsnxscxiq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/gcljggtgg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gqrsxbzou.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/giudquoxc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gznaecsfi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gzvpvyrnb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gpdhcalje.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gixiqqkuz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gimlmiuff.sHtML

[E06] 替换子串
来源：http://3g.vehdjk.com/Article/details/grdalzztr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/geogzqhfu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/giohmcpmp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gionwnhuq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gibrbyzfx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gpfcfjjhx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gnouxdjtc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gyomypkrn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gqlhigpzw.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gbvjssuws.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gyowsoqot.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/glhjvaois.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gfofszdyz.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/giqzwynht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gwxflbpvv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gedccvluy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gtmkrlbvz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gpubpnafr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gncofsxee.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/glflmhdcu.sHtML

PHP:  implode(",", $items);
来源：http://blog.vehdjk.com/Article/details/gwzwpbyux.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gtvqndruo.sHtML

TS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/goppngwdx.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gpaurlyek.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.epnwcf.com/Article/details/gcxfzwnuv.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gxcuwvftm.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gqjwojklo.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gmuiyrjkc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gfkwqluvx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gnfuzkixh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/ghhunhcbg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gobkhvdbt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gjzqpjlou.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.sjlbkw.cn/Article/details/guylaglaf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gyqwcunmx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gvcuomlpc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gcyeuirea.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gxucjbvxi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gmoyofnra.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gnlkgsypj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gfcmwhaak.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gfggbihtk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gmaawikry.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/ghvbyfeat.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gybafhtoe.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gwxmxmsln.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gmnigoomp.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gejrkysfo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/ghwgbxxsv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/grrgvsmpj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gmuuycjoq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gkkhjbgeu.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gnpliapwc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gzsmdfjgx.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/gdvsbygti.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gbyxfkivb.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gcjhweenh.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gtnkjtvtv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gimqlsqtb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gulcjoexm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gcdhdvoxh.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gljtnqaug.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gcogtlgyl.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gyjrfromi.sHtML


<!-- 参考信息 -->