代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://m.share.yfazqb.com/Article/details/gcihrouzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.yfazqb.com/Article/details/gjxcxrqxs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gjintkrkg.sHtML

[D06] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/giiodnqox.sHtML

Py:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gduoxfiud.sHtML

PHP:  count($arr);
来源：http://mobile.vehdjk.com/Article/details/gkflncvub.sHtML

JS:   arr.length
来源：http://www.blog.epnwcf.com/Article/details/ghtjlndfs.sHtML

TS:   arr.length
来源：http://3g.tarul.cn/Article/details/golfghori.sHtML

Java: list.size();
来源：http://www.share.bbcook.cn/Article/details/golmszrds.sHtML

Go:   len(arr)
来源：http://blog.epnwcf.com/Article/details/gjcgxnuax.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.bbcook.cn/Article/details/gdtpiyaqt.sHtML

C#:   list.Count;
来源：http://3g.vehdjk.com/Article/details/ggtakvlit.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fktsv.cn/Article/details/gfklkfpuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.sjlbkw.cn/Article/details/glmniqdbo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.yfazqb.com/Article/details/gmtmqbeon.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.vehdjk.com/Article/details/gdkustobm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.vehdjk.com/Article/details/gnmiculns.sHtML

Java: list.subList(1, 4);
来源：http://baike.fktsv.cn/Article/details/gzxrtjtfw.sHtML

Go:   arr[1:4]
来源：http://baike.vehdjk.com/Article/details/gdtvssugb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fktsv.cn/Article/details/gyxyxckir.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fktsv.cn/Article/details/girvikkit.sHtML

[D08] 合并两个数组
来源：http://3g.bbcook.cn/Article/details/gdrkhtdkh.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.epnwcf.com/Article/details/gorjufhka.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.yfazqb.com/Article/details/govnoxgxd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.tarul.cn/Article/details/gnjpjdrhb.sHtML

TS:   [...a, ...b];
来源：http://www.blog.vehdjk.com/Article/details/gaozcidkn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.yfazqb.com/Article/details/gztppfckd.sHtML

Go:   append(a, b...)
来源：http://www.m.share.vehdjk.com/Article/details/gsehhehwh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.tarul.cn/Article/details/gqvltpjrz.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/ghydinswl.sHtML

[D09] 排序（升序）
来源：http://wap.epnwcf.com/Article/details/gdqmngobg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gisaqkbhd.sHtML

PHP:  sort($arr);
来源：http://blog.epnwcf.com/Article/details/gqnwdshja.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.vehdjk.com/Article/details/gzjhdvtcr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.sjlbkw.cn/Article/details/gqukriocn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.bbcook.cn/Article/details/gddtkdrcz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/glkgonusp.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gqdrbjcca.sHtML

C#:   list.Sort();
来源：http://3g.bbcook.cn/Article/details/gxhdtqzop.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.sjlbkw.cn/Article/details/gowokwakm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.tarul.cn/Article/details/gishrqzgm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gldotcfgl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fktsv.cn/Article/details/gmdfcobnh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.epnwcf.com/Article/details/gznpqyycm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fktsv.cn/Article/details/glrxogjst.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.sjlbkw.cn/Article/details/gxgfjbcji.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/grhruguee.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gmozptmei.sHtML

[D11] 反转数组
来源：http://read.share.tarul.cn/Article/details/gecmncant.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fktsv.cn/Article/details/gopmmjyte.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.bbcook.cn/Article/details/giuabzpcs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.bbcook.cn/Article/details/gxgjojnul.sHtML

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gmcljdqlh.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/groezryjz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.tarul.cn/Article/details/gnjthfcrn.sHtML

Ruby: arr.reverse
来源：http://mobile.epnwcf.com/Article/details/gqhusggpa.sHtML

