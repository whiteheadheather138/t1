代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gnqyfeuoz.sHtML

[D08] 合并两个数组
来源：http://www.share.tarul.cn/Article/details/gdrhgzjku.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/ganyoguph.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.tarul.cn/Article/details/gbbxqmugx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.vehdjk.com/Article/details/gakxznwpk.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/gtzhjrpur.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.epnwcf.com/Article/details/gjzpnnirg.sHtML

Go:   append(a, b...)
来源：http://3g.bbcook.cn/Article/details/gslybdkut.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.yfazqb.com/Article/details/gnkayeygk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.vehdjk.com/Article/details/gejyyvjxd.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gwfeckqhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gnrukwbll.sHtML

PHP:  sort($arr);
来源：http://www.blog.yfazqb.com/Article/details/gxhnsaixk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gxnhixthp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.sjlbkw.cn/Article/details/gjqvxfton.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.bbcook.cn/Article/details/gtvozlyws.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/grwbjidfi.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gzqbpvgui.sHtML

C#:   list.Sort();
来源：http://blog.fktsv.cn/Article/details/gxonkvuzw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.bbcook.cn/Article/details/gpilurrgy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fktsv.cn/Article/details/gikzikjbj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.epnwcf.com/Article/details/gscbiifei.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.yfazqb.com/Article/details/gruhglstm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fktsv.cn/Article/details/gnoivdhgz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.tarul.cn/Article/details/gsqvhxiew.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/gzfpciewr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/grjldnzpq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.bbcook.cn/Article/details/gmeripiam.sHtML

[D11] 反转数组
来源：http://wap.tarul.cn/Article/details/gqadfrxds.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.bbcook.cn/Article/details/glcrjvvma.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/gmypdikks.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gvsxdtunk.sHtML

TS:   [...arr].reverse();
来源：http://www.share.bbcook.cn/Article/details/govhjrjnw.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/gpkariqjv.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.yfazqb.com/Article/details/gwexujjpo.sHtML

Ruby: arr.reverse
来源：http://mobile.vehdjk.com/Article/details/gvindrpwf.sHtML

C#:   list.Reverse();
来源：http://read.share.epnwcf.com/Article/details/gmkybcwgt.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/gowsozfhu.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.yfazqb.com/Article/details/gmekwpozs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.yfazqb.com/Article/details/gurivjnnm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gnrzzxuvh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.yfazqb.com/Article/details/ggtdhcuej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.tarul.cn/Article/details/gtnfdrsqc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gewmacfgh.sHtML

Ruby: arr.index(x)
来源：http://baike.bbcook.cn/Article/details/gjqlavjed.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fktsv.cn/Article/details/grrsnlmza.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gfrnpewhm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.sjlbkw.cn/Article/details/grpkcvumd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.vehdjk.com/Article/details/gsvheeyuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/gmcctsslw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fktsv.cn/Article/details/gwdpeycmx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.yfazqb.com/Article/details/gqmjyvgbj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gkmaobvej.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.vehdjk.com/Article/details/gtwlytoyq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gsdrpmzfj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.yfazqb.com/Article/details/glgpaxaep.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.bbcook.cn/Article/details/gyfntbiqz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.bbcook.cn/Article/details/galvmbtze.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gwfgfsklw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fktsv.cn/Article/details/gdtponies.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/ghfzpptjn.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkgglnya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.bbcook.cn/Article/details/grnmewqoa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/gvstlxsyq.sHtML

[D15] 去重
来源：http://m.share.bbcook.cn/Article/details/ggdvqduax.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.epnwcf.com/Article/details/gdbgkutqg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/ghsqpvotq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/ghcrgyukh.sHtML

TS:   [...new Set(arr)]
来源：http://blog.yfazqb.com/Article/details/gluadysrf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gyanrsxsa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/govfbytwk.sHtML

Ruby: arr.uniq
来源：http://www.m.share.tarul.cn/Article/details/gfqzjrkxj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.tarul.cn/Article/details/gnucfhqbq.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/gvgfvcwbn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gubavsypz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.yfazqb.com/Article/details/gkfxofnrh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gaecenocm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/getriykul.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gxpklhhwx.sHtML

Go:   // 手写循环累加
来源：http://wap.bbcook.cn/Article/details/gufucdodm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gtqzgoxat.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.yfazqb.com/Article/details/gkhwhyukm.sHtML

[D17] 最大值与最小值
来源：http://3g.fktsv.cn/Article/details/gtlkgjwru.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fktsv.cn/Article/details/giphzbqhu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/grwqbxykl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fktsv.cn/Article/details/ghjpdrmdl.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gixubvzjh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.yfazqb.com/Article/details/gteefhvqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/gmxjrgrto.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.tarul.cn/Article/details/gkaukvdsb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/guhybhwbr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.bbcook.cn/Article/details/gysbehbri.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.tarul.cn/Article/details/gdcjmpycn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gwfwykkil.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gdggoiliv.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gwjrlyqax.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fktsv.cn/Article/details/gikgqmvrn.sHtML

