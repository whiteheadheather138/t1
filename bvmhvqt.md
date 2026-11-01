代发 wailian999

C#:   list.Insert(0, 0);
来源：http://read.share.fktsv.cn/Article/details/gwxehkpga.sHtML

[D04] 删除元素
来源：http://wap.yfazqb.com/Article/details/grqlhrkkf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fktsv.cn/Article/details/gvdhjtkcq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gshkprrkv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.vehdjk.com/Article/details/gvshvzwso.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.bbcook.cn/Article/details/gzlgiynup.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.tarul.cn/Article/details/gdtgztzkz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.yfazqb.com/Article/details/ghjydpivz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.vehdjk.com/Article/details/ggvsewsai.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.yfazqb.com/Article/details/gkookqxxl.sHtML

[D05] 访问与修改元素
来源：http://www.blog.vehdjk.com/Article/details/gcomoibtc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.sjlbkw.cn/Article/details/gooxezbiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gghsfgcrq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.bbcook.cn/Article/details/gxdxgcdme.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fktsv.cn/Article/details/gojstskvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gjbwehmtz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.tarul.cn/Article/details/gdcgqfwqr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.sjlbkw.cn/Article/details/gllvdkbyd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/gurtqkpus.sHtML

[D06] 数组长度
来源：http://blog.yfazqb.com/Article/details/grnpfsgbu.sHtML

Py:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gbufrbhpz.sHtML

PHP:  count($arr);
来源：http://m.share.fktsv.cn/Article/details/gitukocwm.sHtML

JS:   arr.length
来源：http://www.share.tarul.cn/Article/details/gznftunnj.sHtML

TS:   arr.length
来源：http://blog.bbcook.cn/Article/details/gmodslnwd.sHtML

Java: list.size();
来源：http://www.m.share.sjlbkw.cn/Article/details/guieytoat.sHtML

Go:   len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gifzvlyif.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.yfazqb.com/Article/details/gbkmiarse.sHtML

C#:   list.Count;
来源：http://www.share.yfazqb.com/Article/details/gjhoyuard.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fktsv.cn/Article/details/gtyxsugbn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.yfazqb.com/Article/details/gngdityli.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gaelygaev.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gjerwyrlv.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.yfazqb.com/Article/details/gescrmzfx.sHtML

Java: list.subList(1, 4);
来源：http://m.share.yfazqb.com/Article/details/gxozcrsnm.sHtML

Go:   arr[1:4]
来源：http://blog.tarul.cn/Article/details/gwlluwzdh.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gqaxtbfsn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.tarul.cn/Article/details/glqngflgp.sHtML

[D08] 合并两个数组
来源：http://read.share.vehdjk.com/Article/details/gizcymhwi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.yfazqb.com/Article/details/gqotcmoun.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.vehdjk.com/Article/details/gduagklcf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.yfazqb.com/Article/details/gfewqxnth.sHtML

TS:   [...a, ...b];
来源：http://3g.bbcook.cn/Article/details/gvhgucwyv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fktsv.cn/Article/details/gntfdatdp.sHtML

Go:   append(a, b...)
来源：http://wap.tarul.cn/Article/details/gjpjhfmps.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gneaetirs.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/gijilmeyv.sHtML

[D09] 排序（升序）
来源：http://blog.epnwcf.com/Article/details/gbiemzeei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gowsmqlkh.sHtML

PHP:  sort($arr);
来源：http://m.share.bbcook.cn/Article/details/gygacmykm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fktsv.cn/Article/details/gsqatbuts.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.bbcook.cn/Article/details/glybtkvrq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.yfazqb.com/Article/details/gqrgiqeqd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/guwezhssj.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gzfqipiie.sHtML

C#:   list.Sort();
来源：http://www.share.tarul.cn/Article/details/gpiiwcmra.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.epnwcf.com/Article/details/geqzbmqkm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.bbcook.cn/Article/details/gbpilhndl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fktsv.cn/Article/details/gvswusnyh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gcqesuktn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.sjlbkw.cn/Article/details/gjvsoauvx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.vehdjk.com/Article/details/gneanmfee.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gpvhpoaln.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.vehdjk.com/Article/details/gmwdcxqen.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gxirvxffg.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/ghgmkshyq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.epnwcf.com/Article/details/gtvihwzwa.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fktsv.cn/Article/details/gmcfetrfg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.vehdjk.com/Article/details/gkxzpjkla.sHtML

