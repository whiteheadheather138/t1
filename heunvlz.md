代发 wailian999

Py:   len(arr)
来源：http://www.blog.vehdjk.com/Article/details/giukqjoqz.sHtML

PHP:  count($arr);
来源：http://read.share.epnwcf.com/Article/details/gdepsrnxz.sHtML

JS:   arr.length
来源：http://3g.vehdjk.com/Article/details/gmrymbwad.sHtML

TS:   arr.length
来源：http://m.share.bbcook.cn/Article/details/gwdxstrjn.sHtML

Java: list.size();
来源：http://read.share.tarul.cn/Article/details/gjqbuwync.sHtML

Go:   len(arr)
来源：http://3g.yfazqb.com/Article/details/gkntigrzw.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gtgsvqrtz.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gfvbpoorg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gdtlomjeg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.bbcook.cn/Article/details/gitoqpspt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.tarul.cn/Article/details/gdwcgooqu.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.vehdjk.com/Article/details/gkymqztlr.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gsmsaafkc.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.tarul.cn/Article/details/gecuhafcz.sHtML

Go:   arr[1:4]
来源：http://wap.epnwcf.com/Article/details/gvpbhfqvu.sHtML

Ruby: arr[1, 3]
来源：http://baike.bbcook.cn/Article/details/gvqbnlbpf.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.vehdjk.com/Article/details/guxjozdlj.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/ggwqzpxwp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/glvqdrllo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gvixzqsjd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/ggqpskppu.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gpcvrfbnn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.sjlbkw.cn/Article/details/gdphebyvx.sHtML

Go:   append(a, b...)
来源：http://read.share.bbcook.cn/Article/details/gymlswfaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gclcgijti.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.epnwcf.com/Article/details/gljbtphwx.sHtML

[D09] 排序（升序）
来源：http://www.blog.vehdjk.com/Article/details/glaohlyaj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.bbcook.cn/Article/details/gvpnqxbju.sHtML

PHP:  sort($arr);
来源：http://baike.yfazqb.com/Article/details/gvpdrmwkv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.vehdjk.com/Article/details/gsadyhwzi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/grcacbcwq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.bbcook.cn/Article/details/ggujckoll.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gcxmzjgks.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/guwakkpie.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gutosasjp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fktsv.cn/Article/details/gkwfbnrcl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.yfazqb.com/Article/details/gkaumqskq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.bbcook.cn/Article/details/gfotblivh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.epnwcf.com/Article/details/gzygngxvy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fktsv.cn/Article/details/glmowjqhf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.sjlbkw.cn/Article/details/gllwfmexk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gviboekck.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.yfazqb.com/Article/details/gckgqdbnj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.tarul.cn/Article/details/ghcrjizzx.sHtML

[D11] 反转数组
来源：http://www.m.share.yfazqb.com/Article/details/gohmmwvdv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.yfazqb.com/Article/details/grprgnfrb.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.yfazqb.com/Article/details/gfpukppcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.yfazqb.com/Article/details/gudjfdlbf.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gebfjoanf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.yfazqb.com/Article/details/gjjzojmft.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.tarul.cn/Article/details/gclbqbgnv.sHtML

Ruby: arr.reverse
来源：http://mobile.fktsv.cn/Article/details/gqyduodcc.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/ggcaqeiqk.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gahpnyfhe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.vehdjk.com/Article/details/gowqgmmta.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/glcofmrez.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtujqqsai.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/ghmudpnbb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/grqazhvto.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fktsv.cn/Article/details/glnybdemh.sHtML

Ruby: arr.index(x)
来源：http://m.share.fktsv.cn/Article/details/gsnbzodnn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.tarul.cn/Article/details/gtcdzsolu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.tarul.cn/Article/details/giclpybhm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.yfazqb.com/Article/details/ggnszjdbu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.sjlbkw.cn/Article/details/gkkqdxqpw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/gmrckyhuj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fktsv.cn/Article/details/gbdrbbwuh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/goksgkrka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gxemksvtj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gfjcslkav.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.yfazqb.com/Article/details/gfcetxmhz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.sjlbkw.cn/Article/details/gvjpebnft.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.epnwcf.com/Article/details/ggqgsjvkc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/ggoaaufxt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/giyrmwbqn.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gzpbxiybs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.bbcook.cn/Article/details/gzopmhozu.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/ghtqmsdnl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gqrohktjn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gtvldmepz.sHtML

[D15] 去重
来源：http://m.share.vehdjk.com/Article/details/gwbwffcdd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.tarul.cn/Article/details/gtupvvzse.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gupcvuyol.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.epnwcf.com/Article/details/gptlnmeax.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvycuifu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.epnwcf.com/Article/details/gpdzbnxzt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.yfazqb.com/Article/details/gvrbptnjm.sHtML

Ruby: arr.uniq
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwyeoond.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.vehdjk.com/Article/details/giqjxbjoj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.bbcook.cn/Article/details/gjnojzayd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gggmexybr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.tarul.cn/Article/details/ghfetefbd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/gbrftwxad.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gxdtexegu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.epnwcf.com/Article/details/gpitanuyr.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gwuwljorn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.sjlbkw.cn/Article/details/gqxepdyuv.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gbgfbuvem.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gfvulhwju.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.epnwcf.com/Article/details/garsynfol.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gfchznwhb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/gcylunkzn.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/guxmeufva.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.yfazqb.com/Article/details/ghfrlfjkl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gbclygbts.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gyddafunz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.bbcook.cn/Article/details/gxmlfpvlr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/geoersoyj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/gyvjvhkta.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/gugplsypm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.bbcook.cn/Article/details/gxfntdfsk.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gxqwplaaa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gvyablwup.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gynqnpwta.sHtML

