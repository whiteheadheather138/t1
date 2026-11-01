代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.share.tarul.cn/Article/details/gnmexyxzl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.tarul.cn/Article/details/gpvockwqi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.yfazqb.com/Article/details/gtgxcwlpv.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.vehdjk.com/Article/details/gphmigcvp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.vehdjk.com/Article/details/gxjocqzfu.sHtML

Java: list.subList(1, 4);
来源：http://blog.bbcook.cn/Article/details/gqtmeyagm.sHtML

Go:   arr[1:4]
来源：http://read.share.sjlbkw.cn/Article/details/gurgpldkg.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fktsv.cn/Article/details/gfdaxzyvy.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.sjlbkw.cn/Article/details/guufnlyvs.sHtML

[D08] 合并两个数组
来源：http://www.share.vehdjk.com/Article/details/gakjvnxdo.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fktsv.cn/Article/details/gdnzengsh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.bbcook.cn/Article/details/gfdumhomo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.vehdjk.com/Article/details/gyihhwdma.sHtML

TS:   [...a, ...b];
来源：http://baike.yfazqb.com/Article/details/gcnmwvchq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.epnwcf.com/Article/details/gvwattezc.sHtML

Go:   append(a, b...)
来源：http://3g.sjlbkw.cn/Article/details/gtoteanfm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.vehdjk.com/Article/details/gaclknwgi.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/glajiutfd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.yfazqb.com/Article/details/glfvonvzh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gwyyeirrl.sHtML

