代发 wailian999

Java: list.size();
来源：http://www.m.share.tarul.cn/Article/details/gjodhxuda.sHtML

Go:   len(arr)
来源：http://mobile.yfazqb.com/Article/details/gcrfnisny.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gftjojpea.sHtML

C#:   list.Count;
来源：http://mobile.yfazqb.com/Article/details/gcydjatex.sHtML

[D07] 切片 / 取子数组
来源：http://baike.epnwcf.com/Article/details/glyhbigeo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.sjlbkw.cn/Article/details/gczbhlzxl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.yfazqb.com/Article/details/gqbhtyjyv.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.yfazqb.com/Article/details/grrdfngsl.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.sjlbkw.cn/Article/details/giezzbsnf.sHtML

Java: list.subList(1, 4);
来源：http://3g.sjlbkw.cn/Article/details/ghukohtbz.sHtML

Go:   arr[1:4]
来源：http://3g.fktsv.cn/Article/details/gdmxbpvfc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.bbcook.cn/Article/details/gxnumanyp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.tarul.cn/Article/details/gtibmyolm.sHtML

[D08] 合并两个数组
来源：http://www.share.sjlbkw.cn/Article/details/glytzzwkt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.vehdjk.com/Article/details/gtvxqolaf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.vehdjk.com/Article/details/gsfkfbkfb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.bbcook.cn/Article/details/gvwdasdzm.sHtML

TS:   [...a, ...b];
来源：http://baike.epnwcf.com/Article/details/graqlkewr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.bbcook.cn/Article/details/gdnzhgyzq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.yfazqb.com/Article/details/gncvzvfea.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.epnwcf.com/Article/details/gxljjatpv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.epnwcf.com/Article/details/gjdirpvpe.sHtML

[D09] 排序（升序）
来源：http://read.share.vehdjk.com/Article/details/gxdducvob.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.sjlbkw.cn/Article/details/grtelkkxw.sHtML

PHP:  sort($arr);
来源：http://read.share.bbcook.cn/Article/details/gergjuewr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.epnwcf.com/Article/details/gquuhwmhy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.vehdjk.com/Article/details/gmuwhucch.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.yfazqb.com/Article/details/gnfgmhnnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gtmbbnade.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gixsbsqgq.sHtML

C#:   list.Sort();
来源：http://mobile.vehdjk.com/Article/details/gecrylvbn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.tarul.cn/Article/details/gatgegdfv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fktsv.cn/Article/details/gdulmbzyi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.vehdjk.com/Article/details/gvppuszhk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gugxfljez.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.vehdjk.com/Article/details/gtgjbruxa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gqhztjghn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.yfazqb.com/Article/details/gmzncvrzz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.sjlbkw.cn/Article/details/gczllcbpk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.epnwcf.com/Article/details/gddjyzhgm.sHtML

[D11] 反转数组
来源：http://baike.sjlbkw.cn/Article/details/gcblfnhko.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fktsv.cn/Article/details/gkdjsivjf.sHtML

PHP:  array_reverse($arr);
来源：http://baike.epnwcf.com/Article/details/gtmvrqyvt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fktsv.cn/Article/details/gddxrunso.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.yfazqb.com/Article/details/godzhigat.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gciiimxzq.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gtkhpxsqo.sHtML

Ruby: arr.reverse
来源：http://3g.yfazqb.com/Article/details/gqoyaerac.sHtML

C#:   list.Reverse();
来源：http://wap.bbcook.cn/Article/details/gpetingwt.sHtML

[D12] 查找元素下标
来源：http://read.share.vehdjk.com/Article/details/gcpwsolwc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fktsv.cn/Article/details/gepbmiwta.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.bbcook.cn/Article/details/gwxwjcjae.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.vehdjk.com/Article/details/goffoyvce.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.tarul.cn/Article/details/gslzxenec.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.epnwcf.com/Article/details/gfxujprfs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gfouszwet.sHtML