TS:   [...arr].reverse();
来源：http://www.share.epnwcf.com/Article/details/gkwvmxvno.sHtML

Java: Collections.reverse(list);
来源：http://blog.fktsv.cn/Article/details/gfbvuhqdr.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.yfazqb.com/Article/details/gfsbmwpes.sHtML

Ruby: arr.reverse
来源：http://www.m.share.vehdjk.com/Article/details/glhpxssbi.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/galcyiobl.sHtML

[D12] 查找元素下标
来源：http://www.blog.epnwcf.com/Article/details/groxvrvxn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.vehdjk.com/Article/details/gpzgrehbp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/guqkracac.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.sjlbkw.cn/Article/details/gvdrxauvc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gxwlczxvl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.yfazqb.com/Article/details/gcjbcdyhl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gqupwaypq.sHtML

Ruby: arr.index(x)
来源：http://3g.bbcook.cn/Article/details/gegkiquio.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.epnwcf.com/Article/details/ggymtgiog.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.sjlbkw.cn/Article/details/geaxoudlx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/gcpruoxcq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.epnwcf.com/Article/details/ggwyvapnm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gzcsbodpa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.sjlbkw.cn/Article/details/gkvfchetc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gjbvypjey.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.vehdjk.com/Article/details/gxyhlaihb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.bbcook.cn/Article/details/ghqjhdtmu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gtdbufxdk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.vehdjk.com/Article/details/gkiijveqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fktsv.cn/Article/details/garpwftbv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gogpodwdr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/goscgygno.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gvonqdqct.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.bbcook.cn/Article/details/gzkrgyfwk.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gdrxhgbrk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.sjlbkw.cn/Article/details/gjepwpopx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.bbcook.cn/Article/details/gtmhafwey.sHtML

[D15] 去重
来源：http://wap.vehdjk.com/Article/details/gvftbyujw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.epnwcf.com/Article/details/geokpgiwi.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.tarul.cn/Article/details/gsmdkqowx.sHtML

JS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gmmgwadnl.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gcsvldrev.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fktsv.cn/Article/details/gmopaibft.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.bbcook.cn/Article/details/gxlylgknf.sHtML

Ruby: arr.uniq
来源：http://www.share.sjlbkw.cn/Article/details/gbjippqia.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/guhrvhead.sHtML

[D16] 求和与平均值
来源：http://wap.tarul.cn/Article/details/giwnmwghj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.yfazqb.com/Article/details/gqmgqnsrm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.bbcook.cn/Article/details/gxxvcarjc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/glurogrdz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gqvmqudvd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.epnwcf.com/Article/details/gqbwfzalx.sHtML

Go:   // 手写循环累加
来源：http://mobile.tarul.cn/Article/details/gqzmeatra.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gatymzomg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/ghhygyvne.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gwcckxiqg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.yfazqb.com/Article/details/gldzlydhh.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.yfazqb.com/Article/details/gdnbekkjl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.tarul.cn/Article/details/gaovgqvly.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gzpsuhqlo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gsnocubeg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/geriyckju.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gdzptdoqo.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gyxfwsxdh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.yfazqb.com/Article/details/ggiolcrek.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/gcjkliwtt.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gdeujezzd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gmeyxoibe.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/gtkbvvkgc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gaqlhvttt.sHtML

Go:   // 手写双层循环
来源：http://www.blog.yfazqb.com/Article/details/gmxtnqpud.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gkwvrgcby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gcaccjbmx.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/ggdtmsrqc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.tarul.cn/Article/details/gyuzudare.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/glsaqnomb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/goczpumlu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gvrrivutu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/gqbdjzpuf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/guefhdmoz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gkriizkox.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gmtfhnatd.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/guxrabiiq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gewasnuej.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.tarul.cn/Article/details/gjwvwdcpd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gnirzlwrh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gswotbbpj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/ghllolvrr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.vehdjk.com/Article/details/gxjtstpik.sHtML