PHP:  sort($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggrdsaefv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.tarul.cn/Article/details/gvlslkini.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.tarul.cn/Article/details/gvpifkkra.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fktsv.cn/Article/details/gtteiaazc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gzbftcnju.sHtML

Ruby: arr.sort
来源：http://www.blog.yfazqb.com/Article/details/gqyvsullc.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gxxibqijp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fktsv.cn/Article/details/giieszywu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.bbcook.cn/Article/details/gxrqlzwdi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fktsv.cn/Article/details/gairepyik.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.tarul.cn/Article/details/gmhudflis.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.yfazqb.com/Article/details/gkmljnigt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.sjlbkw.cn/Article/details/ghonutvur.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fktsv.cn/Article/details/gebwdhhdj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.sjlbkw.cn/Article/details/gkmvvohgq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fktsv.cn/Article/details/gbdckkftp.sHtML

[D11] 反转数组
来源：http://read.share.yfazqb.com/Article/details/gvkdndvjh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.sjlbkw.cn/Article/details/glkeiryod.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.tarul.cn/Article/details/gbqdqhkop.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.sjlbkw.cn/Article/details/gyjzvfxxj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.bbcook.cn/Article/details/gkslacncz.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gpionibvz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.bbcook.cn/Article/details/genfkmnnc.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gveodcgns.sHtML

C#:   list.Reverse();
来源：http://m.share.tarul.cn/Article/details/gfvcwgbgo.sHtML

[D12] 查找元素下标
来源：http://wap.vehdjk.com/Article/details/gvuznpkde.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gyugokbtg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.bbcook.cn/Article/details/gvsyajmjl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.sjlbkw.cn/Article/details/gpvswwegk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.tarul.cn/Article/details/gadzqkwlh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.tarul.cn/Article/details/gkqqmzcnb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gevvxentn.sHtML

Ruby: arr.index(x)
来源：http://www.share.sjlbkw.cn/Article/details/gzkdgqfqy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.epnwcf.com/Article/details/gcbuutnoq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fktsv.cn/Article/details/gymznxfcc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.vehdjk.com/Article/details/gxdzvoqni.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/gsmozslla.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/ggphadldp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gnbunslqc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fktsv.cn/Article/details/ghevriozh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.vehdjk.com/Article/details/gtltrxrla.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.vehdjk.com/Article/details/gvjylveih.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fktsv.cn/Article/details/gtunsbrgw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/ggwyqlsay.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gybhqfami.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gkvyvaylm.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.bbcook.cn/Article/details/gnpunpuqu.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.epnwcf.com/Article/details/gpbpsfhfl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.epnwcf.com/Article/details/gnwoxpxrp.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gkazahfuf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.tarul.cn/Article/details/gonvbwahl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.vehdjk.com/Article/details/gfxltyjvo.sHtML

[D15] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gvgpndxjv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcoxbgfzg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gegaxnlao.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/grqncjukd.sHtML

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gwfezjdyl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.tarul.cn/Article/details/gyrldexyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fktsv.cn/Article/details/gzzoquiqc.sHtML

Ruby: arr.uniq
来源：http://mobile.bbcook.cn/Article/details/gxkeudlhd.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.bbcook.cn/Article/details/gjrhqhhcj.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gtknbznyr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fktsv.cn/Article/details/gnaxgmvaz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gjtpnhugm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gqjoxiaxm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/ggutwqxka.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.tarul.cn/Article/details/gtiykkuoq.sHtML

Go:   // 手写循环累加
来源：http://blog.vehdjk.com/Article/details/gvpqlaqlu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.vehdjk.com/Article/details/gnewchcyo.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/guvuksjdm.sHtML

[D17] 最大值与最小值
来源：http://www.share.epnwcf.com/Article/details/gguoqzome.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gfvkfwbas.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/glsdkqrkr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fktsv.cn/Article/details/gepaetmlu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.tarul.cn/Article/details/gnooputxp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.tarul.cn/Article/details/gkcircrvh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gkiadwzdb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gftapruno.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.sjlbkw.cn/Article/details/gwjscaawo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/gxbzdpmvk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/ggcovbvsw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gsmxevrjl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/ghpxzrnwj.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gzliyihoj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/ghurfapkq.sHtML

Go:   // 手写双层循环
来源：http://www.share.bbcook.cn/Article/details/ggdbtrxuc.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gwuuzjdrh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwqtbimoy.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/ggkfkkhek.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.epnwcf.com/Article/details/gwwqwvuzx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.bbcook.cn/Article/details/gjqvywdiq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/gaowazrph.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gnkyokzvp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gylgspard.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fktsv.cn/Article/details/gqskktcak.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/gjfcqiori.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/ghtfhcfij.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/gbflydsyp.sHtML

Py:   Counter(arr)
来源：http://wap.sjlbkw.cn/Article/details/gicsskbzi.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gcjctduqj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.yfazqb.com/Article/details/gqdhibvcj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gwqqnvitx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gkeducsfy.sHtML

Go:   // 手写 map[T]int
来源：http://wap.sjlbkw.cn/Article/details/gayfyrlap.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/gqdimibuk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gfrglvnxn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.bbcook.cn/Article/details/gmqyjuhrt.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gectfxctj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/ggqwbsfny.sHtML

JS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqwyjagms.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gpwvxvmsn.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gpaeqhjgn.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gmmgmaaff.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.yfazqb.com/Article/details/gwkbjaawr.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gblcrxwnp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.bbcook.cn/Article/details/ghxxeatxz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gegqxtudq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gwnfmbmai.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gxiaxrwqa.sHtML

TS:   [...arr];
来源：http://m.share.fktsv.cn/Article/details/gfoucjxwc.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gjymssdqh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.yfazqb.com/Article/details/gtkgjoghw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fktsv.cn/Article/details/giyercpey.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/gsgikmvnu.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmpiodxe.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gfsoblsyw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gxgohuani.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gohccpykl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/gdsgusktg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gieitpfzs.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gptzudbgl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gnxniwubs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gnljyggjg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gutizrdhx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/ghmxszktp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/ggpgbkehz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.yfazqb.com/Article/details/gcvyeucbe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gtzvunjlt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.yfazqb.com/Article/details/gaqxovjqk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/gfewqagiv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxszyfiq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.tarul.cn/Article/details/gvuoymdwt.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gbefplvlp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gwwlikydo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gazyantlm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.sjlbkw.cn/Article/details/gecvfzlmo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gjgyahkgl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gembhimza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gakveoigl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/giocymbqu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gqamzqxwl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/ggtdauyiq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.epnwcf.com/Article/details/gzeskgian.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gpvdgxnqt.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gxeenpzbs.sHtML

TS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gnjdzqref.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gjntpkkmi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gzfmrqbyo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gioqvdtvl.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gfjhegkms.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gznbgpldf.sHtML

E. 字符串处理
来源：http://www.m.share.tarul.cn/Article/details/gzxvoyaub.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gojakhthc.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gfeiwrvyg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gcsmnjqjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fktsv.cn/Article/details/gayfvlbxr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gnskhvdxe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/ghvvguiwe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/grrgqezea.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gvswkqbnq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/grwdkipdc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gtvjtkhww.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gffdryikl.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gnfqmwzlv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gbqenoetg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gmolygrdc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gaykebucj.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/geoytdwxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gbvacoqdz.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/geotjrcjx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gyeonxwbv.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gdvsrjoue.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxbnvhoc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/grffcfrds.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gqnprowxi.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gzruvuirh.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gwcaffzlg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gxnzjkoer.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/giwtqppgc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/gdhhdobzq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.epnwcf.com/Article/details/gwukscgdj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fktsv.cn/Article/details/gzrpcnpxm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gduaphhrd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gxktktvbx.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gjujkcpth.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gjopzhfoa.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gkvwhdktv.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/guvffqfep.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gyfxshdzh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gdsfnkdrd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.tarul.cn/Article/details/gglstkrvb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gyifwbagn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gatumjdrn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gsmfsobpl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/ggthyucud.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gyqgoakzl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/ghbdaxksb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gjeyhobgp.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/gchjzlegw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gwmugdgre.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gvkozyuxc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gfczbuyng.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gajosqzga.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gcrsukypd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gydlejkkm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gwfpkcubz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/glxxlhvdq.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gpionmxgk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gwosfeomt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gorltwubw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.sjlbkw.cn/Article/details/gdrlkaciz.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gbfyjknsq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gazppbfxn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gllxkoisd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/guxsrldoi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/grozqpxzz.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/ggidwwvar.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/grcdvtcby.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gxvqlrvti.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gbpkxomow.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gxhdlnslr.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gbxmifhbk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gfhefcqeb.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gllzbhwjf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gdxkyjhae.sHtML

[E09] 去除所有空白字符
来源：http://baike.sjlbkw.cn/Article/details/ggkxsfmzw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gsvljpwli.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gtqgzhcnu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gqjnjlnix.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/girvzydrs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gibtesodb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gtkftbwpw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gfhvuzicx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gsscslphj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gnlraeopm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gcldkhcdp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.yfazqb.com/Article/details/gghklkdsq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/ggtifywsr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gcmrtapuw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gsfmruqte.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gjlbgjzgm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gpbrgawpk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/geeptnhkc.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/gecctkefm.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gmfmlcadz.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/gzzttlexo.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gqsiiggbp.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gnhivlmnu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcicdlghn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gbtxbyjvh.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/gixlxmjmy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/golbbkdqe.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/gdlskputy.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/golzbdijv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/gfpotjuoq.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gmqkfwtel.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/gvaeoycwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gqyhjqssi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gqsdpoubo.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gubacfpjz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gkeqowmiu.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gukgguzfi.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/garimllba.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/ghjkagosm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxevbkfl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/geptukwcy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gfniyisyy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gkakxbiff.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/grvmvzaob.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/gkwrbylgj.sHtML


<!-- 参考信息 -->