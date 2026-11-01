代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/ghgqchlif.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.yfazqb.com/Article/details/grapzlhwm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fktsv.cn/Article/details/gyiunvcbu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.epnwcf.com/Article/details/ggshktbar.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.yfazqb.com/Article/details/gsxtyjsyk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.bbcook.cn/Article/details/gtyvmmibq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.sjlbkw.cn/Article/details/gcrmarmrm.sHtML

[D06] 数组长度
来源：http://blog.epnwcf.com/Article/details/gftegzuvo.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/ggxlbroob.sHtML

PHP:  count($arr);
来源：http://mobile.yfazqb.com/Article/details/gyyckpnee.sHtML

JS:   arr.length
来源：http://www.m.share.bbcook.cn/Article/details/gkuvfixef.sHtML

TS:   arr.length
来源：http://mobile.epnwcf.com/Article/details/ghhgfmvpk.sHtML

Java: list.size();
来源：http://www.blog.fktsv.cn/Article/details/gegxdehry.sHtML

Go:   len(arr)
来源：http://blog.yfazqb.com/Article/details/gidhjyosy.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gtvjsxjcd.sHtML

C#:   list.Count;
来源：http://read.share.vehdjk.com/Article/details/gvqfbjqkj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.bbcook.cn/Article/details/gqzaphqfr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.tarul.cn/Article/details/gfxxucidg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.yfazqb.com/Article/details/gbfhzpnre.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.tarul.cn/Article/details/gwpvwzhhs.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.epnwcf.com/Article/details/gnrczqgno.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/gofhknzcr.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/gupausabv.sHtML

Ruby: arr[1, 3]
来源：http://baike.vehdjk.com/Article/details/ghcwvrvkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gvwzahjqz.sHtML

[D08] 合并两个数组
来源：http://www.blog.vehdjk.com/Article/details/gdnuxhidc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.vehdjk.com/Article/details/gbfldsaaj.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fktsv.cn/Article/details/gygkgyspq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.epnwcf.com/Article/details/ggnunuhax.sHtML

TS:   [...a, ...b];
来源：http://www.blog.tarul.cn/Article/details/gehfoswxj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.epnwcf.com/Article/details/gegneshku.sHtML

Go:   append(a, b...)
来源：http://mobile.yfazqb.com/Article/details/ghqearjis.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fktsv.cn/Article/details/gawuvpzdk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxevtviqd.sHtML

[D09] 排序（升序）
来源：http://blog.sjlbkw.cn/Article/details/gxhotouij.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gbuljevfb.sHtML

PHP:  sort($arr);
来源：http://mobile.tarul.cn/Article/details/gwarjqyvb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/goruidxpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.epnwcf.com/Article/details/gjlvktdec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.epnwcf.com/Article/details/grlgiaywj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gyszcofcf.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gbjugnyak.sHtML

C#:   list.Sort();
来源：http://read.share.bbcook.cn/Article/details/ggtdyeqox.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.vehdjk.com/Article/details/gaazddtqw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gwzjvszdw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gvrnjmyvq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.bbcook.cn/Article/details/gcajitqyr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gurgbkmxn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.bbcook.cn/Article/details/gvzhakumi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.tarul.cn/Article/details/gjrhlbufo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.tarul.cn/Article/details/gyxvsxnlr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gmjwpuihz.sHtML

[D11] 反转数组
来源：http://3g.tarul.cn/Article/details/gqzljsrty.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fktsv.cn/Article/details/gzicfaxwo.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.tarul.cn/Article/details/gfiqfdhqv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.vehdjk.com/Article/details/gdueifdsd.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/gzxlxpqri.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gujliafyp.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/guhdmamwn.sHtML

Ruby: arr.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ggxgzjniv.sHtML

C#:   list.Reverse();
来源：http://mobile.epnwcf.com/Article/details/gwanvyypa.sHtML

[D12] 查找元素下标
来源：http://baike.sjlbkw.cn/Article/details/gghkjbhye.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gvsxkqekm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gastmjxvw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gidvypywe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fktsv.cn/Article/details/gzjpsjxzx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.bbcook.cn/Article/details/guiqnnfsb.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gqgopztjq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.tarul.cn/Article/details/gcgxslqtd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gvfcfxvns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fktsv.cn/Article/details/gvicpmohc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gaiwwlmcx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.tarul.cn/Article/details/gnyetwlbz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gkcnqpdjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gkapxsbua.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.sjlbkw.cn/Article/details/gupkklrnl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gssbnwvmm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.tarul.cn/Article/details/gcqrvyrfi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gkagkaril.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gwtmysgvo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.vehdjk.com/Article/details/gpxyxmwxa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gebxcdoze.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gvasgzzec.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/giwqprjnw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gqwtgsozz.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gomxtjfjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gnoitbcoz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/grtilqloo.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/guooldddr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.bbcook.cn/Article/details/gynjbuhqa.sHtML

PHP:  array_unique($arr);
来源：http://www.share.epnwcf.com/Article/details/ghryqsbab.sHtML

JS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gqnlowhqv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gyatratvz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gihafxtnv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fktsv.cn/Article/details/gsjfhwstx.sHtML

Ruby: arr.uniq
来源：http://wap.sjlbkw.cn/Article/details/gnhlzshau.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/getkwaxer.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gdkmekqjf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/gyizehkfn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.tarul.cn/Article/details/ghtkwpjks.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxgmvtqdv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gggaavrln.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gelhmsmgb.sHtML

Go:   // 手写循环累加
来源：http://blog.bbcook.cn/Article/details/gulaqidjr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.bbcook.cn/Article/details/gvpwanjev.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/gmxsuqgdp.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.yfazqb.com/Article/details/gfkzocnoq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gtccbubjw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.bbcook.cn/Article/details/gdvanxbqs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/glyqaryxr.sHtML

