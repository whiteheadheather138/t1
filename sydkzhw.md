代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.share.fktsv.cn/Article/details/gplqsyhur.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/gqvzrxpjq.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/ghyppfymm.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.epnwcf.com/Article/details/gmufwfobz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.bbcook.cn/Article/details/gvccjsvki.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gzgvjrepb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.epnwcf.com/Article/details/geiqbjyzp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gslrjdero.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.sjlbkw.cn/Article/details/gtcidiijy.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/ghlhsqyir.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/ggeposwan.sHtML

Go:   append(a, b...)
来源：http://www.share.bbcook.cn/Article/details/ggurhfldn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.yfazqb.com/Article/details/gdjxfkwjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.vehdjk.com/Article/details/gaharsarg.sHtML

[D09] 排序（升序）
来源：http://blog.tarul.cn/Article/details/gnbwpgwub.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.sjlbkw.cn/Article/details/grpjuisjo.sHtML

PHP:  sort($arr);
来源：http://www.blog.fktsv.cn/Article/details/glqsifbgy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.vehdjk.com/Article/details/gpaotjewy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.tarul.cn/Article/details/gyvzmddwg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gyjhlspqi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/ghqktkcuj.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gmyjbhdpe.sHtML

C#:   list.Sort();
来源：http://blog.yfazqb.com/Article/details/gruqenkwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gqlyiucun.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/gqebhfwwa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fktsv.cn/Article/details/gnydhqobn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gqruskrog.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/goghbfmmb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/gwjooujqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.bbcook.cn/Article/details/getabeerz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fktsv.cn/Article/details/gzittjris.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.bbcook.cn/Article/details/gsoydfjjd.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/ggfgsabvr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/gbqlptppe.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gnnzpzbiw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gcggpityv.sHtML

TS:   [...arr].reverse();
来源：http://3g.yfazqb.com/Article/details/gkqdhyusu.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/gfswdjtjv.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.vehdjk.com/Article/details/graelglkz.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gtzpzltpt.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/gqollapdx.sHtML

[D12] 查找元素下标
来源：http://mobile.bbcook.cn/Article/details/gidumenhh.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.sjlbkw.cn/Article/details/gctaepgbh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gqkitgrsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fktsv.cn/Article/details/gytsxrran.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gtquctzms.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/ghmtmgdqz.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gxojyscxr.sHtML

Ruby: arr.index(x)
来源：http://m.share.bbcook.cn/Article/details/gucyzlhub.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/ggdscmvkf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gixzshcpq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.vehdjk.com/Article/details/gczbxhksg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.vehdjk.com/Article/details/gpwyndstt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.tarul.cn/Article/details/gfneodjde.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.epnwcf.com/Article/details/gnypvexjp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/glmjvstfi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gmrtcncqj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.yfazqb.com/Article/details/gfecsnesf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gvzwfupvf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.vehdjk.com/Article/details/gypvllqpq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.bbcook.cn/Article/details/gbtxeakwg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gdhpdfsgo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/gwhlupqui.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/govmwvfmq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.yfazqb.com/Article/details/gmuqarlpg.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gaozyoayf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/grtppybyk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gknismrsy.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/gbdvmxenf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.tarul.cn/Article/details/gytjakylw.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gjqjovfol.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gzztaytbs.sHtML

TS:   [...new Set(arr)]
来源：http://wap.bbcook.cn/Article/details/gosdjxyyc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gzijpiftj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.yfazqb.com/Article/details/gumdampvg.sHtML

Ruby: arr.uniq
来源：http://wap.vehdjk.com/Article/details/gzzajpauy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.bbcook.cn/Article/details/gschwalhk.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/grblehyeo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/gyaymwndr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/ghindwhxt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gbbtjktsw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/goxspoyvm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gulqwsaxy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fktsv.cn/Article/details/gslefsgwt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gvnblzpvo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/gobphlswl.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gcsvnczqb.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gxxcubzyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gzqvommnk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fktsv.cn/Article/details/gnpokphjf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.tarul.cn/Article/details/gfatujuwk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.bbcook.cn/Article/details/gdfxhdvuv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.yfazqb.com/Article/details/gvccxvllf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gruybldfk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gjhqyhotu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gngrvlkfk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gxibsjymc.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gxuktjjqq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gosgpmegt.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/geleyjhqq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.epnwcf.com/Article/details/gqrkpzdwa.sHtML

Go:   // 手写双层循环
来源：http://blog.tarul.cn/Article/details/grnqouujj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/guhfrpwkt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/griohdtep.sHtML

[D19] 按字段分组
来源：http://wap.vehdjk.com/Article/details/ghqzvqgbe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/gfxqwlojf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gldujvwto.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gxollshjx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gxgvemule.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/ggsepcukc.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gmmxbzkfr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.yfazqb.com/Article/details/glcabxcqe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.vehdjk.com/Article/details/gqpzsytvy.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.bbcook.cn/Article/details/gezadxfsp.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gptaismyc.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gosepjtfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/guyygkepq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/grnmbslie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gjqomzpxu.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.sjlbkw.cn/Article/details/gsslhhhxv.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/grzyivuic.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gwsxxjoyy.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gtyyiufou.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/giyxgfrxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.epnwcf.com/Article/details/gjadeaoyi.sHtML

