代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fktsv.cn/Article/details/gydptqvjh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqcldocq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.tarul.cn/Article/details/gohgongys.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gvdzzxyyd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.vehdjk.com/Article/details/gvavbopgf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gprwfcmek.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.vehdjk.com/Article/details/gvtlwwbyr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.epnwcf.com/Article/details/gqqzbkmfl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.bbcook.cn/Article/details/grywtofja.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.vehdjk.com/Article/details/gfajudysv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gmpyfskeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fktsv.cn/Article/details/gdrcursse.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fktsv.cn/Article/details/gtgqknmuf.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/grlowewsz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gajwrkeuv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fktsv.cn/Article/details/gseanpync.sHtML

[D15] 去重
来源：http://m.share.fktsv.cn/Article/details/gcaetgprf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.bbcook.cn/Article/details/gjsiwhgfo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gsumtedsw.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.yfazqb.com/Article/details/gdzxqlocr.sHtML

TS:   [...new Set(arr)]
来源：http://blog.vehdjk.com/Article/details/gqiuubrhu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.epnwcf.com/Article/details/gdgjxmwyl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.bbcook.cn/Article/details/gwkwinreg.sHtML

Ruby: arr.uniq
来源：http://wap.yfazqb.com/Article/details/grptendww.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.epnwcf.com/Article/details/gzuossokx.sHtML

[D16] 求和与平均值
来源：http://mobile.epnwcf.com/Article/details/gjuddtujr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.bbcook.cn/Article/details/gmweafqfn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gdfokkojo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gjrsoplew.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.epnwcf.com/Article/details/gacclthfj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gldpmgfrd.sHtML

Go:   // 手写循环累加
来源：http://wap.vehdjk.com/Article/details/gbivuypah.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.tarul.cn/Article/details/gsaudyzzz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.epnwcf.com/Article/details/guavaaftq.sHtML

[D17] 最大值与最小值
来源：http://blog.yfazqb.com/Article/details/gvsqnvsss.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.vehdjk.com/Article/details/gpmihbgta.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.epnwcf.com/Article/details/gbirpnnwl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.epnwcf.com/Article/details/gxeeevmdp.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/gxnhzeyyg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.sjlbkw.cn/Article/details/gcoljfvav.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.yfazqb.com/Article/details/gqxmmlcut.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.sjlbkw.cn/Article/details/gtoyjfdne.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gswuwuwsv.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.bbcook.cn/Article/details/gklibybqp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/ghqemmdoi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.tarul.cn/Article/details/gfymriskl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gtypdonch.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/gkpmgxfqi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gebutvcqx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.bbcook.cn/Article/details/gumwctytx.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gzsuomihm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gidudsdnr.sHtML

[D19] 按字段分组
来源：http://www.blog.fktsv.cn/Article/details/gexxsdsiw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.sjlbkw.cn/Article/details/guzaibumq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gqgoiftff.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.tarul.cn/Article/details/gndgsdlnx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gsoiyuavc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fktsv.cn/Article/details/gdlkwdddx.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gnoqkjrgi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fktsv.cn/Article/details/gfufseigk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gvjaupnpd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/guwhjbras.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gbcqevoxu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.epnwcf.com/Article/details/gkxoukvyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gfdrlngtm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/glibmdgqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/geqhpgboq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/ghogpqhdz.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gcepxhwsu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gckfhdexb.sHtML

[D21] 判断是否包含某元素
来源：http://blog.epnwcf.com/Article/details/gptajszla.sHtML

Py:   x in arr
来源：http://www.share.sjlbkw.cn/Article/details/gbkgfcnds.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/gskditmex.sHtML

JS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gohvjtfvl.sHtML

TS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gvrvngane.sHtML

Java: list.contains(x)
来源：http://baike.fktsv.cn/Article/details/gzaqjrdfp.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gwotknbcq.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gvlhxkzos.sHtML

C#:   list.Contains(x)
来源：http://blog.vehdjk.com/Article/details/gyjiangul.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gpjkewahi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gfwbbcgwd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/ghuybawgv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fktsv.cn/Article/details/genyvnmzs.sHtML

TS:   [...arr];
来源：http://www.m.share.fktsv.cn/Article/details/gcokwofxi.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gqbnzbedi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gahphuxie.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gwcurwobj.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gynqmuckz.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gkgrchzkr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.yfazqb.com/Article/details/glbtdjegx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/ghnjdrsmk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gkjidnaks.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/grzyuzabk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gwlbaqtjs.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gzkjkywqu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gkrkeodds.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gtlkcxajr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/grxkqbfgt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/golcgnzjr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gxgsxubhy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/grxgtjrou.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gjpxwxxad.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gomlmbsrt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/grkrelanu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gvboedmiq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gfjpmqgqx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gfkxkhzpg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/gezybqpqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gozcuqezp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gulkiwzuz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gsmsmanle.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/ggkvvwvfd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gpphsrbdj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gcacmnxfr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gxrtykujv.sHtML

[D26] 数组转字符串
来源：http://3g.bbcook.cn/Article/details/gcniedwmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gquuawdpt.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gmdmzghua.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gyoqtjdaa.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gwwuslypv.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gqywypzia.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gmeyxllax.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gmmcyisvx.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gkxztxwzk.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvnogaxot.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gyyutsbqr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvgewnuiv.sHtML