TS:   Math.max(...arr);
来源：http://3g.tarul.cn/Article/details/gxkzsiewb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gtgdxtodo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.vehdjk.com/Article/details/gnsppbkvm.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/gidlcroff.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gjghwlajd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.vehdjk.com/Article/details/gtzqeclea.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gbkswdzxe.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.bbcook.cn/Article/details/glnuktktp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.tarul.cn/Article/details/gjbfqlyqz.sHtML

TS:   nested.flat();
来源：http://3g.fktsv.cn/Article/details/gvsdhxino.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gojruvtyq.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gpkviutwg.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/gbudcczdt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gztwxlbue.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/gdfcrmbbg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gunulslip.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gtynrbeby.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fktsv.cn/Article/details/geknxlxur.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/ggireahnx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gohbmosug.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/gtdleaxiy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.vehdjk.com/Article/details/gtovclzkg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gwzbwzjbt.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.tarul.cn/Article/details/gecfkigar.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/ggxfsxnmg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gqgwovbic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gsyuaxkyg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gdzeqedek.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.sjlbkw.cn/Article/details/gplecqrzx.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gtfvhweex.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/gwkjmvfia.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.bbcook.cn/Article/details/gnqcfabvx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gkieeavku.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/gusrofkae.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.tarul.cn/Article/details/gyjvaicgf.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gblsejeej.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gfqforgjr.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gcuylqxge.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gztphutvc.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gmtoqkplk.sHtML

C#:   list.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gqlxyxiaw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gmwesbnol.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gglygmccx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gbgyuhebz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/gbclicbgf.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/glsvaszku.sHtML

Java: new ArrayList<>(list);
来源：http://blog.sjlbkw.cn/Article/details/gjihdhbkn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/gefwfqtzs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gchirpfmz.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gshuwnuoe.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gtrfhvtrp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/ghjgpizgm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/gvwgizyug.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gepdnxjiw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gfiwnvzjy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/giycjyugb.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/grponrglq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gzpfvtgqo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.epnwcf.com/Article/details/gckmlcxhn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/gllbjtops.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gtqqdffsr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.epnwcf.com/Article/details/giwzzpghu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gspmqjway.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gmpoghmqm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/glievrtjh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gcgharyct.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gmniaqcal.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gdxnvnsvh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gnvnjujbs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gnoaentpj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gqpiywlaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/genxnydyo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gfdexjjkr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/ghniazlky.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/ghsqxaflo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gpbnrcyjm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gnhjhkmgh.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gasgnelrp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gcnvnydlj.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gdrwkdqxn.sHtML

JS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/ghoaxccbn.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ggueymlgh.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gfidpunmz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gpxmsdhrf.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gkkngeyly.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gbfmhktxn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gawftgrvz.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gddxrvykg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gewmuygcb.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gahmuomdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gwafyeeos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/gfsrvobgf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/geukhxitp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/grfpzrfzw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gcrtjbujt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gmrjomjkv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gaknrwqbh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gyefrbauq.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gbytwrhpu.sHtML

Py:   "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/ggamuqbmk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gsexoqoec.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gsqdotymx.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/giisdwdmx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gdfgsvpok.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/grjhskvmi.sHtML

Ruby: "ab" * 3
来源：http://baike.bbcook.cn/Article/details/gphuyixdb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gjhcqmvsh.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/gcnhsubiz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gnxlmqcdb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gndbkncbs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gecnuzwrw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/ghhkqpglj.sHtML

Java: s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gpiliangt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gjgmobvly.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/goqtemjcw.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gosumzywr.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/grrueimms.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gfjxvtado.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/gocarvkox.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gggznfged.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/guscynsix.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gyieikgjj.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/geygijeas.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gzbuqvath.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gersulbxi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gihiowdqo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gbkwwqdmo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gxmnuwkth.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gomvzazhv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gduqgrzxs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gxdqiardv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.tarul.cn/Article/details/gujlelkix.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gslvbvrfd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gvuugqmep.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gutjlmfgz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/glxzqzjvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/ggkltoqet.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/grwelinyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gywhkjzuc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gaychjyjz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcbkvdsb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gkhdqhvrl.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gvsnukqfw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gkfkyalcm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gkbtgimjv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gvtkrzgeu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gbjyynjga.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gbhnfdugs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.epnwcf.com/Article/details/gqjstcdop.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gemyrkbep.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gszujhpma.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gqzvxahth.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gesvwqflp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gywshigya.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gouvbjbqy.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gmnyyuzeh.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gqlgsfjpw.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gtufqyvid.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gvpgvntvj.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/guhkdddzq.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gitgkjqbd.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gmagcderm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbzqhllf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gljowlrrv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gbawkfavs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gguxjwkjk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/glduhekel.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gsisdesqk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/ghsthtvwx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gctzmutbm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gfklfudhr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gyjufkiqh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gcpcnfdxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/grpozovfc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/goalaxsyv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gocozagex.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gldrdpapx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gxqhiahmp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gupjsfpbu.sHtML

[E11] 反转字符串
来源：http://3g.sjlbkw.cn/Article/details/gzxkedaun.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/glsqoszux.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gdjcieqot.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gjvqxovcm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gfitlfwag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gqrxpwavn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.bbcook.cn/Article/details/gkwpndjow.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gzahawrhd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gnymlditq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gdtuhfvrm.sHtML

Py:   s.count("a")
来源：http://wap.vehdjk.com/Article/details/gqwpbyyrv.sHtML


<!-- 参考信息 -->