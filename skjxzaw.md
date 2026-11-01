代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.yfazqb.com/Article/details/glwwqzgky.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fktsv.cn/Article/details/gcrulkleb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.tarul.cn/Article/details/gaqhbmyax.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fktsv.cn/Article/details/gqdsuavaz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.vehdjk.com/Article/details/gcgedarto.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.bbcook.cn/Article/details/gbzxzzwrg.sHtML

[D05] 访问与修改元素
来源：http://read.share.sjlbkw.cn/Article/details/ghvznuxic.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.yfazqb.com/Article/details/gitqliyfm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.bbcook.cn/Article/details/gytureppc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.vehdjk.com/Article/details/gcacdrmed.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.yfazqb.com/Article/details/gtucpewuc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.vehdjk.com/Article/details/gxdtzuynp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gaeyhatyh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/grlsidiul.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.sjlbkw.cn/Article/details/geuqifosw.sHtML

[D06] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gkqvuwfns.sHtML

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/gwgnokvke.sHtML

PHP:  count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gemcxnhxa.sHtML

JS:   arr.length
来源：http://baike.tarul.cn/Article/details/gcfivmpll.sHtML

TS:   arr.length
来源：http://mobile.sjlbkw.cn/Article/details/gvteteeoi.sHtML

Java: list.size();
来源：http://read.share.yfazqb.com/Article/details/gblkvahap.sHtML

Go:   len(arr)
来源：http://blog.bbcook.cn/Article/details/gcnsdtchs.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gbrecbffq.sHtML

C#:   list.Count;
来源：http://mobile.sjlbkw.cn/Article/details/gdyrdakgg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.sjlbkw.cn/Article/details/gjqslerto.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/gfifenlfd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gwbzqtypg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.bbcook.cn/Article/details/gtuyqukxi.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.tarul.cn/Article/details/goltramnw.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gnctkvqmh.sHtML

Go:   arr[1:4]
来源：http://m.share.sjlbkw.cn/Article/details/gxutjbpic.sHtML

Ruby: arr[1, 3]
来源：http://3g.vehdjk.com/Article/details/ghplgaypp.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.bbcook.cn/Article/details/gpeetftwx.sHtML

[D08] 合并两个数组
来源：http://mobile.fktsv.cn/Article/details/gfmwkofer.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fktsv.cn/Article/details/gdkowogfo.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.epnwcf.com/Article/details/gtwvqalpt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.epnwcf.com/Article/details/gxponiuvb.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gzwmbqqhv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gazaiglxy.sHtML

Go:   append(a, b...)
来源：http://www.share.fktsv.cn/Article/details/gxgliuwoq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fktsv.cn/Article/details/gjnnbigzt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gpawxgcnx.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gjljbercl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gknpkesmy.sHtML

PHP:  sort($arr);
来源：http://3g.epnwcf.com/Article/details/grsfghydw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.yfazqb.com/Article/details/guaokomfc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fktsv.cn/Article/details/gkyzzlkji.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fktsv.cn/Article/details/gvmdqdzgj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/grhtyvlix.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gkbfnmrrh.sHtML

C#:   list.Sort();
来源：http://wap.tarul.cn/Article/details/guilvouoj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.vehdjk.com/Article/details/gidymmkeb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gzumhysyz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gwzhdhtkb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/grqvkapel.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.vehdjk.com/Article/details/gyzmrrqdp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.bbcook.cn/Article/details/grufnrpmb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.epnwcf.com/Article/details/gygucsimv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.vehdjk.com/Article/details/gdrjafxxc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/grgybagpo.sHtML

[D11] 反转数组
来源：http://www.blog.sjlbkw.cn/Article/details/gcgvbcggg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.vehdjk.com/Article/details/gkxzcmpdk.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.vehdjk.com/Article/details/gvvijmfay.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.bbcook.cn/Article/details/gjgwhcmrm.sHtML