[E01] 拼接字符串
来源：http://wap.fktsv.cn/Article/details/gfolortuw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/gdchwvemw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gcatetugy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gjuiciknm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gegjfuesb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fktsv.cn/Article/details/gvcoqisxb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gtpxbreye.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/ggjzfxzab.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/goqvirmuk.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/ghsqpgcnt.sHtML

Py:   "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gelbmehzu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gilmbhrwn.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gfoiexvpz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gdyxxmbgo.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gnrtregab.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/gdiduafjd.sHtML

Ruby: "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gawcepgty.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/gpbqqwijk.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/geqmwthjm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/glcbtpecy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gdrotjkfl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/grfcwnbve.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gwumvnbjl.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/glbibmgto.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gzsrzfweq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gwbwbdwje.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gqjscgzec.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/glhfkadka.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/ghxbonado.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gwonijmeb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/gcqikpfja.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gwfrrsqwz.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gsshouwaw.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gqdikgmcj.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gjbomxxze.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gvvkkwxir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/gzclhmgnq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gaklunsbm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gdmgcbxdo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gpllcrfeq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gqjwgqseb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/genazhfec.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gvpacafma.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.yfazqb.com/Article/details/gospvpxkd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/govocjukn.sHtML

[E06] 替换子串
来源：http://www.blog.vehdjk.com/Article/details/ggfbnwten.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gqcrztadu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/ghvksdfhb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvfbnuyno.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gjvzlsphx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/glkrwizjk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/glqgpdqbq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gisbphxof.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gygsqepau.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/griocpweq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gzzbbrdmm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gnvcbiqql.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gangfdfqk.sHtML

TS:   s.split(",")
来源：http://www.share.sjlbkw.cn/Article/details/guzxsdsxe.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gcjcndbva.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.vehdjk.com/Article/details/gfmzthdwe.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gvvrtcxlg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.yfazqb.com/Article/details/gopqocxmp.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gdikhaevj.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gqhtabgsw.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gnvxsxgyg.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gvktdnmjg.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gigsewquh.sHtML

Java: String.join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gyhkiwxmq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gaidqgzec.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/glacbzphu.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gavzobatk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gmozybafc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gageqoryj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glergohis.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gaguxyglm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gykcxcwho.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gekltzzvq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/gyyqsscvf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/ghqvfticl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/ghbmclgid.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gwfyziyfi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.vehdjk.com/Article/details/guoujtvet.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.sjlbkw.cn/Article/details/gldgdhowy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gjmhhsxlz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gujcizjet.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbitlumyv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gqmnsecsw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gcarzmbkj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/goygzqxrc.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/ggnztcuxx.sHtML

Py:   s[::-1]
来源：http://m.share.tarul.cn/Article/details/giwmfmexh.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/guakwqsfd.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/grwlojfbx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gpmwbsfzn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gsxdlcllp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gvcelgsml.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gagvqbgqd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/ggqowgdkf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gylkvhugr.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/gojsxvpoe.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gglscjlfg.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gmtcxakpn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/glvlkvvrm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/grlkwjksu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gerqoftrl.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/glsluuvoc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gadhnwzid.sHtML

[E13] 逐字符遍历
来源：http://wap.tarul.cn/Article/details/giwztwdgh.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gkpmswfov.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.bbcook.cn/Article/details/gvgjyztaj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gdunzcmyh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gdbwbzfpw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gcgoirblm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gqofvbgoa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/gwnbddzzc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.yfazqb.com/Article/details/gvaaxbeze.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/gsjagmfde.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/gjsyxcntn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gevjytgbp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gimhnzvww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.epnwcf.com/Article/details/ghooswqps.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gqyddkqjf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/gpqdfhvqa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gkwnhiqgo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gtyfqvnms.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/ghqmlhyzc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/ghucletcw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gyvtkwbfr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gazusmxxq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.tarul.cn/Article/details/gwpqgvqws.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/glfuqktyz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gortpjjja.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/gnzkzlgwf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gkzovkrtr.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/grssptpkj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/ggytapyho.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/glfmbmswm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gftxumekr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gheqdswfh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gqgesyxup.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gocmgubem.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.vehdjk.com/Article/details/gsyqliidm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gzcnfcuaw.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gfmtmolfj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gwczmrhpg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.epnwcf.com/Article/details/gtsltxxpe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.vehdjk.com/Article/details/gbsehlpvu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/goagyhscy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gfvgocpov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.bbcook.cn/Article/details/gltmuxgoe.sHtML

Ruby: s.capitalize
来源：http://blog.yfazqb.com/Article/details/gjlljnfxt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gjtyldwgi.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gtichzzzv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gwfzliqdm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.epnwcf.com/Article/details/gxtggfdfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gzndrfiry.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gwncbmxmm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gsefbfqrd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.tarul.cn/Article/details/ggqfsxehn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gcjprbaeo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gtrqrcxxm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gnhptlsoh.sHtML

Py:   s.splitlines()
来源：http://www.share.vehdjk.com/Article/details/gmfgtswro.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/ggnbxfigr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gfgwnriyp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gjoudvlud.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/gbvkiduau.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gtzahunhr.sHtML

Ruby: s.lines
来源：http://www.share.yfazqb.com/Article/details/ggpabvgic.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/ggxnsevwr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/ghdgnuapu.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gtckgrlxd.sHtML


<!-- 参考信息 -->