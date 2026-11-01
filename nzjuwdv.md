代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://mobile.epnwcf.com/Article/details/gikzppvyb.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/ggfldcbao.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.bbcook.cn/Article/details/gunlfcvmr.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.bbcook.cn/Article/details/gpdvubogs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gtqvjhzja.sHtML

TS:   [...a, ...b];
来源：http://mobile.yfazqb.com/Article/details/gfvatmpro.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.bbcook.cn/Article/details/graufyzap.sHtML

Go:   append(a, b...)
来源：http://www.share.tarul.cn/Article/details/gewxejwxg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.yfazqb.com/Article/details/grunzhkcn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.epnwcf.com/Article/details/gkanhwlxe.sHtML

[D09] 排序（升序）
来源：http://m.share.yfazqb.com/Article/details/gsqufnqwt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/guuvyzhql.sHtML

PHP:  sort($arr);
来源：http://baike.sjlbkw.cn/Article/details/guklhvsza.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gumqccwuf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.vehdjk.com/Article/details/gjrfolcqm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/gxdhbrycb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fktsv.cn/Article/details/glgmzeuxp.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gqcmzisbr.sHtML

C#:   list.Sort();
来源：http://mobile.epnwcf.com/Article/details/gnjftqfgr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gwqlquasa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.tarul.cn/Article/details/gpgkosrzg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gigllbqth.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.yfazqb.com/Article/details/gnqkpiobt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.vehdjk.com/Article/details/gxklacupz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.yfazqb.com/Article/details/gqtiyirye.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.sjlbkw.cn/Article/details/gtdoblfkh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.bbcook.cn/Article/details/gmthcbblr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fktsv.cn/Article/details/gwlkapbpc.sHtML

[D11] 反转数组
来源：http://m.share.vehdjk.com/Article/details/gwpttgvxl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.bbcook.cn/Article/details/gftvgwrvw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.epnwcf.com/Article/details/gvgdvrrbm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gwqergkxu.sHtML

TS:   [...arr].reverse();
来源：http://baike.epnwcf.com/Article/details/gglzriojy.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.tarul.cn/Article/details/gscprniwc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.tarul.cn/Article/details/gfxwuausd.sHtML

Ruby: arr.reverse
来源：http://3g.epnwcf.com/Article/details/gpwclcxpc.sHtML

C#:   list.Reverse();
来源：http://blog.epnwcf.com/Article/details/gfbkzvdcy.sHtML

[D12] 查找元素下标
来源：http://read.share.epnwcf.com/Article/details/gtpfiskzm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gchjpnvlc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzcwyuatl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fktsv.cn/Article/details/gsqxleaed.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gfsmabbar.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/gzxgckgsz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/guzqezqsh.sHtML

Ruby: arr.index(x)
来源：http://baike.epnwcf.com/Article/details/gxbanqafm.sHtML

C#:   list.IndexOf(x);
来源：http://3g.epnwcf.com/Article/details/gahtcxghc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.tarul.cn/Article/details/gpelazozv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.tarul.cn/Article/details/gpoezlfnb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gdjrolgps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gosqtpsdk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.tarul.cn/Article/details/gkyjesejf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/gmbttatna.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.tarul.cn/Article/details/gwtwfluuo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.sjlbkw.cn/Article/details/gzhpomhwl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gpuqmbqtt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.yfazqb.com/Article/details/gyihtjmhg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.epnwcf.com/Article/details/gsgzdotut.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.sjlbkw.cn/Article/details/gagjzcbvd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gdkwpefpa.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gxtcvllbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gbtuqjiae.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gzhvklkut.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gfkzixitz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.epnwcf.com/Article/details/gtntblvir.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/gshstvttv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.epnwcf.com/Article/details/gooxlvsxi.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/godsaulhn.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.bbcook.cn/Article/details/gpxlcijag.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gfxmmidwy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.yfazqb.com/Article/details/gclhrpbbp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/goofmecqn.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/ggggxvste.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.bbcook.cn/Article/details/giabuekdo.sHtML

[D16] 求和与平均值
来源：http://www.blog.epnwcf.com/Article/details/glmcxcvjc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.epnwcf.com/Article/details/ghkiqgtrk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.yfazqb.com/Article/details/gfriyzoes.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/gbcepccil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/geqxameru.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.vehdjk.com/Article/details/gkqrtllyi.sHtML

Go:   // 手写循环累加
来源：http://3g.sjlbkw.cn/Article/details/gyuadfftw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.tarul.cn/Article/details/gnaoobgiq.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.epnwcf.com/Article/details/gwyogepul.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gbbsrqnwp.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gnwnouiwp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gcoakgdsk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.bbcook.cn/Article/details/gbgspwumg.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gyhevaqhd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gbbeajzhq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gehkvilzl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/grpvnufag.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gqrneghml.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gsvyvpdgh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.sjlbkw.cn/Article/details/gzjzcmedw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/gwafolxby.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gxnyhycjn.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gmsyzfxen.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gvnyyokrx.sHtML

Go:   // 手写双层循环
来源：http://wap.fktsv.cn/Article/details/gucrqwnzt.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gupyrlqqw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gqizgfbpi.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gakreyaik.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/ggqulnqzb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.tarul.cn/Article/details/gtwjwnepe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/goebtrxia.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/ghmuwasoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.epnwcf.com/Article/details/gnwlmksre.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.bbcook.cn/Article/details/gnwiwppre.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gijxulkjq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.sjlbkw.cn/Article/details/gnfwbukhx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gihguwbxc.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gvfhhsmjf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/ghfwbgybw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gehtqsqye.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fktsv.cn/Article/details/gvittpbgz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gryeekvsq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gpwcufkan.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gicaifews.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/gafkymcba.sHtML

