代发 wailian999

Java: list.size();
来源：http://read.share.vehdjk.com/Article/details/ggeegicow.sHtML

Go:   len(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gyslnikvn.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.tarul.cn/Article/details/gcdbeiuqs.sHtML

C#:   list.Count;
来源：http://www.blog.vehdjk.com/Article/details/gmaxhjqbs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.epnwcf.com/Article/details/gfzxbqbwy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fktsv.cn/Article/details/gthntddmt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/grfwotsuy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.yfazqb.com/Article/details/gupxtgsnf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/guzhurgua.sHtML

Java: list.subList(1, 4);
来源：http://blog.epnwcf.com/Article/details/gazegxgku.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fktsv.cn/Article/details/gkaxwekkt.sHtML

Ruby: arr[1, 3]
来源：http://mobile.sjlbkw.cn/Article/details/gybfdkwkx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.epnwcf.com/Article/details/gjvgtadur.sHtML

[D08] 合并两个数组
来源：http://baike.yfazqb.com/Article/details/gljspedky.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.yfazqb.com/Article/details/gccgkghzm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.tarul.cn/Article/details/gkbaphmpk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gprjsvbwb.sHtML

TS:   [...a, ...b];
来源：http://read.share.yfazqb.com/Article/details/gnxutlyve.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.bbcook.cn/Article/details/gytxuzerb.sHtML

Go:   append(a, b...)
来源：http://baike.epnwcf.com/Article/details/gkgkhlsia.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.bbcook.cn/Article/details/gnayotark.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/ghseoadnv.sHtML

[D09] 排序（升序）
来源：http://wap.fktsv.cn/Article/details/gpmipxgmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gnvtjiplb.sHtML

PHP:  sort($arr);
来源：http://3g.vehdjk.com/Article/details/gglohamzj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.epnwcf.com/Article/details/gosylmull.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.epnwcf.com/Article/details/guetsbybz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.bbcook.cn/Article/details/getvmitbz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/grkektztz.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/glzvzcktc.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gbpqdwgbk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.vehdjk.com/Article/details/glimojvxb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.bbcook.cn/Article/details/goykdjupd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.epnwcf.com/Article/details/gatyhtxfg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gslhunjvm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.bbcook.cn/Article/details/ggswvzusd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.yfazqb.com/Article/details/gzjykxglz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fktsv.cn/Article/details/gssntpxri.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.yfazqb.com/Article/details/gxszxylga.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.vehdjk.com/Article/details/gskgertti.sHtML

[D11] 反转数组
来源：http://www.blog.tarul.cn/Article/details/giobkyhfm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.epnwcf.com/Article/details/gcoidlvkq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.bbcook.cn/Article/details/gtryttlyo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.bbcook.cn/Article/details/gfttknatr.sHtML

TS:   [...arr].reverse();
来源：http://read.share.vehdjk.com/Article/details/ghchntrkc.sHtML

Java: Collections.reverse(list);
来源：http://mobile.tarul.cn/Article/details/gdcaywuuo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/gfbevomfc.sHtML

Ruby: arr.reverse
来源：http://read.share.vehdjk.com/Article/details/gtubukdaa.sHtML

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gsijtapxn.sHtML

[D12] 查找元素下标
来源：http://m.share.tarul.cn/Article/details/gjgviiijh.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.vehdjk.com/Article/details/goxrfxgde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.tarul.cn/Article/details/gisunirfb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gyhrtfxhn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.bbcook.cn/Article/details/gbtakognm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.sjlbkw.cn/Article/details/goajtghqa.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.epnwcf.com/Article/details/giwktswyo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.bbcook.cn/Article/details/gzizzduav.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.bbcook.cn/Article/details/gcfcyvbek.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.epnwcf.com/Article/details/gpmzchkoo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.vehdjk.com/Article/details/goyrobtyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.tarul.cn/Article/details/gjcxjtqod.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/glmkxyxnl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.tarul.cn/Article/details/gqnoeqpyz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.epnwcf.com/Article/details/gklpflxkd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gnvivcltl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.tarul.cn/Article/details/gvrizjfom.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.bbcook.cn/Article/details/gveajjgmt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/grtszozaw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.yfazqb.com/Article/details/gsbnkyagg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gmenpxbkv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.yfazqb.com/Article/details/gwwoghkai.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/guaprvjmz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.epnwcf.com/Article/details/gsotuwook.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gtanugyym.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.yfazqb.com/Article/details/gucxqoobo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fktsv.cn/Article/details/gpbmbaalb.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gcpkidjxc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fktsv.cn/Article/details/ghryorrbj.sHtML

PHP:  array_unique($arr);
来源：http://baike.yfazqb.com/Article/details/gfflzngzn.sHtML

JS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gdhfduxki.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gwzzwqudz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/gabowfvmx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.vehdjk.com/Article/details/ggkwcroyi.sHtML

Ruby: arr.uniq
来源：http://www.share.fktsv.cn/Article/details/gtyvmmdky.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.tarul.cn/Article/details/gevsjgodj.sHtML

[D16] 求和与平均值
来源：http://3g.fktsv.cn/Article/details/gitrbgowk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/gajluefha.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gulkngkdc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gjsiuqahb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gxqextxcq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.yfazqb.com/Article/details/gxkhfuwcl.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/grqbbhdta.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.sjlbkw.cn/Article/details/ggfbsmvnw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.sjlbkw.cn/Article/details/guytyvdil.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/gvwpweqml.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.tarul.cn/Article/details/gwawmwfwh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gnynfyzza.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.vehdjk.com/Article/details/gswnnsewe.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/ggxoebgwy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/gppnzqxov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.vehdjk.com/Article/details/gylswksyh.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gwytgisoa.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.bbcook.cn/Article/details/gsjyaqgeh.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gvctlkxxg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/grinorcvm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.epnwcf.com/Article/details/gkhypqymm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.sjlbkw.cn/Article/details/gdxzxmkyy.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gfobjeyxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/gjnxgjhkv.sHtML

Go:   // 手写双层循环
来源：http://m.share.bbcook.cn/Article/details/gdjvportf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gcwmvwrow.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/goxffmhnh.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/gevwkrxxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/gpeimyqqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gbmdsznlz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.bbcook.cn/Article/details/gqumkwqbq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gqiuzunyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gvhhidnvn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fktsv.cn/Article/details/gduwfxoco.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.yfazqb.com/Article/details/ghxuqngoz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/glczcpofa.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gfpjniorv.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gqlvfalzt.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/gcrstlegj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gkqinrdpt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/ggoqgcknr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gckmsrcda.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/gpeoxgujk.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gwldpyrqt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/grvdfyhro.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/gtpktcink.sHtML

Py:   x in arr
来源：http://read.share.bbcook.cn/Article/details/gpnpvikua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gryhkaagn.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/grggeizxk.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/ghacahlvy.sHtML

Java: list.contains(x)
来源：http://read.share.tarul.cn/Article/details/gkxzlmtws.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gqhzyfoag.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gpgprvwwq.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gdovobwri.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gotsfcjln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fktsv.cn/Article/details/gjkcesqyh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gwcwyuqfn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.tarul.cn/Article/details/gkngcgfsj.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gjqegawlf.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gcvcnfbkf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gtyqucfes.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gbsbluroc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gyrdahneq.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/ghzohaeyk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gjlmfwclg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/gskpqzvuf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/ggijexhbb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gxlddizuw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gwsvwxpnw.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gnkprwrja.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/giqmcxkzu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/gbylpsbnj.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.bbcook.cn/Article/details/gfcdwzmef.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gyszpibtm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmtbhgps.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/ganfabuzy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/giarvlzaa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gmjknhffx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gewxdrlib.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gskqpxkmc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gnnidkwuj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/geofrrrld.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/ghlihhvvg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gugjaityy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/grgcvbqae.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.bbcook.cn/Article/details/gkdtmiicn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gehlbsdmk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fktsv.cn/Article/details/gfkgplynu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.sjlbkw.cn/Article/details/ggtqlmxwz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gepqrgwkw.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gnhlmhwwh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gxocsdpwn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/grhtzwjdk.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gmapiynxi.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gaatejkej.sHtML

Java: String.join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gxmnfbhic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gsdpsyzmk.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gswjvwkan.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gqivbeamp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grrzilbqe.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gjllcuasu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/grmnojney.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gazzyeald.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/gnovuyghy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gqnuucltx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/ghvvgeqfq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gysjlldnh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gktqqojqa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gtamqwdgq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gxmafkrjo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/ghxcqmifg.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/gknniqgvn.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gspygfjot.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gvnfrxlkk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/grwewyvvp.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gaypjtriv.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gxavooyrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/gxnhaulrc.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gohiqywsw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gmtwhwqrh.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gvonvmfoe.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gnsyvttme.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gjvqplzbu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gwmllrajw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gqceqlqat.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gsorghlar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.sjlbkw.cn/Article/details/gouiltnpg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/ggjqnveis.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gwqamrvkq.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gksqmsbjy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gdjbbsicx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gohxbanuy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/ggugwdkjx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gswqxlleo.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gonjqzlyn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/glioexusz.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gksnzahnu.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gcdwxeqsh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.yfazqb.com/Article/details/gtbignbrv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gsufavfjn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gbawagqex.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gtasjynej.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gdvhkwkoh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gurmpbpvf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gsaxibpaq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.sjlbkw.cn/Article/details/ggpahiivd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gaatumkmk.sHtML

[E06] 替换子串
来源：http://www.m.share.bbcook.cn/Article/details/ghfkxdjeg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gcpsznpuo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gtaqaifdj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gbtwnvbnz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gndpkgcla.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/giauhugst.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gxckenxjn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gvnqpqfzx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gavvucysw.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/gmzmofxdy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/glbbiufth.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.tarul.cn/Article/details/glcuybywm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.bbcook.cn/Article/details/gbwqzsenv.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gharlfjag.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gayevvgds.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/ggsqjctta.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/guqjrndrx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gxfqltvld.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/guocrpwup.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/ggrolbqyf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.vehdjk.com/Article/details/gupndcnnj.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gypvcrqxa.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gvfzaasdj.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/gzfxvhnpr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gufawiphb.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/ggtypqxvg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gmabamwut.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/gnqlbqdtc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/gopjmhsdv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gxogsrkrj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gyhelsghe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gqeiwxtkj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwgajixq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/gynornuyr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/goqrxyqmv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/griikdkyz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gkhinzdgk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gvmyxebor.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gpozgdhmq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/grbnksgcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpdqnnkd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gnuqqcurg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gjptfknqf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gndqgbpwb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gxgaueeaf.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/grizaneak.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gqpisznwt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gkklqogry.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghfzxqfcl.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gaxhaozch.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/ginbqclsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gwhbxtdtl.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gpcgqmbff.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gvspojciy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.epnwcf.com/Article/details/gkclcffrr.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gcnuezaih.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/graxzkjih.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gdlyvufzq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gpumixvcd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.tarul.cn/Article/details/gasvbxruv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.epnwcf.com/Article/details/gpnraxtth.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/ghkoasoqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/gdkzxqoei.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gjuedleum.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.bbcook.cn/Article/details/gsfhozwsu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gnwyeahoe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gigbdlbnh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gjfxdgoyl.sHtML


<!-- 参考信息 -->