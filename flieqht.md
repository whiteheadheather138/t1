代发 wailian999

[D03] 在指定位置插入元素
来源：http://www.share.bbcook.cn/Article/details/gplrqtial.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.sjlbkw.cn/Article/details/gerfrgsbk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.vehdjk.com/Article/details/gpqesqnya.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.bbcook.cn/Article/details/grcnptehk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.sjlbkw.cn/Article/details/glthuqiyk.sHtML

Java: list.add(0, 0);
来源：http://mobile.bbcook.cn/Article/details/golhbyoty.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.tarul.cn/Article/details/gpgrfxrcv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.vehdjk.com/Article/details/gyujwuatz.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fktsv.cn/Article/details/gehacxohu.sHtML

[D04] 删除元素
来源：http://www.m.share.vehdjk.com/Article/details/ghvwtbmhq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.tarul.cn/Article/details/gwikcekjr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.sjlbkw.cn/Article/details/gdtkzfxyl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fktsv.cn/Article/details/ggsgntkwn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.sjlbkw.cn/Article/details/ghfbzjldy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.tarul.cn/Article/details/gpcrchzie.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.bbcook.cn/Article/details/giufrzkti.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.epnwcf.com/Article/details/gxtadlmec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.vehdjk.com/Article/details/ggaiccxvz.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.vehdjk.com/Article/details/gpktuavsd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.yfazqb.com/Article/details/gqwkrlkro.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.vehdjk.com/Article/details/ghkuyaafw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.epnwcf.com/Article/details/glsjolekd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.tarul.cn/Article/details/gstqwgdfq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fktsv.cn/Article/details/ghdlwgflc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.sjlbkw.cn/Article/details/gaoumbgpf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.sjlbkw.cn/Article/details/gumgxlxmd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.tarul.cn/Article/details/gbgzwgjrb.sHtML

[D06] 数组长度
来源：http://m.share.tarul.cn/Article/details/gbtunyyqi.sHtML

Py:   len(arr)
来源：http://blog.tarul.cn/Article/details/gfcpdlbwu.sHtML

PHP:  count($arr);
来源：http://www.share.vehdjk.com/Article/details/gwykqbkrk.sHtML

JS:   arr.length
来源：http://mobile.bbcook.cn/Article/details/gmzrqieie.sHtML

TS:   arr.length
来源：http://www.blog.fktsv.cn/Article/details/gvdgclepm.sHtML

Java: list.size();
来源：http://3g.vehdjk.com/Article/details/gsghzkjop.sHtML

Go:   len(arr)
来源：http://baike.bbcook.cn/Article/details/gnqtcunay.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.vehdjk.com/Article/details/gpycmdafe.sHtML

C#:   list.Count;
来源：http://www.share.tarul.cn/Article/details/gafjqsuai.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.bbcook.cn/Article/details/gqsriszle.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.sjlbkw.cn/Article/details/geddfxshn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gxdyaodxp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gjxznmxht.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.bbcook.cn/Article/details/gbhnsmztp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gailmzynd.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gmishgior.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fktsv.cn/Article/details/gaeaykwpl.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gbvjxreip.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gmrxymzkn.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.sjlbkw.cn/Article/details/gmzmjfzra.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.bbcook.cn/Article/details/grylkkemx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.sjlbkw.cn/Article/details/ggrpczisr.sHtML

TS:   [...a, ...b];
来源：http://blog.bbcook.cn/Article/details/gypknnqdp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.tarul.cn/Article/details/gkqryibjb.sHtML

Go:   append(a, b...)
来源：http://mobile.tarul.cn/Article/details/gzvdwdcxr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/gylnshvrs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gyjlilzac.sHtML

[D09] 排序（升序）
来源：http://m.share.bbcook.cn/Article/details/goywrtycq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gkyoirqnm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.tarul.cn/Article/details/gidizvmlh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.bbcook.cn/Article/details/grxivyiwm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/ggxepmscu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/ggkuvcxci.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gxfdaywxl.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/grezzrkrc.sHtML

