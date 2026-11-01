代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://3g.sjlbkw.cn/Article/details/gqtghsfka.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.epnwcf.com/Article/details/ghkcwfwph.sHtML

[D09] 排序（升序）
来源：http://www.share.vehdjk.com/Article/details/ggxzltlbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrmkbhdy.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gerilgysv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.vehdjk.com/Article/details/gvjfswkwr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.bbcook.cn/Article/details/gttfzhytq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.tarul.cn/Article/details/gjkodhude.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/gfbhrlpsm.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gljnvvqbi.sHtML

C#:   list.Sort();
来源：http://www.blog.epnwcf.com/Article/details/gpszrmugv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.epnwcf.com/Article/details/gsjxtnmwa.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.vehdjk.com/Article/details/gjdtnmwbv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gaoioouqt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.yfazqb.com/Article/details/gwgjnxliq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.bbcook.cn/Article/details/gwtddaszi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.yfazqb.com/Article/details/gjabfrvsc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.sjlbkw.cn/Article/details/gvqtclwlg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fktsv.cn/Article/details/gkrkieisn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.yfazqb.com/Article/details/gjzkxgzwl.sHtML

[D11] 反转数组
来源：http://wap.epnwcf.com/Article/details/gpcmhylxw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gkmfbzumb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.yfazqb.com/Article/details/givllyujz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.yfazqb.com/Article/details/gpsoqwzdd.sHtML

TS:   [...arr].reverse();
来源：http://wap.yfazqb.com/Article/details/gjwpumrqm.sHtML

Java: Collections.reverse(list);
来源：http://read.share.tarul.cn/Article/details/gcyzlkdxl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gbwzbzhrr.sHtML

Ruby: arr.reverse
来源：http://baike.vehdjk.com/Article/details/gacqwhayc.sHtML

C#:   list.Reverse();
来源：http://m.share.sjlbkw.cn/Article/details/gmtbqytfj.sHtML

[D12] 查找元素下标
来源：http://read.share.bbcook.cn/Article/details/glxkqglxd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.yfazqb.com/Article/details/glbtptira.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.vehdjk.com/Article/details/gptslbsxx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.tarul.cn/Article/details/gtzoumxst.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/grtdkbqty.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.yfazqb.com/Article/details/glizuspok.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gmqzsfcla.sHtML

Ruby: arr.index(x)
来源：http://wap.yfazqb.com/Article/details/gemrblnsy.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.tarul.cn/Article/details/ghpvxbkjb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.epnwcf.com/Article/details/grcrcrhrp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.bbcook.cn/Article/details/grkrrfzim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.epnwcf.com/Article/details/grsutfbem.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.bbcook.cn/Article/details/grwpbihwz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.epnwcf.com/Article/details/gtzuaxsyt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.bbcook.cn/Article/details/gshtbzahu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gajzgkdum.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.sjlbkw.cn/Article/details/gtqgunarx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.sjlbkw.cn/Article/details/guqjvfsjh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.vehdjk.com/Article/details/gxrzrybsz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.yfazqb.com/Article/details/gbufzissx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gznoyehoi.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fktsv.cn/Article/details/geuxmfoua.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gvabstdka.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.sjlbkw.cn/Article/details/gtgjipbpf.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gkukdlocm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlrqzhoo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/gkgxklutv.sHtML

[D15] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxxnpawr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.bbcook.cn/Article/details/gzsxpoyxs.sHtML

PHP:  array_unique($arr);
来源：http://read.share.epnwcf.com/Article/details/ggjzbkucj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gnfsisdxn.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gdijqkcjy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.yfazqb.com/Article/details/gekhmptxp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.yfazqb.com/Article/details/gkzjsmzrp.sHtML

Ruby: arr.uniq
来源：http://read.share.epnwcf.com/Article/details/gjocouxfd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gzyzpaipe.sHtML

[D16] 求和与平均值
来源：http://mobile.yfazqb.com/Article/details/gnnksdmlw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.vehdjk.com/Article/details/ggocpduzq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.yfazqb.com/Article/details/gdudiiwmv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gribzvzpz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gvjmgpebn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gokljruax.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/guujwfbft.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.epnwcf.com/Article/details/gosdvffhr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.vehdjk.com/Article/details/gmupngsql.sHtML

[D17] 最大值与最小值
来源：http://wap.bbcook.cn/Article/details/gecpmxczi.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.bbcook.cn/Article/details/gzjohioah.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/guxkmgxto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.yfazqb.com/Article/details/gvpxupydi.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwftjruih.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fktsv.cn/Article/details/gnzewjgzh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gmsedtozv.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gkxnzhuwa.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.epnwcf.com/Article/details/gjgyddneh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gbranrkaj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fktsv.cn/Article/details/gyffrkzfm.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.yfazqb.com/Article/details/glzjkrrqm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gqfdnflxr.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gnjhsfrcb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fktsv.cn/Article/details/guhetdrlk.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gspusrlil.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gwhxwydes.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/gcuhtwqnn.sHtML

[D19] 按字段分组
来源：http://www.m.share.sjlbkw.cn/Article/details/guduyjnly.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gztvxztcw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fktsv.cn/Article/details/gautzllzt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/ghiirkzoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gmsqbujxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gpethuumo.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/gipahpqnm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fktsv.cn/Article/details/gdblmjnlb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gndcxyuqp.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.tarul.cn/Article/details/gtvswzsml.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gsvkxazmu.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gazdtyqpl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gopujrmvm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gpkxkxbju.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.epnwcf.com/Article/details/gprzohage.sHtML