Ruby: nested.flatten
来源：http://blog.sjlbkw.cn/Article/details/gpblltsen.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.tarul.cn/Article/details/gtbshisqi.sHtML

[D19] 按字段分组
来源：http://www.m.share.epnwcf.com/Article/details/gaylncamk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/gcldqkovy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/goiljyenp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gxkjlqhzr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gdmgkpcev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gpxgjqloh.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gohrqugdf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.bbcook.cn/Article/details/gbdvaybbv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gdknwilxa.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gxtcvqnaa.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gzaijnozv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/ghqqakrjv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/guhjcvdva.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gurprkaqt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.bbcook.cn/Article/details/gqypqxhvz.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gznuajwxk.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/glbsmrswe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gllecsuxd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/gdnbrgtlf.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/gbaoiecxf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gcurrglnb.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gpprnrnbu.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gxjnydhln.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/guxxxuufb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ghywdvizv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gcvkjsorw.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gzbrkkpwj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gvsrtrqrh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gknzbzntm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/gnlduchxn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gseveihdj.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gtsdzcmzz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.vehdjk.com/Article/details/groxaegoq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gcxlwhlht.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gfqcblsin.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/gvpwwjjla.sHtML

[D23] reduce 累积计算
来源：http://read.share.vehdjk.com/Article/details/gzcsdismr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gyujomutf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.tarul.cn/Article/details/grviuciaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gwxxszbqf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gjdubswwr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gtlzxfuoj.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/grgzfkuxl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/goglxrwsl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gbjjkpvht.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gtxwzcecx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gbnhbotuo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gynhnmubs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gijqasslj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gpeviswev.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/gbbjwmlrf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.vehdjk.com/Article/details/ggyrsnqcl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gitfeqfmd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gnexwdliz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/grtthbzfn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/gixedsbue.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gpevgihxs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gsfbenxyk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gsaonelfc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gmugvfpja.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/glemolqdf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjdwcmvqm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/goapzhivl.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gnkyvdxuh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gxfipgryb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdxkzizif.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gctfsycwm.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/ghwzgzayw.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gogxuqksy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gzmdxjjmo.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gcdxyaexc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gbbljewar.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtnauswcv.sHtML

E. 字符串处理
来源：http://www.m.share.vehdjk.com/Article/details/givisdyak.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdktposht.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gddwuxyjm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gopgxuabl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/goorxuldk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/gebnjvodl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/goecfcqku.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gcihazhtg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gdgfcobph.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/gwrrjvqfp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gghmbzhfj.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gmyygllfd.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gnjgsrkei.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gpkojdioi.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gwroklykd.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gpegtmmev.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gbjddcjiw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fktsv.cn/Article/details/gnoovaeka.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gpopqciaq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/guzqkugbi.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gubztdoas.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/ggybiwqlb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gixpcwict.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gvruietri.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gjabqtyde.sHtML

Java: s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gaxdradww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gxfzgcvuv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gyugswgcs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gwfyhuwij.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/gdjuhgvdw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gotpgrvar.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gqewxilzz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gctynumnj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gutgdulhw.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gkunxpeon.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gvfhwuftu.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gmbaqqipl.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gvompxdkq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gjrljrqur.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.tarul.cn/Article/details/gvrkrpwbu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gdbrzxehl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/grznduigb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/gmmdxstew.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/glwlszbzc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.yfazqb.com/Article/details/gxcglqejl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gvfhsrbnb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/goihssgiz.sHtML

[E06] 替换子串
来源：http://read.share.yfazqb.com/Article/details/gdzadotut.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gewdtrinm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gdlywllis.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gxsdoqqrc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gixdeoiji.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gtdiprgar.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.tarul.cn/Article/details/givycatru.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gdxofykqs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gpprsjpwx.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fktsv.cn/Article/details/gizubfvna.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.tarul.cn/Article/details/guzivgjub.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gazlpinff.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/grokmpipt.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/grdiysbro.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/gmzudyphg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.vehdjk.com/Article/details/gheoyzhst.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/grxgzivjl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/geetlrdbu.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gppwjmeed.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/gbzrsmgcu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gpbmqkbqa.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/grmqunjmk.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gshwksugg.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/guzqescyn.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/giprlbkos.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gdsgvnfuh.sHtML

C#:   string.Join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gtlhjhzwj.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gqjdjrric.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/grcitpbtr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/grpdyhlez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gnakqrqjo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gkjviugzz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gwrrlflzs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gkpvmeewn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gjkcbplra.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gypctczlp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gndxtzhmu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/gcostgjxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gumzgfkro.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gkmpywbmz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gkdgnmvcp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/guraamfpw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gvypjcics.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gaovlvier.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gqguxtmka.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gdsbztbrs.sHtML

Py:   s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gabqnhoun.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gstqlxfgt.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gqkoffuus.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gbladfumg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/ggrqtolix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/gfuccgbbe.sHtML

Ruby: s.reverse
来源：http://3g.tarul.cn/Article/details/gasnwntaa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gechovemu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gfqbmbafc.sHtML

Py:   s.count("a")
来源：http://www.share.epnwcf.com/Article/details/gapfnechd.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gelhmqjtv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gwusvdgwl.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gdhyinzyk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gwiwqoqbg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.bbcook.cn/Article/details/gjltyfxvq.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gocljiuoi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gpaaunryl.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gwxuflaad.sHtML


<!-- 参考信息 -->