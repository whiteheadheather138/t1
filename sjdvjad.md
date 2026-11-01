代发 wailian999

Java: list.size();
来源：http://blog.yfazqb.com/Article/details/gfdbzisqb.sHtML

Go:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/gtuwbajuv.sHtML

Ruby: arr.length; arr.size
来源：http://baike.yfazqb.com/Article/details/gyoopzjzt.sHtML

C#:   list.Count;
来源：http://wap.bbcook.cn/Article/details/gipkocqwj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.yfazqb.com/Article/details/gdxcagcyz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fktsv.cn/Article/details/gkrwtutpt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/gxiywevel.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.yfazqb.com/Article/details/gknjqhyof.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.bbcook.cn/Article/details/gsqwvfhjk.sHtML

Java: list.subList(1, 4);
来源：http://baike.vehdjk.com/Article/details/gvtydrsnu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gxrembubp.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.vehdjk.com/Article/details/grjdtjskc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.yfazqb.com/Article/details/gtykpjowz.sHtML

[D08] 合并两个数组
来源：http://www.share.sjlbkw.cn/Article/details/gxldkqjxe.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.yfazqb.com/Article/details/gcbjvjfku.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.sjlbkw.cn/Article/details/gnscjahef.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.epnwcf.com/Article/details/gjfifbsky.sHtML

TS:   [...a, ...b];
来源：http://mobile.vehdjk.com/Article/details/gatxgfjdn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.vehdjk.com/Article/details/gzcueitpm.sHtML

Go:   append(a, b...)
来源：http://3g.vehdjk.com/Article/details/gcqflfuiz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fktsv.cn/Article/details/gaqwchbjx.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.yfazqb.com/Article/details/gdeprsiyr.sHtML

[D09] 排序（升序）
来源：http://3g.epnwcf.com/Article/details/gzqcdedvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/ggyzbxydf.sHtML

PHP:  sort($arr);
来源：http://mobile.sjlbkw.cn/Article/details/gzybcetpw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gnbvewcfs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.sjlbkw.cn/Article/details/gyzukzbun.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.vehdjk.com/Article/details/gapjjxbwy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gsbpazjkl.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gnkpoxdlx.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/glpolwqei.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/goqmcrntx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.epnwcf.com/Article/details/gqjhbmdsw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/gyiecxibk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gyzavzjgz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.yfazqb.com/Article/details/gciohrmbj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/gwbbpdsxa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.tarul.cn/Article/details/gcnytfttg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.epnwcf.com/Article/details/gdiqwdrxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.bbcook.cn/Article/details/gkshcgwio.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/gkyrorasq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fktsv.cn/Article/details/gminytfsy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fktsv.cn/Article/details/gtdyloiqq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.epnwcf.com/Article/details/gtdtldlmd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.vehdjk.com/Article/details/ghfpaxwup.sHtML

Java: Collections.reverse(list);
来源：http://blog.sjlbkw.cn/Article/details/gbyzwhcvd.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gjcrknuai.sHtML

Ruby: arr.reverse
来源：http://read.share.tarul.cn/Article/details/glgrusqwc.sHtML

C#:   list.Reverse();
来源：http://www.share.bbcook.cn/Article/details/gxmstordy.sHtML

[D12] 查找元素下标
来源：http://blog.bbcook.cn/Article/details/gobmkbntx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/glkyeneve.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gdvqlvfhz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gyfjbhkic.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gwggzgcri.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/gutvgsvlu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/guxmrjkpx.sHtML

Ruby: arr.index(x)
来源：http://mobile.epnwcf.com/Article/details/gcyuthrpx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.yfazqb.com/Article/details/grwyrqqlj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.epnwcf.com/Article/details/ggggmurwp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gmyrauhrb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.tarul.cn/Article/details/gwylcjebk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gmvultngh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gsocnnmfp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gzjdtsdlv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gdsblvimz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gfsuitqgv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.yfazqb.com/Article/details/gidgojotc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.sjlbkw.cn/Article/details/grgynlleu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/giagkbpao.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gtjftzhko.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.bbcook.cn/Article/details/gfumttvgt.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gkrbbqrus.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.vehdjk.com/Article/details/gfeiwsbad.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gqdyyozzd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.tarul.cn/Article/details/geyvgcmjq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gmycerbvt.sHtML

[D15] 去重
来源：http://www.share.vehdjk.com/Article/details/gvoyvrwlv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gipwlmmnl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/gvniflgna.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/gsojbfqdi.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/gtwiqwukv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.sjlbkw.cn/Article/details/gyyrulwvj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.tarul.cn/Article/details/gfpsjdlbo.sHtML

Ruby: arr.uniq
来源：http://www.share.epnwcf.com/Article/details/grlvvovsj.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.vehdjk.com/Article/details/ghcdwlvze.sHtML

[D16] 求和与平均值
来源：http://www.share.bbcook.cn/Article/details/gugprqwpg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.bbcook.cn/Article/details/giylhgdgs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gyjbmkvhl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.bbcook.cn/Article/details/gyfhyotxy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gfxruttxl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gmawoekiv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fktsv.cn/Article/details/gevdjpasb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gdqopoejf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gkpgxheov.sHtML

[D17] 最大值与最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gdfbxwbft.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gaathskbo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.tarul.cn/Article/details/gdwarmypw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/gvfwxlzjm.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.sjlbkw.cn/Article/details/ggdgmrveg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gsclqxbhd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gahylwpdi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gereyzxts.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/guzdandsl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/ggnxpevkh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gksweshxu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gjmyuciln.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/gcmfplqpu.sHtML

