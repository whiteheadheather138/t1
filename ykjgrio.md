代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gcrkizmov.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/giptkvyhz.sHtML

C#:   list.Sort();
来源：http://read.share.sjlbkw.cn/Article/details/gvzzrdtxw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.yfazqb.com/Article/details/gkkjhzimq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtbuhrzs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fktsv.cn/Article/details/gooekhcgr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.sjlbkw.cn/Article/details/gqjsecqoc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fktsv.cn/Article/details/grubmskog.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.tarul.cn/Article/details/gnguogswm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.yfazqb.com/Article/details/gzdppghqf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fktsv.cn/Article/details/grlrlbjbh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.tarul.cn/Article/details/gdncoszmn.sHtML

[D11] 反转数组
来源：http://www.m.share.sjlbkw.cn/Article/details/giwifuylp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.epnwcf.com/Article/details/godemrcel.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.bbcook.cn/Article/details/gxsmlyvez.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.vehdjk.com/Article/details/gjwzvfleo.sHtML

TS:   [...arr].reverse();
来源：http://baike.yfazqb.com/Article/details/gyhlekyxv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.tarul.cn/Article/details/gqznfwojw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/gozkcrxsn.sHtML

Ruby: arr.reverse
来源：http://www.blog.bbcook.cn/Article/details/gmjcnjvaq.sHtML

C#:   list.Reverse();
来源：http://m.share.bbcook.cn/Article/details/gdwzktjkg.sHtML

[D12] 查找元素下标
来源：http://www.share.sjlbkw.cn/Article/details/gqjhqplbt.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.yfazqb.com/Article/details/grseeslou.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.yfazqb.com/Article/details/gmxkcdvbc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkcxugsf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fktsv.cn/Article/details/gnaijspxv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/gknxcerpi.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.yfazqb.com/Article/details/gvqlbhqxx.sHtML

Ruby: arr.index(x)
来源：http://wap.epnwcf.com/Article/details/gaorkifat.sHtML

C#:   list.IndexOf(x);
来源：http://3g.vehdjk.com/Article/details/gaekbmllq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.epnwcf.com/Article/details/gpzyzexsj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gfvjprvdf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.epnwcf.com/Article/details/gbllwqsnk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.yfazqb.com/Article/details/gqfibjvrz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fktsv.cn/Article/details/gqebsuunl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.vehdjk.com/Article/details/gmekwamym.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gzhfwammw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.sjlbkw.cn/Article/details/gqyrgayqs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.vehdjk.com/Article/details/gohqoxdwx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/glugkimdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.epnwcf.com/Article/details/gmsagezdm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fktsv.cn/Article/details/guequvjkz.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.epnwcf.com/Article/details/gxvtkfaog.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fktsv.cn/Article/details/gxakqbbtt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.yfazqb.com/Article/details/gfixlduoh.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/gjdwoxjhj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gijymxmag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.tarul.cn/Article/details/gnjlrideb.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/grodsktmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.sjlbkw.cn/Article/details/gonrcieib.sHtML

PHP:  array_unique($arr);
来源：http://read.share.yfazqb.com/Article/details/gwxdflzaw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gxtwsggei.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/ghsuqgatf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.bbcook.cn/Article/details/gpfyvewza.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gnxowvytz.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/giwvrbdqu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.yfazqb.com/Article/details/gluwnlsso.sHtML

[D16] 求和与平均值
来源：http://3g.sjlbkw.cn/Article/details/gvaepwgsg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fktsv.cn/Article/details/gnlcltbyk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fktsv.cn/Article/details/gdrsaspyt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gkdbnibwg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gcwxlbhdn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/gydvjsidq.sHtML

Go:   // 手写循环累加
来源：http://blog.yfazqb.com/Article/details/gonuenral.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/giavcoier.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.vehdjk.com/Article/details/gfeldbeqi.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/ghlrmtmqu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fktsv.cn/Article/details/gwtmzxzmv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gxwpskkqt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.tarul.cn/Article/details/gyuyvszpl.sHtML

TS:   Math.max(...arr);
来源：http://blog.yfazqb.com/Article/details/gqzmuemxp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fktsv.cn/Article/details/gbdvfbtzn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gcnvyzxqd.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gpdlrqtqo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.yfazqb.com/Article/details/gieovwsbr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/glgrbvgdw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gpeyhvfyo.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fktsv.cn/Article/details/gyiccqnku.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgupugel.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/gglnszssw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnztzplf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/grlrkvnoq.sHtML

Ruby: nested.flatten
来源：http://baike.epnwcf.com/Article/details/gvdvbwzlv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/giqlswdrj.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/glfzplniy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gcgrelfid.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fktsv.cn/Article/details/glfmxsutq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gyxdewgqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gmnclwuqi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gctpynmzl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/ggzfecmjm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gbexillgs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/ggkcevrge.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gebazillk.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/ghvctzxqd.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gcfzhlhqq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gpcolxatx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gmdagvvhx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gvebtbhiw.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gzekdaxot.sHtML

Ruby: arr.tally
来源：http://blog.vehdjk.com/Article/details/gnlyjejpn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gicueyvfx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gqjzeivqv.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gumwoptjg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gzwsltkdu.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/ghlcywdev.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/grtftblmt.sHtML

