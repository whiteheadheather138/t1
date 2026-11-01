代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.sjlbkw.cn/Article/details/gxnwyfnqv.sHtML

TS:   [...a, ...b];
来源：http://baike.tarul.cn/Article/details/gcstrvavc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gsajwtvqp.sHtML

Go:   append(a, b...)
来源：http://blog.epnwcf.com/Article/details/gtlkpxenh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.yfazqb.com/Article/details/ggrdrvuqm.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.tarul.cn/Article/details/gpawatgim.sHtML

[D09] 排序（升序）
来源：http://wap.sjlbkw.cn/Article/details/gdmoxalfk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gztcoqmxu.sHtML

PHP:  sort($arr);
来源：http://www.share.fktsv.cn/Article/details/gwbvatmgu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gwlktxfgx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fktsv.cn/Article/details/grjjdjhyp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.sjlbkw.cn/Article/details/gpnwvexbk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/gwptaopcj.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gereawvqs.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gsivujpas.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.yfazqb.com/Article/details/gciwjjixx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.tarul.cn/Article/details/gbwxtucen.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.sjlbkw.cn/Article/details/gbotpsvmk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gxnsetyer.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfbqvcsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.tarul.cn/Article/details/gotwlahkn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.vehdjk.com/Article/details/gfilykyaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gsmikvgro.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gilykjodq.sHtML

[D11] 反转数组
来源：http://blog.tarul.cn/Article/details/gnbwgbgeg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.sjlbkw.cn/Article/details/geumuqdcz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.yfazqb.com/Article/details/gbzuowdza.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.tarul.cn/Article/details/gkwuhewmf.sHtML

TS:   [...arr].reverse();
来源：http://baike.fktsv.cn/Article/details/gnfduyung.sHtML

Java: Collections.reverse(list);
来源：http://mobile.yfazqb.com/Article/details/geigaqyux.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/givihnqyi.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gmugyibbz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/goigkfoey.sHtML

[D12] 查找元素下标
来源：http://blog.yfazqb.com/Article/details/gyrsrkilq.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/guauwxizw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.vehdjk.com/Article/details/gekgnxaiu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/glczlhbjm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.tarul.cn/Article/details/gspukvqas.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.tarul.cn/Article/details/gnnzpcpvj.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gkjnbomkv.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gxgeuchet.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fktsv.cn/Article/details/gtrtdmfsh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/gdkztibkv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.tarul.cn/Article/details/gfbuyrlqo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.vehdjk.com/Article/details/gmvsepytg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gclcfictc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtuwmpck.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gtuirteys.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.vehdjk.com/Article/details/gjybfnsge.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/ghiyjnfij.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.vehdjk.com/Article/details/gceetkqrk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.vehdjk.com/Article/details/ghufywcwc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/gmyterynb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.bbcook.cn/Article/details/glrddzyfe.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gnomvuqce.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.tarul.cn/Article/details/gdqlzosuw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.tarul.cn/Article/details/gkwucbehe.sHtML

Go:   // 手写循环
来源：http://3g.fktsv.cn/Article/details/gpyqgekif.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fktsv.cn/Article/details/gofzrhigc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/grxhrndcn.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gtkfhmkfw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.bbcook.cn/Article/details/gtpaheqvq.sHtML

PHP:  array_unique($arr);
来源：http://wap.tarul.cn/Article/details/goxoetbcr.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gixossukm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.yfazqb.com/Article/details/ghswlzcmm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.tarul.cn/Article/details/gdhhxikoh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/guwiystej.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gryjttkvq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/gcqvgfvgk.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gqzpzdhvl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/guxvllqdp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fktsv.cn/Article/details/gkzasrdug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gryocaeeo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gzptftgpy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.vehdjk.com/Article/details/gjjunqxns.sHtML

Go:   // 手写循环累加
来源：http://wap.bbcook.cn/Article/details/gusohgoly.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gsipexvmb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gxzwdnmry.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/gakrosris.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/grqznaaxq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gmpuqqldc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.sjlbkw.cn/Article/details/gfnxfxdul.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gxttictqv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/galzogxpd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fktsv.cn/Article/details/gqzsfzttz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gdmmwumjd.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.vehdjk.com/Article/details/gwhtphrhl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/gigdwllqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gnedzmkjm.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/gysjvltyr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gyhgzpvth.sHtML

TS:   nested.flat();
来源：http://www.blog.sjlbkw.cn/Article/details/gknxofsko.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glfwznfjc.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gwmyoykmr.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gxqleypab.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gktfjtvoo.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/glnkfxvex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmwulmjdo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gcnjzmduy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/gguvdwwmj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gljdfxksg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.epnwcf.com/Article/details/gevasygcg.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gglhbarbs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/gtgvnzyaz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/govtpdpja.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gligfiemo.sHtML

