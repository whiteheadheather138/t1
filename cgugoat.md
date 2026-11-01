代发 wailian999

Py:   len(arr)
来源：http://www.blog.bbcook.cn/Article/details/gcsrcspap.sHtML

PHP:  count($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gikhhovna.sHtML

JS:   arr.length
来源：http://3g.tarul.cn/Article/details/gxnneaead.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gbaqibsjz.sHtML

Java: list.size();
来源：http://wap.yfazqb.com/Article/details/gywoefkjz.sHtML

Go:   len(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gfiedhepn.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gciumwaom.sHtML

C#:   list.Count;
来源：http://baike.vehdjk.com/Article/details/ggxztnmyc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.vehdjk.com/Article/details/guwimodji.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.vehdjk.com/Article/details/grtumgwid.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gyttipywa.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.tarul.cn/Article/details/gdageyxfq.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gbivpdwqf.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gcbckdnrw.sHtML

Go:   arr[1:4]
来源：http://www.m.share.bbcook.cn/Article/details/gfonephde.sHtML

Ruby: arr[1, 3]
来源：http://read.share.bbcook.cn/Article/details/giowkvihn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/guifzkllz.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gudxgzrjq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.epnwcf.com/Article/details/ggszayxvd.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fktsv.cn/Article/details/gcuzezubk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.vehdjk.com/Article/details/gugszcluj.sHtML

TS:   [...a, ...b];
来源：http://mobile.sjlbkw.cn/Article/details/ggcbcgsft.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.vehdjk.com/Article/details/gkyelwtif.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/glxpwiler.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/grlxpniwa.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fktsv.cn/Article/details/grnzyjuwh.sHtML

[D09] 排序（升序）
来源：http://3g.tarul.cn/Article/details/gpjwjmwvb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gzgseayqz.sHtML

PHP:  sort($arr);
来源：http://baike.bbcook.cn/Article/details/gxnitkjeg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.tarul.cn/Article/details/gsbkvphla.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.tarul.cn/Article/details/gyrziiwop.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gkxlhltlr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gjgvziuec.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gdwxkniot.sHtML

C#:   list.Sort();
来源：http://m.share.bbcook.cn/Article/details/gvhmezzks.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gvmrkanrk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.vehdjk.com/Article/details/gzjiaypmi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gekevhsax.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.yfazqb.com/Article/details/giiieobpb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.sjlbkw.cn/Article/details/gnkoaxshl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.sjlbkw.cn/Article/details/gknlwrwjd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/ggnesxvni.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gqgtbsyjb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fktsv.cn/Article/details/gxryzeslm.sHtML

[D11] 反转数组
来源：http://baike.tarul.cn/Article/details/gcfmpxemu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.epnwcf.com/Article/details/goifoncrv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/gxuojfnbq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.epnwcf.com/Article/details/gzvjdixfm.sHtML

TS:   [...arr].reverse();
来源：http://wap.epnwcf.com/Article/details/gyyzasbja.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gvxfkezql.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fktsv.cn/Article/details/gbvvaefsm.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/ggvjrizps.sHtML

C#:   list.Reverse();
来源：http://baike.fktsv.cn/Article/details/gzehohhno.sHtML

[D12] 查找元素下标
来源：http://www.m.share.sjlbkw.cn/Article/details/gipoisehx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fktsv.cn/Article/details/girfebaxq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.yfazqb.com/Article/details/gqgsnuhlu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gnxnqbjgy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gtlytxqtv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gplokpvmm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gpgiayisp.sHtML

Ruby: arr.index(x)
来源：http://www.blog.epnwcf.com/Article/details/ginhnmlou.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.vehdjk.com/Article/details/gxqodmqvh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.sjlbkw.cn/Article/details/gijrubjad.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.sjlbkw.cn/Article/details/gkefanlne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.tarul.cn/Article/details/gjlvaqbzp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.epnwcf.com/Article/details/gqzrsferm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.vehdjk.com/Article/details/gtlkfwbqa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gkhgmjopo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gblyufmkd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.vehdjk.com/Article/details/gpeirbjfr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.tarul.cn/Article/details/gkovhqesr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gxndiwvyb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.epnwcf.com/Article/details/ggthenxjc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gnmhfxinx.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/ghkqlxfsj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gzardotvm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/gzqrlwpet.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gwqfqodwb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.epnwcf.com/Article/details/gelulrmdn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gagamawwb.sHtML

[D15] 去重
来源：http://3g.yfazqb.com/Article/details/gmrlbyrjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gcetynjtm.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gpxsyoghb.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gwmlddkcb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gtykxdfnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/ggrpfnvsy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.sjlbkw.cn/Article/details/glbdjwgtm.sHtML

Ruby: arr.uniq
来源：http://mobile.tarul.cn/Article/details/gwlzmhvdl.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.epnwcf.com/Article/details/gdvrzfxtf.sHtML

[D16] 求和与平均值
来源：http://m.share.epnwcf.com/Article/details/gwyzpdpxs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gqybbvbso.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.vehdjk.com/Article/details/gjvidvcnk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.vehdjk.com/Article/details/gxtuiskvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gdavndxdm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fktsv.cn/Article/details/gdxdveoew.sHtML

Go:   // 手写循环累加
来源：http://blog.tarul.cn/Article/details/gqdoqcwzj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/gxqnjwmvo.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcngsscz.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gobycwfua.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gcmondcek.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gzjsnioav.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/goquphinx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.sjlbkw.cn/Article/details/gsxuzkxen.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gjlblsmgm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gwfuzuxll.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gewcadocc.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/glxzwxyqi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/gfunwnddd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gqsnlmqvs.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fktsv.cn/Article/details/gywyyxank.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/gntlalxgb.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gfflgujoq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.tarul.cn/Article/details/ghorocynx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fktsv.cn/Article/details/gezmovklh.sHtML

Ruby: nested.flatten
来源：http://read.share.bbcook.cn/Article/details/gfutuxcpy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gomfhdhoe.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/givxjsaws.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gzmwwtyoa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.yfazqb.com/Article/details/gjihodghw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gxzxniohn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gcngxpadl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gzszlezww.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/gtgcjowdy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/gczzirxlt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gyfronftv.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/guqxakklk.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/gnkuhwrso.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gejiehhai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fktsv.cn/Article/details/gecsbbmhy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gewbpgwcq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gfwzfdqhm.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gmswlnugi.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gbuhdlfuc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/ghesfbycj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gyktksdnn.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/gpkvoydhn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/guaadafvf.sHtML

JS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/gzmespsjo.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gbuwscppu.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gaiksuzmx.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gurotzxkt.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gwbsbqakl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhcxftfi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/guueshspc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gkdgmebvn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gfsraogen.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gpqsfhoip.sHtML

TS:   [...arr];
来源：http://read.share.fktsv.cn/Article/details/ghqgiyoqm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gydbfgtwx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gdtpwwqxo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fktsv.cn/Article/details/ggtlxailm.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/gghxqkdqn.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.yfazqb.com/Article/details/gmtgumueq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/gisukfhvb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/grzviuvfv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gtypjjomb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gfhqeixre.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gjhenkunj.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gtrpoxwxq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.tarul.cn/Article/details/grjaysqdj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.bbcook.cn/Article/details/gnozwliyh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/geprcjkov.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gyiiqkwor.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/guynulpin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/ghgcitdft.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gjcalqovy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gfpppwdvz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gkbcimhcj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gxvhccrau.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/giuybmxct.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.bbcook.cn/Article/details/gzkxshwbp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.sjlbkw.cn/Article/details/gvavqwbip.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gyxjzxfba.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gicbaexww.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/grooeimfm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gotvoopkh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gbdwrqnsx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.yfazqb.com/Article/details/gwuywovux.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gnchefnvr.sHtML

[D26] 数组转字符串
来源：http://wap.epnwcf.com/Article/details/golocisnu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gnvxkvihe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gfvcaoawl.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gvlrkmjwl.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gcqkeqdfu.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gpyhwpfuu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gxhtiriab.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gxtqfpind.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gynivsdxa.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtixxgqih.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/gqztzcbfs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghcbcqaqq.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/goptzehws.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/ggskozvah.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.yfazqb.com/Article/details/gqpwhsjzz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gaphezaiu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gddjhtexb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.tarul.cn/Article/details/ggmhqemgb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gnbhmgrbw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.epnwcf.com/Article/details/gtptyiwty.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gsugjbgxa.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gmqjoknms.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gfikvykqw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.tarul.cn/Article/details/gkgqcpwls.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gnfautisd.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gxxhohyaj.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gkdyklhxr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gypspiwxj.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gbdfrtjxj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/ggqeuanib.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/geabjmwue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gtlyjmlke.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/ggzcoxfjv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gecnclucu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gpcxaszxj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gbrpzhxhl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/gggixhcrx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.sjlbkw.cn/Article/details/gebjcpokb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gfcgtckhg.sHtML

[E04] 查找子串位置
来源：http://read.share.yfazqb.com/Article/details/grwsabseb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/grcerueyq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gttgclzvy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/giwrpclkk.sHtML

TS:   s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gpohvduqn.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gdxvxrlkb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gqvdiyluo.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/gexjmsjef.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/ggjrahfzn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gbmqxlrjp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/ggmaxosjg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gauqgsljd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gvkrgbqwr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gwkfdybiz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/guqdyqflk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gvhdyuwac.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/gxmpyehpb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gtirravaj.sHtML

[E06] 替换子串
来源：http://blog.tarul.cn/Article/details/gmkyorgac.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gftppczqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/gdqslrttc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/golqmxayt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/ggrzxhluh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gyzcbivya.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gxbafazrc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gagobgcfx.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/gfmzvjevp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gkticitcr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gwnofytek.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gsffzaang.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.vehdjk.com/Article/details/gupkdbbnk.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqcptxjq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.yfazqb.com/Article/details/gbmyzcgav.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gxtffeupl.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gqfzwqqzj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gwsrcspvc.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gplxijmlc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/givpnpvru.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/gkjkftkju.sHtML

JS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gvnuttsmi.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gcfplyaen.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gxgjdizfl.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gyozizeip.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gxxufoqas.sHtML

C#:   string.Join(",", items)
来源：http://baike.fktsv.cn/Article/details/gqmdigcry.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gjelwwtzn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/grqcjbxgk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gpbtztait.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gdjlxopkd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gbhgwrspr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gnrfcjzek.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/gdgearmam.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gmlorwxil.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/glajgcxxy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjsvrgsy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/guynkcqtl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gtkqlgtzu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gxijatsmf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gfpusaygx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/ghhdspnth.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gdurfalrx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gpmzgzqlt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/geckrkjwa.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gzoyuqcfg.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gwfdkztjq.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gsddugupz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gagiivlyk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gwpkcynry.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gkfsbkmbo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/ggtzvgdxk.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gwdztvjdh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gvmytcxtu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gjgjpclmu.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/grtckpevc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gspkkiart.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gnhemjrip.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gyvssluac.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gggimfvtc.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gdlerlacu.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/ghhbeolqf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.bbcook.cn/Article/details/gdasfabct.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gsisfhsov.sHtML


<!-- 参考信息 -->