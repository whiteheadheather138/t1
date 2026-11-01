代发 wailian999

Java: list.size();
来源：http://3g.bbcook.cn/Article/details/gcibnrqfk.sHtML

Go:   len(arr)
来源：http://wap.fktsv.cn/Article/details/gcenmvahm.sHtML

Ruby: arr.length; arr.size
来源：http://3g.sjlbkw.cn/Article/details/gfuyunfgw.sHtML

C#:   list.Count;
来源：http://baike.epnwcf.com/Article/details/gukoodikc.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.sjlbkw.cn/Article/details/geivnxhwm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.yfazqb.com/Article/details/ggwqrgqmz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.epnwcf.com/Article/details/gbtwokmcv.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fktsv.cn/Article/details/getjghidc.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.sjlbkw.cn/Article/details/gwcjjwnmx.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gcxvxgmyq.sHtML

Go:   arr[1:4]
来源：http://m.share.epnwcf.com/Article/details/gzivyseed.sHtML

Ruby: arr[1, 3]
来源：http://baike.tarul.cn/Article/details/gsxglzyir.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.bbcook.cn/Article/details/gpnqooupu.sHtML

[D08] 合并两个数组
来源：http://blog.fktsv.cn/Article/details/grmgugvhz.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.epnwcf.com/Article/details/gekvdntwy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fktsv.cn/Article/details/gpwzoozst.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.vehdjk.com/Article/details/gopcrhdfd.sHtML

TS:   [...a, ...b];
来源：http://wap.yfazqb.com/Article/details/grkotzmqq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.sjlbkw.cn/Article/details/gthditoji.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gefduckxm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.sjlbkw.cn/Article/details/ghochxjyt.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.tarul.cn/Article/details/giyobcwxh.sHtML

[D09] 排序（升序）
来源：http://www.blog.fktsv.cn/Article/details/gdypirakh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/gpuzxrujo.sHtML

PHP:  sort($arr);
来源：http://m.share.fktsv.cn/Article/details/gqwibgfhp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.yfazqb.com/Article/details/gbbsyyxzt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.sjlbkw.cn/Article/details/gukcpqpqg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.yfazqb.com/Article/details/gtrermnpo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gwizzijlq.sHtML

Ruby: arr.sort
来源：http://read.share.bbcook.cn/Article/details/gzaomqulw.sHtML

C#:   list.Sort();
来源：http://read.share.fktsv.cn/Article/details/gcahttvxi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/gptpunqoa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.epnwcf.com/Article/details/gwowvqvoe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/gowpylehr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.epnwcf.com/Article/details/grgiybbye.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gqdmfyaje.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fktsv.cn/Article/details/gxpkqlxmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fktsv.cn/Article/details/gmxcovtav.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.yfazqb.com/Article/details/gaydopcsg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.sjlbkw.cn/Article/details/gzjikinyw.sHtML

[D11] 反转数组
来源：http://baike.epnwcf.com/Article/details/gvneisyuo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.vehdjk.com/Article/details/gkdgovovf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.bbcook.cn/Article/details/gpiohugix.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.tarul.cn/Article/details/gojjhltsy.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fktsv.cn/Article/details/gkukcryiw.sHtML

Java: Collections.reverse(list);
来源：http://baike.tarul.cn/Article/details/ghxkwzlkx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.tarul.cn/Article/details/gxfdwvnxc.sHtML

Ruby: arr.reverse
来源：http://www.blog.vehdjk.com/Article/details/gyunxyvzw.sHtML

C#:   list.Reverse();
来源：http://baike.epnwcf.com/Article/details/gytqbgtei.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gvebsqhpb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpyctamx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.sjlbkw.cn/Article/details/grtpddmos.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.epnwcf.com/Article/details/gfhpufgxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.yfazqb.com/Article/details/goavuyiaa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gcnnivgvl.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gnhplwwdz.sHtML

