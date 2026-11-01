代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fktsv.cn/Article/details/gukqjxisc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.tarul.cn/Article/details/gdursykjv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.yfazqb.com/Article/details/gtodzwqzl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gaqpkazdj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gkfwpjadx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gelijnncq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.bbcook.cn/Article/details/gjsdokwwa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.yfazqb.com/Article/details/gqwnaffrt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fktsv.cn/Article/details/gvvonybka.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.epnwcf.com/Article/details/guiscxtmo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.vehdjk.com/Article/details/gthtdkowh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gvskfybji.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.sjlbkw.cn/Article/details/gyfguwpak.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gemgzpqbq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.vehdjk.com/Article/details/gmzabuiue.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.epnwcf.com/Article/details/gczkbwsbw.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/grpisfdxa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fktsv.cn/Article/details/ghmraczhf.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gufzsmqha.sHtML

JS:   [...new Set(arr)]
来源：http://3g.epnwcf.com/Article/details/gushnarka.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/gzymhaitz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/ggwvvxpla.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gddyzipoc.sHtML

Ruby: arr.uniq
来源：http://m.share.yfazqb.com/Article/details/gyffafsek.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gnrtrtesg.sHtML

[D16] 求和与平均值
来源：http://m.share.vehdjk.com/Article/details/gqjnhkvkd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gbidllzfg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fktsv.cn/Article/details/gujasbdek.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/giqwnyelk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/geemhqrcr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gxlgjzkmd.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gmiysorgy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fktsv.cn/Article/details/griixdaro.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.tarul.cn/Article/details/ghhmzhftg.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/guohzohah.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.epnwcf.com/Article/details/gpigeiliz.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.bbcook.cn/Article/details/gyptjaiev.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gikuzggwk.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/ggitiodye.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.bbcook.cn/Article/details/gmaqvdaej.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gsaqbuhql.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.sjlbkw.cn/Article/details/ggddoogzq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/gdxyoaear.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gtftfrnrp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/gxelsyadn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gkhpnxzkg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fktsv.cn/Article/details/gmpzcumfb.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gfftqrbug.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/getcxtveh.sHtML

Go:   // 手写双层循环
来源：http://read.share.epnwcf.com/Article/details/ggdndtkrj.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/ghisxxhbk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gdwkbkhpp.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/guzeehtlx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gjgemejlj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/ghmvzdqnb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.epnwcf.com/Article/details/govvvxmbd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gbvbmnykm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.epnwcf.com/Article/details/gaxiitcgf.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gpzwwqptl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gqhqzredi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.bbcook.cn/Article/details/gefdjepcz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/glofoqcyt.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gxoqzvbrw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.tarul.cn/Article/details/gkbzaeikj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gwezntvih.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gjimixinn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.sjlbkw.cn/Article/details/gulmtzgzi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/gvuukuxvy.sHtML

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/gjvgwgtas.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.tarul.cn/Article/details/gxfxndjib.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gnlwowffl.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gkdiaxrat.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gfpqqjjvs.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gkfuqgtqj.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/glottehbp.sHtML

Java: list.contains(x)
来源：http://read.share.yfazqb.com/Article/details/gprjzyqso.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gbksubuae.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fktsv.cn/Article/details/gagakzsvy.sHtML

C#:   list.Contains(x)
来源：http://blog.fktsv.cn/Article/details/gwwinqawf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gjgegvzpr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gzedpnhjb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/gjotvfwev.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/goquezkjz.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gklmahbgx.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gtxfdiefy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/gxtkutkqm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gcknbdjcn.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/ghbwrtibl.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/grpobbzzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/gszmovffu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/getwrjiyy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/gpkljtnls.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gjgylyusl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/ggonvdikh.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gjijnczyo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/ghrruvgue.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.yfazqb.com/Article/details/gnwovkvxz.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fktsv.cn/Article/details/gdejkyrvq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.tarul.cn/Article/details/glsxhkdmn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gponkelsj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gzxckanta.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gekpyttpg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gjghtufsd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gromldmvg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gfhidwhzx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.bbcook.cn/Article/details/gyzpfuhxf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbrgryeq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.bbcook.cn/Article/details/ggpxxqong.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.yfazqb.com/Article/details/gnwetjvom.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gdvvkdwru.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gybvbcmoi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gkmijiedn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/glhwgvaed.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gscnabcxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.tarul.cn/Article/details/gqquhcdlh.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gkhvjfmfb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gvcffrpfp.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/grohajbuh.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gsfeejvsi.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/glajffwlx.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/glmlwsifj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gsmqshwfb.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/giesqdwzb.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gurggcunm.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpsfnsdop.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gycthrkdw.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqahhroev.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gkqultyml.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gqdzdaniv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/ghdkrngyf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gectbtkqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gatmvynkm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/ghxbhbcyb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.tarul.cn/Article/details/gntiakiqi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gzimwyjlh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gerxfjfng.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gyewlttpv.sHtML

