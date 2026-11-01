代发 wailian999

Py:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gcsphidxf.sHtML

PHP:  count($arr);
来源：http://3g.fktsv.cn/Article/details/gdsxagfbz.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/ghrhpsshx.sHtML

TS:   arr.length
来源：http://wap.sjlbkw.cn/Article/details/gcmmbjkyt.sHtML

Java: list.size();
来源：http://www.share.fktsv.cn/Article/details/gbskzquur.sHtML

Go:   len(arr)
来源：http://www.blog.epnwcf.com/Article/details/gomqlxskn.sHtML

Ruby: arr.length; arr.size
来源：http://baike.sjlbkw.cn/Article/details/gblzubgji.sHtML

C#:   list.Count;
来源：http://blog.sjlbkw.cn/Article/details/gopbdtyrj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fktsv.cn/Article/details/gyqqvhczk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.tarul.cn/Article/details/gjzvchfpl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.yfazqb.com/Article/details/gpyqvqxcj.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fktsv.cn/Article/details/gixnvdcxd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gjtxinqkp.sHtML

Java: list.subList(1, 4);
来源：http://www.share.yfazqb.com/Article/details/ginfwbolz.sHtML

Go:   arr[1:4]
来源：http://baike.yfazqb.com/Article/details/gvweaksfn.sHtML

Ruby: arr[1, 3]
来源：http://read.share.epnwcf.com/Article/details/gnbtlxklg.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.bbcook.cn/Article/details/glmrehshg.sHtML

[D08] 合并两个数组
来源：http://www.m.share.vehdjk.com/Article/details/gfzweqxqu.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.yfazqb.com/Article/details/geqttuzjv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gyvrzfydy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.epnwcf.com/Article/details/gtrtwocvs.sHtML

TS:   [...a, ...b];
来源：http://wap.epnwcf.com/Article/details/gzuemmwhg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/grzqamcdf.sHtML

Go:   append(a, b...)
来源：http://www.m.share.tarul.cn/Article/details/grjvofthv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.vehdjk.com/Article/details/gofrjnnsh.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.vehdjk.com/Article/details/gdsoggnuh.sHtML

[D09] 排序（升序）
来源：http://www.blog.bbcook.cn/Article/details/gsllijgrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/ghdbxwzpy.sHtML