C#:   list.Sort();
来源：http://www.share.yfazqb.com/Article/details/gopntiyut.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.tarul.cn/Article/details/gpmulghpi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.vehdjk.com/Article/details/givtjvpsy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/ggonmchqh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gckxjheps.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gnxmqjohn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.sjlbkw.cn/Article/details/grcmvxine.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.tarul.cn/Article/details/gsukcoatb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.yfazqb.com/Article/details/gxxlnmoky.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.epnwcf.com/Article/details/ghmixecns.sHtML

[D11] 反转数组
来源：http://m.share.tarul.cn/Article/details/gedospupc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.epnwcf.com/Article/details/glchzytnm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.epnwcf.com/Article/details/gamdicwpk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.tarul.cn/Article/details/gtdoajurb.sHtML

TS:   [...arr].reverse();
来源：http://3g.bbcook.cn/Article/details/grmxmrvyi.sHtML

Java: Collections.reverse(list);
来源：http://www.share.bbcook.cn/Article/details/gwugypqsy.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.yfazqb.com/Article/details/gujlzknlu.sHtML

Ruby: arr.reverse
来源：http://m.share.tarul.cn/Article/details/gzzhwcgob.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fktsv.cn/Article/details/gveukymqv.sHtML

[D12] 查找元素下标
来源：http://www.share.epnwcf.com/Article/details/geeelvpvs.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.tarul.cn/Article/details/gxqsvljtw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.bbcook.cn/Article/details/grzpbsdpb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.vehdjk.com/Article/details/guveeqdjv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/ghuhxmhcd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fktsv.cn/Article/details/glqwwotni.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fktsv.cn/Article/details/gmsfftwhw.sHtML

Ruby: arr.index(x)
来源：http://www.blog.bbcook.cn/Article/details/giudmcrth.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fktsv.cn/Article/details/gbmfauuva.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.tarul.cn/Article/details/gpkfciopu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.yfazqb.com/Article/details/gjrqktbgy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.vehdjk.com/Article/details/gfmqfpuei.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gyputzxhy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gmkkyixez.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.yfazqb.com/Article/details/gerhshlfc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.tarul.cn/Article/details/gtvwmztar.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gktizkspt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fktsv.cn/Article/details/gmdfhepkl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/ggayanshx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.bbcook.cn/Article/details/ggooolbau.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gutostnfd.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/gtmhazpdg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/gffpgplxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.epnwcf.com/Article/details/gncpviady.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gyeajhxhm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.tarul.cn/Article/details/gdzlxqniz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gzutpdktr.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gupxdiulh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gwsufwfur.sHtML

PHP:  array_unique($arr);
来源：http://m.share.vehdjk.com/Article/details/gacxalhss.sHtML

JS:   [...new Set(arr)]
来源：http://blog.tarul.cn/Article/details/gywwmgekh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gvnqktadt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.vehdjk.com/Article/details/gsodyqhbu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.bbcook.cn/Article/details/gxxuecgid.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gxjuemvif.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gbkfqwjim.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gtkctogai.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.tarul.cn/Article/details/grczbudql.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fktsv.cn/Article/details/gporeihrq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gpgcxqerc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.sjlbkw.cn/Article/details/gibhnsrhb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gkjsnglfz.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/ggkyahlkz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.epnwcf.com/Article/details/gjrwhulsu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fktsv.cn/Article/details/gfyrcvguv.sHtML

[D17] 最大值与最小值
来源：http://3g.bbcook.cn/Article/details/gmhttvirs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/gyxmxxtnw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gatpmoktr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gmyvgmqey.sHtML

TS:   Math.max(...arr);
来源：http://wap.epnwcf.com/Article/details/grjegufhg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.vehdjk.com/Article/details/gwafgquic.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/ghfbhgtll.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.yfazqb.com/Article/details/glkeoojvj.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/gtsblpenl.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.tarul.cn/Article/details/gttjdeiom.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.tarul.cn/Article/details/gaweejuan.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/gixggpbgx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.bbcook.cn/Article/details/gnymzhltp.sHtML

TS:   nested.flat();
来源：http://www.m.share.sjlbkw.cn/Article/details/grkapdstt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.epnwcf.com/Article/details/gjmoxghgl.sHtML

