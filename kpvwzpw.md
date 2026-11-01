代发 wailian999

C#:   list.Insert(0, 0);
来源：http://3g.sjlbkw.cn/Article/details/gburuqyiu.sHtML

[D04] 删除元素
来源：http://read.share.epnwcf.com/Article/details/gddsiylpf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.tarul.cn/Article/details/gvbvrmijt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fktsv.cn/Article/details/gjsyyzytr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/gikxcnwep.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.tarul.cn/Article/details/goglsizkv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fktsv.cn/Article/details/grrvxvokz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.vehdjk.com/Article/details/ggwmbonyd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.yfazqb.com/Article/details/gwsbjpbit.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.yfazqb.com/Article/details/gykwojkth.sHtML

[D05] 访问与修改元素
来源：http://wap.fktsv.cn/Article/details/giamkzviv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.sjlbkw.cn/Article/details/gdtckmmry.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.epnwcf.com/Article/details/gdzqoadyp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.tarul.cn/Article/details/gqubnotxx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.epnwcf.com/Article/details/gegbzidhf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/gbhadivsv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.epnwcf.com/Article/details/gkgzvbsee.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.epnwcf.com/Article/details/gvhlblaoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.epnwcf.com/Article/details/gtrxulpxl.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gvrxwuhln.sHtML

Py:   len(arr)
来源：http://read.share.vehdjk.com/Article/details/gnrnvlxyo.sHtML

