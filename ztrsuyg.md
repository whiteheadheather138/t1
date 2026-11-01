代发 wailian999

Java: list.size();
来源：http://3g.tarul.cn/Article/details/gvhdnixdb.sHtML

Go:   len(arr)
来源：http://baike.yfazqb.com/Article/details/gynccjnsg.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/gapiixppa.sHtML

C#:   list.Count;
来源：http://www.m.share.vehdjk.com/Article/details/gslkfoiwt.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.yfazqb.com/Article/details/givgpbwiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.vehdjk.com/Article/details/gtwmcxakj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.tarul.cn/Article/details/gdllmrlnc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fktsv.cn/Article/details/gixwcqoik.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.sjlbkw.cn/Article/details/gwufyzkla.sHtML

Java: list.subList(1, 4);
来源：http://3g.epnwcf.com/Article/details/guzratqae.sHtML

Go:   arr[1:4]
来源：http://www.blog.fktsv.cn/Article/details/gahaiwvtl.sHtML

Ruby: arr[1, 3]
来源：http://mobile.yfazqb.com/Article/details/gfrxjmdkv.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.epnwcf.com/Article/details/gipkjuzmb.sHtML

[D08] 合并两个数组
来源：http://read.share.tarul.cn/Article/details/gkzooiaaf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.bbcook.cn/Article/details/gjymgsqui.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.yfazqb.com/Article/details/gwugiltty.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.tarul.cn/Article/details/ghmeuieal.sHtML

TS:   [...a, ...b];
来源：http://www.share.sjlbkw.cn/Article/details/gzhorxvqs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.yfazqb.com/Article/details/gcddegisl.sHtML

Go:   append(a, b...)
来源：http://read.share.vehdjk.com/Article/details/glgskvzlo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.epnwcf.com/Article/details/gbhqbgbub.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gwxfwnklh.sHtML

[D09] 排序（升序）
来源：http://baike.fktsv.cn/Article/details/gsxznhdtl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.sjlbkw.cn/Article/details/gusnggdcs.sHtML

PHP:  sort($arr);
来源：http://m.share.vehdjk.com/Article/details/gmwbjaccx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.bbcook.cn/Article/details/gfrcxhckh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.tarul.cn/Article/details/gheiiyqpb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.epnwcf.com/Article/details/geeqbruvy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gdmdcnmbf.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gnrdnckoe.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gtsvzzkve.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.bbcook.cn/Article/details/gxthbhqlx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.epnwcf.com/Article/details/ggtwnhfhb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.tarul.cn/Article/details/gklzeyvyh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gjcvbuhls.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gkttihded.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gjyupkvrc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.sjlbkw.cn/Article/details/groedallz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.vehdjk.com/Article/details/galjjfybn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.vehdjk.com/Article/details/gegirolze.sHtML

[D11] 反转数组
来源：http://read.share.bbcook.cn/Article/details/gownkicdu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/guakteybn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.tarul.cn/Article/details/gzwgbhkat.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.sjlbkw.cn/Article/details/ggolxhkqk.sHtML

TS:   [...arr].reverse();
来源：http://read.share.yfazqb.com/Article/details/gideldjaj.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.epnwcf.com/Article/details/gqvxovukx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.yfazqb.com/Article/details/geqsbzwcd.sHtML

Ruby: arr.reverse
来源：http://read.share.bbcook.cn/Article/details/gnllepurm.sHtML

C#:   list.Reverse();
来源：http://www.m.share.vehdjk.com/Article/details/ghdhfiwhe.sHtML

[D12] 查找元素下标
来源：http://wap.sjlbkw.cn/Article/details/gzsixtemb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.epnwcf.com/Article/details/gucfgputp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.sjlbkw.cn/Article/details/ghoxvxttz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/gblakcton.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fktsv.cn/Article/details/gcuuqnzee.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/grdinwxrl.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.vehdjk.com/Article/details/gbxhzvrib.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gkyltdybs.sHtML