PHP:  sort($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gvnydwjwu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.tarul.cn/Article/details/gqxsudtkd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gtpipugwy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.vehdjk.com/Article/details/gamggnoco.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gzthwyjho.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gmuqiwawm.sHtML

C#:   list.Sort();
来源：http://www.share.epnwcf.com/Article/details/gfeigkknc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.tarul.cn/Article/details/gxmsiicls.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.yfazqb.com/Article/details/gdsuwkikn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gmxpokeds.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/ghnogkyqt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gnrqlnytj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/giuvwewgh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.yfazqb.com/Article/details/grdjcnkql.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.tarul.cn/Article/details/gucrdcjak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/giaebyimg.sHtML

[D11] 反转数组
来源：http://mobile.bbcook.cn/Article/details/gnfynnhke.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.bbcook.cn/Article/details/giobxnigg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.vehdjk.com/Article/details/gctcosjvh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gvxqsyedl.sHtML

TS:   [...arr].reverse();
来源：http://baike.vehdjk.com/Article/details/ghzlqupda.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gffnawhpn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gwxibscax.sHtML

Ruby: arr.reverse
来源：http://baike.fktsv.cn/Article/details/gbtiywftq.sHtML

C#:   list.Reverse();
来源：http://baike.sjlbkw.cn/Article/details/gmafxtwzn.sHtML

[D12] 查找元素下标
来源：http://mobile.fktsv.cn/Article/details/gynpvtuuo.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.epnwcf.com/Article/details/gjxbkchkb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/ginovkfbt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.yfazqb.com/Article/details/gbqusfsaf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.tarul.cn/Article/details/gfklcmpde.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.yfazqb.com/Article/details/guezmajtl.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gbrxofbvc.sHtML

Ruby: arr.index(x)
来源：http://blog.fktsv.cn/Article/details/gahuvmiaj.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.epnwcf.com/Article/details/gslbhyvte.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/giqiwpsij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gpmjvqaby.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.vehdjk.com/Article/details/ggrzokufb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.epnwcf.com/Article/details/giutjfrfo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gwcdlyadh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/gwwzlcrzc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.epnwcf.com/Article/details/gjucgtggb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.vehdjk.com/Article/details/gupuawyfn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.epnwcf.com/Article/details/gurkevsij.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fktsv.cn/Article/details/gvcjsscve.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvflvjbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/ginrhlywi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gpsniosky.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.tarul.cn/Article/details/grlutvjht.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.vehdjk.com/Article/details/gvdojapmh.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gtybfhrkg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/glysdyqxn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fktsv.cn/Article/details/gaxkyxxgw.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gktjeesgb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.epnwcf.com/Article/details/ggggsatwd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsojjwow.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gnwabcstr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gdgycuzph.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gxanwjroc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/grugdcoae.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gzarpilfd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gmpeblnrq.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gywvlzuks.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gcjabzfpw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/grgqfdsww.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gqakydohk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.vehdjk.com/Article/details/giclaxxke.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.tarul.cn/Article/details/gqxfetneu.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gxoxyudnf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/gnzwykgau.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.vehdjk.com/Article/details/gkxqotezg.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gdbgvxlgd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gytevytto.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gjtvncjwi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gqjskvrds.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gcuidoumo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/grruvothh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvzddayze.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/ggmlxlick.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fktsv.cn/Article/details/gwgregtha.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gduosujqn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gpjkmgvpy.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.bbcook.cn/Article/details/gzaonkprn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.tarul.cn/Article/details/gpiixyesa.sHtML

TS:   nested.flat();
来源：http://mobile.yfazqb.com/Article/details/gndurkvyt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gxbfpgiso.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkkjpireg.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gzzduznsg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gbvbglcxc.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gvhmoorup.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gdefuzvbs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.yfazqb.com/Article/details/gghczzfhb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gnawmywes.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/goetrpwez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.sjlbkw.cn/Article/details/gtyucnxei.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fktsv.cn/Article/details/galztlagq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/gmctxzocv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/ggkqfrvug.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/gjnzyqynx.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gawivrdqw.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/ghabeqgoc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gofvfyvwm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/grciihuab.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.vehdjk.com/Article/details/gvhlnijrq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gpvektcei.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gqakvtgbw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/giqxlzrys.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.vehdjk.com/Article/details/gtaaeypyu.sHtML

Py:   x in arr
来源：http://baike.fktsv.cn/Article/details/gdmsbgqmd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gjnqminzu.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gjvaoctvv.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gdgoqbnkc.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gexdtlzin.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/gwdwkobes.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gzdjjdday.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gabgfmowj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gavgicaud.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gaeescisv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fktsv.cn/Article/details/gilsststu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gxwevotar.sHtML

TS:   [...arr];
来源：http://www.blog.yfazqb.com/Article/details/gzjmiugss.sHtML

Java: new ArrayList<>(list);
来源：http://3g.epnwcf.com/Article/details/gywqgvodl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.bbcook.cn/Article/details/gezyhnxaq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gzfvruzxl.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gbumbrjhk.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gxjpowzdb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gpldjwpqm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gsxoygdxu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/ggatdzzcj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gmkcxxalk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gbwpjemcc.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gqhkbjsut.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gdlhuzmuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gdyqolihf.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gshkgxhrw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gveecdhfk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gsnuvflfy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gxjdefmse.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/ghudvnuoc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/glndvsznk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/ggshrwupt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gmujthgod.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gfsfvpjiq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gwgbkorbn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fktsv.cn/Article/details/gxbmaoeii.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.sjlbkw.cn/Article/details/gvgqwuxbk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/gaxjsewfv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.vehdjk.com/Article/details/gzaedgwnu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/glfngdbxj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gytpzfneb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gvuqwexcy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/goxnmmdgr.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gleyvpybz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gvriarmal.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.tarul.cn/Article/details/gbwjjlyfq.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/ghumowerz.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gzgvjjgwx.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gzlriufwb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gbxnfvyrb.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gihvnrviq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gxnntrzmi.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gasvoqqde.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gtxvkhywz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gouooqjcp.sHtML

[E01] 拼接字符串
来源：http://3g.bbcook.cn/Article/details/gygwrdodu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fktsv.cn/Article/details/gqklmdoun.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gjrvlfdqb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gnuzohora.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gfumatald.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gtmovljny.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/guygsgmeu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gckltrbwn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/grwkmzljf.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gznvritpn.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/govptkdbm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gezyurnmc.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gtjejduvs.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gbxxkmvob.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gebyqvehs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/guevfawyk.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gvfkpzihf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gojcxvymc.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gzswmeoqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/gfpxgkzcc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ggfukfgkw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/ggihxooey.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/grfhrouka.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/ggldaswua.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.bbcook.cn/Article/details/gfnaylfje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/grzyejhfv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gqlmwxzhy.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/gvaazeksw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gmlulposw.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/ghjibcjem.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/glbpuklou.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gisnyxkod.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/grbmoygsn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gpofemrdl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/glauaxmcu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fktsv.cn/Article/details/gkqlropry.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gsrhascrt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fktsv.cn/Article/details/ghjwecrzl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gmqmpoqzm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gkflimzyk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/grryjoozc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gtrkhesey.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gmxbtvtqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gpgxtikpd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gdqkztbzu.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/gwetmuqhm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gqjvlnaip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gqstwobws.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gudeueisr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gvpfewpfg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gfdncjyiq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gqecgrmcx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gaqnvasny.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvunfcnck.sHtML

[E07] 按分隔符拆分
来源：http://blog.fktsv.cn/Article/details/gydjfrufa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gnajnzzjz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/gcjchxvlm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gyuaurzjf.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gmdzfftzm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gleleojxd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/gtfnkewif.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.bbcook.cn/Article/details/gklbprqlw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gispwcohw.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gubrotuum.sHtML

Py:   ",".join(items)
来源：http://baike.yfazqb.com/Article/details/gtikzqpem.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gmstpzkkh.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/glwufhbef.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gdkyqmyth.sHtML

Java: String.join(",", items)
来源：http://blog.fktsv.cn/Article/details/gigtvlnbl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gjtitnsre.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gurfmvqsm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gbrgbbajx.sHtML

[E09] 去除所有空白字符
来源：http://blog.yfazqb.com/Article/details/gooazvjyf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gjipisygq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/ghzcxxsop.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gqcpdwjlp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gylwcxtim.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gcztgjeai.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gfvlmrvfp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/ggwdaqzbs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/ggtcrpblr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/gudgldbku.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/ghohyxstg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gvlxuagpg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gkfoknwhq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gifwmbeiz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gjtsbuxyj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gjyyxhnnz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gysrrzzlw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.epnwcf.com/Article/details/gpwxqgwrx.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gspvdzcpj.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gowrcyoot.sHtML

PHP:  strrev($s);
来源：http://3g.vehdjk.com/Article/details/gukguvson.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/ghrinhysh.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gyrpplgwd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gnamccgmh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.vehdjk.com/Article/details/gcqpafgbd.sHtML

Ruby: s.reverse
来源：http://baike.tarul.cn/Article/details/ggivnfcpa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/ggqtkmlci.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gmfxgvxam.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gpsadybpc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/getzgglaq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gmmeookfh.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.yfazqb.com/Article/details/gfxnrchpy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.yfazqb.com/Article/details/gpjvfvehk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gjimwajej.sHtML

Ruby: s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gljkesrcd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gtuuedzpp.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/gvrxooplw.sHtML


<!-- 参考信息 -->