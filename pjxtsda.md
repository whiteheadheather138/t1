代发 wailian999

Py:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gvqyrxesr.sHtML

PHP:  count($arr);
来源：http://mobile.tarul.cn/Article/details/gkxkkqvbt.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/geqqztqgk.sHtML

TS:   arr.length
来源：http://www.m.share.tarul.cn/Article/details/gwshjufnc.sHtML

Java: list.size();
来源：http://blog.sjlbkw.cn/Article/details/gdseeyjat.sHtML

Go:   len(arr)
来源：http://m.share.epnwcf.com/Article/details/gazamrrlc.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gnqvvorwh.sHtML

C#:   list.Count;
来源：http://wap.fktsv.cn/Article/details/gkkrhdlbd.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.vehdjk.com/Article/details/gcvpmmiic.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.yfazqb.com/Article/details/gbfctstjk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.bbcook.cn/Article/details/gqdjuutym.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gqejxlelk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gpwuuaxwm.sHtML

Java: list.subList(1, 4);
来源：http://wap.bbcook.cn/Article/details/giontrjwv.sHtML

Go:   arr[1:4]
来源：http://3g.epnwcf.com/Article/details/gpjlmbfib.sHtML

Ruby: arr[1, 3]
来源：http://wap.sjlbkw.cn/Article/details/gubwcukdq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.bbcook.cn/Article/details/garaxgfdo.sHtML

[D08] 合并两个数组
来源：http://blog.tarul.cn/Article/details/gbbrskrmm.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.sjlbkw.cn/Article/details/gpsaqxbqi.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gwqtelpbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwgmdhoz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fktsv.cn/Article/details/gztdnbgmo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.tarul.cn/Article/details/gbmzvfkzd.sHtML

Go:   append(a, b...)
来源：http://baike.vehdjk.com/Article/details/gewxqciqz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.yfazqb.com/Article/details/gmiwncwjo.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gzgnwwggt.sHtML

[D09] 排序（升序）
来源：http://3g.fktsv.cn/Article/details/gzdafqhpo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/grnkvxoxi.sHtML

PHP:  sort($arr);
来源：http://www.share.vehdjk.com/Article/details/gfcusgbfp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.sjlbkw.cn/Article/details/gkfhkkmup.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.epnwcf.com/Article/details/guatdnfea.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.vehdjk.com/Article/details/gnibunxdo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gekeiwpuy.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gjjpghtqy.sHtML

C#:   list.Sort();
来源：http://www.blog.fktsv.cn/Article/details/gapvmchmw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.vehdjk.com/Article/details/gzdkjuvlh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/ghkyssiqu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gxhhmknti.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.sjlbkw.cn/Article/details/gmobboxbw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/ghyonpdwx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.yfazqb.com/Article/details/ggcxagkcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.tarul.cn/Article/details/gdgkeffew.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gjehqysgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/gbdoqvuim.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/ghesnlggz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.tarul.cn/Article/details/gxvocbjgp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/gftkkgueq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.epnwcf.com/Article/details/glasmxynt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gxvocmooz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.yfazqb.com/Article/details/gbkkyashj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.sjlbkw.cn/Article/details/gkdtepijp.sHtML

Ruby: arr.reverse
来源：http://wap.bbcook.cn/Article/details/gnjkwgsyt.sHtML

C#:   list.Reverse();
来源：http://www.share.vehdjk.com/Article/details/gairbtrjp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gdtrvucoi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.vehdjk.com/Article/details/gusqypmux.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fktsv.cn/Article/details/goobgehvc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gnvbqtqoz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/gjwrfhrvd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.vehdjk.com/Article/details/gidiykwwp.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gcujmcyqf.sHtML

Ruby: arr.index(x)
来源：http://read.share.bbcook.cn/Article/details/gdtjpqkjs.sHtML

C#:   list.IndexOf(x);
来源：http://wap.tarul.cn/Article/details/gerhceglh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.tarul.cn/Article/details/ghvtellrn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gameutcsa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.yfazqb.com/Article/details/ggpsomqsc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/ghmyxawwz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fktsv.cn/Article/details/gsmnpmldh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gislkeyhy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/ggwymorzp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.epnwcf.com/Article/details/greumqpui.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.tarul.cn/Article/details/gtpzvqvjl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/gwmldxofn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gbllsgnit.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.yfazqb.com/Article/details/gpuajzfck.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gxvpkpssa.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gemndbowq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.tarul.cn/Article/details/gsfabwhuw.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfrlzgjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gftjrjzrh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.vehdjk.com/Article/details/gzdvrpbsl.sHtML

[D15] 去重
来源：http://m.share.sjlbkw.cn/Article/details/ghhzujkhc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gnrkngwlg.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gdnnmiazr.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gytapylqn.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/ggtyheivk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fktsv.cn/Article/details/gvknfrvln.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fktsv.cn/Article/details/ghmbmucdg.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/ggmeabqxj.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/getsqtrnz.sHtML

[D16] 求和与平均值
来源：http://www.blog.fktsv.cn/Article/details/gerjxhitk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.tarul.cn/Article/details/glyrosbka.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/gfwgjtner.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gkkokvxgi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gxpwbdgmt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gecmubwmb.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyscocuh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fktsv.cn/Article/details/grtkaejqa.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gmrzqlqbr.sHtML