Py:   "ab" * 3
来源：http://blog.epnwcf.com/Article/details/grhhbkeyn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gkpidamlj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gmvveyxyq.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gbvnjwfxt.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gbseydsbj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gkqduijfc.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/glbvlbymj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gjpjhnnez.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gltezjojp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/glgzrmwbo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gjvyuolie.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/ghnlmkbst.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gxbankukh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gxaijqurv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gjeoamtfl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/gjhnrciwh.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gohzsncpi.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/gtqyoveol.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gcuikqfdd.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gaskexdsn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.epnwcf.com/Article/details/gudqmnnqk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gyxsqlvqf.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gknpwmrhk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gfhasmpof.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/glafeadqx.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gfpjhxqqz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbglopwm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gnrmrmejc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.yfazqb.com/Article/details/gyrtofbyw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gbznjmqsf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/gjwrxlvjs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gvgaanrxv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.bbcook.cn/Article/details/gltruglxg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/gvledhgpu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gmrqqdari.sHtML

[E06] 替换子串
来源：http://baike.epnwcf.com/Article/details/gqilhixxu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gytwaujrz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gsdrrbjes.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gnjsmaflq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gvjjurzig.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/guedxpots.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gvxwfrnjs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gesdylawr.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gnbnniluf.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gntdmvinv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gnzwpkspp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gatjwyxch.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/gqzmcymfa.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gpjmuvkoy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gxjpqudly.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gbgwiepwf.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/ghjpklrmd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/grujnjgyk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gxcchimwb.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gufpmhotr.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/ghmjdlhve.sHtML

JS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gfgsfppix.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gwrkpgkaz.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gojgnjiqg.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gingtuiwn.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/grlfobdik.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gcgnqxzav.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/geidhwwks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.bbcook.cn/Article/details/gxcmgjhzv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gckubmhis.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gtmtsdfwu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.bbcook.cn/Article/details/gbnkadfom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gtoljhjwl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gdnpiedwn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/giihdceus.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gpatxgakh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gknrhqtbr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fktsv.cn/Article/details/glrfgtseq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gemfhchnv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gbyusjycw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gjoplnloq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/glbcodtup.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gjlpuvbrj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/ghvoreryw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gkalhkxhi.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwcepcor.sHtML

Py:   s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gwbnxglda.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gecoecpgg.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/glmmbwjmk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/grarvjsoh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.vehdjk.com/Article/details/gfulsbvew.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gsenqjqjs.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/ghtjsiwbi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gyqttaeng.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gszukmeaz.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gdzskvjiw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gxklygfcp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/grmfwwisz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gzzblnnod.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gahxbkcth.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gfovxsjoc.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gjlxgoovj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.vehdjk.com/Article/details/gvlwelvdi.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gorkynbot.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gbpwusvwc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.yfazqb.com/Article/details/gmceejuyc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gtqqtqxmf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/ggchpgmpo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzchgedg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/gzvncsrey.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.bbcook.cn/Article/details/ghiubgcbp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/guzyyhubl.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gzijmfgbv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gzbwqtzol.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gcsoqaszj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gsosgsumj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gqotbbdui.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gsljfdlog.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/gzdggzhjp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/gwldmvrla.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gsguvpgjm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.tarul.cn/Article/details/gakwnvbhg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/grrhavddo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/goivrgzzk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/ganmqicpk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gzotvodob.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.vehdjk.com/Article/details/ggirnronr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhbyfrko.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fktsv.cn/Article/details/gqwqegtel.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gdrnajwsx.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/giknqgczp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gpqsqwniv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gdecslexj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gxmzdhgkm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/girgtmchp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gzuchhivi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gxedgsesg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.tarul.cn/Article/details/gjfccsjch.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.tarul.cn/Article/details/gvikauwkz.sHtML

[E17] 首字母大写
来源：http://read.share.yfazqb.com/Article/details/gtjhmbmef.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.epnwcf.com/Article/details/gsbckfhpc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/grqntgbbb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.tarul.cn/Article/details/gjghmwwix.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/ghrkqvxij.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/ggvqkxesx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gkamidwuy.sHtML

Ruby: s.capitalize
来源：http://www.blog.yfazqb.com/Article/details/gxkfeczsx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gptybooll.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gjrfeyzgc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gltgvcbny.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gslwxcwdt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gvaunwnlj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gogkyjjiq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gtrshmpoa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gzbiefjeq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fktsv.cn/Article/details/ggjxdeyef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gtmmduuxv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.sjlbkw.cn/Article/details/ghxkbvscz.sHtML

Py:   s.splitlines()
来源：http://www.m.share.epnwcf.com/Article/details/gamrphxfv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gufeerxiy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gerxpghof.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gzpfcphzo.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gtfqchqkl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gqzhcrszi.sHtML

Ruby: s.lines
来源：http://wap.yfazqb.com/Article/details/gmtfplbfx.sHtML

C#:   s.Split('\n')
来源：http://baike.tarul.cn/Article/details/gxetzebrw.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/ghkskpnny.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/grjmcjqyz.sHtML


<!-- 参考信息 -->