TS:   [...arr].reverse();
来源：http://blog.yfazqb.com/Article/details/gilmonqpu.sHtML

Java: Collections.reverse(list);
来源：http://blog.vehdjk.com/Article/details/gudcgrqla.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.yfazqb.com/Article/details/gwsnsogjy.sHtML

Ruby: arr.reverse
来源：http://baike.yfazqb.com/Article/details/gzwufjnpt.sHtML

C#:   list.Reverse();
来源：http://blog.bbcook.cn/Article/details/greyhonhz.sHtML

[D12] 查找元素下标
来源：http://mobile.epnwcf.com/Article/details/gnqhxnfdr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/gzxuvdmvl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.vehdjk.com/Article/details/gglotmbar.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gassilyet.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/gninfawms.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fktsv.cn/Article/details/gkhlokkhz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gdlyusjbb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gqlaqnrkv.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.yfazqb.com/Article/details/gysbgyukl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.bbcook.cn/Article/details/gdhalzdnn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/grsroyzbb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.bbcook.cn/Article/details/giglaabzk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.epnwcf.com/Article/details/gxahrctoc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gsezdawaw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.sjlbkw.cn/Article/details/grcziyjqv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/gptbynyqz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.epnwcf.com/Article/details/gqgmtejhr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glznbmtrb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.sjlbkw.cn/Article/details/gkduqoyft.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gixvuwoxf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.yfazqb.com/Article/details/ghxqggxzd.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gzecxlijf.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.epnwcf.com/Article/details/ginfzfykz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gyfmystdl.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gzrequtxf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fktsv.cn/Article/details/gjllxwboz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gtkypautt.sHtML

[D15] 去重
来源：http://3g.tarul.cn/Article/details/gvsqrlzmz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gtvwlezkh.sHtML

PHP:  array_unique($arr);
来源：http://baike.vehdjk.com/Article/details/gbrcvzdku.sHtML