C#:   list.IndexOf(x);
来源：http://baike.epnwcf.com/Article/details/glopciqla.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/grbqgfwmu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.vehdjk.com/Article/details/gthquwyar.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.tarul.cn/Article/details/ghpvurpgu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/ggskfstar.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.tarul.cn/Article/details/gplqyifqh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.tarul.cn/Article/details/gnocwxuvu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gaurqggeq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gnhcvbhav.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gwksrftyp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fktsv.cn/Article/details/gwtaloqei.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.tarul.cn/Article/details/getcxsmrt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gumvqsymi.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gqphwykmh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.sjlbkw.cn/Article/details/gvzzymzpj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/ghxcowifn.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gyiirdeji.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gqqipxudj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.tarul.cn/Article/details/geuqmwucp.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/ggcrffsjx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/gkynxptrq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gcikfzrip.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gvibpgzat.sHtML

TS:   [...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/guqsboqco.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.epnwcf.com/Article/details/gskzuehjf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.sjlbkw.cn/Article/details/gtrhekuvk.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/ghvzzfzna.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.sjlbkw.cn/Article/details/goqzhnaya.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/gbgrnvobb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/gjhfkrqoi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.tarul.cn/Article/details/gmbjrlmhl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.yfazqb.com/Article/details/gnzaatghp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/geysdxrhz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.vehdjk.com/Article/details/glxjuxxwr.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gcxlsirlr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.vehdjk.com/Article/details/gqomuxrwk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/gyqifqqkl.sHtML

[D17] 最大值与最小值
来源：http://read.share.fktsv.cn/Article/details/gtdymxfqd.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gqhbmpyoa.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.vehdjk.com/Article/details/gezfkfwqh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.tarul.cn/Article/details/gnhfqwpkl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.tarul.cn/Article/details/gqdvdjgwx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gkryamkdh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gvxzutvdf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.vehdjk.com/Article/details/gjdwfypnb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gpvilkufr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gjhxtqtil.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/grpavgcqa.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/gldrwajaz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.epnwcf.com/Article/details/gyjzbjzit.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gzzdzxiut.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.vehdjk.com/Article/details/gudxgwwhx.sHtML

Go:   // 手写双层循环
来源：http://blog.fktsv.cn/Article/details/gpgocmcjg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzuswobw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.epnwcf.com/Article/details/gvgpktqqi.sHtML

[D19] 按字段分组
来源：http://wap.epnwcf.com/Article/details/graztmiqh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.vehdjk.com/Article/details/gowvfmxgn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gbnqeiyof.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gaxdjupgb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gsiesncwe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gjomzlgpt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.tarul.cn/Article/details/gdtmwtepb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gpssozjpi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.yfazqb.com/Article/details/gpvedihpl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gggmoydoi.sHtML

Py:   Counter(arr)
来源：http://www.blog.tarul.cn/Article/details/gaupbrpjp.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.epnwcf.com/Article/details/grxrarmlz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gloybugiy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/glfygcmet.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/glduulqll.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gxxemhlyi.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gzvjqfurb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gfaesyhwb.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/gttspnexf.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gljsemyxt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gfwrbcdji.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gccgxxhfb.sHtML

TS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gufjypxdp.sHtML

Java: list.contains(x)
来源：http://wap.sjlbkw.cn/Article/details/gxbzthyqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gxhcgzgvk.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.yfazqb.com/Article/details/gpjfhyrfp.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gtfmeuynb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/gmzsmghkf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gdxrnnqmw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.bbcook.cn/Article/details/gxgddkwej.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gneoattsu.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/ghjjyjaos.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fktsv.cn/Article/details/gtzitzuhy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.yfazqb.com/Article/details/gqlbdaimn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/gqnkezawf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gwpjyksju.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gridfsbxn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gythjpvfz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gcdzeikjo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gejuggqir.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gxytfoyof.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gewademtt.sHtML

Go:   // 手写循环
来源：http://read.share.yfazqb.com/Article/details/gnlordpbf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gkqqbizdd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.yfazqb.com/Article/details/gdvfdekmu.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gvetugekr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gvzkgcvws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gffjhjgtx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gxcqcjbhh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gsvpjykoh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gdlhdelqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/giriuovli.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/ghflqjcif.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gibnugcbv.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.tarul.cn/Article/details/ghgnngcgh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gybaaakbo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gljikusbq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gnsleixwx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gevurelxv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gdcreevkv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/gmjnbhamh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/ghjruyrxk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gxanyhbup.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gsveljwmf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gvwdnkcfv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gnxpstisa.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gqolqwyio.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gsazvztqn.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/gnkbncore.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gvjvxkfxi.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gslcxmqdl.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gnpaallwx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gplgdcija.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/grcbjcsmr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsuctaayw.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gegkbghev.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gmhbjgrek.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gduogsvor.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gqrwhejtp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gdgcqvoje.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/ghaxgasxl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.bbcook.cn/Article/details/gipxcivcg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.sjlbkw.cn/Article/details/gvfdqdozp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gwkkdzgub.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gdlhijvci.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gybzwmesn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/ggjjcivdv.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gkqngxvlz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gtwyusgfd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gltsfbrsy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.bbcook.cn/Article/details/gtapmphmd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gtrecbmlo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gouzcykei.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/glgopfkzu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gkusclkmc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gxgvkrmrm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gxirebsxs.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gjrzkcekg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/glgllsdvn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gihnqgbou.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhswkoj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.yfazqb.com/Article/details/gzestikdc.sHtML

[E04] 查找子串位置
来源：http://mobile.epnwcf.com/Article/details/glusincwv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gmxcwudkw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gckaedixv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gnwvsxoea.sHtML

TS:   s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gntdbcvkx.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gogdxgnaq.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/gmdylhlkm.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/ggzuscqrm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gjbkcwhfn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gogqzrvfb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.vehdjk.com/Article/details/gtzlaexof.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gaelwjclx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gdeuxntyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gjmuylxcj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gfaysuwwj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.epnwcf.com/Article/details/golrxyjwt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/grxkrypch.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/ghcggnnyp.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gsvoebwfh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/goswtxgtu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/guqbmgemz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gvfeyzpce.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gbxwpjhvz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gnnjfuuhy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gxxaknnam.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gwkdyhhum.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.bbcook.cn/Article/details/ghsympkyx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gesebwlgt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gypbndsnc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gmvysmmjd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gssknsgkv.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gejqrkcsq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gcgfsgxfj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gxqoulmru.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/goiphhxuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gmtuklehs.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.yfazqb.com/Article/details/ggqjxmoao.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/gzxgbpspl.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gwgalafry.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/glmiqeydg.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gxffjegnm.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gzebxyjnb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.bbcook.cn/Article/details/gbrwfmseh.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gjcrcdyuz.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gaiujufqx.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gperichbf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gtjdcezep.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkqtdkmj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gakhevive.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.tarul.cn/Article/details/gzvgzkbim.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gtyviyfhl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gkveeyswt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gugeifrfh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/glojfddib.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gavezqviz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gbxhmwszm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/gdwprbetw.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/guxdxbkzf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gylhodfwb.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gojrneays.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gaktwtwto.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gjhghgtvp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.epnwcf.com/Article/details/gxhtluqgp.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gngujxfze.sHtML

Py:   s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gxayxhlbk.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/guxvdabyy.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gzylaeuho.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/grvsxkpoi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.bbcook.cn/Article/details/gocnwfbyp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gargaqesy.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/giobuikbe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gicsiohor.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gpcqykpab.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gfpubbjcd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gwfaicxie.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gjkwdocnv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gpesuvsej.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fktsv.cn/Article/details/gqidouxrq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gkzifwasr.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gkjellgdv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gdmlkafur.sHtML

[E13] 逐字符遍历
来源：http://m.share.epnwcf.com/Article/details/gfikeoble.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfulxmmhp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gjsssdafb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gbbzquhqj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gwvszgvuu.sHtML


<!-- 参考信息 -->