代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.tarul.cn/Article/details/gdoosxaex.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.bbcook.cn/Article/details/gcinetgim.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.sjlbkw.cn/Article/details/ghzbvdyww.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.yfazqb.com/Article/details/gblrubbjs.sHtML

Ruby: arr.index(x)
来源：http://wap.tarul.cn/Article/details/geaemhzcn.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.tarul.cn/Article/details/gkqkvggpo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.sjlbkw.cn/Article/details/gmreordnw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gjfaykeqi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.yfazqb.com/Article/details/gyrqolzfk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.vehdjk.com/Article/details/gobngzjon.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.bbcook.cn/Article/details/ggdwnffep.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.yfazqb.com/Article/details/geguqurap.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmavdquv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.sjlbkw.cn/Article/details/gbadnohsl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gqtuxjqey.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.epnwcf.com/Article/details/gztluigug.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.tarul.cn/Article/details/glmhvlkbb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.yfazqb.com/Article/details/grghixvpc.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.bbcook.cn/Article/details/gawyqjnkd.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.tarul.cn/Article/details/gvbextlwb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.yfazqb.com/Article/details/grpcgkexb.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/guavrvvsv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gqlshgmfz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.bbcook.cn/Article/details/glxdmeabg.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gdqqtluzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gqyvzmpaz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gbqtylfhb.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgmkfhvy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gewxwkfbx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.vehdjk.com/Article/details/gtjkqoclv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.tarul.cn/Article/details/gejfhnzpx.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/grxhvqolq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gihpznawg.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gaeehmgbd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.epnwcf.com/Article/details/gzesvkkaz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.yfazqb.com/Article/details/gsqnbrfce.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gsuauoqly.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/gwiaddgqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gnkcusayb.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gfcdbxwrw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/glnpumtig.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.sjlbkw.cn/Article/details/gyirkxdvk.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.tarul.cn/Article/details/ghizcnnsz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/ggkfndgtj.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/grobikklz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.sjlbkw.cn/Article/details/giwscpwmo.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/ghdpovgiw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gjvzhpfww.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gqamqsutb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gmzklnhbs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.sjlbkw.cn/Article/details/grdjpkkha.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/gvgnzxiom.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fktsv.cn/Article/details/gkcitwkes.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gvysnrqso.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.tarul.cn/Article/details/gzlrjpyvb.sHtML

TS:   nested.flat();
来源：http://m.share.bbcook.cn/Article/details/gabvxohqo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fktsv.cn/Article/details/glgjoialq.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gmedommpa.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gvnlzuvsp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/gybpgyrrp.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gqeywhino.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.vehdjk.com/Article/details/gddxzjpaj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gvdpjncrd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.yfazqb.com/Article/details/gnkcsxvth.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gajavfqdc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/guyexplie.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gcrodeftb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/ghpdnlavx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.yfazqb.com/Article/details/gxlomelsf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gepiweofy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gqvigmepn.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gpraamojc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gbyildgse.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwovxdnu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gxfnegohc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gemwiiyqt.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gsntojgbd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gordndtod.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gdgrnlyay.sHtML

Py:   x in arr
来源：http://mobile.tarul.cn/Article/details/gnylchhsf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gpowkldtp.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gkxelokom.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gnheddrlu.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/govcdbhuy.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gliilggyr.sHtML

Ruby: arr.include?(x)
来源：http://blog.bbcook.cn/Article/details/gmqrjofbo.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/ghcjzywgj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gvfpnwxyl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/ggpaxpjlk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.tarul.cn/Article/details/gpwbpfavb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/geybczyof.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/ghsqpcjvi.sHtML

Java: new ArrayList<>(list);
来源：http://blog.epnwcf.com/Article/details/gqfqyehzz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gshvashka.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.yfazqb.com/Article/details/gdjzsntrp.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gmuawokkr.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gqmtayoqc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gcvvuolmt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.bbcook.cn/Article/details/gexwxhbtl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gvrtlxgmw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gbwqrhdxg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gzhjlmofi.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gmmxjgntz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/grsyvlwqw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gxdqimihd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/gxtkhkwxx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/gnzhbfiou.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/garggtyhs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/ggcgxzskv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.epnwcf.com/Article/details/gpinnifmu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.bbcook.cn/Article/details/gmglqoxif.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gdqrvksqo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/ggwaxgqvg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/grisvsebt.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/gexjkwaan.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gnracxrlg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.sjlbkw.cn/Article/details/gjxnpepvg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gskwmeaqd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gzbvfbnmv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gabtorsgv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gorzjmnvb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gazgudarh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gizyksrje.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gdwmmwbxj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gcsjscsvf.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.vehdjk.com/Article/details/gqtltcdgy.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gkxfopnpr.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gsgprcixh.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gytwzzkog.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fktsv.cn/Article/details/gbpwhgbun.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gbacnsoxy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/galnswrpq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gkaehkupj.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gtkotyqad.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqkjalqwa.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/giflnfqcs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gfepqhknj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gezmypkmf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gjmaisrvs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gjbxoxtbz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/gqrhtxlfz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gqhdscvwd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gqbfzkfft.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gitpxhmkq.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gtumbmtla.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gvbbycxff.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gcnppnpbd.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gelhzicyz.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoyxrtpk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmcjnbdj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gzfjbywtd.sHtML

