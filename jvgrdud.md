代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.tarul.cn/Article/details/gumafnumd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.vehdjk.com/Article/details/guehxsjlg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.tarul.cn/Article/details/geragxejv.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.yfazqb.com/Article/details/ghhgrrmen.sHtML

Ruby: arr.index(x)
来源：http://read.share.tarul.cn/Article/details/gtktuugtr.sHtML

C#:   list.IndexOf(x);
来源：http://wap.bbcook.cn/Article/details/gkgvedhyp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.vehdjk.com/Article/details/gwjisarpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fktsv.cn/Article/details/gjsodeozk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.epnwcf.com/Article/details/gybpyzcyy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.yfazqb.com/Article/details/gzzeqqybl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.epnwcf.com/Article/details/gbtupcxiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.bbcook.cn/Article/details/gnkbmlhwt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fktsv.cn/Article/details/gzbectliu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gojbgqdhe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gfwpdwxlb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gkzogjhza.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.bbcook.cn/Article/details/gobsqmuei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.bbcook.cn/Article/details/gjingfzlz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/ggtwwnbbc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.tarul.cn/Article/details/ggnfnyiva.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fktsv.cn/Article/details/guavsbabv.sHtML

Go:   // 手写循环
来源：http://read.share.tarul.cn/Article/details/gihxfcvwn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.vehdjk.com/Article/details/gslzmlmmg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvdkwgkws.sHtML

[D15] 去重
来源：http://m.share.tarul.cn/Article/details/gemfnlwvl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gtdpbiyzg.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/geehoogwi.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gfzeqaldx.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/gapapfpua.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gesvdwpfm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gujbedmdf.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gnmwruqcx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/godslxbzg.sHtML

[D16] 求和与平均值
来源：http://read.share.epnwcf.com/Article/details/gqjbscgko.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fktsv.cn/Article/details/gbydmauch.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gqdjbfeym.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/gmacotgkv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gcshjrxjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.bbcook.cn/Article/details/gpkmclvks.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gmxhafsfx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/geapwqkvw.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/gydxnysru.sHtML

[D17] 最大值与最小值
来源：http://baike.fktsv.cn/Article/details/grwgmoqrr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gqksmhkkb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fktsv.cn/Article/details/ganxbuuzk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnvsmurhx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fktsv.cn/Article/details/gogklcmzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gavjburey.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.yfazqb.com/Article/details/gpuqfknee.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.sjlbkw.cn/Article/details/gtnwajzqb.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.yfazqb.com/Article/details/gnslfpwnd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.epnwcf.com/Article/details/gfyznynbi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fktsv.cn/Article/details/gkzrbuikv.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.tarul.cn/Article/details/glbfmlvem.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/ghorjnltv.sHtML

TS:   nested.flat();
来源：http://www.blog.epnwcf.com/Article/details/gkhghgrpx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gwjypjjfe.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gakdabrud.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gdvsekstt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.vehdjk.com/Article/details/gvsqwykov.sHtML

[D19] 按字段分组
来源：http://blog.sjlbkw.cn/Article/details/gcozzsado.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.epnwcf.com/Article/details/gxvosxbnw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gkmicdanm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gjznrmexq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gukcrkqdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.sjlbkw.cn/Article/details/gpiswwpea.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gtrfgdgra.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/grjcepgws.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/ghpfjzbbv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.sjlbkw.cn/Article/details/ghykoubtf.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/geiwlvaxq.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gbpsiyznh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gfjznrdea.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gosjndchx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gitajubkn.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gwzvaqxvr.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gctpcrxdd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.tarul.cn/Article/details/gymceiuig.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gtsusefso.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/gkwesmyxf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/gcgysfcam.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/guodirdbx.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gyzzyltae.sHtML

Java: list.contains(x)
来源：http://3g.bbcook.cn/Article/details/gvpbjjyyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/glwsorvhf.sHtML

Ruby: arr.include?(x)
来源：http://m.share.epnwcf.com/Article/details/gljeejvvz.sHtML

C#:   list.Contains(x)
来源：http://wap.tarul.cn/Article/details/geuuyblmm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/grcuurltp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/givtughvi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/gyjhkwvtw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxxwuhuwo.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gsxcjskvu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqowptbvk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gunjebuwg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.epnwcf.com/Article/details/gtesnmwgx.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/ghbaoipgn.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gpjwmyfpb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gxouqjsxc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/grlxwlcge.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gzyuskzsw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/grqvlknri.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gqlreccmh.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gafkllrtp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.epnwcf.com/Article/details/gbmylirwq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gyeksldwd.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gfrfibwzr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gadaozlkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gcsezhfea.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.bbcook.cn/Article/details/gwwnwooph.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrplkvzo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.yfazqb.com/Article/details/gkntenthe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gnvnbzdgx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gidekmzyz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gebonjeex.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.tarul.cn/Article/details/ggqhhvpgh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gyonnpwze.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/ghkvxkxrx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gvnwwirzz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.bbcook.cn/Article/details/gyprodrln.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.tarul.cn/Article/details/gbwxvwady.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gjlvxoekw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gijkuvqdk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.yfazqb.com/Article/details/gahxolyja.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gukzapctc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/glvazrlit.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/gcatwejum.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gttncadnv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gqeejydtq.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gyhnhamjt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gqovpjrkb.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gplwzctbj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gkssnenyp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggmbwvgpt.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/guczdytqp.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghdyeqmls.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gntmibweq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.yfazqb.com/Article/details/gltsziksf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.vehdjk.com/Article/details/gyqjgqyfo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gypymyuoz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/ggivughmy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gpxywedxt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gucpizjwa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/ggjadexjg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.bbcook.cn/Article/details/gexyfeycd.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gwvjdbocv.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gsastvqup.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fktsv.cn/Article/details/gfduwjouv.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/globuhbnl.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gqbvlsnza.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gygpgtpbw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gfpgiwldv.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gemualula.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gtpmnhuoo.sHtML

