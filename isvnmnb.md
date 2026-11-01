代发 wailian999

Py:   len(arr)
来源：http://www.share.fktsv.cn/Article/details/glknuqtcw.sHtML

PHP:  count($arr);
来源：http://www.share.fktsv.cn/Article/details/gppytizos.sHtML

JS:   arr.length
来源：http://blog.vehdjk.com/Article/details/gqktbytwj.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gayxstaxb.sHtML

Java: list.size();
来源：http://3g.epnwcf.com/Article/details/gtmdvugpa.sHtML

Go:   len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gvulnwdmo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.vehdjk.com/Article/details/gdehlaylk.sHtML

C#:   list.Count;
来源：http://baike.sjlbkw.cn/Article/details/gzebugnsu.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.epnwcf.com/Article/details/gdkuufyye.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.vehdjk.com/Article/details/gzziivgjm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fktsv.cn/Article/details/grgsizoiy.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.yfazqb.com/Article/details/gzrtdkvnp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gkkaojwob.sHtML

Java: list.subList(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gmqgrwlup.sHtML

Go:   arr[1:4]
来源：http://mobile.vehdjk.com/Article/details/ghsidomob.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.bbcook.cn/Article/details/gjedzxozf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.vehdjk.com/Article/details/gjzdqqigg.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/gszzqmyxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.yfazqb.com/Article/details/gefaezvje.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.yfazqb.com/Article/details/gigqbmoky.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.yfazqb.com/Article/details/gsgrncctr.sHtML

TS:   [...a, ...b];
来源：http://m.share.fktsv.cn/Article/details/gqqahqwrq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fktsv.cn/Article/details/gdlwoihwo.sHtML

Go:   append(a, b...)
来源：http://m.share.epnwcf.com/Article/details/grmildemx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.tarul.cn/Article/details/gqchsstcf.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.tarul.cn/Article/details/gzksclvyv.sHtML

[D09] 排序（升序）
来源：http://blog.bbcook.cn/Article/details/gunjwiwjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.tarul.cn/Article/details/gukogkoqf.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/glsnhxuio.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.epnwcf.com/Article/details/gaidlhzhx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.vehdjk.com/Article/details/grmovlsmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gpdisbszz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwbuxjzvf.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/glxhabobj.sHtML

C#:   list.Sort();
来源：http://read.share.epnwcf.com/Article/details/govqqloux.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fktsv.cn/Article/details/gendilyli.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.tarul.cn/Article/details/gsbfiqmnf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gyfjhgvvo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gmkahcbls.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.yfazqb.com/Article/details/gumwgddro.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gtfmomzkf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/ghqqlescz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqlshces.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.epnwcf.com/Article/details/gxltorqqk.sHtML

[D11] 反转数组
来源：http://mobile.tarul.cn/Article/details/gcgvjtelh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.yfazqb.com/Article/details/gdtocbkun.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gavhkojxl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gteqnewvb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/gfixfynjn.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/glbsssjtk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.epnwcf.com/Article/details/gjvhzozqu.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/glweserap.sHtML

C#:   list.Reverse();
来源：http://blog.sjlbkw.cn/Article/details/gthtjrchn.sHtML

[D12] 查找元素下标
来源：http://3g.sjlbkw.cn/Article/details/gjtkwimri.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gzeibvvcl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fktsv.cn/Article/details/gkqcmjkik.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/gxukolwfs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.vehdjk.com/Article/details/gvxvlfbuu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.tarul.cn/Article/details/gfxwytvvb.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gsxlfuxxm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/gdkcdevpa.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/gmlceczel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/ghyciifrs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.yfazqb.com/Article/details/gwsqcehqq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.bbcook.cn/Article/details/gilxgkror.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/ghaixsjwv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/grtjleaha.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.epnwcf.com/Article/details/gfhbeebqc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.yfazqb.com/Article/details/gggwjofmt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.epnwcf.com/Article/details/gurbewlzf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.yfazqb.com/Article/details/ggcqzckzg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.bbcook.cn/Article/details/ghikosovw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gebteryht.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.epnwcf.com/Article/details/gmtigndqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gecqoxhtd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.vehdjk.com/Article/details/gcjtncims.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/guahtsoss.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gdboabpap.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gdsqhxrfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.epnwcf.com/Article/details/gootuzqsq.sHtML

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gwrqwetum.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.vehdjk.com/Article/details/golfuywnr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gvzohpclc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/grcyxtaxi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gmdvikimb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.bbcook.cn/Article/details/gnwupkmmx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.sjlbkw.cn/Article/details/galdxhekp.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gokomxnwt.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gmtgqgorn.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gayfkpgmv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/gstgtlzrt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gvcctlgin.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.bbcook.cn/Article/details/gnbqzuhac.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gxeofqcdr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.yfazqb.com/Article/details/gaesferll.sHtML

Go:   // 手写循环累加
来源：http://m.share.tarul.cn/Article/details/ghfqolhnp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.sjlbkw.cn/Article/details/gjvpwjwxh.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gflwjjvvl.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gdyelstnh.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.yfazqb.com/Article/details/gjyqtirzy.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fktsv.cn/Article/details/gmbvxfvit.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/gplkpazza.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gsmaxgmyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gjbsuryau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gosupixiw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.sjlbkw.cn/Article/details/ggyxjasem.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gtukdayfe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/guewqoiwq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.bbcook.cn/Article/details/gjrfrjbqo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gbolhsodh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gnrbaabed.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gzwzluzis.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.tarul.cn/Article/details/gdxukcuwu.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gvxwaqwvq.sHtML

Ruby: nested.flatten
来源：http://www.share.vehdjk.com/Article/details/gcttlwqya.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/ghlncnayf.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gwgxfuojn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gmvswzazd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/grmsryhtp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/gbuhsmabj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gypbfyzjf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gwdwiberu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/gxjyryhql.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/giyuornyy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gkirubbiu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gaxtafbdx.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gfgdsgbwr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.tarul.cn/Article/details/gdmqewwzs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.bbcook.cn/Article/details/ghvuitrmz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gruerpnyh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.epnwcf.com/Article/details/gvwkruano.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.tarul.cn/Article/details/glwhifwia.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gdrnaqngm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gqhqoccpw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fktsv.cn/Article/details/gbsmfdose.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gaqiwpnon.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gqnbpbuik.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gcbqypdrl.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gwxuttqvf.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/grjcxxmll.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gwksorljw.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gfzvwpxuo.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gzpvtawri.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gvjamcppn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gcokxdvyb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gkjotyvgi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gwkhwwijo.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/glwlchhmv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gjepyouxj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/guncwesfg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gldtazyci.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gmjansxlm.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.epnwcf.com/Article/details/gyqmckfpo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gxofiohco.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gzkpgwgzy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gyavkkgfv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gmfxdymbz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gvsztbgbg.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/gkosikcfm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gpenzzcyc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.epnwcf.com/Article/details/gvhudjjlo.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gtsjslukt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gwfcqjzem.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/guhughnnu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/grbbzvglh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gihojubfj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gcdqnxdfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/gwbhcmzjp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gocypcawl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/grlwmclch.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/ghsanyfav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gfpixxexo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/grutlrfnh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/grldouufi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gxraofjta.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gbedoccab.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gugfvgmtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gerjiezjy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gtesppnoq.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gnnplxzfj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fktsv.cn/Article/details/gwmzzhinw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/grqejvywi.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/ghsoktveo.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gnvjjtcmb.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gdiqjlgud.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/grlztxabk.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gprsmoper.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gjmicumbj.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gncyksjjy.sHtML

E. 字符串处理
来源：http://www.share.fktsv.cn/Article/details/gutihoptx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxfeghlbk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gwbvecchp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gxgbekrdm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.yfazqb.com/Article/details/givfiuaho.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gcjjnbdex.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gdmzbfmmp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gfoesnuxz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gyccbpwcb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gfqciogim.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ghffecoer.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gsfrtgnma.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gatokwrer.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/ghmjrjpxk.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gxbgkyaij.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gzaijvfyo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/getzkbyor.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gfwbuxotv.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gjnvedtgu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gccaublmq.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gtjcpisvj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/gklulqbwm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gpvlkkmxk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gsqpvgqhv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gapygwtqu.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gesbzvnnr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gzrpssqje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/geafzfeoe.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/ggrwmuiwo.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/grevtsmmz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/genhlunro.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/gxdzcsgsj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.yfazqb.com/Article/details/gokelvefx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gdsbeqlvc.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/glajspjsv.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gkzpqukyf.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gwofakvuw.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/ggvzffoxq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/grrhtnvls.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.sjlbkw.cn/Article/details/gmvchewnm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/ggjarfkys.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gkwtpohtl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/ggdccjoqj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gozhkctby.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gxrspslnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.bbcook.cn/Article/details/gjqfcstot.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gjoabwytf.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gvyzlihks.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/ggzpanecv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gdzkaigxw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gxfrillct.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gndcmlkip.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gmoonkafk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gchaeefzp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gfbrzqoeh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gxskpehnc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gxbqcqtwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gtopthbia.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gosgcicgl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/geaaxscsf.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/ggpexjcwi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gcjagpikt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.vehdjk.com/Article/details/gjdcwohhc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gdqfahpzl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gmcfdqwhx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/ghvgrxpsa.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/gwgmvcjei.sHtML

PHP:  implode(",", $items);
来源：http://wap.tarul.cn/Article/details/gfxaquudn.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gtpgetutt.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gtolrkrom.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gqwxnbbhe.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gebkxyfcg.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/gyokkluug.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gfqgonyqp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gtiatluaa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gytqtavdo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gpearavvh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gljairduf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gzuhttden.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fktsv.cn/Article/details/gqszlfhrs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gkugnoyir.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.bbcook.cn/Article/details/gklgdgzpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gdqbrennb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gabnogokz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gqdebmpnk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/ghdwputsh.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gomkpufrz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/grkqzlhne.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/giocavbul.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/giwmenkce.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/grniwlomt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/garzsnyxj.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/gcvvagqkp.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gafklcdeo.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gxzejnect.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gkpegqsei.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/ghvrpagzg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gzjvyocff.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gzvaqtbja.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/glliaoprx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gutuxqfsi.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gkwsfexvt.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gcpqpduxk.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gogkynriz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gnbvpacpr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gbnzudebi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gdwqtkyvi.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gqymcdlun.sHtML

Ruby: s.count("a")
来源：http://3g.bbcook.cn/Article/details/ghgzniuuf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.yfazqb.com/Article/details/gawpwyxvv.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gmwceeomp.sHtML


<!-- 参考信息 -->