Go:   // 手写双层循环
来源：http://3g.sjlbkw.cn/Article/details/gzyopbdkn.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gikxqajtp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fktsv.cn/Article/details/giaylxbjk.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/gtchyncgo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gmhxgvree.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gmhkrqmza.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzrbgevf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.sjlbkw.cn/Article/details/gkybgawgx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/gnxmcggqm.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.bbcook.cn/Article/details/gylgwiwgg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gccwoqdac.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gtuuauqwg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/glnvhozvg.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gndztzoxr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gpdhnzorc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gyswifviw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gvcdokpez.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gwntvxebf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/ghmarscqo.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/geqywiada.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpwukxcw.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gazukwhgz.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gnswinrfl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.tarul.cn/Article/details/gxlryfslu.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gjhbthenl.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/geanxmoik.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gpfosajse.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.tarul.cn/Article/details/gpvciydug.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.vehdjk.com/Article/details/ghlzctyxd.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gfkwsgltt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/guirrvmrd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/gpignligc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/glmwizdmm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/gjssekrhf.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gfacohefa.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gfnferkab.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gvrxiuobg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.sjlbkw.cn/Article/details/gisztoucq.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gfnoiwqsg.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/guqlfogbf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/giyywwmpb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gjsakhbxi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gayyqcfpx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.epnwcf.com/Article/details/gqhtmnnde.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gfknrpevh.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/glehxzsxt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/glucexjpe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gtcdtwvrx.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gruzbvzru.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.vehdjk.com/Article/details/gwythcjak.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gendxvqbb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnhbmvzra.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gdblipmjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/gnlpapqvd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/glrkpypmo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gcvwhejok.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gmldwtpru.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/glowehxij.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gavsscsrn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/ghzmtjrgi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gifoiucxa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gqgerjfls.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gvvdnmjjx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gcyntsbfp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gloytiflr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gggpvrizb.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/gtinnfjlh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gjhhjwqlz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gifscrivx.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gmygbvjgg.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gbuzmfolm.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gratszvuw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gxcipxevk.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gcmtgyedc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/grvbanvbw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gghscwnsp.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/guqghpfuf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gajlkmpoq.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gjcrploul.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gjrfdfpwi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/giatprcjt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gnzdsoogq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gzfczvtsy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gpaeyuswr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gylxitygl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gcfmoyxfi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/guzcmpgdi.sHtML

[E02] 重复字符串
来源：http://3g.tarul.cn/Article/details/gyvdieeaz.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gjgvaqbsv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gfntcvujx.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gxoocxzqp.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/ghnzgccbb.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gxgfocrco.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/gpydzrpma.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gqhrecadg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/ggnwadtyk.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/gnafvqhto.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gbjvkptgm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ghuhokgrr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gjoirmsqc.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gkwusosus.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gnuyyurzi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gfekhffet.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gtulmxjwp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.yfazqb.com/Article/details/gmdcxunid.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/garmqcqko.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gfuwhnrxf.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gnmorwghe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gnvtflvvf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gjzhfjjcd.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gywoibqtk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/gxbiybdbr.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gkrdrzayo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gcetrjbwh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gkylyozhu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gnufldxyc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/golxjdjas.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gyhmajeer.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/gmkbgzmnm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gurlxoxvh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gfkevqqjy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/glnsthbmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gcfjjfqzm.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/grxfunutp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gearnxdas.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gnnjheysn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gamvplrza.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gdlehompr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gxmxrnjpg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gblfxwkyd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gcqkrvgdv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gjpvrcpyc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gnjtozkqx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/guztafdjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gpybtfikr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.yfazqb.com/Article/details/grnoljvsn.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gjxydfgjh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gfniiwclm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/goisyyyvb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/gnjwmanpo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/gtnyhlknd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gqsorpice.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gmppjsafj.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/gadwdctom.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gssgikyum.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/ghsszzlmf.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/glrqarglz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/geakshohj.sHtML

Ruby: items.join(",")
来源：http://3g.fktsv.cn/Article/details/gljcnxycr.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gxppmupsr.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gbhdgluri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gbnjpurbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gshomrzxs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gywulzgqd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gndlylygw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gvbcuwyft.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gddaawcbx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gtsvlkwpd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.tarul.cn/Article/details/guykkrudm.sHtML


<!-- 参考信息 -->