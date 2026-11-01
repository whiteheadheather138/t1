代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fktsv.cn/Article/details/gilpkecxk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fktsv.cn/Article/details/gvuvweouw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.sjlbkw.cn/Article/details/gupntniqf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.epnwcf.com/Article/details/gunjgpego.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.tarul.cn/Article/details/gwvdgtvud.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.epnwcf.com/Article/details/glgyrvmlw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.tarul.cn/Article/details/gxmlovybv.sHtML

[D06] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gfmaoamxq.sHtML

Py:   len(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gdkjxdgwn.sHtML

PHP:  count($arr);
来源：http://read.share.bbcook.cn/Article/details/ggkirkxoe.sHtML

JS:   arr.length
来源：http://www.blog.bbcook.cn/Article/details/gyjlvghdk.sHtML

TS:   arr.length
来源：http://read.share.fktsv.cn/Article/details/ggiwuyzzv.sHtML

Java: list.size();
来源：http://www.share.sjlbkw.cn/Article/details/gymlbxtfh.sHtML

Go:   len(arr)
来源：http://wap.vehdjk.com/Article/details/gzmoribhv.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fktsv.cn/Article/details/gbmeuhynh.sHtML

C#:   list.Count;
来源：http://www.blog.bbcook.cn/Article/details/gadkbmlly.sHtML

[D07] 切片 / 取子数组
来源：http://3g.sjlbkw.cn/Article/details/grynehbtj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.vehdjk.com/Article/details/gnmvllxgc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvbfsosnu.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.tarul.cn/Article/details/gosvknbkr.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.bbcook.cn/Article/details/glidhnkws.sHtML

Java: list.subList(1, 4);
来源：http://www.share.epnwcf.com/Article/details/gywbmkopz.sHtML

Go:   arr[1:4]
来源：http://www.blog.tarul.cn/Article/details/gweiedtew.sHtML

Ruby: arr[1, 3]
来源：http://m.share.tarul.cn/Article/details/gyteaoaea.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fktsv.cn/Article/details/gzjblhmxy.sHtML

[D08] 合并两个数组
来源：http://www.m.share.yfazqb.com/Article/details/gtrrmfrcg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/ghhtrrpke.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.tarul.cn/Article/details/guddrairo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fktsv.cn/Article/details/gznrhdamn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.epnwcf.com/Article/details/govwcscul.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.tarul.cn/Article/details/gulkmcgab.sHtML

Go:   append(a, b...)
来源：http://www.share.epnwcf.com/Article/details/gmaxegqql.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.bbcook.cn/Article/details/gvfqxyopv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fktsv.cn/Article/details/gkzksasfj.sHtML

[D09] 排序（升序）
来源：http://www.m.share.sjlbkw.cn/Article/details/gaedpzqek.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gzhfcbbjh.sHtML

PHP:  sort($arr);
来源：http://mobile.vehdjk.com/Article/details/gvamszqpz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fktsv.cn/Article/details/gvoqjvugn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fktsv.cn/Article/details/gkrdykmqc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fktsv.cn/Article/details/gtamisftm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/glrkbpoii.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/govsuwrtq.sHtML

C#:   list.Sort();
来源：http://baike.fktsv.cn/Article/details/gldjbkegn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.epnwcf.com/Article/details/gafdyhyik.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.bbcook.cn/Article/details/ggwnphwqw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gpizuacvc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.vehdjk.com/Article/details/gxxwlriny.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.yfazqb.com/Article/details/gjthncsus.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.sjlbkw.cn/Article/details/goadrjqyz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.sjlbkw.cn/Article/details/gfipgtigo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.epnwcf.com/Article/details/grzazydai.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.epnwcf.com/Article/details/gmldkpgnj.sHtML

[D11] 反转数组
来源：http://3g.vehdjk.com/Article/details/gpqkqvefb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/goghnedjy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.tarul.cn/Article/details/gxiienhvv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gxfibgflv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fktsv.cn/Article/details/gibxmwlcp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.epnwcf.com/Article/details/gyeaangrx.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.bbcook.cn/Article/details/goddzgwhl.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gghcwgdik.sHtML

C#:   list.Reverse();
来源：http://www.m.share.epnwcf.com/Article/details/ghwbskere.sHtML

[D12] 查找元素下标
来源：http://www.blog.tarul.cn/Article/details/gtvpfblmd.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gswkqkwoe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.sjlbkw.cn/Article/details/gvpwvmawm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fktsv.cn/Article/details/gxexbmmme.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/gpbafjkfk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.vehdjk.com/Article/details/gbhhhsdoa.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtqhcmvji.sHtML

Ruby: arr.index(x)
来源：http://baike.fktsv.cn/Article/details/gvqnmfdpi.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fktsv.cn/Article/details/gtzhxpfzo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.yfazqb.com/Article/details/gvrwaaqqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gflempvgo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.vehdjk.com/Article/details/gywfvgobr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gppkfqnjo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.bbcook.cn/Article/details/gxgzoldan.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.yfazqb.com/Article/details/gtvrbkccz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.bbcook.cn/Article/details/gsuvzmfzm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.sjlbkw.cn/Article/details/gjobzwzgx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gseydbtwa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fktsv.cn/Article/details/ggqhhfzde.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gzvgdzjmj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.yfazqb.com/Article/details/gqusjgfro.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.yfazqb.com/Article/details/glkuxdarz.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.bbcook.cn/Article/details/guvyphbgd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.tarul.cn/Article/details/gbvqfwtau.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gcvhwyfvj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gemztquan.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.yfazqb.com/Article/details/guvqklmvy.sHtML

[D15] 去重
来源：http://read.share.bbcook.cn/Article/details/gzmsysavt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.bbcook.cn/Article/details/gpetclmug.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.vehdjk.com/Article/details/gzvkgqxiw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gtxjzumbg.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/guvncoljk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gnudtzdgs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gcdcckknx.sHtML

Ruby: arr.uniq
来源：http://3g.tarul.cn/Article/details/gdpvejspk.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fktsv.cn/Article/details/gghfnlbhn.sHtML

[D16] 求和与平均值
来源：http://3g.fktsv.cn/Article/details/gdizbkfwq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.sjlbkw.cn/Article/details/gomrzaidj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gjblaufoc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fktsv.cn/Article/details/gmokzleyw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gnykkvltn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.tarul.cn/Article/details/ggcwsajah.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gpnlcnswe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gmzdxmdgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fktsv.cn/Article/details/gxfuzxowl.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/ggfnqmmjm.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.bbcook.cn/Article/details/gnftjtrlp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gxosnwwja.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.vehdjk.com/Article/details/gyoyeqnpg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gmencwzlv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.bbcook.cn/Article/details/gwgpejbwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fktsv.cn/Article/details/gktgdsavh.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/ghuffazua.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.tarul.cn/Article/details/gxfwjxgbw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gxkcxgiae.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.epnwcf.com/Article/details/gwojbzvsq.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/ghbnwerfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gjdisqwvw.sHtML

TS:   nested.flat();
来源：http://www.share.sjlbkw.cn/Article/details/gedgylyuz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gkuodjedh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gyimlicuu.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/grlhnknfe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.yfazqb.com/Article/details/gurneynbh.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gravaqmra.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.sjlbkw.cn/Article/details/ggzpfkcev.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gsghtlnhc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.tarul.cn/Article/details/gcyakgelu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gzbkjgcpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/gfiinjnig.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/glkmenzil.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.sjlbkw.cn/Article/details/gahrchngn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gifjdbxdw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.vehdjk.com/Article/details/ggyjrhubi.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gfdhlqrnd.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.yfazqb.com/Article/details/gypmdwyzf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/ghrreyztv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gdjacfkxr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/ggpkjzksk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/ghcfukaib.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gsyowbjdl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/gyjdkpfnr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/gauoxduev.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gxvrdccfu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.tarul.cn/Article/details/gqxfktzbz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gwdfpilak.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gaxdojgsi.sHtML

Java: list.contains(x)
来源：http://blog.epnwcf.com/Article/details/gxkumkyzg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gfajtxvfr.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gdezkupax.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/ggkfotwwa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.tarul.cn/Article/details/gxtrhmamn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gwzqdibew.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gzoadxfam.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gazyftrne.sHtML

TS:   [...arr];
来源：http://blog.epnwcf.com/Article/details/gfowlofbk.sHtML

Java: new ArrayList<>(list);
来源：http://baike.tarul.cn/Article/details/gmtcgyqxv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gofqdfjjd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gfinprltx.sHtML

C#:   new List<int>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gutlgupbn.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gircuycfc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/ggjlvdomh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.epnwcf.com/Article/details/gzrrnwyhs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gbxqqjwoq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gxedryygt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gjozdcmkz.sHtML

Go:   // 手写循环
来源：http://read.share.fktsv.cn/Article/details/gykzladaz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.sjlbkw.cn/Article/details/gioycojlq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.bbcook.cn/Article/details/gkrjcwici.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gvnlbcbkf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fktsv.cn/Article/details/gvkwoeewb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gugttlulv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/gieojosyg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gmfbnqcgs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gwmxkualx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/glbvylltv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/gkznemufc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gaodniwls.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/glvtwlzsf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.epnwcf.com/Article/details/gvkvfxltw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/gtirkikeu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gmnjzgfia.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gcqonqwac.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gexbkgjim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gjaxeuqhd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.tarul.cn/Article/details/gdhzwnqbn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gurbycdsh.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/gphcdrkck.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/giwyhmcly.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gygwejnrw.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gscrnjced.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gqjxpfzta.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gypimpibj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gkbnparse.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gaxzyggtw.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/gfsvsisdc.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gapdemylf.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gswdjaxdn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gduzpegzv.sHtML

[E01] 拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gohjkwdbi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.bbcook.cn/Article/details/giluilets.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gksrglooz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gcdgcinxh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gazwqutad.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.sjlbkw.cn/Article/details/gnfzhsclk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gcfvtbacp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gvmqlykas.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/ggyfbipkl.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gmwrawxiw.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/ghlrsmgvn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyiesqhr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gykarsrup.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gshfrfusp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/geucxmmby.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/gwasnomph.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gbufuyyjs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.sjlbkw.cn/Article/details/gawnsavfm.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gwrptfaan.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.bbcook.cn/Article/details/gviemjpoa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gyxpqvyuq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gurqhzerp.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fktsv.cn/Article/details/gqfeqrkxz.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gpmbzgbto.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/grmvqzagn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/genomrnrv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gclrpyhff.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gtwgrlapd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gvazhrhcn.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gouasfbum.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.tarul.cn/Article/details/gypgtfwxr.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gmgnwfpgd.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/ggkpyfqoq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/ghmkpihpw.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gpyfndzsv.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fktsv.cn/Article/details/ghhgzzkss.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gdejswgst.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/giujamard.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gbwferybh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gtrxcwler.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gcejcdqsl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ggxednwjx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.yfazqb.com/Article/details/gcgzxglop.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gewiirgjf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.yfazqb.com/Article/details/grggcioay.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gihdbhwks.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gopdrakyt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gkiokjqqp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gjorcbncf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gtmomjrte.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gbarzwfjx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gxuxhjtgq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gwlcufycg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/glheslmvp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gsvvyzaav.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/glqyaqgaw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gutuyjqmk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/ggurcnvow.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gvnmetwsw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gpqhitrlx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gerianpsd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gikxvgphs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gbzxcetjs.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/glmbqisxn.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gkfihigcm.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gzzipbluv.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gjihgkcsm.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gcupgmyuy.sHtML

Java: String.join(",", items)
来源：http://wap.yfazqb.com/Article/details/gnpslwwsb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/guufqfzgj.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gaaonuert.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gyobrrlwn.sHtML

[E09] 去除所有空白字符
来源：http://wap.fktsv.cn/Article/details/gvogzshio.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/guucbnmad.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gcknwfhsi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gtxhutivj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gjjdxpddm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/geguksjxu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gbxeayowm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.bbcook.cn/Article/details/gkgirgkrq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gdloagxgx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gmvgfmjnz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.tarul.cn/Article/details/gzdcsmghf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gvduoahpv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/goyvuwodz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gywnyrtxm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gahzwgylz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gijnqogfa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gkmntuqfx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.epnwcf.com/Article/details/gbpbzrgbu.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpssgfjfh.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/giincexzs.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gdccfblpy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzxbdyoih.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gvnoacyzm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fktsv.cn/Article/details/gvvxwvony.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gurtzafva.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/ggkythjiq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gigfsjbtz.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/goxxqewjg.sHtML

Py:   s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gygqfhgzb.sHtML


<!-- 参考信息 -->