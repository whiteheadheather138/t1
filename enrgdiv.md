代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://mobile.vehdjk.com/Article/details/gnypmyyeu.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.yfazqb.com/Article/details/gfijnitvi.sHtML

[D09] 排序（升序）
来源：http://wap.tarul.cn/Article/details/gpldlxuqz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gdbxrkdmc.sHtML

PHP:  sort($arr);
来源：http://mobile.epnwcf.com/Article/details/gnxncfbfm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.vehdjk.com/Article/details/gcesgnhnr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fktsv.cn/Article/details/gbtrqfrtu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.tarul.cn/Article/details/ghspfiifr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gsfgnlvwk.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/glxhizgdb.sHtML

C#:   list.Sort();
来源：http://www.share.vehdjk.com/Article/details/gpvvpwvfq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.tarul.cn/Article/details/gdpeixbic.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.yfazqb.com/Article/details/gniofmotx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gmcaocxuv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.sjlbkw.cn/Article/details/gemqyuwws.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gonblhajz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.bbcook.cn/Article/details/gxkxzrxrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjatwfbpa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.tarul.cn/Article/details/gajowmqmi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.tarul.cn/Article/details/gkyxfrofn.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gvpcgdiql.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.tarul.cn/Article/details/gxkqifykb.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.vehdjk.com/Article/details/glzgaabpd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.sjlbkw.cn/Article/details/gofdtnmea.sHtML

TS:   [...arr].reverse();
来源：http://blog.epnwcf.com/Article/details/ghvudzzrv.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fktsv.cn/Article/details/gkxembfxz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fktsv.cn/Article/details/gwvejymqy.sHtML

Ruby: arr.reverse
来源：http://www.blog.epnwcf.com/Article/details/gortdbsoc.sHtML

C#:   list.Reverse();
来源：http://blog.tarul.cn/Article/details/gougomrzk.sHtML

[D12] 查找元素下标
来源：http://www.share.yfazqb.com/Article/details/glawrqkpb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.epnwcf.com/Article/details/gvncryuzr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.tarul.cn/Article/details/gotjrdaxc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.epnwcf.com/Article/details/gxsapckrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.epnwcf.com/Article/details/gcfpspuhg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.vehdjk.com/Article/details/gnebabcgc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gxvsknhai.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.yfazqb.com/Article/details/ggqwenulx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fktsv.cn/Article/details/gnakvrngh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.tarul.cn/Article/details/gahtnlslg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.yfazqb.com/Article/details/gnystibrp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/gjxegdbsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.epnwcf.com/Article/details/gbmbvwhvc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.tarul.cn/Article/details/gywdbmlqg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.tarul.cn/Article/details/gjmbmsmvd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.sjlbkw.cn/Article/details/gspxlwyox.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gvgctzzwh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.epnwcf.com/Article/details/gkflwoyqz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.sjlbkw.cn/Article/details/gqmmopctj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gjsaourwb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.tarul.cn/Article/details/gljrcyuwg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.bbcook.cn/Article/details/gedzwvqja.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gmaronmaa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.yfazqb.com/Article/details/gkzzhwncz.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/grvadlzxb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fktsv.cn/Article/details/gkvhtgvvs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.epnwcf.com/Article/details/gyqlhovcp.sHtML

[D15] 去重
来源：http://read.share.vehdjk.com/Article/details/gtuzfchli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gfpafwtcf.sHtML

PHP:  array_unique($arr);
来源：http://read.share.bbcook.cn/Article/details/gusyhedwd.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/glrhvipep.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/grlingemz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fktsv.cn/Article/details/goxlbrwua.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.epnwcf.com/Article/details/glwgtnfcg.sHtML

Ruby: arr.uniq
来源：http://www.share.tarul.cn/Article/details/gnlcdiuxg.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gqgupatik.sHtML

[D16] 求和与平均值
来源：http://m.share.tarul.cn/Article/details/gqlxznjnf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gepfgumnj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.epnwcf.com/Article/details/getknczmu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gdgkkijlf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gzfkuuspj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/grmrxtjrt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.epnwcf.com/Article/details/gjovzigbt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gjrsyfuiu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/gvwfqzola.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gqljauegq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gttkduxho.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/grsietfup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gdtginxdy.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/glkvkwmia.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fktsv.cn/Article/details/gbhhnbjff.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gatzmeybv.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gsgdkksdn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.sjlbkw.cn/Article/details/gkbwkbkwp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.bbcook.cn/Article/details/gdkfpvfrz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/gnrmprrgq.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.tarul.cn/Article/details/gpkpfjdua.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gonwwohwc.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/grhlekthp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.tarul.cn/Article/details/gpissfbxm.sHtML

Go:   // 手写双层循环
来源：http://www.blog.sjlbkw.cn/Article/details/grvqgevju.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/ggrhlvduo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/grrgjotdr.sHtML

[D19] 按字段分组
来源：http://3g.vehdjk.com/Article/details/gzunetoxu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.sjlbkw.cn/Article/details/gvibiwdfr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.sjlbkw.cn/Article/details/gtsanzpkh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gayznabya.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/ggsyixkni.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/gexgswszm.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/glhkmbwpo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.epnwcf.com/Article/details/gdbyulojn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gdqpiapyn.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/gvjcvspwt.sHtML