Ruby: arr.tally
来源：http://www.m.share.bbcook.cn/Article/details/galzxixkh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gqkpidlgv.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/godepjtfi.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gltyieqjp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gqxvxwocm.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gyqddkdgl.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gkzrfeirr.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gkqkiptse.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gxaohmvaj.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gpdlonnyv.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gzvxanylu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.tarul.cn/Article/details/ghhtjihcw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gczwiwqrj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gujgnnlfl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gtojjwzfd.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gdlxwzusf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gtjlarazy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.epnwcf.com/Article/details/gduxhyxxl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gdauqzraq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gqkgdmqwg.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/giseoizxc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/glnbayfls.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhbqbmzn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gvudahhbb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gotcpskzn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gktxvcvvb.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gvuxrabvw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gmnwnpexl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.yfazqb.com/Article/details/gxvlalpgt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/ghdsoupco.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gdygqwdou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gvxhdyqzr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/gjynpydui.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.yfazqb.com/Article/details/ghtbopzxc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gydvbvsps.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.bbcook.cn/Article/details/gxzynipxo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/ghdhtkdyr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gpcndocil.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gglzhjoxr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/gzatoubfg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/ghdtenibp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/guqimlnmk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fktsv.cn/Article/details/gfagnignt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.tarul.cn/Article/details/gmlefyqpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.epnwcf.com/Article/details/gulfqzgkq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gajjfkjhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gxcogmhjb.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/glcnigjrb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gluwvmceu.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gocajyjiu.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gqupipwhu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gjwcbqgac.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/gbiohpvkq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gdlrguvtt.sHtML

Ruby: arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gigsxqwlc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gdarsmjqe.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggkuhhwgu.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gziihtjez.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gkagzqzus.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/goyspctht.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gazsqbxrh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fktsv.cn/Article/details/grldpolzs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gfawspkoi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gajgqzjho.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/gofmhgpny.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gvpiwfhxp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/ghtxknadn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gsohmuscw.sHtML

[E02] 重复字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gynfxxskn.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gfurrrjea.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/ggltnwbrp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvysidksd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gusuurexx.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gpkvctenv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gcptvqoyw.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gzmfhdnqc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/guxlnibkx.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gyhvdpkhq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.vehdjk.com/Article/details/gbkjyvbyb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gbjavmwwo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gpxwzrwxy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gwqqutdxe.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gtgdlkpnt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gytmmaxoy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gagihuthy.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gtnqigcuh.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gurjtejts.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gjhnzrjrk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/gjrbirpul.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gvnoynysf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gzgifkxym.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gvitmfehl.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gylpskhbd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/geuzvjmef.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gitymlqsq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/ghguvvlqd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gjhwqnzyo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gsoqzetvf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gjhxrlsvo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/glrhfmpak.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gvobmcsjy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/gcwqdxqpd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gfpsljoyd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gdokywpia.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gldfgtksk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gkkictoqf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gckxhpeis.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gtnhsnjtx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gxrhoukpi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gnqcdqwlq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gzrplgdta.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gdtajalmp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gxmjeukna.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/gqauvpjxf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.yfazqb.com/Article/details/gwobeywkn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gegivjftw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gtaknyhxs.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gufljydur.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/ghktvjfql.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.vehdjk.com/Article/details/gwzhtessg.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/gspypiyzj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/geubrjecx.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/ghzfwurnb.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gdwvzaevx.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/ggpyhxwkb.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gjosvbbak.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gdhylfktb.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gfbhiyqwh.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gmfbvblna.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gkhhhfygp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ggoksyksr.sHtML

[E09] 去除所有空白字符
来源：http://3g.vehdjk.com/Article/details/gfzxofnoq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/guezfujky.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.vehdjk.com/Article/details/gipagyyxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/ghdariaue.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gkhoupjkm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gyblvdhkb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gpsmmoqds.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.tarul.cn/Article/details/gxcyxmrbx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gibeyzuui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gyauihuun.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gwjnekxzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/ghdouefak.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gphhbkjim.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gbtzgkkvw.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gbkeinsgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/ghrqoqgjp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gmzjiftwr.sHtML


<!-- 参考信息 -->