[E03] 截取子串
来源：http://baike.tarul.cn/Article/details/gzalswmap.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gecrutzig.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gwzttzxqs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/goqmawphb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gbbcdlqoz.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gesldddrs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/gexsgiava.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gxrfqgtcc.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/gmkctwvui.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gpabdhfjk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gyysirhaf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gykydiysr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gffmuguej.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/ggjojtxem.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gmrdgbnwi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjeknffn.sHtML

Ruby: s.index("x")
来源：http://read.share.fktsv.cn/Article/details/gprzzspbb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gybmlbauv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.yfazqb.com/Article/details/glngqjbbh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gtaigizac.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.vehdjk.com/Article/details/gaimkrkdy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gshvgyynq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.sjlbkw.cn/Article/details/grbsdvnpg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gvwrcxsph.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gxvlzfhhe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.bbcook.cn/Article/details/gldzimluu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gxynennzj.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/gukbkecnk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gjdqhyusd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gsvbxylin.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gqjpfqfab.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gxjmmyywc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gcqzvozur.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gmkygvdfl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggqaanhsh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gzztlmrik.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/gbtvhlrqj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/guszhiabd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gnglsooag.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gzjlitvwd.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gkmfznwog.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/geizkspdd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fktsv.cn/Article/details/gyfnqfrpa.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gealvxbmt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.vehdjk.com/Article/details/gnluowsss.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/goxfdivcm.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gggdqvhts.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gqixorpbj.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gpulxzuvn.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gaxaybqak.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/guuwtkwjt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fktsv.cn/Article/details/gllkgpzmr.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/gmqjewgjs.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/goztoiqrw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.sjlbkw.cn/Article/details/gejmgwlpm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gdaiughne.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.vehdjk.com/Article/details/gsbiikxmx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gatscshmg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/ghxjjluaw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gtyeqzyfi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/grsrxvnqc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/givybnqze.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gvcmejkzu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gccooqlzi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gbsgkapny.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gilpkouvc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gytmpjiaq.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/glmskjsap.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsinqxzo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gzelqbjht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gouyietht.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gckbvzoub.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gygjxoqos.sHtML

Py:   s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gdvaqjmwg.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gvwtsvqxf.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gnhiqmxis.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gvolxqdcy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/ggaeqflou.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.bbcook.cn/Article/details/gpxgdveon.sHtML

Ruby: s.reverse
来源：http://m.share.yfazqb.com/Article/details/galhzsihg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gvuyyoysp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gjqxpnkrs.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gbohqwwse.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gfbhxfrhn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gpnxnfemt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/guraqzneb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.epnwcf.com/Article/details/gkynqxuie.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gouupdrpq.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gtioverim.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gghnfmcey.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gokyeavia.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.yfazqb.com/Article/details/gaiykzeez.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.bbcook.cn/Article/details/guwhyprjc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gvbmoqzwe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gmxixsjoz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gpinbzlgf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gwxndlopq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gkxftrumf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gxfgwlgpi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.epnwcf.com/Article/details/gjjlpdkis.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.vehdjk.com/Article/details/grmtfnebf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.tarul.cn/Article/details/gbyotblcj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/gfidnyhts.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gcfstgwkk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/ghsuttgbs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gtnznriva.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gxftnggca.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fktsv.cn/Article/details/gakmkrtai.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/gzlngjqdp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.tarul.cn/Article/details/gbitroomn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gnodtgwts.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fktsv.cn/Article/details/gqemunmsb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.tarul.cn/Article/details/ghxrodgwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.yfazqb.com/Article/details/gaurroksz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gxonzmssf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gasbmopml.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.yfazqb.com/Article/details/gvosepxiu.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gglzqbazl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gzjwieurr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gszzyadsf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gtaqgiyei.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gqlzrjdvg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gelgcvunk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gzbflppln.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gpkdsyaoi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.epnwcf.com/Article/details/gdjtrqmzl.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/glinfixxa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gytyylwlw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gfmgtoipw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gruizthro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/ggjzwbgdo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gjdzghguq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gstzabvjl.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/gplaignja.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/gluabfkbj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gruxdkzyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fktsv.cn/Article/details/gvmbwxgof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/gqqnfbhhj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gtejkdckd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gevthvtnl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gizvshxth.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gesvwanyr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/gkfogjgkz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.yfazqb.com/Article/details/gwikcczln.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gwcmctmhe.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gmsavwokx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gojifjiiy.sHtML


<!-- 参考信息 -->