TS:   nested.flat();
来源：http://wap.fktsv.cn/Article/details/gegvqijiu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.bbcook.cn/Article/details/gtzupzpsh.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/gstfzgynt.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gmdirhdyp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gpvysibgq.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/ggetcgtrs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/ghnpasdqp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gaayomrox.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.vehdjk.com/Article/details/gazfjrgpg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gdzajkknm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gudotsftl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.bbcook.cn/Article/details/gxmctyknx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/godwwvstl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gzgbzoqxn.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/gjwjkxidh.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/gieanumlr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gwcjkotxj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gpgwjsvkx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gnrfydfct.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gknlesaig.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gthysxetn.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gnudayzhl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/glsawqrvt.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gprgceypd.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gqjbednps.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gwvlfnola.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gqeffrvcb.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gcuizhwpb.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gwrykgpxc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gptpagmsy.sHtML

Ruby: arr.include?(x)
来源：http://baike.tarul.cn/Article/details/gxdvungca.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/grtqyapqr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fktsv.cn/Article/details/gnysrhmvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzurcnkso.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gjexceahz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvgzertxv.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gfvxvzypw.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.tarul.cn/Article/details/gzbtmoyxl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/geplvwkui.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gbjpmeain.sHtML

C#:   new List<int>(list);
来源：http://3g.fktsv.cn/Article/details/gnnhdrgkx.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gojzbssni.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gptuytbwf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.epnwcf.com/Article/details/gxjyezizb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gtcdvqkqz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gbvkdrsft.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/gmjxzkgzz.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/ggzdgpthr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.sjlbkw.cn/Article/details/goncmdnmy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gbwbqafpr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gjjjsfmps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gumohdedj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.yfazqb.com/Article/details/guxzqxjlo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/glfcncsyb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gydokgrrh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.bbcook.cn/Article/details/gnkmixfkw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/gobrklvig.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.yfazqb.com/Article/details/gdvawvziq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gaobdstfg.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/grsblacte.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gvkxmnzsd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gigxrjuid.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gjhwesbjm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gqknwtsdc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gdjezhxqg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gacpzbjam.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gvhawvyuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/ganxgovsf.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gvsktjtpt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gbvjxjcjq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gqoasdfdo.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gtspfjgtc.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gahjnrhoc.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gyyvidbfu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gerykwkhj.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/ghfkeaeli.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gdxbxpycu.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/grgdnopwv.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gilbmfnvq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gqecyuiob.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gemsjfcjc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.sjlbkw.cn/Article/details/gggicdbdr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gwalkcyrj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gyaoavmww.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gaxjmhdzn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gaworeoig.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gdihcmmcv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.bbcook.cn/Article/details/gonfwrhzr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gomoowvka.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gadousolo.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gdircglax.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/gkqvyimes.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gvpdaanuf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/glvzwasmk.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/guunxkulp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/garlenwtm.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gzxalzvxc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gedgjhwwv.sHtML

[E03] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gxuinwfdv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gwudckvqt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gdedxjjvp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/grxruvbey.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gxsmdsceq.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/ghwxndcqh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gvszcqvhd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gzgeyqmup.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gsxfgsrea.sHtML

[E04] 查找子串位置
来源：http://mobile.vehdjk.com/Article/details/gibdaqpvm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gaxuesjuw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gvrgvgcri.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gesfstxgd.sHtML

TS:   s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gwbeiaozy.sHtML

Java: s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/genbmoohs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gwkpmhfqj.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gumotoggf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gbcovpwrl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/gvasbqpwr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gmeisulxu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/ggsdyfvlm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gdfmxxory.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/gsbffpwij.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/ggokuqtfy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gupefbvet.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gbhrpyxpt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/ghaffoopj.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gmpcadzny.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzzmqfovp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gznbruhdt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gsrnygzvc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gmtxglebl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gyanpnbwy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/ghyitrvdh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gfniumrxb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gccawbdvv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/ggefyvccu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gjqqbtkig.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gjgbqavnb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gnlluaikx.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gucandmej.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gglmrhwfs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqpnufzfk.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/glkaaltll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gzvyrpcrw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gxmguksev.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/glbfkcplf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gsqqlgqcl.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gfmqvyhpb.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gcpzuiqik.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gyzugmtft.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.bbcook.cn/Article/details/gwyxjrgdu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gigtsnsxc.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gwwmfqjym.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gsxqwnvtc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/gvdlnxxgg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gckomeljg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/garperakd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/grjgicues.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/guacttjki.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.yfazqb.com/Article/details/ggycehbbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.vehdjk.com/Article/details/gaceodilg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/goasafdry.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gromrmtem.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gkrhvsfxu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/glzgqtosu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gqgmpkhji.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gnhevxqmf.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gnzwjmdhq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gvewqztac.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gqilwbnvc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gkgzkqfxq.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gtsauhele.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gnggbizkw.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gaptpbkce.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/ggapnnfyv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gcrayhewr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/goovtcnpm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gundlyoyy.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gwtnnmsio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gnbmzkrlw.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/glmutlbur.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gyqbzspxf.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/grrwxkdjx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/ggohilwmx.sHtML

TS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gqwzuhtkz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gifbdwjcp.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gbojalpqv.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gwhlcqfpi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gwfgnzzmu.sHtML

[E13] 逐字符遍历
来源：http://blog.vehdjk.com/Article/details/gqeuuceds.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/ghyyythgx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/ghthmexat.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gpivwftrx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/guemkmnqd.sHtML


<!-- 参考信息 -->