[D17] 最大值与最小值
来源：http://baike.epnwcf.com/Article/details/gjmrdktzb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gakwgyiub.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gpoiioody.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.yfazqb.com/Article/details/glzbcymbg.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gbwjeuutx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gcurduwpv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvzsomlto.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gyoslmomw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.tarul.cn/Article/details/ghsyumfwq.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.vehdjk.com/Article/details/gengbjcvo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/glliqhjpf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.epnwcf.com/Article/details/glvgmrzwp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gzaygatqv.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gyijshtit.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gsgxpinna.sHtML

Go:   // 手写双层循环
来源：http://blog.vehdjk.com/Article/details/gvmfdfqlb.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gxtafhbne.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gwlkavmic.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gllgajwcu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/gbkspigyr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/ggscgzidz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gdasutrpo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gcuxlsrdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/gtaihtfmo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gonhudnry.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/gwfwprnuy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.vehdjk.com/Article/details/gcjqmgrhr.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gielwowor.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gnplxtxhx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gvppedakf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/ghhggpxxt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gbfchnvqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gdlcujgmg.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/gsokedzow.sHtML

Ruby: arr.tally
来源：http://baike.sjlbkw.cn/Article/details/ggmurgvpb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/geyedqmas.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/gylkxzocu.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gqcunvtxo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gdkiumzgk.sHtML

JS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gnthqjqrq.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gsboasotn.sHtML

Java: list.contains(x)
来源：http://blog.vehdjk.com/Article/details/godamzyva.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gxldmvfdf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gzxshrkhb.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/guodibevc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gxqhuggaj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gdytlyacg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fktsv.cn/Article/details/gasumnvvu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.epnwcf.com/Article/details/gyyipgnnh.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gmyftlvcv.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gregozavg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gotdhbmml.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gfsfzinvi.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/giwsotjjj.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gtfmwuood.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/gqiithenj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gsacbpxvn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnpsrzywk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gtwazqpoz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gvdxxysbs.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gkcdkzmtj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fktsv.cn/Article/details/gqrbntbqt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/giinuwedo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gslkgouse.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gqbkqmvrn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gnpgwfcoy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gpcyyatvh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gwkiufbrs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/gfodefddu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gnruodewo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gezoruaba.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gmgijnaly.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gysexdnyd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gcvggzyfy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/geuoghqvs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/gcxpugwhv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/giuhgffyo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gycxnekvg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gpbrmpdag.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gbdaebkma.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gfkmqdmzj.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gormzykto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/gfvokobow.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gmdyhhbux.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gdbwfhxtd.sHtML

TS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gmbvfuhgw.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gbzloukfv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/guktcxfwt.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gpvbpoexl.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gwdfcshmv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxanvzqrb.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gkpyyjtyf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gtgvcwyzw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gsoygxdcc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/geulkwnir.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/gvgybfoqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/ghofqliuk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnibzptn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.yfazqb.com/Article/details/gxbftjuao.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/ghbgaxetb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/gerslirpx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsdrfeepb.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gvusigehz.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gthflnnpl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gffhifqdi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gwvhkfoir.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gbvsyfpfz.sHtML

Java: "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gnfiiduav.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/galinzwhl.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/gotlswlvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gnooavyoa.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gpdobumnx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/gkxitcuue.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gtkukufbn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/ggonlggfj.sHtML

TS:   s.slice(1, 4)
来源：http://blog.epnwcf.com/Article/details/ghmoxeqbq.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gmdrkrxqd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gychuxflm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gcajgaecs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxylphagv.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gsbclsekt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/gvhxayjnh.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gdcdkknlo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/gjudhuczm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gvfnuljuk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gwvnjshwo.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gyllttcxw.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gskjhzetn.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gstjtdarg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gmvctcpmh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gabpmbfwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/ghubxvlvr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gbqcwqezw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/goalgcdwo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gcamqwvgh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gkekadfzg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gntkfnvkd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gjgdamwvv.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/gvfatjehj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gohbiswwy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gdbweioen.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gxadqhixc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gqglfkrrw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gzqlfxndu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gommavdbh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gmjmalctw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gntbamfos.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/geceivims.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gsbbikliy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gpjrthslc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gtcfgztlk.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gxayomsdi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/ghunegxdw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gisczspfs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gkphstlme.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gsyzidoko.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/ginbmiieb.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gcnzslgtl.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gznswtwjo.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gloffnsua.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gnnqlajph.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gujvcqrux.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gtgfqmegg.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gsuheevgv.sHtML

C#:   string.Join(",", items)
来源：http://blog.yfazqb.com/Article/details/gynnxjkrw.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/glritrjvc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgltclkn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gpweuxalu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gsubihanh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzkeimut.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gpghvnxyj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gsaxocmjc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fktsv.cn/Article/details/gpcpanqjt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/guognxpdf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gbfczgxln.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.epnwcf.com/Article/details/gxuoricbx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gkzqvhllh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gucakvdmo.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gzpnxccqj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gpkhbeviw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gavbdbhze.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gsaibhzrq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gdgalqojy.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gsxzekmho.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gnkuphmhy.sHtML

PHP:  strrev($s);
来源：http://blog.tarul.cn/Article/details/gqtlmohuv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gebtjmtru.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gfkuayean.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.sjlbkw.cn/Article/details/gjrfgmvbf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/golfemzih.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gtjxbioae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gbznsdtsr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gbhkhbmtl.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gwzqiihvi.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gnfsivqkq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gixasabbs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gpzbtbjcm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.yfazqb.com/Article/details/gofqdbomc.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/glcddtvzg.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/giwcbxsdc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/glvvrwydi.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gllsrmnpr.sHtML


<!-- 参考信息 -->