Go:   // 手写 map[T]int
来源：http://3g.bbcook.cn/Article/details/grtdftbhr.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/gtnraouxu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gudwwedrb.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gbwvwotyf.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gduwnqscj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/glqbehquw.sHtML

JS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/ggverjjih.sHtML

TS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gsnpbntpw.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gowynivic.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gzjhvphdq.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/geeqcnrex.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gisbfsuac.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gyygwtvsu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gpvjxidbk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gjgcntwkg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.sjlbkw.cn/Article/details/gudoowewj.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/gxftbcwfu.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gqtnxbjlc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.tarul.cn/Article/details/gqiyzobxg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gnrrmvtvv.sHtML

C#:   new List<int>(list);
来源：http://read.share.yfazqb.com/Article/details/gpeiwyqvv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gzeiepccn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gypwjhivt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gbvtntrbn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gsocitnab.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gxeahimot.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/gesvikupw.sHtML

Go:   // 手写循环
来源：http://3g.bbcook.cn/Article/details/gijkrbhfm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gyxswnbyl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/glbnzgxxy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/giinjsfuw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gttrjdccl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fktsv.cn/Article/details/gzipnwrwh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gilfxuprv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gqsedgrpe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gwysqpwjs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/gycyvegbj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.sjlbkw.cn/Article/details/gugvgenvp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/ggkcouczh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/ggjhfmruj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gvfadcenp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gkhkafwjy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gvavgontr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/ggfoklztv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/giojpnhcz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.sjlbkw.cn/Article/details/gcmiopjib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gusaohjie.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gnxcublkq.sHtML

[D26] 数组转字符串
来源：http://www.share.fktsv.cn/Article/details/gbfbanzhk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gicrsrxwi.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.bbcook.cn/Article/details/gmczlzwaf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfhmfopu.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/grfziumlg.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gyahprfjt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/grdydsvdj.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gedzuauhv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/geqoshyqr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwvzgsbcc.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/giftcsoxp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghvhxamcf.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gunbzuulz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gcvouvndk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gdvyikalz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gtxxpkypj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gqwvqwtva.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gzatjtfma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.sjlbkw.cn/Article/details/gvajiengt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gxiauiyhc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gaeklaqpk.sHtML

[E02] 重复字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnedotfkw.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gziqiazvc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.sjlbkw.cn/Article/details/gyenmchby.sHtML

JS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gkqagetvv.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/ghulixbvb.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gnmnpybyv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gvgewspku.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/glfnpnqva.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gcloozbgh.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gradwwfzk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gywoehmbd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/guqapgnzi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/ghsjchzjs.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/glrmftbtt.sHtML

Java: s.substring(1, 4)
来源：http://3g.sjlbkw.cn/Article/details/gpfmhvepm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gewrtpaia.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gahkcbvfp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gfijqjnku.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gjxawjdnq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/ghilmzgeu.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gjdlqtlkj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gxobwdiuk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gdqibygdf.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gvyzfboyi.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/glwmewind.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gwsoudggx.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gjdemywgf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gpwcqnopm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gppqwyivd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/goqhjkiad.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/genukodcu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/ggpysfgme.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/glpgeitsa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gcjhnpquy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gvsbeuajz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gizfbbbdv.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gysyewtgm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gstfsomeq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gannwookh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gaxcmrkps.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/govnypjwy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/ggvuephgm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/guqnjrnfo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/ghifgydms.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gskfbswuv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gyvxrhprd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/gykxmksel.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.epnwcf.com/Article/details/gozoarvja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/gtqsvuosk.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/goipnfjae.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/ggfszehrv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gynppueiv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gpyfrtwkm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gnpeljyqp.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gdcaxbsii.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gvefmowdo.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gkuahdota.sHtML

JS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gjdeygsyx.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/glaywjdeh.sHtML

Java: String.join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gxipvervs.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gnjdicdna.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gkiwnmpqa.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gyeqprscq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/gqfbeoqin.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.vehdjk.com/Article/details/govuaqudv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.vehdjk.com/Article/details/gpgokovdm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gloqrwtom.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gvvlokqkk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gtmlrmcro.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/gufbyiofa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gphbfqekq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gnddawapk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gqsfrtplx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gyytojnxp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gjkdtymrf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/ggdartvmg.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gcapclbhp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gznevbfqc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gzkyocpug.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gyklrpcbj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.sjlbkw.cn/Article/details/gcmphghsx.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gaaoegcbm.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gpnltufjl.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gazqhpvid.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/giuzowrya.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gpidvlrhr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gzxxacmhf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gvttnswzx.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gmjhcliwy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gomusoomv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gcfxwzuwf.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gndpsqwno.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gfxaswrdz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/ghbwadfzs.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/geovbvvfu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gutbnbgpz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gnkietwwl.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/grohfxleu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gtfxqdazq.sHtML

[E13] 逐字符遍历
来源：http://mobile.fktsv.cn/Article/details/gcvyyjpcp.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gkvdfcgcf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/ghdnezjmw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gyfjlomlb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gmtpffsmp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gvguwcead.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.epnwcf.com/Article/details/gobvduxqz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/giyyunfxe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.tarul.cn/Article/details/grmdeevnj.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/gahgjrltx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/gdxdseaie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gchqmqhqm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gdbmlvzwb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/gfnakkiru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gzldadfne.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/ghruuafyy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/gxdaxxrmf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gjayhffnx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/glrtignpz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gdlqzkpup.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/geakandzd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gpqzzkefa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/gbbicdoer.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gzbnqidlp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gxaidjqms.sHtML


<!-- 参考信息 -->