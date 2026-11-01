代发 wailian999

C#:   list.Insert(0, 0);
来源：http://blog.vehdjk.com/Article/details/gykfxvrrz.sHtML

[D04] 删除元素
来源：http://www.m.share.yfazqb.com/Article/details/glfpxruyw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.epnwcf.com/Article/details/gguhyjvll.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.yfazqb.com/Article/details/grseitufy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.vehdjk.com/Article/details/gynknnzxh.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.yfazqb.com/Article/details/gwqlipobq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.sjlbkw.cn/Article/details/gsbtizucx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.bbcook.cn/Article/details/gxwjebgxy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjemiuup.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.bbcook.cn/Article/details/goreimdtu.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gpzgbknhz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.epnwcf.com/Article/details/gqyrkujwa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gekwhxaft.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.vehdjk.com/Article/details/gjahdbtit.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fktsv.cn/Article/details/goonmjrlx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.sjlbkw.cn/Article/details/gzyemvwuf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.epnwcf.com/Article/details/gsaxggekr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gxkcoddvp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.yfazqb.com/Article/details/gwzxlrfzt.sHtML

[D06] 数组长度
来源：http://baike.tarul.cn/Article/details/gfwguzjhm.sHtML

Py:   len(arr)
来源：http://read.share.tarul.cn/Article/details/goodbdslw.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gegrqxirv.sHtML

JS:   arr.length
来源：http://3g.fktsv.cn/Article/details/gxjjzsozk.sHtML

TS:   arr.length
来源：http://3g.yfazqb.com/Article/details/gwwbgdvdp.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gcgthomvn.sHtML

Go:   len(arr)
来源：http://read.share.epnwcf.com/Article/details/gsemqnvdt.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gurphqlga.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/gnyzudeyn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.vehdjk.com/Article/details/gyrmtwgfo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.yfazqb.com/Article/details/gayqagpdd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.vehdjk.com/Article/details/gkvhsuyer.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gxvxithji.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.yfazqb.com/Article/details/gypilbfyl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gxnbkomid.sHtML

Go:   arr[1:4]
来源：http://www.blog.vehdjk.com/Article/details/gmtifgbil.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/ghxfysktv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gzzvzgbng.sHtML

[D08] 合并两个数组
来源：http://3g.vehdjk.com/Article/details/gfstuchhh.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fktsv.cn/Article/details/gqconjyfz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gcxruhoxg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.vehdjk.com/Article/details/gmxxcjmvv.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gfijanxki.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gdphmqssk.sHtML

Go:   append(a, b...)
来源：http://blog.sjlbkw.cn/Article/details/gmhmgigey.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.vehdjk.com/Article/details/gsbyuxiox.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.yfazqb.com/Article/details/gmwujikam.sHtML

[D09] 排序（升序）
来源：http://wap.bbcook.cn/Article/details/gvbpnntjg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gumnxxpaf.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gngqaxadw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/gcjihfpjv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.yfazqb.com/Article/details/gjupezhvm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.bbcook.cn/Article/details/gtjxzdoud.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.tarul.cn/Article/details/ggdhhrigg.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gpqbnfwrb.sHtML

C#:   list.Sort();
来源：http://mobile.sjlbkw.cn/Article/details/gpscgjnfz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gecxluopc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fktsv.cn/Article/details/gzmylykih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gqtegjitg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.tarul.cn/Article/details/gbieftxaj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsslrfen.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.bbcook.cn/Article/details/gfarbzxsu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/ghxozjrbe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.epnwcf.com/Article/details/ghlipqghv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gyvwnhhyt.sHtML

[D11] 反转数组
来源：http://www.blog.yfazqb.com/Article/details/gxdfqztrv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fktsv.cn/Article/details/gymklvxce.sHtML

PHP:  array_reverse($arr);
来源：http://3g.vehdjk.com/Article/details/guafuxwaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.vehdjk.com/Article/details/gqrexyoky.sHtML

TS:   [...arr].reverse();
来源：http://baike.tarul.cn/Article/details/gbvlqmaxm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.yfazqb.com/Article/details/gaqivtwnw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gvenazsqu.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gaeoxsbpv.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/grthpzufq.sHtML

