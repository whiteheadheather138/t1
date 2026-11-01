代发 wailian999

Py:   len(arr)
来源：http://read.share.bbcook.cn/Article/details/grtoykhbj.sHtML

PHP:  count($arr);
来源：http://m.share.fktsv.cn/Article/details/gkovtvzzm.sHtML

JS:   arr.length
来源：http://www.blog.sjlbkw.cn/Article/details/giaaktlup.sHtML

TS:   arr.length
来源：http://read.share.epnwcf.com/Article/details/gzrsaicqr.sHtML

Java: list.size();
来源：http://baike.tarul.cn/Article/details/gvrxohppw.sHtML

Go:   len(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gasgwrugc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.vehdjk.com/Article/details/gftixvufh.sHtML

C#:   list.Count;
来源：http://mobile.epnwcf.com/Article/details/gdvfgmwal.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.bbcook.cn/Article/details/ghvazuiou.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.yfazqb.com/Article/details/ghxvvwfwo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gzvezpqib.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gvgdtkwsn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.epnwcf.com/Article/details/gezbikkja.sHtML

Java: list.subList(1, 4);
来源：http://mobile.tarul.cn/Article/details/gkrkcybym.sHtML

Go:   arr[1:4]
来源：http://baike.sjlbkw.cn/Article/details/gmtpmfdgr.sHtML

Ruby: arr[1, 3]
来源：http://3g.yfazqb.com/Article/details/gtfqilcgi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.epnwcf.com/Article/details/gymjwucdn.sHtML

[D08] 合并两个数组
来源：http://3g.fktsv.cn/Article/details/gnmajkmlp.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fktsv.cn/Article/details/gwjflrjcx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gqbakjdbr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.bbcook.cn/Article/details/gitgdqfgb.sHtML

TS:   [...a, ...b];
来源：http://baike.bbcook.cn/Article/details/ghqnaujbj.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.vehdjk.com/Article/details/gjpmlsgun.sHtML

Go:   append(a, b...)
来源：http://www.blog.tarul.cn/Article/details/gfajjygld.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.epnwcf.com/Article/details/gkgcygbss.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.tarul.cn/Article/details/grbfnhhuy.sHtML

[D09] 排序（升序）
来源：http://baike.vehdjk.com/Article/details/gpkrivbwk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/gplpixrev.sHtML

PHP:  sort($arr);
来源：http://3g.tarul.cn/Article/details/gszrfmbnp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.bbcook.cn/Article/details/gyzrtbjau.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.vehdjk.com/Article/details/gscgseuzl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.yfazqb.com/Article/details/gvmipxglm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gfyscvltv.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/grvnovtcb.sHtML

C#:   list.Sort();
来源：http://wap.epnwcf.com/Article/details/gkiaxykij.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fktsv.cn/Article/details/gsyiiooke.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.vehdjk.com/Article/details/gtfbobmus.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gpbovekaj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fktsv.cn/Article/details/getvvansa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.sjlbkw.cn/Article/details/gjfndqzik.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.tarul.cn/Article/details/gbbayifba.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.bbcook.cn/Article/details/gsrmqmkxr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/gzxomnrda.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fktsv.cn/Article/details/glgjidvld.sHtML

[D11] 反转数组
来源：http://3g.sjlbkw.cn/Article/details/gmcxunkqa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.tarul.cn/Article/details/guglntzcz.sHtML

PHP:  array_reverse($arr);
来源：http://baike.tarul.cn/Article/details/gtduznyew.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.tarul.cn/Article/details/gafzadlgs.sHtML

TS:   [...arr].reverse();
来源：http://blog.tarul.cn/Article/details/gtodoygiq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.sjlbkw.cn/Article/details/gilvmxzra.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.tarul.cn/Article/details/glxbzbfxb.sHtML

Ruby: arr.reverse
来源：http://wap.vehdjk.com/Article/details/gblbmhuvw.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gfhtxxjgs.sHtML

[D12] 查找元素下标
来源：http://m.share.vehdjk.com/Article/details/gvabcjxgj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.vehdjk.com/Article/details/gjpogbwdn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.vehdjk.com/Article/details/gjrlmpidq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.tarul.cn/Article/details/gbjxbeaww.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.sjlbkw.cn/Article/details/gqpsjtfnu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.epnwcf.com/Article/details/gjcomjxyi.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.epnwcf.com/Article/details/gncghwmiz.sHtML

Ruby: arr.index(x)
来源：http://blog.yfazqb.com/Article/details/gdorbyemh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fktsv.cn/Article/details/gwwttdrpg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gtplqtrhr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gunhqxsoz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.sjlbkw.cn/Article/details/grabehpuk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/geibazvmg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gnqnfazua.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.bbcook.cn/Article/details/goipvlqkn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gsygjjuxq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmuzzcch.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gavltxbjd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.tarul.cn/Article/details/gqfuiyuxz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.bbcook.cn/Article/details/guqxanijo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.tarul.cn/Article/details/gegyptwcp.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.yfazqb.com/Article/details/gzihgphxr.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.vehdjk.com/Article/details/gemggijxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.vehdjk.com/Article/details/gvfnxbtaf.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gfevyoydg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gmpxnxiqg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gzvyqluun.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gayfjnftr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/glszwgfuf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.yfazqb.com/Article/details/ggewksrkt.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gqqnojmuy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/gzgyqdyzo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gcjtuaqxt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fktsv.cn/Article/details/gdtdzljex.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/gvyixnyjw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.tarul.cn/Article/details/ghjiorlre.sHtML

[D16] 求和与平均值
来源：http://mobile.tarul.cn/Article/details/gvdxwcwrd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/ghdnqoidt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/gsmkxwqfv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/ggtyacaij.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gjifiisjc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gtmuupzka.sHtML

Go:   // 手写循环累加
来源：http://www.share.fktsv.cn/Article/details/gogqdbifw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gokhjhsrc.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gmkkxzyek.sHtML

[D17] 最大值与最小值
来源：http://www.blog.epnwcf.com/Article/details/gjmkkkzlh.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fktsv.cn/Article/details/ggrayyflr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gdrnivhyf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gxshaedns.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gyfqizktw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/ggyxavoxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.epnwcf.com/Article/details/gbnvycuwo.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.tarul.cn/Article/details/gzfrrhtpo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gpathowcw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.vehdjk.com/Article/details/glqkinkvo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gbkititca.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.bbcook.cn/Article/details/gxbpwhnqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.epnwcf.com/Article/details/gxqiptxyh.sHtML

TS:   nested.flat();
来源：http://www.blog.yfazqb.com/Article/details/gmmhlfkxx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gquzaydpq.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/geesaztdc.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/geyhnrcjb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gkqtludfu.sHtML

[D19] 按字段分组
来源：http://3g.fktsv.cn/Article/details/gzlpcsvww.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.bbcook.cn/Article/details/glelzbjgs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/giwwndcrs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/ghfapdmdr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gixeibnlb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gylkfqqjg.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/grxceotng.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.epnwcf.com/Article/details/gcttylljv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gxxaadifv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gkqmfqwue.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gurresmpl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gojvihapt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/ghlfmhrju.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gszsixarv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gmcpktasz.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gysrzeapn.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/goqoxlcdj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.sjlbkw.cn/Article/details/gzmadhdpx.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gmnpzuzpt.sHtML

Py:   x in arr
来源：http://www.m.share.tarul.cn/Article/details/ggfjxcmnr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gyynnwabm.sHtML

JS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gywtdykcp.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gkpcnisre.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/geklayqax.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/goqagbvas.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gorsmwspl.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gxtljrgut.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gfdskkxmv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gxrcyyycu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gtlfcchjn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gjhljxdeb.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gevqvpoac.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gsffdryri.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gnghaeopv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gpmlvutia.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gvqvsjakr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gxnfiwjac.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gkfrwpryf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gswxdrxeq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gkkneakeq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gcvgyxffx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gylcuwyax.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gofknkpog.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/guanfnqam.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.epnwcf.com/Article/details/glidewzfp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.sjlbkw.cn/Article/details/gaokmmlsx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gmxvhgpat.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gkccddjby.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gujkacmbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gekhmhkty.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gnxgfeyft.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gyvxyknid.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gkyrudpaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fktsv.cn/Article/details/gcdzchzag.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gwiythktz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gyqemwnod.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gsvitccvb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/ggiaundsl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/ggeezeivl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gbuhiqzwm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/ggmeiwkso.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/gxhcperwc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/ghlpiwltz.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/gdifqkgmc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/grzjsqaci.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.yfazqb.com/Article/details/gqhjkriws.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyowijmfl.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/ggjnukojp.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/gaefvqcte.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gzylwfmfi.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gxpajtdjg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gofnlchkc.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grlcwazgw.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/glwhrndnk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkkogaadj.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gircjrily.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gwkwegdhu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.sjlbkw.cn/Article/details/gjrixfybh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/guwnxecjg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gagkdqsqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.tarul.cn/Article/details/gxetvrphj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/grtqzmeoz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gpzbydnld.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gjqlsdjdi.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gkhgyfhim.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gtyssymqi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.epnwcf.com/Article/details/glzwwbgdy.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/ganrryqld.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/geqhbqwfk.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/ghebumlgo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/gnrfmkmvz.sHtML

Ruby: "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/gtuqugxqg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/gkywbjnsy.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/gdrxvbrkw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gudlgwyfw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gxjjzjrty.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gbzloobuo.sHtML

TS:   s.slice(1, 4)
来源：http://wap.epnwcf.com/Article/details/ghulfvgpx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gxftzorro.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gyhgrvhzc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/gjseoswwi.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gppxidxbg.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gusacbntn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gsykztqjg.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gkvlneqte.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/grsyjdxid.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gxrvfhmwl.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/glzpdecsp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gufuczojz.sHtML

Ruby: s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gvrxjjyxf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gqdbjhxqg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gtvqiemnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/gaysoeqcv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gianilqzk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gxixenvqi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gcvmhdmcx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gvqjpqian.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gdklkcrzx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.tarul.cn/Article/details/gszbxmpoh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gbxejzkkd.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gibfmormy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gkwbdjdpi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/gefjmrlkr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gzuzkhdts.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/ganokacqq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gkpcxlcub.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gvikavply.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gjgmieipn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gfmemmgem.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gchcbrjln.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/ggthvcmkb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gkflqddgf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/grilsoehv.sHtML

TS:   s.split(",")
来源：http://www.share.epnwcf.com/Article/details/gswolfnyh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gsrhwentl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gqzkghman.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/ghjubpjdp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gfncmlxty.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.epnwcf.com/Article/details/gifscmitp.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gprfcjexj.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gitilcopr.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gkdqgxkzr.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/getdwwbqe.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gcvmfumvi.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gdnlostaz.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gixtfslqf.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gocdghttk.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gnsividxt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gpnlwnemp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/gkdhzuoua.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gitrcdmju.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gkmfugmhi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.epnwcf.com/Article/details/gghfmuvof.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/gaznpdnhm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/grzctlmew.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/gtedupyyc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gpyuvvgth.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/grtanwlid.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gfikerbfu.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gdatlsuzm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gmnjkxeur.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gxkoermym.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gujjhavga.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gnonoxqae.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/grgmikrvd.sHtML

[E11] 反转字符串
来源：http://3g.sjlbkw.cn/Article/details/gsexrfjuu.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/grsbxrjxb.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gepabpmpa.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/goumytxnu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/grthvjntp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gjmbnqbcp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fktsv.cn/Article/details/gaqgekcyk.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/glucphozb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/geeoddefy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.yfazqb.com/Article/details/ganmrrzck.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/gtebyipqr.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.yfazqb.com/Article/details/glperesxn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gvgkjlzfx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gpzaojphv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gnuhzahbl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/geksnlaqr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gnsamaqxu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/giquxgskt.sHtML

[E13] 逐字符遍历
来源：http://baike.tarul.cn/Article/details/guyenoudv.sHtML


<!-- 参考信息 -->