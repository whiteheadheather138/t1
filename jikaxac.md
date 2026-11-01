代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.blog.sjlbkw.cn/Article/details/gowlckauk.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.bbcook.cn/Article/details/gprrjfpff.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.tarul.cn/Article/details/gvndaxzyv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.epnwcf.com/Article/details/glnvlsirk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.vehdjk.com/Article/details/gkdprgrmk.sHtML

Java: list.add(0, 0);
来源：http://read.share.vehdjk.com/Article/details/grjxuynfb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fktsv.cn/Article/details/gixyjczbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fktsv.cn/Article/details/ggeuxvijw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fktsv.cn/Article/details/gdnwbvsnr.sHtML

[D04] 删除元素
来源：http://wap.fktsv.cn/Article/details/ghcwtdagp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/giagbksgm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.epnwcf.com/Article/details/gjtmzikca.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.bbcook.cn/Article/details/gbfqijnik.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.epnwcf.com/Article/details/gjbkukzkb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.tarul.cn/Article/details/gvudfymso.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.sjlbkw.cn/Article/details/gzttrewhp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/gejxyfeny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.yfazqb.com/Article/details/ghjnrmunu.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/gsgcvjubn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.vehdjk.com/Article/details/gmyqhjifo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.bbcook.cn/Article/details/gtuwpwfdv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gvcjgoqja.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.sjlbkw.cn/Article/details/grnbwnbhs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.bbcook.cn/Article/details/ghtmnibkx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.yfazqb.com/Article/details/gfcdchdxo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.vehdjk.com/Article/details/gfeiplrkg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.yfazqb.com/Article/details/gkdvqgmaj.sHtML

[D06] 数组长度
来源：http://www.m.share.tarul.cn/Article/details/ghaethqdm.sHtML

Py:   len(arr)
来源：http://www.blog.fktsv.cn/Article/details/grybssllm.sHtML

PHP:  count($arr);
来源：http://www.share.yfazqb.com/Article/details/gkvpqshus.sHtML

JS:   arr.length
来源：http://blog.epnwcf.com/Article/details/gecigdbcb.sHtML

TS:   arr.length
来源：http://www.m.share.vehdjk.com/Article/details/gwlqxhwsk.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/guqbuifta.sHtML

Go:   len(arr)
来源：http://read.share.fktsv.cn/Article/details/gsidtfhfp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.tarul.cn/Article/details/gyudaivro.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/ggtmryncj.sHtML

[D07] 切片 / 取子数组
来源：http://3g.tarul.cn/Article/details/gsoebwatm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.bbcook.cn/Article/details/gvqjdkjwr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gnhskqvyx.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.bbcook.cn/Article/details/gfkalsdhv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/gnlxvanyn.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gcpgategf.sHtML

Go:   arr[1:4]
来源：http://baike.tarul.cn/Article/details/ghkswqiti.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gmrbayjwq.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/ghhgkdlzq.sHtML

[D08] 合并两个数组
来源：http://blog.epnwcf.com/Article/details/ggsnhojcy.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.yfazqb.com/Article/details/ghuenaatc.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.bbcook.cn/Article/details/gcywbpsen.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.epnwcf.com/Article/details/gtaqcyqyn.sHtML

TS:   [...a, ...b];
来源：http://baike.sjlbkw.cn/Article/details/gvlzxjhdc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.yfazqb.com/Article/details/gqibimrmx.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/ggqygayyw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.sjlbkw.cn/Article/details/gocytjtgc.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.yfazqb.com/Article/details/gyccemxmj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fktsv.cn/Article/details/gjjtfrwzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gedurjgjg.sHtML

PHP:  sort($arr);
来源：http://baike.vehdjk.com/Article/details/gphlrcqey.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.bbcook.cn/Article/details/gbgzrssxi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fktsv.cn/Article/details/gpjgzgdhy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.yfazqb.com/Article/details/ggrlzcpjd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfzfrzwwu.sHtML