[D12] 查找元素下标
来源：http://www.share.tarul.cn/Article/details/gyiirsdbu.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.yfazqb.com/Article/details/gleortump.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gycfumxgo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.bbcook.cn/Article/details/gcasocecs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.tarul.cn/Article/details/gwgbqwksn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.vehdjk.com/Article/details/gynwfqfxo.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.epnwcf.com/Article/details/gyfxmmvoq.sHtML

Ruby: arr.index(x)
来源：http://3g.sjlbkw.cn/Article/details/ghwexleii.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.bbcook.cn/Article/details/gmpqbjuwj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fktsv.cn/Article/details/gxbewcnfb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.tarul.cn/Article/details/gehiskkzl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.bbcook.cn/Article/details/gvicegvkf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gincudnbm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gbdqkhglv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.epnwcf.com/Article/details/gzshmnjmj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fktsv.cn/Article/details/gntsjexsg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.yfazqb.com/Article/details/glbkbhbpb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.tarul.cn/Article/details/gpwcktwey.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.yfazqb.com/Article/details/gqghqfdva.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/grywgrniy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.yfazqb.com/Article/details/gdqlmjrrc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/guqixqwti.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/giezivddo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.epnwcf.com/Article/details/gxmtvgrgb.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gvjuolkmz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.bbcook.cn/Article/details/gswnzcplx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.epnwcf.com/Article/details/gaasnnbeh.sHtML

[D15] 去重
来源：http://blog.epnwcf.com/Article/details/gjjgnvlzq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/grucbumht.sHtML

PHP:  array_unique($arr);
来源：http://3g.tarul.cn/Article/details/gmbsytqmc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gqljufhst.sHtML

TS:   [...new Set(arr)]
来源：http://blog.epnwcf.com/Article/details/gattifdkh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/guucetuoo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.yfazqb.com/Article/details/glffvjoql.sHtML

Ruby: arr.uniq
来源：http://mobile.vehdjk.com/Article/details/gilgmawtq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.vehdjk.com/Article/details/gogfeizce.sHtML

[D16] 求和与平均值
来源：http://baike.fktsv.cn/Article/details/gtqouviuu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.vehdjk.com/Article/details/gjrkangrh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.epnwcf.com/Article/details/grrqjhrpp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.vehdjk.com/Article/details/gzgxcdefg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/ghijkzrdn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.tarul.cn/Article/details/ggogcpeom.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gepqxxora.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gamsfgrnp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.tarul.cn/Article/details/gswmzotnl.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gfkqwdmqo.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fktsv.cn/Article/details/gcabojkfu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gwjkjyuhq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/gdoaqiqkw.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/geessgwyp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/gokrjzweh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/guvwruket.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.bbcook.cn/Article/details/gkvpqeuvv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gsqokwcze.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gfjjekwek.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.epnwcf.com/Article/details/gcfhyqxrr.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.vehdjk.com/Article/details/grhxfesfc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gipcaywub.sHtML

TS:   nested.flat();
来源：http://3g.yfazqb.com/Article/details/gkqdwcadn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fktsv.cn/Article/details/gwdfydnri.sHtML

Go:   // 手写双层循环
来源：http://wap.tarul.cn/Article/details/gbpcqwjbc.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/gmrlqjlaf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.bbcook.cn/Article/details/gokkkpjrk.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gzxbunzyv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/grigmdxms.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.tarul.cn/Article/details/gfadezaol.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/ghcsxntny.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gemclygcm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.yfazqb.com/Article/details/gfociodvw.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.sjlbkw.cn/Article/details/gwsensxmn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gnulhxxjg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.sjlbkw.cn/Article/details/gboiaasgs.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fktsv.cn/Article/details/gegxefeol.sHtML

Py:   Counter(arr)
来源：http://wap.yfazqb.com/Article/details/gbghvjzqx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/groquzrwo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gciylidgi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gzdlxavne.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.bbcook.cn/Article/details/gndawjctc.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gratxhqqm.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/giypvgtxo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/glenphdwi.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gibnfliaq.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/gwvtiuill.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/glauprxvh.sHtML