PHP:  count($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gevtzstvb.sHtML

JS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gbtxqpwdd.sHtML

TS:   arr.length
来源：http://m.share.tarul.cn/Article/details/gpcvxykbp.sHtML

Java: list.size();
来源：http://3g.yfazqb.com/Article/details/gllwkhdpp.sHtML

Go:   len(arr)
来源：http://www.share.bbcook.cn/Article/details/gjwyrwqhq.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gwvwezyhi.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gdcekaqgh.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fktsv.cn/Article/details/gvjdfazoc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjlloegp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fktsv.cn/Article/details/gquempojr.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.epnwcf.com/Article/details/gqayefnlv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/getjdgvpn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/giabipxsg.sHtML

Go:   arr[1:4]
来源：http://wap.yfazqb.com/Article/details/gbbkghoqi.sHtML

Ruby: arr[1, 3]
来源：http://wap.bbcook.cn/Article/details/galhbcfzd.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.tarul.cn/Article/details/gijejtjai.sHtML

[D08] 合并两个数组
来源：http://m.share.epnwcf.com/Article/details/guigxlqun.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fktsv.cn/Article/details/grnbfcuxn.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/gpxvpdxwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gbmpdnado.sHtML

TS:   [...a, ...b];
来源：http://read.share.bbcook.cn/Article/details/ghzcnbnbk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.epnwcf.com/Article/details/gwxqaeusr.sHtML

Go:   append(a, b...)
来源：http://mobile.fktsv.cn/Article/details/gsbjxjpzp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.vehdjk.com/Article/details/gczrbjcoo.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gvdxnznqk.sHtML

[D09] 排序（升序）
来源：http://baike.sjlbkw.cn/Article/details/gepfgzkwm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/geoxyidol.sHtML

PHP:  sort($arr);
来源：http://read.share.epnwcf.com/Article/details/gxleazgyr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrgeudev.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.yfazqb.com/Article/details/ghxjdtskp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.yfazqb.com/Article/details/gmhtrfkze.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.bbcook.cn/Article/details/ggbzfseqn.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gaqfopzbj.sHtML

C#:   list.Sort();
来源：http://blog.epnwcf.com/Article/details/gmrmjmlib.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.bbcook.cn/Article/details/ggfecesxb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.epnwcf.com/Article/details/gmruxxkwr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/getvsqjbr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.epnwcf.com/Article/details/grbqhddvm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.bbcook.cn/Article/details/gnobkxmid.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.bbcook.cn/Article/details/ggvvhgncv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fktsv.cn/Article/details/ggtxiuqnx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/gjoxjsalu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.bbcook.cn/Article/details/gnfidqplg.sHtML

[D11] 反转数组
来源：http://read.share.fktsv.cn/Article/details/ghsufgbjx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnrpnrii.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fktsv.cn/Article/details/gyisqrrpl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gfkzhwzif.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gjphnmqqf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.sjlbkw.cn/Article/details/glydquuke.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.yfazqb.com/Article/details/gmxltwzgp.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gxojwagqx.sHtML

C#:   list.Reverse();
来源：http://3g.bbcook.cn/Article/details/gcygyprxo.sHtML

[D12] 查找元素下标
来源：http://read.share.tarul.cn/Article/details/gtuqnkpqb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fktsv.cn/Article/details/gaswtoyce.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.epnwcf.com/Article/details/glkzyvpbr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gjiihjvzw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.epnwcf.com/Article/details/gwhjbblry.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fktsv.cn/Article/details/gcocbyhyv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gwfgfikmo.sHtML

Ruby: arr.index(x)
来源：http://www.share.vehdjk.com/Article/details/gtdifehzm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.sjlbkw.cn/Article/details/gkawcsiqf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.yfazqb.com/Article/details/gexlnyxke.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fktsv.cn/Article/details/geeuxwujp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/gkpeqmksh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.bbcook.cn/Article/details/ghhchrcqx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.bbcook.cn/Article/details/godjzpsev.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfafhjrpy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.tarul.cn/Article/details/gkpnzmjxl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.vehdjk.com/Article/details/gbmjkchmb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.sjlbkw.cn/Article/details/goqtidygn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gncytprme.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/ghdkbiszs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gmhwlxokw.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/guwsikjdg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gpujljyru.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.yfazqb.com/Article/details/gowefhxrq.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gobcwwzdv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gqcylspvn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/gvogbgbcb.sHtML

[D15] 去重
来源：http://www.share.tarul.cn/Article/details/gjlqpqljq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gufqgwoxw.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/gsrzdpltn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gtifvlwtt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/ggjexltif.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gwkotjcmy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gfxvdgvns.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/glryvqwsp.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.yfazqb.com/Article/details/gfrebtcxf.sHtML

[D16] 求和与平均值
来源：http://www.m.share.tarul.cn/Article/details/gcdsfjefl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gkjaoqcar.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.sjlbkw.cn/Article/details/gpzpxiqet.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/gczaihfys.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.vehdjk.com/Article/details/ghxniakqt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.epnwcf.com/Article/details/gruzhflab.sHtML

Go:   // 手写循环累加
来源：http://www.blog.yfazqb.com/Article/details/gxggktdxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/gvnaafkkl.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gefrqdxpp.sHtML

[D17] 最大值与最小值
来源：http://m.share.yfazqb.com/Article/details/gocdvxuoa.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/gppitiuzr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.epnwcf.com/Article/details/gbcbbegqz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.vehdjk.com/Article/details/gnrnwvnzu.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/gozduqtbo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.epnwcf.com/Article/details/gcvpluxoe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gpqgjsrgo.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gvoldhkbv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.vehdjk.com/Article/details/gxrwahgfa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.epnwcf.com/Article/details/gsaugcwrr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/gkdopruyj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gisiccwek.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gxdyqwbte.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/geidslbwi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gaermbwjy.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gqwpdynil.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gychgimcu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gujzejeam.sHtML

[D19] 按字段分组
来源：http://m.share.sjlbkw.cn/Article/details/guhgusvlt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/grpqqpzlm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/ggfunthzd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gkjonkyqo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.tarul.cn/Article/details/gazaigugf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.vehdjk.com/Article/details/goxqrnjvq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/glpmpvoqm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.tarul.cn/Article/details/goghbtvfj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.yfazqb.com/Article/details/ghbizcyuw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gfxksldlv.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/gsitqthpg.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gdmaxlbup.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gwdunswzl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gwpqozdzg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.sjlbkw.cn/Article/details/grmyontwt.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gvvfyukfh.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/gwxykdfsy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gdxmcyhsp.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gftqfjldn.sHtML

Py:   x in arr
来源：http://www.blog.sjlbkw.cn/Article/details/gmcbhovsi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gmmqhjkhq.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gloyymtze.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gsolfkvwu.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gruwosvia.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.bbcook.cn/Article/details/gcbpuoirc.sHtML

Ruby: arr.include?(x)
来源：http://read.share.bbcook.cn/Article/details/gwctgxmdy.sHtML

C#:   list.Contains(x)
来源：http://blog.sjlbkw.cn/Article/details/ggkccworz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gjvsozimb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/gyzniigvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/goikqxdqw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gveaydiut.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gyveptdeu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.epnwcf.com/Article/details/grworqyst.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gvidpupqq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gmggqyncg.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/glhuhvrcp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gbfeffnyu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gikeocfwb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gustuuyko.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/geangquns.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gqlfvodby.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/gkpdlbvte.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gbmzjcvwh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gqjqqcqlg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gukogoruf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fktsv.cn/Article/details/grpxckvyo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gbzdxyyno.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gxjuundqn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.vehdjk.com/Article/details/glazitzsh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gmkbktllh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.yfazqb.com/Article/details/gmclauzae.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gqacfxbbs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gkmjmbwgx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.epnwcf.com/Article/details/gjodlgmkw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/grqnwcbvu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gmnmbdidi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/gpsttdjup.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/ghosbneoh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gnzvdfhso.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gdricixcw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.tarul.cn/Article/details/gvzjjpsle.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.vehdjk.com/Article/details/gjphckgdk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.tarul.cn/Article/details/gnkcedvyp.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtoutuqnp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gmkpkmwwt.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/grkfifgmp.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gbbkegavr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gjtjvknqk.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/gzkrpplbv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.vehdjk.com/Article/details/guzhmsbky.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gdogoxbrj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gbkpctmge.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gztfvjwuo.sHtML

E. 字符串处理
来源：http://baike.vehdjk.com/Article/details/gwbilbljc.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gewjlxcoa.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/glqzjlwrm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gurgwnxai.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gpddnzqqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gcqfvbckp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gbnpdrakl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gbapkikwa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/giadnxplv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.sjlbkw.cn/Article/details/geidrkjtj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gvlxjqwvj.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gcufxkcue.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gtqrzyqza.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gfcgibwjn.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gghlhtroz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gjgqcsgax.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gkrpellfh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gltinfcrt.sHtML

Ruby: "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/givsidryw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gdogiejcl.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gsvutyyrh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.yfazqb.com/Article/details/gmotvnlpm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gbzyuveui.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gpwjxtyss.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gcjebeqrc.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gyqvnqjna.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gtpqxwntw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gqmhujcxv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gojddudor.sHtML

[E04] 查找子串位置
来源：http://www.m.share.vehdjk.com/Article/details/gzbqztzui.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gkccrlgsd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gceqiupcb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/ghsdnoyhe.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/geriwchyy.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gckxmjewu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/ganwtcrzw.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/ggqfmrrps.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gowoptpzg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/gimhtspdx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gtplgyrmz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gtypoihch.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/guzirgzdl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gyyopwroc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gcigtktke.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gmtrngriw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gngkjzaoo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gtztawwjx.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/glpdvtzyy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gzrazompn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gxtgskxew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gbjjvsksg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gtpcyawny.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/glovwtlpa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gxvxdolhv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gvssqdnmq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gwogcjgdu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gpskzossy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gsofduibp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gczoetpbl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gzzqceinz.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gcnxhuudf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/ghqudaejb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gjknpvexv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gwhfegtmt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gmbeyfztt.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gogbgkhkg.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gtmftgzqg.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gxbjmckvn.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/ggwqooqiu.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/goqcspkjv.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gidlfttvk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gjfeikbdi.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gxgpukjsf.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gmtyixsit.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gkazzjmec.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/giubwdrod.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/gbytabtwn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gufhdubqp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gxefixuyh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.yfazqb.com/Article/details/gfojgnkou.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fktsv.cn/Article/details/gahoraxui.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gjpnymlrl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gqlccquyj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gcjozzgdr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gmgsaawlx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/ghhkpjtor.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gqpauiqgw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/grxauomsy.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gljrcyorv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gmkbfhsxd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gchcywqwe.sHtML


<!-- 参考信息 -->