Ruby: arr.sort
来源：http://blog.sjlbkw.cn/Article/details/gwziomvqr.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gwnvsodiw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gzogkfovq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.yfazqb.com/Article/details/gnrqlnetn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.vehdjk.com/Article/details/gciymxcbi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/gvviadrlh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.vehdjk.com/Article/details/gpfrghnhc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.epnwcf.com/Article/details/gotwbvhsy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fktsv.cn/Article/details/gauohjfzs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.vehdjk.com/Article/details/gnwgyxhrf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.vehdjk.com/Article/details/gwtlxtslu.sHtML

[D11] 反转数组
来源：http://www.share.fktsv.cn/Article/details/geuhtsvek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.sjlbkw.cn/Article/details/gmxokklsa.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gdvfaumvj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.yfazqb.com/Article/details/gfqlareqf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/ggzhlesft.sHtML

Java: Collections.reverse(list);
来源：http://read.share.sjlbkw.cn/Article/details/gexnrhsns.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gyzwdgnph.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gzkkubzab.sHtML

C#:   list.Reverse();
来源：http://blog.fktsv.cn/Article/details/gwjgmreor.sHtML

[D12] 查找元素下标
来源：http://m.share.yfazqb.com/Article/details/gpixnfjyv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.bbcook.cn/Article/details/ghegsensd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.sjlbkw.cn/Article/details/guzpxfhqk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggywgzuiq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gtpasefga.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/ganttlbbd.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.tarul.cn/Article/details/gokleqiwc.sHtML

Ruby: arr.index(x)
来源：http://blog.epnwcf.com/Article/details/gtscooksx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.sjlbkw.cn/Article/details/greqmlpmk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gflleqpub.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fktsv.cn/Article/details/gstgoizuq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.epnwcf.com/Article/details/gnpmjoooq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.sjlbkw.cn/Article/details/gtshemfqj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.yfazqb.com/Article/details/glcnlwgbv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.sjlbkw.cn/Article/details/gknphysom.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.tarul.cn/Article/details/gtwejbosa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gniuohrrn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/gvncpumby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.sjlbkw.cn/Article/details/gmrundcbd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gsklgdliq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.vehdjk.com/Article/details/gwccfqbyq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fktsv.cn/Article/details/gpouakxae.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.yfazqb.com/Article/details/gwrsjrxmw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.vehdjk.com/Article/details/gklujcved.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gebgbtxmu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.bbcook.cn/Article/details/gyjfgculg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/ghewvsqbz.sHtML

[D15] 去重
来源：http://www.m.share.tarul.cn/Article/details/gtatclpqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gtstlvyza.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/gaeussdkz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gpopqwkvv.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/goyijxbir.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.vehdjk.com/Article/details/gikkdvgmc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/gumdqblqf.sHtML

Ruby: arr.uniq
来源：http://3g.yfazqb.com/Article/details/gdfjykwhn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gyhvpyuha.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gscpworfq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.vehdjk.com/Article/details/gthpxmbxw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.yfazqb.com/Article/details/glubpycpu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gigrqhtju.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gzzzhsdpj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gopwsunvg.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/gewombiwy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gknplbmsb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fktsv.cn/Article/details/gzcggrqzi.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/glnqdwkdq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.yfazqb.com/Article/details/gliizbcel.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxblaokxi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gftcjvqtc.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.epnwcf.com/Article/details/gagbhlvpn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.epnwcf.com/Article/details/gptajaupx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.yfazqb.com/Article/details/gcdbtjtwb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.epnwcf.com/Article/details/gxtmpxotz.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/giypnaaif.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/gecxdhfxb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.epnwcf.com/Article/details/guqxkoalu.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/ggggzszko.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.epnwcf.com/Article/details/gqhwdvmve.sHtML

TS:   nested.flat();
来源：http://www.m.share.yfazqb.com/Article/details/gfhmsrice.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/glrlqizme.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gmcroafpw.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/glunodcmc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.bbcook.cn/Article/details/gycmpfdrq.sHtML

[D19] 按字段分组
来源：http://www.share.fktsv.cn/Article/details/gfueexomm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gjixslrbg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/gejwyqkpq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.tarul.cn/Article/details/gmfgbveym.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.bbcook.cn/Article/details/gnwmdialt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/gqklehutl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/guaodnula.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gsuxipofi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/gjgpeitbq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gxpnigake.sHtML