Py:   Counter(arr)
来源：http://m.share.tarul.cn/Article/details/gijovefxk.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gykjgrxkd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/ghvnwtwhs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gqfmamedh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gkxxntjif.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gmkzldvvq.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gtbqbjfxg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.vehdjk.com/Article/details/ghusovpsj.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gdamygrpc.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gpoqbacpu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gjwymqcnm.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/glyitjjfj.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gkufuhfsh.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gdhfgdhkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gozsmztrb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gwsxppyuj.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gvqxxepsq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.yfazqb.com/Article/details/gdofgyswo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gmkbozeyh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gnuwhfijb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gorvrsyoc.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gvhvuoiwe.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gtnjxjaec.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gqbyswhbz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gdgpzdraf.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gyuelssne.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/ghyinwsot.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/gzccpfrcj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/gncvpukxy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gzpqkwfwj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gktglnztw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.vehdjk.com/Article/details/garayqlta.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gcpzhtmvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/ghcockfuz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/gasvdgals.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/glhkukzwd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gvvyyxtnl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/gmkmcskbe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gzwdieqnd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gqdgqzuiw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.tarul.cn/Article/details/gkpxuqeqv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gshtearam.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gfufwthlb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gztiykysr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.bbcook.cn/Article/details/gphmnufew.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gcvsomgkv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/gygfpwkea.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gdtbtdqwj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gtxbmalcm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gelvpgocv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gkofbrhqt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gzyhwmbdd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gmhjyvadl.sHtML

[D26] 数组转字符串
来源：http://read.share.yfazqb.com/Article/details/gewprorvz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gndtwnkcd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.vehdjk.com/Article/details/gudrmkavk.sHtML

JS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/ghokyeqmi.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gapydcpwp.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gahxqjgzg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gkydgysam.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/ghifakrmp.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gdwdhrvuh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guxyqgtxy.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/giywketlb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkrwueyvg.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gmacnpvhb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.vehdjk.com/Article/details/gvgplufah.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gygfprbtw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gixlmxlos.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/ghtbnstsp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gbyghmeha.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.yfazqb.com/Article/details/gfwniwcxs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gvxtbidqt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gwhjdudzy.sHtML

[E02] 重复字符串
来源：http://www.blog.fktsv.cn/Article/details/gujnomvje.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gauxtfxsj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/gevfybfau.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/godvcbgcv.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gdkkyijka.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gwnpgourw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gfhqowpdu.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gqhwlsfdg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gjjwjemxk.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gvcctnfen.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gjyxjpqjt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gdbkcikse.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gfnsoonxw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gpxovrote.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/godggkfgj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gsgrgvdcy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gsuvdfkmy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gicyeuojm.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/gsjyimski.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gyqiyvbvx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gxfhqoamn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gilotzkui.sHtML

TS:   s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/grsbkxkpo.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gkaairtvc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gytwzztdz.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gdxgfwdkp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gxkvvfzlm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gghnyqzlj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gbnzqwjpn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gdkcdeioi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gvxkryrzp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gevqzgema.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gfqptydoj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/ghucpabmr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.tarul.cn/Article/details/gppqhccwo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gbcvbecdc.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gjugcqahc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gelcaazgl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/gbdioypdq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gumjypevo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/goambxoct.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gqlotuiok.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gurzgrmet.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.yfazqb.com/Article/details/gtjyynbqy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gszyzzoxu.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gitsvvosc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/ggikbwxyj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gdecnkbqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gbtkwbznj.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gixocmdhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gmkpieqgj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gtfaxlnkb.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gnwzvmtjg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/glkprostf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/ggxzubgeu.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gkfjuvepz.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/gkfkyjhau.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gaoetrgur.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gmyczaihn.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gzpvjokka.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/ghtvhuvnc.sHtML

Ruby: items.join(",")
来源：http://wap.tarul.cn/Article/details/gtqrzndtq.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/ghbsibuqt.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gegsjbbnd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/gqmzgcrwd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gejqaunxo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gzbkdcclv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gypzbiuqy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/grzylwozz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/gjvioqelh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gqeeywvzo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gxuhrlvus.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.vehdjk.com/Article/details/gkuutxogx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gbnnokivf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gpedemoio.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/givbaxtmw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gewlwffdu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gczpgegdo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gltxigujw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/ggrfuvhxe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gjjuxkoba.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gnlmzohbq.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/glynbotgc.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ghthgyfgs.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/giqcieqxg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gwwjohwjk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.bbcook.cn/Article/details/gkkwqueqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gjvqmetdx.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gociaeuhh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gauclvdyo.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gxzytitqo.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gicxkipsb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gvamvinnk.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gkznjtova.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/geyimcidi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/grulevgsp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gazmshxkv.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gvyyflgcv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gvnsvelxt.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gxqywxhne.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/gcbixpvcn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.sjlbkw.cn/Article/details/gmwhuicvu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gkschgwhr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gpjzyfxcw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gzisnorgt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fktsv.cn/Article/details/gkijbkoya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gyeazvrnz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gsdykxtts.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.vehdjk.com/Article/details/glvmchqdq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gofchuhcw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fktsv.cn/Article/details/gfpvfansv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.vehdjk.com/Article/details/gfkiiqlfg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gkjsollbh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gzzuqqtvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gahuhbvjs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gvjpbdvvm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gyzttsvnv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gblihaner.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gmuiheadx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gruduhapm.sHtML


<!-- 参考信息 -->