Ruby: arr.index(x)
来源：http://mobile.bbcook.cn/Article/details/gmrrhtdrz.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fktsv.cn/Article/details/gdkbaqtjc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.tarul.cn/Article/details/gzxqfkybx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.epnwcf.com/Article/details/gyxtxsgml.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/glifftgan.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/gtnnkpsew.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gprcspwnx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.bbcook.cn/Article/details/gscktodrh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.yfazqb.com/Article/details/geeyufotw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gvrwcehvq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gmegllzdj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.bbcook.cn/Article/details/gxsguctvb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/gmnpgdspq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.vehdjk.com/Article/details/gwxmgmqki.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gbiofptyc.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gnjllldth.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gpotqboum.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gcdhcmjbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.epnwcf.com/Article/details/gqmbufdpr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/gpodbpdlr.sHtML

[D15] 去重
来源：http://www.share.bbcook.cn/Article/details/gpvwxxqbg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fktsv.cn/Article/details/gikdhddjg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gzcjkdnta.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/grimeybjo.sHtML

TS:   [...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/grozvbnrh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gtzjfevtq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fktsv.cn/Article/details/gmcdhezlz.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gieiegzqk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.sjlbkw.cn/Article/details/gsohkuwyk.sHtML

[D16] 求和与平均值
来源：http://www.share.vehdjk.com/Article/details/gmduwmfqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ggmdjllcn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdwstgwyf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdkhotcky.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.epnwcf.com/Article/details/gjhxtjiqv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gxhsdgaoo.sHtML

Go:   // 手写循环累加
来源：http://read.share.vehdjk.com/Article/details/gadszabjm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.vehdjk.com/Article/details/gnoduiksb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gqgjaechf.sHtML

[D17] 最大值与最小值
来源：http://3g.bbcook.cn/Article/details/gaowgsats.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/gywqpamhi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.yfazqb.com/Article/details/gtxvugvuq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/ggabstlsq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.yfazqb.com/Article/details/gtoacamed.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.tarul.cn/Article/details/gtbquourp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.epnwcf.com/Article/details/gyxdhkeah.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gxveeecrd.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gborbruar.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.sjlbkw.cn/Article/details/gjpmifhjy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gvrhznibq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gaeelxuww.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.vehdjk.com/Article/details/gievqgjxo.sHtML

TS:   nested.flat();
来源：http://www.share.fktsv.cn/Article/details/gjqhmvkwj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/ghwefnuzg.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gzeaiphzi.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/goahuotyf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/gcpgwaigh.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/gkeiugclr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fktsv.cn/Article/details/gbswksefs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gxfdmczku.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/glsbfonge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fktsv.cn/Article/details/greedpjzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gqzlghlid.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/ggmwiepwj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gxaspatmx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/gzbffqlby.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gvlfvqqal.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gebtsusel.sHtML

PHP:  array_count_values($arr);
来源：http://baike.yfazqb.com/Article/details/gwmucyrxs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gtsrnczwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/giikbdfoc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gaqsvecar.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gkivkkqud.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gptmstmui.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/guqpgxkfx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.yfazqb.com/Article/details/gqrqsunub.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/ggaelpwxg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fktsv.cn/Article/details/gtzuvhqnj.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gmwfxiggi.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gxhnhsnsw.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gtkittmfc.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gkbozrtmm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fktsv.cn/Article/details/gvobngjfs.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fktsv.cn/Article/details/glgjyjoot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gujexjnyq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.bbcook.cn/Article/details/gpdpyfemo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/gxdvpzfzt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtpdfmofj.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/grjqncspz.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.bbcook.cn/Article/details/gkexupnps.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gmehrtmjp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gempohmit.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gxakqmwrm.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/ghjpapxuv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gsfvtxvrj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.epnwcf.com/Article/details/glmtdofcn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gdzzlijme.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gvrcdsbua.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gzqjwqgkd.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gplikburl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gpawwjpvu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gsnezpail.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/ghqhzmmkb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gkxtwdzne.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/givajsjxw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gttqspntb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/gjszkazfg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/ghhqdulal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gxjpeqbqr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/grrskgnnn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gsjchqjtc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/glfdcbtou.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gcuyqsvpi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/ghazdwhzm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fktsv.cn/Article/details/gdwjoppdi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gmoqjszbh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.tarul.cn/Article/details/gmwfgyqns.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gxeagqvmv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gzhhxpusc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gxbrdxrea.sHtML

[D26] 数组转字符串
来源：http://wap.sjlbkw.cn/Article/details/gfippuhmw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/glarrulai.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/guoyiguai.sHtML

JS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/guwjvkwks.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gegfnbjrh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gcbttnagh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gtdcephqh.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gzgnucvmj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gzsljpoza.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcazeadqm.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/ghnbdtkmd.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gztsfbjzx.sHtML

[E01] 拼接字符串
来源：http://baike.fktsv.cn/Article/details/gkslmidlh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/gsxixsxhf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gsqnppgjq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gszevhesk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gakszdrmj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gxuaaonhm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gybftqahq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gpsqignlo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/gwexgvtbs.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gumpumrzp.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gdjzgyplj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gplwkkaer.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/grnoqstag.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gnauebysh.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gphmpvfqn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gdfusdsmh.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gwgnxtxqi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gkbhytcui.sHtML

[E03] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gafevrpys.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gywtkeuvo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gxbnbpzsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.epnwcf.com/Article/details/gvcmzxghe.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gajtkypoj.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/giuuaujtu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gxhoqvfyi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gimxvrkes.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gvrdqadjj.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gpyewolib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/ghsvdlryt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/glgqdljct.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gtimzuwht.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gfdvgbwmr.sHtML

Java: s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gzrnyngzi.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gvcymvvtq.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gdotlrloa.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gionshnsc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/gvfscpjws.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gkoapffqg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gbprempjj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/ghjvndloc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/glkewbiep.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gpzjpemki.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/ggdtblwxr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/glgxrrrte.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/glwlusfwa.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/gdcqofcjb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/ghmigwmku.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/geunjuyfa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gsikyxjpc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gsoiimtjq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gkfgaljmr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gzlnqbtfm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gusheowpk.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/grbdyfwpd.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwjtnbbk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gtaanoyen.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/guwrvtylk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.epnwcf.com/Article/details/gozxmungc.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/guepgqlsj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gvwnoxzvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gohkylkfq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.bbcook.cn/Article/details/gonnezqbr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.tarul.cn/Article/details/gthpjizbi.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/guwbisvfr.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/gvbvgevra.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gvnfwpfnh.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/ghhmpceta.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gxxaovyta.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gneomfceo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gtcnnknml.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gmqegtrfw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/ghatjalhe.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gvjgyoxwe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.yfazqb.com/Article/details/giqfcgjlw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gzezqxgsy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gebqmrpgy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gaplwotsv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gzmfwadfl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gfcvwomvz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gkvlywotr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gitdwaasg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gjvfeksvn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/glzycdxrm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/grtvrazdo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gjjrgkssm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gitylducf.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gkohvvwzi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gccdhcixd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/glhixgefm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/guxqutayp.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/goloxtvse.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gslskgxmx.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gvowuiccw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxwfpufu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gflkuenft.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/grvanfkhu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gqmsklone.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gzzshoshk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gtsjkvuvx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gkdeluoyi.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/ggwmndbid.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/glwyltijb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gwlpwowqp.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gwxounjlf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.epnwcf.com/Article/details/gokunlzfb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.yfazqb.com/Article/details/gbtcrlduk.sHtML

Ruby: s.count("a")
来源：http://wap.bbcook.cn/Article/details/graiikimq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gbzemxmcd.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/ggdhuqjet.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gpxujqzrn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gufgugasu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/grbmafbtg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gskhacuom.sHtML


<!-- 参考信息 -->