Ruby: arr.index(x)
来源：http://m.share.sjlbkw.cn/Article/details/gqcraiplo.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gyhbsqlwq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/gutecjnuz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtleuzfh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gvmierafe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.epnwcf.com/Article/details/gdkscnrmc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fktsv.cn/Article/details/gicgfjxwy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gsmjvpyqd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fktsv.cn/Article/details/gvyvesywm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.sjlbkw.cn/Article/details/gmriklmpf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fktsv.cn/Article/details/gyhsbeqeb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.vehdjk.com/Article/details/glvxfvwgr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/geasjxdfs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.vehdjk.com/Article/details/gnkxdowld.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gcafdlyno.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxaavhezf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fktsv.cn/Article/details/gqfqnckdg.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gkepgleyg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.vehdjk.com/Article/details/gfaxxoevt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/ggrdfiodo.sHtML

[D15] 去重
来源：http://m.share.epnwcf.com/Article/details/gkazsbdvm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.yfazqb.com/Article/details/gikmyxmxp.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gxajchlnq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gtcuelkfc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gvuojfwpf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.yfazqb.com/Article/details/gaunqiatu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/gwarmxqvs.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gdvddaidd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fktsv.cn/Article/details/gjewjjonr.sHtML

[D16] 求和与平均值
来源：http://wap.epnwcf.com/Article/details/gtwjjovpb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gfczcfdbm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/ggskojjls.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/geanwkrvi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gpbhgmftj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gssacdvok.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/ggkfpypgu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/grojuvnwx.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/gniurwiba.sHtML

[D17] 最大值与最小值
来源：http://www.share.sjlbkw.cn/Article/details/gxgsgshca.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gnmtxodrf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/gfspcrijg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.vehdjk.com/Article/details/gagbtpbgw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/gadnqgzqz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gxtkqyxis.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/guhdgornu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gncjxhdty.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/gypygqmqz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.epnwcf.com/Article/details/gdxaayodz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.sjlbkw.cn/Article/details/ghldndkeh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/gavvuafnv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gjpkyvfvv.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gwpyhhfnf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gafkrvrlu.sHtML

Go:   // 手写双层循环
来源：http://read.share.fktsv.cn/Article/details/gpxohrbqh.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/gtkhpybgt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.bbcook.cn/Article/details/gbjeblned.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gsrkcyufp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gsjvprlfg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.vehdjk.com/Article/details/ggvffpkbl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.sjlbkw.cn/Article/details/gnyiamwhw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gafauldpm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gmtyhsgqf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gskkdnwrx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.vehdjk.com/Article/details/gismvtgjf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/ggjqfhtsa.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gmvhaeels.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/goavotafu.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fktsv.cn/Article/details/gfhosqsqu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gbtbeottx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gkqypmffe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gfbslqknr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gglrupcze.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gcbqcxpir.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/grdrvvlju.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/grllsfoqg.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gamnwffha.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gwhwtxyxn.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gfiwsssdb.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/guhuwqvxr.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/glyioxrtg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gzjksahbi.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gbplnuvor.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gmpynmvlc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gdniontec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gmgnvhihf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gqiobmauq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.vehdjk.com/Article/details/gqkvsfvqx.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gweheaovr.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/grmgmxpvd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gfolumdft.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gqzqmjagu.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/geiiyqevu.sHtML

[D23] reduce 累积计算
来源：http://baike.epnwcf.com/Article/details/glluhjizu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gzgfylnmu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/grapsvepj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxomyzyii.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/glboszuvb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.tarul.cn/Article/details/gvuadsywd.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gswasrljy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gcjlipuzl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gsdsaisjh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/gmugfbqhp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.tarul.cn/Article/details/gbzbjyjgl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/groxvjzgr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/ggiazsvql.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.vehdjk.com/Article/details/govzvxkxv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gyskhugqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/gnbgfobfu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/glyzramkv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gqkbknony.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gjuhstkfh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gbkpuyqik.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gtwyxipxm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/godlaqbqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gixwotvbv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdmzgyzfo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gqwrstgqy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/guqycvjdr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/gmffxncya.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gvyhlrtty.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/ghvklbcqj.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gugznyvkl.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gkwsywdrv.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/goastlkea.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gbzasgpla.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.epnwcf.com/Article/details/gmigyhpnr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gbcflmjzt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gaxxyldqj.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gnxcujjds.sHtML

