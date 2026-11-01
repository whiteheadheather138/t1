代发 wailian999

Java: list.size();
来源：http://m.share.yfazqb.com/Article/details/gugrfojiq.sHtML

Go:   len(arr)
来源：http://www.share.tarul.cn/Article/details/gxzqhphyx.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.yfazqb.com/Article/details/gzxzjnrmk.sHtML

C#:   list.Count;
来源：http://m.share.bbcook.cn/Article/details/ghazxjkiz.sHtML

[D07] 切片 / 取子数组
来源：http://blog.epnwcf.com/Article/details/gatoifrmc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/gsymkadsb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnuicgpx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/ghbvmbsqf.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.yfazqb.com/Article/details/gglixxlmn.sHtML

Java: list.subList(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gbnbutehu.sHtML

Go:   arr[1:4]
来源：http://3g.yfazqb.com/Article/details/gpjdtlnlj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fktsv.cn/Article/details/gquqmjotn.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gbpnrcnxg.sHtML

[D08] 合并两个数组
来源：http://wap.sjlbkw.cn/Article/details/gmvynpirr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.vehdjk.com/Article/details/gwqurdzdh.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fktsv.cn/Article/details/gvigmunbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.tarul.cn/Article/details/gounavkwy.sHtML

TS:   [...a, ...b];
来源：http://blog.vehdjk.com/Article/details/gcklnkwnl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gzckbtqqw.sHtML

Go:   append(a, b...)
来源：http://wap.sjlbkw.cn/Article/details/gehjkdaop.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.epnwcf.com/Article/details/gdhovnrfe.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.vehdjk.com/Article/details/guxygrqii.sHtML

[D09] 排序（升序）
来源：http://mobile.bbcook.cn/Article/details/gqjthkxmb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.yfazqb.com/Article/details/gdhzumjmj.sHtML

PHP:  sort($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gilkoiljr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.vehdjk.com/Article/details/gljemelju.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.epnwcf.com/Article/details/gifymnidn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.yfazqb.com/Article/details/gqglanude.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gkvgwatem.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gkcexvduv.sHtML

C#:   list.Sort();
来源：http://3g.tarul.cn/Article/details/gvesrequz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.yfazqb.com/Article/details/ggiwojzba.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.bbcook.cn/Article/details/gbbrtzqwe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gfbfmeuvo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.vehdjk.com/Article/details/gpatuntlv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/giujimrno.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.vehdjk.com/Article/details/gxlcjkgxe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.epnwcf.com/Article/details/glyfndxwa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.vehdjk.com/Article/details/gqtozohwl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gezooeimv.sHtML

[D11] 反转数组
来源：http://mobile.yfazqb.com/Article/details/gdsejgqgc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/guifrlvgm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.yfazqb.com/Article/details/glcwsmtvd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.epnwcf.com/Article/details/gqouhcrbf.sHtML

TS:   [...arr].reverse();
来源：http://m.share.sjlbkw.cn/Article/details/glshjopkl.sHtML

Java: Collections.reverse(list);
来源：http://3g.epnwcf.com/Article/details/gcuwxdqld.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.vehdjk.com/Article/details/gsgqtpgay.sHtML

Ruby: arr.reverse
来源：http://read.share.fktsv.cn/Article/details/ghfbbwzww.sHtML

C#:   list.Reverse();
来源：http://mobile.fktsv.cn/Article/details/govsfdepi.sHtML

[D12] 查找元素下标
来源：http://blog.vehdjk.com/Article/details/glrnsnoih.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gyyqplomc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvvpeqwik.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gqbilbzet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.yfazqb.com/Article/details/gvxzolhyo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.sjlbkw.cn/Article/details/gwqgdullv.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gchqxufnh.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.epnwcf.com/Article/details/garktavfa.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.yfazqb.com/Article/details/gkixsxoiv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.vehdjk.com/Article/details/gbmrukuqq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.epnwcf.com/Article/details/gfaupmily.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gtlxjnzff.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fktsv.cn/Article/details/gqqxzqylp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/gafdjhspf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gzhmyqdvx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.epnwcf.com/Article/details/gyqioowak.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.tarul.cn/Article/details/gsuhdesxq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.epnwcf.com/Article/details/gggvksgxc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/glqtyjygp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fktsv.cn/Article/details/gmuarbbwc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.tarul.cn/Article/details/gxfsfecvt.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gbfgtjewe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gwwkimlje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gybtyrdjr.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gvykfqybv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.epnwcf.com/Article/details/gefrtedyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.epnwcf.com/Article/details/goywjwgua.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gcddkmsvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.tarul.cn/Article/details/guktkobno.sHtML

PHP:  array_unique($arr);
来源：http://3g.bbcook.cn/Article/details/gqfrxnapy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gkxlastng.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gkmznbdri.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.sjlbkw.cn/Article/details/gpfdkbsrr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.bbcook.cn/Article/details/gscgnbftv.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gehlhmzge.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gtzhhrwny.sHtML

[D16] 求和与平均值
来源：http://blog.tarul.cn/Article/details/ghweowrme.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gwyojeavj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.bbcook.cn/Article/details/gksnwpuar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/giqjlusil.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gnwqgosxa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.sjlbkw.cn/Article/details/grqfufufi.sHtML

Go:   // 手写循环累加
来源：http://wap.yfazqb.com/Article/details/gahdplqhy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gwjmuyqgc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/goqhlagli.sHtML

[D17] 最大值与最小值
来源：http://www.blog.bbcook.cn/Article/details/gudqrhwxm.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.epnwcf.com/Article/details/gwnxjnnpz.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.bbcook.cn/Article/details/goelhwnfi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/grzoccuyy.sHtML

TS:   Math.max(...arr);
来源：http://baike.vehdjk.com/Article/details/gdwdwxwxv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gxmhdmlym.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/ghykzlptu.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/gobkzdztz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gvxhpguod.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/ggpedzoos.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gflslhich.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gbyiqcuou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.vehdjk.com/Article/details/gzmbdkbvg.sHtML

TS:   nested.flat();
来源：http://www.blog.bbcook.cn/Article/details/gkmpekdkl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gpfqhruux.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gwaomkpjj.sHtML

Ruby: nested.flatten
来源：http://wap.vehdjk.com/Article/details/gcoqdldck.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gaenxnoax.sHtML

[D19] 按字段分组
来源：http://www.blog.yfazqb.com/Article/details/gfwxbzxjw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/guqdxchca.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gadkwplst.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gsmkxopqv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/grhvexnwn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/geshtcpgx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/ggzuuvdip.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gsbksntak.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fktsv.cn/Article/details/gpasnjxhv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.tarul.cn/Article/details/gzucytmso.sHtML

Py:   Counter(arr)
来源：http://www.blog.yfazqb.com/Article/details/gmlibrvko.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/galiajzcu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gxrmwkjdo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gcjxebzxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/gpaluhhmw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gccshroqy.sHtML

Ruby: arr.tally
来源：http://3g.fktsv.cn/Article/details/gnatkghjc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gfjiowpce.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gjyljzifu.sHtML

Py:   x in arr
来源：http://www.share.tarul.cn/Article/details/gplejsraa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gosqawuwq.sHtML

JS:   arr.includes(x)
来源：http://www.blog.vehdjk.com/Article/details/gliegdatx.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gdudufvhe.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gtouftpmu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gibmrttwv.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/guqlsqvwr.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifjryhhb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/geawzvkpu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gevwlxqji.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gqtnmxyde.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.yfazqb.com/Article/details/gvsauxdwr.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gvdkehowq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gcvydkyzk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.tarul.cn/Article/details/gktihwncz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/ganyyiypc.sHtML

C#:   new List<int>(list);
来源：http://3g.bbcook.cn/Article/details/gyoetvyfc.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gpbtqxjfu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/givbnbyur.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gfzktbvdw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gcvcgualx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gjcqygylq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gpoutghic.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gwyogdupx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gnlcngnbo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.sjlbkw.cn/Article/details/gvistdrsz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gfjilzpjq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gksjwigmv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/gwbkjyycd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gxnlvmjoh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/govsasydm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gpcfwmbpg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gpgpqnilr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gfeuifvnm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gvifrngjn.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/gwmunjdjn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gjasvhwde.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/goegctvpj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.yfazqb.com/Article/details/glpgbmuta.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gzmdgzxxx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gzubgmsca.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gyhboljly.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gdyrsrpiq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gdphqhrwe.sHtML

[D26] 数组转字符串
来源：http://baike.vehdjk.com/Article/details/gbllidrcq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gffwypzya.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/grlibjhlq.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gqljxcuhi.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gzceonckm.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gavxvnesb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gkixyoubv.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gngqzjibq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqojfuvwj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbqtexpcb.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/gaanwwvas.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gonpknsss.sHtML

[E01] 拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gbwaocsln.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gsvuzgdxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/ghptfixam.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gmuogmann.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gbqebvlfc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gbmgnphjq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fktsv.cn/Article/details/gtyjqvswc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gvrsgjlgq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gpugwjdru.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gynhskibj.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gvgebkwxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwvcjolix.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/geizyuqxy.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gbqofxmbt.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/ggvilicah.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/gzxtycmqf.sHtML

Ruby: "ab" * 3
来源：http://blog.epnwcf.com/Article/details/gfzmvmmvv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.epnwcf.com/Article/details/gdxymccjz.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/ggqaiuefj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gfvmxmrvw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gutkquwce.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gnqugyxrk.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gsgaxaonm.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gmmrlngxa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/glkmralop.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/grxzktxpj.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.tarul.cn/Article/details/gbpxyxirp.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/gtjvizlsj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/glzqetkps.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gveypfbcv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gxpamjtvz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gdghfptni.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gwahaccbj.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gpmbfoogi.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gigvbzkax.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/grjvlljca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.bbcook.cn/Article/details/gzwlqixzp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/gmugtehle.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fktsv.cn/Article/details/gziyhsytw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gaopgagye.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/giisvtbul.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gsqcunrzs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gfppcfjdp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gjgdfwxos.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhueiaad.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/geewczxxr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gmtzumpuh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.vehdjk.com/Article/details/gzmjpkmwi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gjbbilcqx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/guvworyqu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/glquvdnog.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gtxazfpsn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/grvxsrvfa.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gwkbhkpan.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/ganyxhvhg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/gjuglknfi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gntexxlnl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/ggptutsje.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/gjtspmelt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/grgqkcuur.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gfrdgmbqe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.sjlbkw.cn/Article/details/grgdarhkx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fktsv.cn/Article/details/gpsjpfttq.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gizfimmas.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gtotfudhh.sHtML

PHP:  implode(",", $items);
来源：http://3g.fktsv.cn/Article/details/guvpgzufl.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gaavtnxom.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gueihhaon.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/ggydiiuif.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gpwzsmeij.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/gxkenjohp.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gmvowbpii.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gbgjtyxjj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/ghxjcgivb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gdybnqdxn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gkjmkltga.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gudhbpeah.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.vehdjk.com/Article/details/gnkehyjus.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gijbxqrvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/ggwwgoyif.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.tarul.cn/Article/details/gpljkaxuv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gccmyvknm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gipycjwbu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gsgcwmfwm.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gcbwlktno.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gehbmssse.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkfjjjr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gqgpskarq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gjruyieyx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/grusyqxlx.sHtML

[E11] 反转字符串
来源：http://blog.fktsv.cn/Article/details/ghvxxxweu.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gimwdijkg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.tarul.cn/Article/details/ggzughnll.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gmasppere.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gokuadbuw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gqfcnwihz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gddbelhoc.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gvdnvjfpb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gmbzgruch.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.vehdjk.com/Article/details/gttscskzk.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gdctwgdkj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gskfmwcnb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gaeercspy.sHtML

TS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gyqcgtbqa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/glojdvrss.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gukvyshco.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gpusqqlqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/gbzojkldb.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gpmvdsrid.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/granwsrbs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gorojaijk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gvyjpwmzq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gzdfarfsy.sHtML


<!-- 参考信息 -->