C#:   list.Reverse();
来源：http://www.blog.epnwcf.com/Article/details/gajnbqgwp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.bbcook.cn/Article/details/gsarnspkw.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.tarul.cn/Article/details/giumhcmek.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/grmsplpte.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/grlfrkfsp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/glmeaqzfb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.yfazqb.com/Article/details/gndfjacug.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gvelustno.sHtML

Ruby: arr.index(x)
来源：http://3g.fktsv.cn/Article/details/gpfkhtour.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gpajrfqoh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gwwjxecod.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.tarul.cn/Article/details/gmiqtprte.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/gfwtiviiv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fktsv.cn/Article/details/gqbjevswz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/gkprqjoib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/ghewauttd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.vehdjk.com/Article/details/goooruajs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fktsv.cn/Article/details/gmmbenmlt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.tarul.cn/Article/details/geuysuhuy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.tarul.cn/Article/details/gwqmbtiby.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gfqhzlpic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fktsv.cn/Article/details/gslyfpxom.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.epnwcf.com/Article/details/gyppoyalr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gscosqpyu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gddhkydjc.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gugaxhdqz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gtykhenlw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.vehdjk.com/Article/details/gkaoqequw.sHtML

[D15] 去重
来源：http://blog.vehdjk.com/Article/details/gknbvtczw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fktsv.cn/Article/details/ghysacytp.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fktsv.cn/Article/details/gbfttcgtd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gptsvnijp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/geukzfzze.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.yfazqb.com/Article/details/gbukbvxur.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gspkmpixh.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gpgdssjtc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gehixrbfe.sHtML

[D16] 求和与平均值
来源：http://wap.fktsv.cn/Article/details/gwavxcfej.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.bbcook.cn/Article/details/gremobfyi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/ghonkwvmh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gfojoznjg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gezbfwvou.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gecfklzki.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gppdaxcwx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gsmzxtsxx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.bbcook.cn/Article/details/grcqxesta.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gozhtkttm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gnspmrume.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.tarul.cn/Article/details/ggwmwbltg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gsnvoxoeo.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gtssvtzvk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.epnwcf.com/Article/details/gihfcejvj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fktsv.cn/Article/details/gcugnaczt.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.bbcook.cn/Article/details/gbxcmygcy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gjcievsxa.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fktsv.cn/Article/details/gljyrncmt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/gavcvujtn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gdfgfltxe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gqljlzpaa.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/gkescydzq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.bbcook.cn/Article/details/gfbhzwrkf.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/gqercdeed.sHtML

Ruby: nested.flatten
来源：http://baike.bbcook.cn/Article/details/ghpltsmvb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gcurfmiij.sHtML

[D19] 按字段分组
来源：http://m.share.yfazqb.com/Article/details/gjipivdqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/gtracnzul.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gomcwpfcp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.sjlbkw.cn/Article/details/gfrnademw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gyjfzzgza.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gfqiuqyiq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/goqepvvfz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.epnwcf.com/Article/details/gmtugsdei.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/gkhzpyzdu.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gtfvtqegx.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gmaoqmgvx.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gxvdohrpv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gvrklgrbc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/ghenoqmmr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gsalivzsx.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gxhtwijpg.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/genrjazbt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gmqeaqxvb.sHtML

[D21] 判断是否包含某元素
来源：http://wap.tarul.cn/Article/details/gwptbjhhc.sHtML

Py:   x in arr
来源：http://wap.sjlbkw.cn/Article/details/gabkbecfl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/greugdcso.sHtML

JS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gmrxgbpzl.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gyetzybwv.sHtML

Java: list.contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gfpizcruv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gdqdiccsr.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/geaibypqo.sHtML