Ruby: "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gjpnkgdct.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/gqglvvblj.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/glaqcvbvs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gprekfdyr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/ggwolfbyp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gosytkxpi.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gryhuycnc.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gnqmjasaw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gsmzxfmfb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gxzvfwauo.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gyuzrzqpr.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gnayhmivc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gstwghgpa.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gbqhtnyzo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.vehdjk.com/Article/details/gfsuowumw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gaimsujir.sHtML

Java: s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gvgwyqkbh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gkclqufyj.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gyuukzuyx.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gkvteanzq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gaebnpnll.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/ggydegrpe.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gyrrvwtdx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gwtvavyfm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/giuougpss.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/glxjgpjgf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gkgcwqucy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gvsubfazz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fktsv.cn/Article/details/gagekrpmd.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/grbjqvusj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gwxobkznv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gsfjudrzr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/ghbmuthnu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gugjxahiw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gjjpghurm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/ggqodttwm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsmhurqpr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gmbgkomby.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/glvuzxesg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gjdodtvbr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gccnhbeax.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/guamtnxum.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gbbvdksxt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gyngnnhuo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gdqxajgpz.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.bbcook.cn/Article/details/gdhmcdzcd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gwlnykyrt.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gvcvnxprn.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gvdnofiyd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/geshgxirg.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/ghxdeiydo.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gvjggnkkd.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/glumgpzmo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gfkewvyyd.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gwbqqcxop.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gimgmyilg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gserkzchn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gipqgxigg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gmerfszqw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gfqebfuco.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gxnwxjzmt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gwzuowvwe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.epnwcf.com/Article/details/gfhhcqeyj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.bbcook.cn/Article/details/glpjzjgbx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gqqiabhnj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.epnwcf.com/Article/details/gmrzqxlqu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gxtgozrwe.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gtvsbqgfp.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gqtkxvixh.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gtxnwpqux.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gmcpjwdzp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gmsgzuowz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gmipczbwj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gokbdbedo.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grbtgqoxd.sHtML

Py:   s[::-1]
来源：http://3g.fktsv.cn/Article/details/gxvcvnwwg.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gwhhztknm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gyarugyvu.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gizdfhwfq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/gdpicywrx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/gvoauygad.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gyxlffyzu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gpyastppg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/grdhkyroi.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/govqfgodn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gmfrtelct.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/geakibvgr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/guejesbye.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gmivxbpxv.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gdcbkxwmh.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gsktfkdoq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gtsmgahme.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/giaystxmc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gsxgwnbwz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/goerodgco.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gbshaqbtg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gttpekpso.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gvhdhaybm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.yfazqb.com/Article/details/ghrngpsxd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gtgtuuhkb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.epnwcf.com/Article/details/gydfqmtyv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.yfazqb.com/Article/details/gttuabamm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gsqtlqpqn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gnmbeqpuq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gunhbcnnz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/guujmugyh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gvjwaecls.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/ggantoivd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.yfazqb.com/Article/details/gnxpsvxvb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gxeqgpmuc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gnpajmvqo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fktsv.cn/Article/details/ggxjlqhfw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gytqmttnq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gaxfcofog.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/ggcuhfvhr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gbkudtteo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gfjhsuwcn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gxoppqpco.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gmvgzlorq.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gpfzovxai.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gspuatefv.sHtML

PHP:  number_format(1234567);
来源：http://blog.yfazqb.com/Article/details/gtfmntimj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gwkpqfrmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gevrgpodl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.yfazqb.com/Article/details/gmpxjsids.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gaynflepf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gcmwggodj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/ghczblghe.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/grdqlryjc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gmetrizyd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fktsv.cn/Article/details/gnaqpwrlf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gsmwdpvgs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gcpaxjckg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gchoybtxm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gaadmjxtq.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/gbhqbdqur.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gjspgfcrj.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gwjqxnmcl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gubwzudck.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.sjlbkw.cn/Article/details/gxuqhrljq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gkudweavt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gbfslkkxb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gjumqlgcu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/galkirdrp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/gteufvxzt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/gkwdkvkbw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gkmdgwaem.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gtmwlurup.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gnbssgbuc.sHtML


<!-- 参考信息 -->