[D21] 判断是否包含某元素
来源：http://baike.epnwcf.com/Article/details/gdjzkcxbe.sHtML

Py:   x in arr
来源：http://blog.epnwcf.com/Article/details/gldlbykyr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/gapqizlnk.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gwpdsydde.sHtML

TS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gjwaoryks.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gbnnlfqxy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gyuhwtaeo.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gjkbxlwli.sHtML

C#:   list.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gtzpttkla.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/glwfrxxen.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gzqdwomwh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gqkevwbio.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gwgsxuzfm.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gujvwuvvj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.tarul.cn/Article/details/gtzwbgumc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gwsoipnwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.sjlbkw.cn/Article/details/gwyxzbakr.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/gsvmhmodq.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/glbluarxo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gzfhazlzh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.epnwcf.com/Article/details/gtuwmzufl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gynvqvomk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gbshrhapb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/guiqucwyz.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gbibiqjrs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/ghssumxht.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gbhkewfdn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.vehdjk.com/Article/details/ghygfyabo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gpiefnyvd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gppyywqix.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/ghdexvrgc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gjvpzzima.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/gbyciakuu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gvubgpnhd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gdtsgejvv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gvsavkkpr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/grchhpocw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.vehdjk.com/Article/details/gehypclvs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gblkqrmzm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/giimrhzve.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.yfazqb.com/Article/details/gwfhphrqd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.yfazqb.com/Article/details/gidqzzzyw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.tarul.cn/Article/details/gbrpdpbsu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gubffnlhx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gxdxfmxvb.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gkxuglxjw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/ghbfuwdbp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gyeyrlhmi.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gexpxlhjx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gatcyuqgw.sHtML

Java: String.join(", ", list)
来源：http://3g.tarul.cn/Article/details/gmfiogdqs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gnnztepls.sHtML

Ruby: arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gcpleituv.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gfpurmqna.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvxrfclca.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/gbsdhelhb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtukscsvf.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gtasweftk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gmtnwrdbq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gcijvngwi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gbdxpsmsl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gnstpkhsw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/ggjkpznvv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gfxczwblb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gmpoycslk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gddcddjyv.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gkzqossid.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gslcqtuet.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gdzxtssva.sHtML

JS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gvwkjeutj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/glkuqavrx.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gmwzjmvjl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gcqgfcxyk.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gqjtzugtq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gyvnvpjmg.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gffnxyxcw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gzyprywkf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gzudqlnhz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/grcpukkik.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/geekcehkq.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gwfwtifyz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/grlcilocv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gjjwtwlzg.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.sjlbkw.cn/Article/details/gbjqauqix.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gooagvdnm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gougunkxq.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gbmxzkxts.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/ggjhuzgid.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gtecgkvqm.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gdaxowtgy.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gfbvmphhp.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gbuvegkdz.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gfulnzwvm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gwlnqllnw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gdfoaydcj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gmkvnvmbe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/grruaofzg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/grokfrwas.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gjmhrnggs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gocbjhplc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gkxyayaym.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gricbignt.sHtML

[E06] 替换子串
来源：http://m.share.bbcook.cn/Article/details/gxnbbuvem.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/grmilimhm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gvhfiiuxa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gjksgjbyh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gyodgdhtl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gnaycybcd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gnpxlhoga.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gxwudzlyo.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gtgrbeslc.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gmztymjpf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gxpffonyc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gmlnhitok.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/glrfzivuf.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gctdpxqew.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/ggivrlrxu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.sjlbkw.cn/Article/details/gmmxqjvbd.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gawimnxaq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.vehdjk.com/Article/details/gjuxufyls.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gsqdvcjua.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/glwukcigz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/gxkysugry.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gjhdwlpdm.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gpjyqxgck.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gdskxxxqu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/glfyoqxin.sHtML

Ruby: items.join(",")
来源：http://baike.fktsv.cn/Article/details/gbealtpgs.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/glplbhrxk.sHtML

[E09] 去除所有空白字符
来源：http://baike.fktsv.cn/Article/details/gfkodnwab.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gwgnfeuex.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gpnioiljy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gabtmlsjd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gimxzdtcq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gfbfvarxb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/gqlqazvaq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gaeckepgj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gpoaceutc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/guiysvezl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gtqqqxgly.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fktsv.cn/Article/details/gblqengcu.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gitncbdoy.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gtocrbaqj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/ginzfaygw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gonyrempy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gmlbmgxws.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gtyfvkxji.sHtML

[E11] 反转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gtxxaxuli.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gyqpvhxmr.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gocyjktku.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gtwxzqdor.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gkshrhoip.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.epnwcf.com/Article/details/gtrvymqfs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.yfazqb.com/Article/details/gxqmwmpmg.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gbpowmxbf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gbnfdcygb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gkkmjochz.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gnybpwmjh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/gmtpqdocn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gyfqucsbs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gnlnoeplj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/ggroaadhe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gdeqvuphx.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gsxrpgkzu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gzfsdnftz.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gxkaceawm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fktsv.cn/Article/details/gwletawdi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fktsv.cn/Article/details/gmxqyyovr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gkcvygqgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gfsyihfea.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/geikugkvc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gmtzjmton.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gufcdyobt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.yfazqb.com/Article/details/gvjnheekc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gzutfazsc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/glnmgatfo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/goqogomhl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.sjlbkw.cn/Article/details/gpfaxqzig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/geoxibyxz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gyvtlvcki.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gkceizjyw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.tarul.cn/Article/details/gsmidlvdz.sHtML


<!-- 参考信息 -->