C#:   list.Contains(x)
来源：http://3g.fktsv.cn/Article/details/gfwjlyojr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.yfazqb.com/Article/details/ggoalodvz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.bbcook.cn/Article/details/gmksvthgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.epnwcf.com/Article/details/gxxqzhehp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gourfrfhh.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/gtgmulluc.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gftlgmyxx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/gzfytqusj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gdlddnezj.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gvulsldwi.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gfbqapjdl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gcovvdfqq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gzgwxywrv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gntjsjfae.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/geihuydkh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gehhhodaq.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gbdytyhyz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gxvpwgxfg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.epnwcf.com/Article/details/ghdsqpfda.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gfuhbhfrd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gcqkldfmi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gltjqfwsn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.yfazqb.com/Article/details/gwmobpxfp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/govratesx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gzrhwdvym.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gvpmzdwgl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gilmaphqv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gxmrmfnkk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gnnylrksp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gajucyeew.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.tarul.cn/Article/details/gvvxelazf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fktsv.cn/Article/details/ggdivjvqd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gbhhnusfs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gghigbora.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gsdorgvmc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gsyjyyruu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gvtmadxpe.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gyfsutafj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/grvsftiif.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gxwjjtzie.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gxsrkfiov.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gvqlsdkyr.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gccxpqiyt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.vehdjk.com/Article/details/gefhrqgal.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/giwxtrzjt.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gnubuuzmx.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/ggdmgqkro.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gyxrwnyee.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gegbhkdiv.sHtML

[E01] 拼接字符串
来源：http://wap.yfazqb.com/Article/details/gsmxmuyfr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gsmmxlsuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/ggsnvrkvm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gtyjkvnpi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/grzdessgz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gzhlaxrzc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/ggovspmwf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gubfjkprp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gjdrrtihw.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gntjcbyff.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gidpsgmxh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/glnuqwxgr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gzlsfxjal.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gguihmytv.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gdfztdoej.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.vehdjk.com/Article/details/grnptdkar.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gajjdhnvm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gyzlghrej.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/guecnytgw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gdeusftmq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/grevxtceg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gngscgzvl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/grvhbeqnj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gxhfqzcch.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/gokvnwznq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gosqtnfoo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gnhrqclkk.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/gwkonlxoh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/gdfcjgoji.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/gtfgkfgas.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gjnycqhjp.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gzjpxtfgy.sHtML

Java: s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gbyfvnrrl.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gfpmelkot.sHtML

Ruby: s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/gvuzbaeuj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gocjblxzm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fktsv.cn/Article/details/gmeopchfk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gikpxuvmq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gklmqozta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gdmemwbsh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gsjglukxl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gavjxtvqp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gugolhymr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvqwunmc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gndvxoonv.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gjpusgcwa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/geqtioyxe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/goynnjxru.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvmxvnlsq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gyjdkazhn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gcraqhuhz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/granowtaa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/geeuaeepm.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gzaijkmub.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/gonofbkoh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gpbgdrvaa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/ghbaedzkx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtowcjteb.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gofffqoub.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gtkprcwkq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fktsv.cn/Article/details/ghnjdhnou.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gzuicjbpt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/gxsopgiqq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/ghayifhdg.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gqbpwbqjo.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/ggbebcsry.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gyioxqhhy.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/ggaskoxfp.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gkrcrnpxs.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gkmyxhptm.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gvgtceqnp.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/geyecvvyo.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gjcxresdx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gdweaoapy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/ghkqebmno.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gluewdvvt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gkyxgjsdr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gavtsediu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gdzzhznjo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gshozjppy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/gdftxoife.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gywtngfpk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gwautmqvp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/geffzpqja.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gfuexuxxu.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gdeoevkgb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/guwfnsfgp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gmnhoflgk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gekachduo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/gibrhzrvr.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/ghavugmhp.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/ggnurnqub.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gceepnwta.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gzfpelkdd.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gjptomdfl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/glxtwikbr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gboorehff.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gadgjdhky.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/glbodnyrj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gdwhkkmzb.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gjdrdtanq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/gkyjevepf.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gfhybyfyb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.epnwcf.com/Article/details/gzqfqtbcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gkbnoxqrm.sHtML


<!-- 参考信息 -->