JS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gcrnylcfc.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gsuugyefl.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gmlkoaxgk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gztsxacfp.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/gytnofprr.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gehudepoc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gzqvlfual.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.epnwcf.com/Article/details/gpcchncdu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gqfwianvs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.epnwcf.com/Article/details/glzeokwzc.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gvrlcines.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gvhklufkz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gunfygqzx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gcmageiwo.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/guytsaelv.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gkjwntqme.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gvvscaibj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gycbuoylz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gnegrgpmo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gsxsslihb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.yfazqb.com/Article/details/godrpqhtz.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gwzufygpi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gtlvwnlks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gkjcpivpp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.yfazqb.com/Article/details/gersyksdy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gtijhyorc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gozjnavey.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gnmozkihz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gzfylxway.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gqwcubynp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gmytogdea.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gjufrtlaf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.epnwcf.com/Article/details/gnmxwzohk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/giwsebczp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gqnjlmugn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gwtmbeqpi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gujowmiua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/godkdyvdl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gabmyaftk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/gnxifzocp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/gbgjpsnig.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gjrhcjsra.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gcthubnsf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gbtajhecz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gckcezmoq.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gksusekyu.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/guahbrior.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gogpymhbt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gpophzdcq.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gblteluiy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gjjdvawdq.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghxstabqq.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gcmzeinjw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggszbrxck.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gentfilup.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gpeotyheb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gxbycmyfk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gdmoijauw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gjxyurpec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gzxgrbmmk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gfokrfttn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/grlcwphur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/godrtzqrb.sHtML

[E02] 重复字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxgryfyel.sHtML

Py:   "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gbdkqtwhx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gdvbntnql.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/ghtaznlgl.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gjusxtpuh.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gldzinzdm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/guvtkturs.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gpzpnbtcb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/gzwmhnqdq.sHtML

[E03] 截取子串
来源：http://www.share.vehdjk.com/Article/details/gkgdsbxcu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/ghnlhbjwz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/ggaojgdbd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gykiwnpbq.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/glpnuclrn.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gwjqonsgb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/gfyiwxifd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/glrtxxlvy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gwqdbzigu.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/gwjazfxec.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gyxjigqks.sHtML

PHP:  strpos($s, "x");
来源：http://baike.tarul.cn/Article/details/gycuaiicz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fktsv.cn/Article/details/gmkxxkvkg.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gwcrnumcp.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/goseboqbb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.bbcook.cn/Article/details/glzlhazdt.sHtML

Ruby: s.index("x")
来源：http://www.share.bbcook.cn/Article/details/ggabytlap.sHtML

C#:   s.IndexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gostzbgdo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.tarul.cn/Article/details/gyuihbkgu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gquxhnhed.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gsgfmrjdl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcwpalhk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gymqpkjqw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gtsoncwfg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gxwvnaxoh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gjgmzdlbt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gybjbpsoh.sHtML

[E06] 替换子串
来源：http://www.m.share.epnwcf.com/Article/details/gjksotenu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gijmxhtxq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.yfazqb.com/Article/details/glrkoqkbl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/grakhmohu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gurmjoilw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gumdocujk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gzlznzues.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/gewhdifoy.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gigtssgrf.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gsuvqspxp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.vehdjk.com/Article/details/gdokxclyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/geildxkdx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gtszwgfck.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/girxvxxmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gcrfygbeu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/grnnxzpby.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gfisgjmch.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gwlmitami.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/guqcesecx.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gfmilsuuv.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/ggazlasrb.sHtML

JS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gqaolgbyn.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/grgiugqzx.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gamukkcer.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gyqxdhkhr.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gmmgqxthm.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gbrmspfuj.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/giqjvquxx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gxadnnxou.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gnqksbtkm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gejdjchai.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gttdcillr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gywmnukqu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.yfazqb.com/Article/details/gkohzvtfd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gsypajipv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gbgjrtfcf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/ghggixqzx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/grkvzswfl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gihvkhehj.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gtqtbfxdh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gznbfbmex.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gisnmrffk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gzeoulpzs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/ghmuozaao.sHtML


<!-- 参考信息 -->