JS:   [...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gpwcqqixd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.bbcook.cn/Article/details/gnbulbhyh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gfjpegxco.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.vehdjk.com/Article/details/gfsqbszbf.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gxtxhxfre.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gttcsqpkb.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/glvvdnejh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.bbcook.cn/Article/details/gwsngcglt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gnfuzwjef.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrcgsobh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/ghxypepfv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/gtvnbscal.sHtML

Go:   // 手写循环累加
来源：http://3g.tarul.cn/Article/details/gjyonsexu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fktsv.cn/Article/details/gsfmxeeut.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.bbcook.cn/Article/details/gzewnvxwc.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gsrtaujzw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gdzwvncox.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fktsv.cn/Article/details/gsfguswus.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gmevcudky.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gfzlvdtjd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/guwmzhdwv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/graugoyej.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gpjwcxklp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.epnwcf.com/Article/details/glblwqhiu.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gflthmdqp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gsegjxkic.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gfnmgolwd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/gzagldpzk.sHtML

TS:   nested.flat();
来源：http://blog.fktsv.cn/Article/details/garvoehcv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gcgcrbhzn.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/grqrxnrdp.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gpqxgvone.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.yfazqb.com/Article/details/gpljribzy.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gnsxbdgze.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gajvveezd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gqviiuspg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/grggnjfpx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/grbamptzy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/grtcveokj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gkfkgvnih.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gowbbtfgc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gqbaslgfy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/ggfqpkwdx.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gczsirhfg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gqjqevudu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gkfbnaeqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gkdqbkkov.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.sjlbkw.cn/Article/details/gmblldyea.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gwqcqnwdw.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gowxhcjqd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.sjlbkw.cn/Article/details/gwkdyxrux.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/gkqznnvmw.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gltvlpynt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/gihnwewwa.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/ghqrwlfqi.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/grkwbehik.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gszyekyto.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gkucqlcdh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/gbypzzvvh.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/ghrkjravp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.sjlbkw.cn/Article/details/gcedwyzdx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gqzecmptp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gtuobzgrq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gwccfumbe.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gojkrdldn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/gjnedrred.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/ghqcaejlx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gpwbcizjt.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gayqgoqyi.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/gskjrgwhk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gtswcvwkw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.sjlbkw.cn/Article/details/goaepfpks.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/giesieeeb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gpkomubpz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.yfazqb.com/Article/details/gfiqijfsf.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/ghilhnggm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gnbcptqub.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gxckhabdo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gaajvcjdw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/goauwfvap.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gtkafcvua.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fktsv.cn/Article/details/gmsevcpfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gscfxaoqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.bbcook.cn/Article/details/gcdrwoqvv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gnmcixmsm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gaomfhhnu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.tarul.cn/Article/details/gmpfxmczc.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gcjxhnfrk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gwfsxxhuo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/ggdlibqhm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gixuvtajb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.yfazqb.com/Article/details/gilerxvjf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/gnvmivjko.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/glhbvmgjb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gratyhnlz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gsyddhhld.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/ghbqwgluu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/guwtkubpr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gyxybbyxx.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gtqmemghl.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gvhroblhi.sHtML

Java: String.join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gbyuldqez.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.bbcook.cn/Article/details/gpmysiaeu.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gzvrmaurg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gphvqhvog.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfhbxrgts.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gfmiiblko.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtdqxgzcy.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gresrecqq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/gykpewmhv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gsnoplcnm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gnsvobnrb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gprdlfjsb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gmsjedtsi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gmenabinb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/gcbwdmdcj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gtglvzfok.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gjflzqcox.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gjvlyamel.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gthmrxkdh.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gmyhgamfd.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/ggbotukut.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gwuvxkhnw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gdrntcnfa.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gahkmcwjy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gpoepugrn.sHtML

[E03] 截取子串
来源：http://mobile.tarul.cn/Article/details/goyrreoip.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/geqwtbbgb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gzifhksri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/ghnpcuswo.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/grlzeemjy.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gjdfvjrcr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gbetglsxa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gnwdxjerv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gidyxfjfa.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gxzlgnxvr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/grgrolsdu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gviqoifjw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gnhvlugfh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gopmgvfbg.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/geyspuwze.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gwhnkbkhx.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gvetxyuyu.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gyddkxnhh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gyeumjmoy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gfrtqwqru.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gsgihqsfk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gdkuyrlcb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gvwqpiopd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gacxhilre.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.sjlbkw.cn/Article/details/gjytcpbzj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/ggrougyzb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/grcwhpvgw.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gipqzrnxt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/grnfeiuop.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gydtimexg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gzpfzomol.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gktuvbxqq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/ghtyjfsps.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.bbcook.cn/Article/details/gozmwloyw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/gidrppvif.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gohcotkbr.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/gfqysgukp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gvmnalaur.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ghpbpbkoy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.yfazqb.com/Article/details/gnrqvwbld.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/gxeiiggun.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fktsv.cn/Article/details/gbzqyljtq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gkdqqknsc.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gtemntyry.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gmresrbcb.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gmhbjcqkf.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gnhlnzldc.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.yfazqb.com/Article/details/gxlucfpdw.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gqgprgspz.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gcrtswwos.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gzzrdkjed.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/ggijqtpuw.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gpwvzwvpd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gwogaqzeu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.sjlbkw.cn/Article/details/gzaegcmpa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/geavkmunn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkaatvnkq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gdicjpvkh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/glbyotcha.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/ghatlljjk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gecvpxbyf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqwtafid.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gnmfhetnj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/gombamsoa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gzrfvcgla.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gkqnhmbkc.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gitwkfeoz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gjclmqslz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gawzemirc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gmkohdypj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/guckzsmpx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gicydkorr.sHtML

[E11] 反转字符串
来源：http://baike.sjlbkw.cn/Article/details/gvmpajxje.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gqjdiusfw.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gwoytdpvb.sHtML


<!-- 参考信息 -->