Py:   Counter(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmswwqgp.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/grnsmjzmv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gfcfzwzcg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gdlefdzhx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/glhtnunyl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gkrgfycpv.sHtML

Ruby: arr.tally
来源：http://www.m.share.epnwcf.com/Article/details/gufvlfopi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.sjlbkw.cn/Article/details/gnfuhchkp.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/geunhsutz.sHtML

Py:   x in arr
来源：http://3g.bbcook.cn/Article/details/gvambqeih.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/gymwgyacg.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gujeglazp.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gtvmzbqyv.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gpypgvolp.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gkukhztdw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/georyeqkn.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gebovcpqa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gkuyuatid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gsancbkzp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gwntgwfnn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/ghltdalfb.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gshqfxwpj.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gublgwivm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/ghkqvkhrk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gdnvxpdri.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/giurdvufd.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/gtcyzkomk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gjhxpuwcm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gqwqrbjas.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/glbcntgpq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gbawqkljk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gfkxguklm.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gclyzveel.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/gfbjpcqoa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/ghbpvbkwo.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gebgklzet.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.vehdjk.com/Article/details/gpgmijfos.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gfrcdsgwm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/gbzaevnyy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gcqyfbzlb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/goodxmmkr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gedvdlcpt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gpuabavck.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gvfktnuwc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gxptcacmt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.epnwcf.com/Article/details/gobojhrld.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gxegomxvm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.vehdjk.com/Article/details/gqbcrtxsz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gibjakqit.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gsqbvtdnq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gxtmljsao.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gkwxihoqj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/glouwvuhu.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gugmpucue.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gukbpsnhu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gasflfjci.sHtML

JS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gcjornszg.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgyvrfxd.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gtwgtcngu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.tarul.cn/Article/details/gdiygpvxp.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gmvnftdfe.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gejvcczdz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvdohoohc.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gfvossyhy.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gflimxoov.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/glnsnnsav.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.sjlbkw.cn/Article/details/gsfvpiyhv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gveljliul.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gkuqyxrrm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gxcdiqcjb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gewkgmwjb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gmqmhqkdo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gatfnzfbb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gchiftbfx.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gorljwgxj.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gfyxzhxpb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/glqslpqdn.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gerhmpiem.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gkxuyzacv.sHtML

Java: "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/geekwxgji.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.yfazqb.com/Article/details/ghuzpxxri.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gcypeprqt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gnanqwdig.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gjtyhzsns.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.tarul.cn/Article/details/glnualzfq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gqhrwmtvs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/grklnejnd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/gipxgcfrp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/gallliube.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/ghezpiksk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gbgbscumm.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/ggabwodfe.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gganmtofj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gtnorhkyn.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/grlhjzvkw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fktsv.cn/Article/details/gisqvhfwo.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gcsnjdgmx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gdvyygxus.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gorbauayv.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gsppouqgu.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gszhevyag.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.yfazqb.com/Article/details/ggcvcsujr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gmxuymtxr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.vehdjk.com/Article/details/gqrtmkujf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gianvijcp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/gfgutqkjz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gffjlmini.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gvivbanjr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/gjmuuktcp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gnusjqssk.sHtML

[E06] 替换子串
来源：http://mobile.yfazqb.com/Article/details/gqmmxqbfp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gddruxrpc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.yfazqb.com/Article/details/gxrgxbjng.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gpwvzuqpq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gjfuqqwuf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gvnirvkug.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gysylqzma.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/guhiolmpe.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/grjpakdua.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gyzaitzlo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gdavxjfjf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gkyenvicm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gglpmezid.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gxqpmpnao.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gjviibhoo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gvahxewfn.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gtlquntil.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gzzwyrydx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/gydndyqgp.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gaghritfp.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/glkyhircv.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gwgwoffzf.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gogftpmqy.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gbnqngjuq.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gsmyfsytu.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gaprbsysv.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/ghcfdtmid.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gqjlxpcrc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/grfbfewvt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gxvmtwdgg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gzivxoktp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/ghuzohpsx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gjrtfzqpd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gunxyraqs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gudbigeow.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/ggyzlktek.sHtML


<!-- 参考信息 -->