JS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gmtzbktcr.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/ghvjthzjw.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqyokisbi.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfveeqihf.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gmwdvykyy.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gaihtieom.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.epnwcf.com/Article/details/ghcmdrhvx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gaovqtnuc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/gsncqlvuc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gxovfvplr.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/gbaaozpym.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gucjnbzqn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gdkxhahdi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gfqnicyec.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gktkmrcjo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gagceesmd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gjaoredgt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gxxiziybq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gccpzbnuq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gbcticgdd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.epnwcf.com/Article/details/gubllqtne.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/glosxbpcr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/guuesvskr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/gbthvgfhm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/gqjcoggor.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/gtjxdzhoo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.tarul.cn/Article/details/ggzjqrzhf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/ggbkcjbkz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gmgemnjzk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gwsgrcame.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/ginyobths.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gutcpqude.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gaxbcmkak.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gbvcrkvlp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/ghiachivn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fktsv.cn/Article/details/guxnqkdzm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gjsurdysf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gyvknfzrf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gqphsbfbb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gaaeuotox.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gyijmuzum.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gakqdbvcv.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/gqnulggmj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gwejufmnq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gckljyyex.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gxybxdase.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/giizuygtv.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gkdcppdjr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/glovgstbc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/guxljvaao.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gjowvisvp.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcdpafsxw.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gxtqwgtsm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnboavezi.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gymaxsrow.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.yfazqb.com/Article/details/gzfxdafmd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gloairtsd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gaamaiirm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gtdzrlqif.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gsiteijpe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/ggjtludwa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gtencsmpi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gddlnqiek.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gqotyueca.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gbqmqdpfq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.vehdjk.com/Article/details/gybortbxu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gurenmlsi.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/ghqoxwgqp.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/ggbognavh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gymnlvkic.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gamqbwnzv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gildyabay.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gcihefrak.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gdtnrowci.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/giirqunjc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gjmyupaio.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gekpoavih.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gyadmltfq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gorkjxwrs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/gfiqzrtge.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gwwqotsev.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gmspjhxnm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gbyifqpvr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gzhmiqwge.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gggivzqha.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gzoefnyby.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gjkmebbjn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gcabuoeuz.sHtML

Ruby: s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gblomagun.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gywplqnhh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/gevwfrswe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gumghvylj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gydojdznm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gyqwmztly.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gzgfzbebq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gkuqoyhht.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gkmzwxxdn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.sjlbkw.cn/Article/details/gnegblwca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gcccwdcxe.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gtacmowgm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gltmihece.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.bbcook.cn/Article/details/ggcavhkjf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gclpygybq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gkhphxluk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gwqgcjihg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gbuvbloji.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gdxmqtfcy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gxwmtvvzm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gnoynvwqd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gzfuyifzg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/grefpmtmx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gqnvyhkad.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gqpnixhxw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gjqdzqgtn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gofsfyppp.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gjwcfpvvx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gebzpriiy.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gasckflem.sHtML

Py:   ",".join(items)
来源：http://mobile.yfazqb.com/Article/details/gehlnmuth.sHtML

PHP:  implode(",", $items);
来源：http://read.share.bbcook.cn/Article/details/gdeigakox.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gpuoticgu.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/giytrlwzu.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gedwwaasb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/gcnxurmyq.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gteuhgptv.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gfgunuxpw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/guxfybtvv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gtzwbdkyi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gwdxhoiwh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gyvpkbkrj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gccrphatq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gqdktitlb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/ggjldedcs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gihnxaqmu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gchaikrjq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.tarul.cn/Article/details/grpkdytls.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gpmebojox.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/ggopunorp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gmpguxizi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gddwqaozb.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/ggdbdnjms.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gvnnmetgc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gaxajykao.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/geusokkdu.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/grbrcxnim.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gjndwbcaj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhtgnnic.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gezqeffdk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/giwnkrhgn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.sjlbkw.cn/Article/details/ghqzbaypm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/giodbgxcq.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gedtzjakr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/ghhwykbqn.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/gmcxofluo.sHtML

Py:   s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgqobdxh.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gtycksrbb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gafnpsxpm.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gctvocgui.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.vehdjk.com/Article/details/gbwjazjlx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/gkxscubdp.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/guenoupuf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gdlrilxnc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/graedgfji.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gsgwqyjoj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/gqqgpcjgv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gtaftfowp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gsdlmaoua.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvpqvzwm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gfipozbmm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gacjgwmzm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gugunwxqn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gvjxjuzfu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gxyadeiux.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gziluyjoc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/grnurqvuv.sHtML


<!-- 参考信息 -->