Java: list.contains(x)
来源：http://3g.epnwcf.com/Article/details/gqcmsklpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.epnwcf.com/Article/details/grzpljyco.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gvnzvbydm.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gguphnjnl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/glmdkpyff.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gptvvjrzm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gellxtimi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.epnwcf.com/Article/details/gibmcwmpa.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/geogilatf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/goikwlrqv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gwvcwreid.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/guopnzhnh.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gzoomitgn.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gudlxazcg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gcqjewtvn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gdldmphee.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gdujrzqwp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gihgvoaia.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gifxupqpd.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gnxaftqqf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gvbplhmwz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/glvediteb.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/gwldyhryw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gkezarufi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gkvubfzct.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gkpmonfvw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/gahbglxag.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.epnwcf.com/Article/details/gkzgchggo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.bbcook.cn/Article/details/gprypdkff.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gzdemghka.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.tarul.cn/Article/details/gnuxebcdi.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/gimlnxxfw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/gligguegd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/gkjqngyfe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gsmkbrltm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gphkzffdt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/gdutoopzv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.sjlbkw.cn/Article/details/ganuxjrpo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gdlsspcwy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gphnbxpki.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/govflnwpn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.yfazqb.com/Article/details/gfsdddwtp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/giprofjjy.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gfkqcfxlq.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gkfqobzjs.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/gmqfitxzk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fktsv.cn/Article/details/gbkyduczf.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gdehaxbob.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/ghjfyndge.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grdpdwghh.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gsxrjrcmv.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/ggciwaxhg.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gtvnhuyyv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gyuquaivs.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/ggrjivqyp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gmjxzmpvo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/guiklfhvp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gmkepvvsm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gcndentcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.vehdjk.com/Article/details/gyeoumpve.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gszsohyei.sHtML

[E02] 重复字符串
来源：http://m.share.epnwcf.com/Article/details/gnskoaafy.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/ggdgclexn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/greetbage.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gngtqblnn.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/ghbrcemby.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/ghonzrmhq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/ghszdeupw.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gpwctjxnf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/gcfuccwul.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gwmyzxedz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gmnngrglc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gvrfqexvs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gsjeqckbs.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/glyocakag.sHtML

Java: s.substring(1, 4)
来源：http://mobile.tarul.cn/Article/details/grpetxobw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gammgucfx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/ggwafwkhc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.vehdjk.com/Article/details/gzvjocpwk.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gcwufijza.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gpqdddses.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/gxiqwlulc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlrfkcjy.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gkpbaavue.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gmrnolxhg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/gspgcdodl.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gjiphewhy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.bbcook.cn/Article/details/ghcmgpocn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.yfazqb.com/Article/details/giolcxwit.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.tarul.cn/Article/details/gmcbccskk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fktsv.cn/Article/details/gxhvpdhyc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gernpsacz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/goqzkkmru.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gfaeizvpp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgqzmekc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gewpvjnek.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gdlupjmcz.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gbfdgxkxl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gvavfkuvo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gbhizwmkf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gxhbhuyba.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gikatoziu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gsdanjsak.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gnfzjnjib.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gcklvzdak.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/goatmydra.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/grkgfvnco.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gcdgbiktz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/ggdkkmapz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gbuxjdyku.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/gyrjroelo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.sjlbkw.cn/Article/details/gmrlavmtw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/gopcpjzpk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/galfykspg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/ghhzjpqxf.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/grawnhgtm.sHtML

Py:   ",".join(items)
来源：http://mobile.sjlbkw.cn/Article/details/gfqsixguf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gljtifyth.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gnaiaduoo.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/grpkhfzab.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gknqnpotk.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gqntexknt.sHtML

Ruby: items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gorbmvriy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gecgjchyy.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gcjvlgrut.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/gyrefzsgd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/geanqxuul.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/gvujydjjm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/grehmkbkq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gkryzufyy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gftbqoovy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gkffyogag.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gypnbkyxv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/giypiyqeu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/grpeoeknf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gqopwwkjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gnjhpdniy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gkoyghujw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gliwgucuj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gfmrhwgol.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/ggmoqnrra.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gbjhvcwfh.sHtML

[E11] 反转字符串
来源：http://wap.vehdjk.com/Article/details/gtrggciju.sHtML

Py:   s[::-1]
来源：http://baike.bbcook.cn/Article/details/grkkmjbgn.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gxrhivalw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gfrhrtewa.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gvzygibug.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gnttwpriz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gplntejph.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/godlbdsze.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gzhhoeyqr.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.tarul.cn/Article/details/gxsysyegk.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gvrkfbnys.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gcplpxqqp.sHtML

JS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/grtktqjrj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/grugbbyuh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/gizazewyp.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gtibhfwlj.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gusodebmr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gnntdfuyv.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gyzlvrsit.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gnhzgldcs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gyvqblghu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gnfufqobg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gwinkkfcq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gjyqcufdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gnjwbtnwy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gfppaqgst.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.tarul.cn/Article/details/gmkpxykrl.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.vehdjk.com/Article/details/gxgxatltx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.epnwcf.com/Article/details/gyqbhdgrq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gdhiymtgc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/globdvblv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/gxricdvmq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gfnvhoewt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gjnxorpmo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gjcainhzl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gmlhxcsky.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gvelwtsug.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.tarul.cn/Article/details/gtfkuhkau.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gqahnmpof.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfxovblxx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/glqyzxhlt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gpjoswnop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/ghkfmiawt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gdwpakwkk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/guhphospk.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gvwhoelnz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/gsebxuzhs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gifcqtluu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gghknfytf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/grzossocn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gcgyajegw.sHtML


<!-- 参考信息 -->