Go:   // 手写双层循环
来源：http://3g.vehdjk.com/Article/details/gnivdwkag.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gwzcylrwn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gkpmcieaz.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gskytvuib.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/greczsbhh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gsqplrwcf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gssmgknbu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gxubenwss.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.tarul.cn/Article/details/gycckacif.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gmixlphxq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/glunoylla.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.sjlbkw.cn/Article/details/gppkqxncc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gwzcygbcy.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/ggvxgknff.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/geigxpcvn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gcpsfjdir.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gqfifsizu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gictnbivj.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gvevkbjfz.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gussejtnc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.sjlbkw.cn/Article/details/gttdadqla.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gedcsxvjx.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gtcgccqln.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gjkkdcovt.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/guftskocb.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gyuquwrax.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/ggkbsbmao.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gkhqvjwot.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/gaenniweg.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gadofjinz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gjfezikcy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gnflkoydn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gceyckygw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gykrcarza.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/gskmvbqpt.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gmqqeqydz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gdwrcfxcs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.sjlbkw.cn/Article/details/gyuwbetoo.sHtML

C#:   new List<int>(list);
来源：http://read.share.epnwcf.com/Article/details/gzcelgmxe.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gcylalrbg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/guxnzubix.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.yfazqb.com/Article/details/gfjgcirqd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gmipjgcvx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gxvivdzjc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggokxwyle.sHtML

Go:   // 手写循环
来源：http://baike.sjlbkw.cn/Article/details/givebvxin.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.vehdjk.com/Article/details/gfedyiykw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gbkosmyss.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gvykntnea.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gjorcfygb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gbzwxteig.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gwmzydmlj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gkookxjph.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gkocsadps.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/ggntgipfk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fktsv.cn/Article/details/gsvpvxxoj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gvuuqxovl.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gxljiyblq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/ghspknroe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/ghguivuru.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjqrikiel.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gzdvuhnka.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gknjpnuqw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gsoecexao.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxeuvcsxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gzryuwnvz.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gvoddsoek.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/goakopqbc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gszuyipnk.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gvmmyxxfp.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gmxszvnqp.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gdozmmjzo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gtgzdkaye.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gapmfiepv.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gtgzasvzl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gqgzhwbqo.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gcjzhvybg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzcsrfaia.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gajuufwov.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gwfjjyljk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/ggyibqgqi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gbrcbfmsu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gbdtzyxfp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.yfazqb.com/Article/details/gutjieadr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gmjocppnp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gyrwidlpp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhgmprjb.sHtML

[E02] 重复字符串
来源：http://m.share.yfazqb.com/Article/details/gtomkiflc.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/ghtlconnr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gwmkpbtjy.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gjbsyjxep.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gmpofpmhm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/grwtpzpps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gsqppqomr.sHtML

Ruby: "ab" * 3
来源：http://baike.tarul.cn/Article/details/gyqsoitxl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.tarul.cn/Article/details/gluaoyftg.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gwrrcbvcl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/ghyyubcgi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gpmbvfxyf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/giyyvfpro.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/guhjembqr.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gpzexfoqz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.vehdjk.com/Article/details/gtdnbozlb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/ggxkdvbkr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gkpnqtphw.sHtML

[E04] 查找子串位置
来源：http://mobile.vehdjk.com/Article/details/gkfvfkgou.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gdjqbulju.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gknvowmqa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/gnkqwasba.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/ggizfmzjy.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gbxeoedwi.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.sjlbkw.cn/Article/details/ggdiubssd.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gndhudauz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gmhybzhxx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gdmfafaud.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gyuchgotv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gjcxprqig.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/geqltbhjn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/ggaavlizb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gwzhsecho.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gwvlskoxb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gcnhgwnxz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/grfxudhag.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/guspdwnde.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gwvsswagk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gsqboyxfw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gyxluhbow.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/grraqospx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/grmbrmxsf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/grmxuyonk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gwlbiddmz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gedfkipsb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gqjfwwhko.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gspsngfnf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.bbcook.cn/Article/details/guifsgtlz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/gddwumbvk.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/gbdberhyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/glwclrztz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gjkolhjzt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxplkshq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/ghslicqzk.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gajorenie.sHtML

Py:   ",".join(items)
来源：http://www.share.yfazqb.com/Article/details/gurnnowuk.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gobhbjdaj.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gngwakvrj.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gbescxskj.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gxzhoiilb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/gurriklok.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gngcdqzuo.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrrsquv.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gezjbkfqo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gvqukvcdr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gfgbkmeaq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gcztnesjy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/ggshlgnqq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gviyazymg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gaxgriyyz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.sjlbkw.cn/Article/details/ghqlpvoea.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gqsjfpheo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gngfairky.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gmganqvic.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gbbtsiobh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gfmincjzm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/giylwlceq.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gdnrxidab.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gzvemtrmx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gjrrqdoff.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gkwpucszp.sHtML

[E11] 反转字符串
来源：http://3g.yfazqb.com/Article/details/gbmvnuonh.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gxeuyavuv.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gvfqzcknn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gjkyfhocu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glejcprkq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gbuoquxwu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gysbaoftt.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/glkhbyaui.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gthbljgxp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/grjdlyvpd.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gpiaokkfk.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gdubptfjx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gkrjotidu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gcqiszqmh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.bbcook.cn/Article/details/gwszszzmt.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gzmglfmca.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gcdtguejb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gbvsltwxg.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gmkvgxvmd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gykwgfeps.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gopxkelmm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gveewserw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gijenfprk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gqocdkxva.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/ggvkrlwib.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/giezwktco.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gglseqogk.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gvbjutedg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/ghyqepxct.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.epnwcf.com/Article/details/gwfvstxnv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gwyoddrtz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gyzohxnix.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gmyaefkad.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/grgbxpgip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gdfjmllai.sHtML


<!-- 参考信息 -->