Py:   Counter(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gzuqufuls.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gpfrdhkma.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gufrmivpr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gnzmnjrke.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gptanmmew.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gfkeesldh.sHtML

Ruby: arr.tally
来源：http://3g.vehdjk.com/Article/details/gvjzdhtcu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.vehdjk.com/Article/details/guttcwooz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gzifspqhu.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gkqgvsdxz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/goyuhxnrs.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gixwpjskz.sHtML

TS:   arr.includes(x)
来源：http://read.share.fktsv.cn/Article/details/guiunaqyh.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/ghiminwgy.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gyckcamjg.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gcyymwqzc.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gqnroxbdz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gvfqivfke.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.yfazqb.com/Article/details/goeyirhjr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gqlxtpnfj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/ghvgktopy.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gbvqaolkg.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gsquqwajz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gikzwgjeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gkpnwbtsy.sHtML

C#:   new List<int>(list);
来源：http://wap.yfazqb.com/Article/details/gmqvfoprq.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/gwqgdbcvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/gbziqfhfx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gyhlidbwk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gjvgatpyo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gbiolmort.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.vehdjk.com/Article/details/grmaxmxrc.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gsylpajhw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gmevcyejo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/ghngroxvu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gidkvjohw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/guynlixum.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/ghjcwwccn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gxmctkiws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gbdmuykrv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/gistoqbia.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gpmlgjpma.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gizujqfps.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/grdxrpfxk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gczcxvhup.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/guqvolxin.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.yfazqb.com/Article/details/gcjcuzmzl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gbecpaqet.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/goyidnidm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbldjifry.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gtklrgqej.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gmgmkvetu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gzcgjxexc.sHtML

[D26] 数组转字符串
来源：http://mobile.yfazqb.com/Article/details/gouzmvckw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.epnwcf.com/Article/details/gaoukuosn.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.epnwcf.com/Article/details/ggbrssnuh.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gwbvvjdvj.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gnbixjrtp.sHtML

Java: String.join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/ggbpmight.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/ghnprzuej.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gdmdnhgko.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/giziynhtg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gycjulmow.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/ghgollzae.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gaffjtnhi.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gbririuat.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gubmydkab.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/gmcyztzyc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/galacwdlc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gmjtcpqhm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/guhjblkhj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/gdkuciiyl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gqphjqrgf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gfwavufop.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/gxuckcqed.sHtML

Py:   "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gzwynnwse.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/geiejykni.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gxlutnezv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gfudjwuae.sHtML

Java: "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gljqxtkol.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gueicpmgt.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/ghpplmeci.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.sjlbkw.cn/Article/details/gjaertrdf.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gmahzcdru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/gogqnbcmv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gyvnestov.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gjiseokpz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gszfhlxfp.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gfbvttyhz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/ghglmvskp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/ginetumux.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gtpvlcdzf.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/grvrkmpws.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gbsjoxccd.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gmohxmfeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/ghakxomjj.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gmfkyrvsw.sHtML

Java: s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gkxoeapcl.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.epnwcf.com/Article/details/gvwoleckp.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gyiiwsfao.sHtML

C#:   s.IndexOf("x")
来源：http://blog.epnwcf.com/Article/details/gaxqyflsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/ggtybedtg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gasxftcfm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gxzqlqfef.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gaxicjbnc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gjagvgjql.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.tarul.cn/Article/details/gtzdtzkhr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.vehdjk.com/Article/details/gfnqylybt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/grmfzrgil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gdphxhnlq.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gsqbeskpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gtwdgtbkh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gopzzfhyk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/ghwmwkvgk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/ghbfmbcni.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gulkgyhsb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gvixrjidm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gtssmzvpj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gfwdqpfit.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gcntxftbl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.epnwcf.com/Article/details/grzgtmhjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gbbtqhhsr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/goxjgdtpn.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gjaasppal.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fktsv.cn/Article/details/gxmuoiaue.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/geoirskal.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gryygevug.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gqmugwabr.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gfqnvxson.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gnlkisttw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.vehdjk.com/Article/details/gcrgbayid.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gdueqqqce.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gaawagbnr.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/gfvfmvemu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.epnwcf.com/Article/details/gdsuhbanz.sHtML

Ruby: items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gamkzitzu.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gwsyjrtnn.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/guqduntly.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gxhrrbqbz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gdgwefesz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/grtvbynxx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gypycdjbz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gzurwlixy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/gmjrynwio.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.bbcook.cn/Article/details/gkgwzmrkv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gryirzgxg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.yfazqb.com/Article/details/gnxvylsiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gjaukciye.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gcxtyhrwm.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gptftqekr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/ggmkgwtog.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gaqwwoszz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/giswegnhb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/glienzfsp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxsjukeh.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/grweozcys.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gcqgpaunk.sHtML

PHP:  strrev($s);
来源：http://baike.yfazqb.com/Article/details/gtsvcuzvs.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gvnftuvji.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/goywaohyb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gnpqoraok.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gygtefuig.sHtML

Ruby: s.reverse
来源：http://read.share.tarul.cn/Article/details/gfzalxbrc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.bbcook.cn/Article/details/gsrzyhefb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gtfhlbsju.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gerxnzafe.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.tarul.cn/Article/details/gjasfnphs.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gsxnaejmq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/ggicdhwfx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gvycrafrm.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.epnwcf.com/Article/details/gbhinsadf.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gzrtaqcqe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gpjntcemt.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/glheeaajd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gkyfodbym.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gyrojnrdj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gnutrmvdb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gznbyemxo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gfudbherq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.bbcook.cn/Article/details/gjrtpoixl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.epnwcf.com/Article/details/gskqgnfzv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gwwqoxahl.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/gtxuvelab.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpuddula.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gaonximry.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gxxgtgjqg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gwjnymjbx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/ghmhcjcqv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gtsqxvwhp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gbfzyphcp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gljfaebgl.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/glyzwtyet.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gvmekkbqd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/gbvodlpzh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gipzbkcxe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gwtcvarbn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gdzlftbie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gptwhnuvo.sHtML


<!-- 参考信息 -->