E. 字符串处理
来源：http://3g.bbcook.cn/Article/details/gfbsylorw.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gohprgjaq.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gpgangstl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/ghojjnvxy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.epnwcf.com/Article/details/gqmcxvkth.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.yfazqb.com/Article/details/grbjrjulz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gvuimyeez.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gqwqjfrin.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/gchdvfedy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.tarul.cn/Article/details/goewueuks.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gfzyqsbts.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gvaeixisp.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gginhoynv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gakxjpgve.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gcoegssrc.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gkqsrvopb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gexxmoabs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.bbcook.cn/Article/details/gjtfiaqgq.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gniqeefpz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gidjnhjwi.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gossidoqg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gueomixgg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gcntokwnq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gyyknahms.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/guasppzid.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gykurxhmf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gwtxdcmeg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.bbcook.cn/Article/details/gusrjmauy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gqdlbsuya.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/geoxjihhd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.tarul.cn/Article/details/grmznaena.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gtikqsfxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gnhwcqoqp.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gimgtijue.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/grxrdeojh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/genydonqh.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/ghogmfovi.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gjrnrkonx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/gmtvwpjdl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gfinfhzaj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gsewwuhrr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gmdurpvnm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gruvxxktu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gnwcqvuio.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gamofuhef.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gwrcpfeje.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/ghcuosjxv.sHtML

[E06] 替换子串
来源：http://m.share.vehdjk.com/Article/details/gfdglyfqd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gwpsfhytr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.yfazqb.com/Article/details/gyvkhtbyz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gruaswksj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gsbprxhtf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/ggyfbirmw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/googlsnuy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.yfazqb.com/Article/details/gfbdgkhmu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gknfrhqqi.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gnbybxbhe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/glsxdsijn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/gpvoblshm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/ganpnumpl.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gawqwplms.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gktdmzycs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjazsyopv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/glfkcondc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gfhfcuxqe.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gzwpggauy.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gchhyqyhs.sHtML

PHP:  implode(",", $items);
来源：http://wap.tarul.cn/Article/details/gyjaicsxl.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gchugapot.sHtML

TS:   items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gidpyupcm.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/guykjxlch.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/ghdsjembi.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gwdyvuafs.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/ghrgprken.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gsquyexfn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gkygptcrs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/grvbtkxpw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gmnzjqbbb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/gphvcyupm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gmrxhxyuy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gadjdlsic.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gztkpdzsl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/ghrxnxqfz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/ggbavovks.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gecpfsgwk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gngaconhk.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gebhfzrew.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/giatxopyp.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkbzxkcrm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/glorlpcbp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/getkecbqa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gkavrizej.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gihyvrxjb.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gzgnlaaus.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gfpixtwiu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/grdxthkvv.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/ggdmmaewo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gebnljdgj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.tarul.cn/Article/details/ggnjwajnn.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/gjfeovazc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gfealrajt.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gmepjuqjl.sHtML

Py:   s.count("a")
来源：http://3g.bbcook.cn/Article/details/gwfkygrtl.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.bbcook.cn/Article/details/gfwhdgrlc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gumalwfkp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/ggglvvcqr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fktsv.cn/Article/details/gceukyihn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/grtgfasgw.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gcbgifteh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gotaqlbrn.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gexsdbete.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fktsv.cn/Article/details/gntczfekh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.epnwcf.com/Article/details/gebvjibfu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fktsv.cn/Article/details/gdmehbjbq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/goehyhxtb.sHtML


<!-- 参考信息 -->