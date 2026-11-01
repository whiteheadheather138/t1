代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.tarul.cn/Article/details/gtixyktyx.sHtML

Java: Collections.reverse(list);
来源：http://wap.tarul.cn/Article/details/ggifpnkfx.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fktsv.cn/Article/details/ghllptrdw.sHtML

Ruby: arr.reverse
来源：http://m.share.vehdjk.com/Article/details/gnwrrgvbc.sHtML

C#:   list.Reverse();
来源：http://3g.yfazqb.com/Article/details/gvzltpzyf.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gzvkjnysp.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.tarul.cn/Article/details/gouepezck.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gugmkhkpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.yfazqb.com/Article/details/gormbbxqq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.tarul.cn/Article/details/ghnttuygu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.tarul.cn/Article/details/gjlutdoho.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gjutopvve.sHtML

Ruby: arr.index(x)
来源：http://wap.bbcook.cn/Article/details/gwzfzobzu.sHtML

C#:   list.IndexOf(x);
来源：http://baike.bbcook.cn/Article/details/gbunsbhtr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.epnwcf.com/Article/details/gumwhkjpa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gafravrtl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/guwhdtlut.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gsrcfjjxd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.bbcook.cn/Article/details/gnedzvpzl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.bbcook.cn/Article/details/gglqeuwve.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gddckbbmx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.tarul.cn/Article/details/gqhunvdbm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/gghedbqlf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.vehdjk.com/Article/details/grjiairsx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.vehdjk.com/Article/details/gxaaxuxbw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gtywpuxdy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.vehdjk.com/Article/details/gbnrzfats.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/gnujgybep.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gkgabnbui.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gcjgrkbnv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gnnbbqgal.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fktsv.cn/Article/details/gazaqihur.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gkpjhinrj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gflzuvzyx.sHtML

PHP:  array_unique($arr);
来源：http://m.share.bbcook.cn/Article/details/gidbskvnu.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/glfacvofm.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.bbcook.cn/Article/details/gxxlykhzi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.tarul.cn/Article/details/goywbifap.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/gbyhnlzgz.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gncrjnjzx.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.epnwcf.com/Article/details/gusncetgo.sHtML

[D16] 求和与平均值
来源：http://3g.yfazqb.com/Article/details/ggnavpmuq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.epnwcf.com/Article/details/gsejdnuck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gmzoefqts.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.bbcook.cn/Article/details/gceksvwnt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.epnwcf.com/Article/details/gsrpdwguq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fktsv.cn/Article/details/gnwhjmovq.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.epnwcf.com/Article/details/gktgxqyaf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fktsv.cn/Article/details/gizmtksvt.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.epnwcf.com/Article/details/gpsfopsqk.sHtML

[D17] 最大值与最小值
来源：http://mobile.epnwcf.com/Article/details/gzjnghkki.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdboloebb.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.epnwcf.com/Article/details/gbhwnovhs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.vehdjk.com/Article/details/gcdebmzau.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fktsv.cn/Article/details/gmflyvfdm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gdcgzbcmf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.yfazqb.com/Article/details/gannlaydd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.vehdjk.com/Article/details/gkznohulj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.vehdjk.com/Article/details/glhoobhzc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.epnwcf.com/Article/details/gdxdsddsm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/gntmizqri.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.vehdjk.com/Article/details/gqxuxblfp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gqpyaxaux.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/goutuubgs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gesappgyv.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gpetrimwd.sHtML

Ruby: nested.flatten
来源：http://m.share.bbcook.cn/Article/details/gnljurhnu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gqikfgvet.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gvmrcxzpg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fktsv.cn/Article/details/gegjqhmts.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gomvtvmqw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gajjplxtf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/govifumwc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.bbcook.cn/Article/details/gefanhkjt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gjaqfiqof.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.bbcook.cn/Article/details/gyrednhjb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/gpzejsdyq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gmuvxwggi.sHtML

Py:   Counter(arr)
来源：http://mobile.fktsv.cn/Article/details/guiisiytk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gnvryhfya.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.bbcook.cn/Article/details/gblfivjyv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gdpdqcgtr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gsedfiqoh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.bbcook.cn/Article/details/ghftsyopb.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gkccdkvok.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gauohngqs.sHtML

[D21] 判断是否包含某元素
来源：http://wap.epnwcf.com/Article/details/gfvdjvgpv.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gtmppkoux.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fktsv.cn/Article/details/gxenmafrj.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gtbdvqpso.sHtML

TS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/gvyamclxm.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gohobdvmh.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gxajrahkq.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gkdzsqgwa.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gnfnqimmq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fktsv.cn/Article/details/gkloplykz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/guyvxwcyl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.vehdjk.com/Article/details/gfthzvbos.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ggxfehzcx.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/gxtdvjupj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/gmllgflyu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gpzzjzzbe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gxveawapj.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gnjteyymc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gjglnadnx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gnytxuofr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gmmxdvazr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gtdhoxqbp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gyudteofq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gjcitkqqj.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/gmgybamzj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.vehdjk.com/Article/details/gqnxfqolb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gdksfbtni.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gmjfneojt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsaznwgp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gtpptxcnc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gktivfqgs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gygjhzrvg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/goxgzuokt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gvujhxhmj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gwqswbqac.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fktsv.cn/Article/details/gcaqmllkq.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.tarul.cn/Article/details/gayvqjqky.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gzwlifxtw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/gjpmwfhjv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.bbcook.cn/Article/details/gbzqufgoi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/gpilipsec.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gayercgfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gkuudkqem.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/gjyqsrsvz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gmdnaaakz.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gvgtxresd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gtmcibdpu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gvmepxldb.sHtML

JS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gnwwfxond.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gbcwrqnis.sHtML

Java: String.join(", ", list)
来源：http://wap.bbcook.cn/Article/details/ghjfyqyxp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.vehdjk.com/Article/details/ghcopnjuz.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gxsbceqof.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gwzzceyih.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gbhvgzwil.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gvyejolxg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/giszbncum.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gcirkrjxj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/gnunjkyev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gkobtgxqj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gteivbpnn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/ghqrxsxka.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/giczroffh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/gizdoddui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/geeyrbdur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gxymeelbg.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/grzxwrxdb.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gqspmyoby.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gsdtmackk.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/ganzxbked.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gkkbtzyww.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/glanzyszi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gfvximxzp.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gyzhnhavv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.bbcook.cn/Article/details/gwqrvtqqq.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gnjvsdeib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gwgibabvn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/grlkjsppr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gxzvkipka.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fktsv.cn/Article/details/glkobjrxs.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gocxcllor.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gaqbyodvp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/ggatevped.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gflqhaoys.sHtML

[E04] 查找子串位置
来源：http://mobile.sjlbkw.cn/Article/details/gxjcafeoc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gnltdqobe.sHtML

PHP:  strpos($s, "x");
来源：http://baike.vehdjk.com/Article/details/gdvfypxwm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gqwdnyyhg.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gtscivygh.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gnojixmlu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.tarul.cn/Article/details/gkpcvuolg.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gtjkmsjpq.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/ggcjhphqd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gprtihflm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gkzcrmdai.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.sjlbkw.cn/Article/details/gmtjbzyeq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gnkwwmsop.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gkzpjhhpu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gyxsfucta.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gaqqvwecv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gupwgkhtc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gflctolbo.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/ggtnjrnhy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gykkklphn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gtdeofdjo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gwdqwfjqn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gwrrqswyd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzdovexq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/ggcijlzjc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gkchccyoq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gpwsdjohm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gltocmtqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.yfazqb.com/Article/details/gfloiapnk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fktsv.cn/Article/details/gosmjlzjk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/glxoqwhxh.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/glgcynqlt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gcvfcgmpu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.vehdjk.com/Article/details/graklmjst.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gidmvmftv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/guyozjxlc.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.bbcook.cn/Article/details/gmxsxvymw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gdamsucsk.sHtML

PHP:  implode(",", $items);
来源：http://wap.tarul.cn/Article/details/gssuirhrx.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/glfraucks.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/ghonpwsoo.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gzdhedfnb.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gdjxnrfwh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gltkagthx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gnvasbcpf.sHtML

[E09] 去除所有空白字符
来源：http://m.share.bbcook.cn/Article/details/grwofkqnz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gfekhhxaz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gbujnksvc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gihcxldju.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gdhealohw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gpvxsheqj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/guvhejpbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gytldgynl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/guyoflifk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gixqjdqfj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gsvtcwjap.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.yfazqb.com/Article/details/gcunprsvq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gogfimewe.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtcuydkta.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gzaoulktv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gowwlkmxr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gnxeexurl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gsakizjot.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/gclnubabg.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/guvotzuwz.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gixflbaww.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gamtfktfw.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/ghmgcqndo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gfmpibtwz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/ggglabejt.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gnwzuwymm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gjcoktpzl.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gyfqhfjzz.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gwmkthzoo.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/ghguuuxjw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gtxebtbbu.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gwvntgxdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/gultygxsf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gfjbrzotf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gjlokvypd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gmaifkrbu.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gznuimdby.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/gznmfptbg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gecdvcalq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gqoyjzigf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitskrhmc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gpwzipknt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/guydqoonu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gtrmpdvec.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/grghhifqt.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gcyjtejnk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gyuytepun.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gnpbhbhwd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gfsgocemg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.bbcook.cn/Article/details/ggqrikobc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gyntppcev.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.yfazqb.com/Article/details/gffzhztta.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/ghgpfrtlj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/gbeokfxuc.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/grweasyak.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gnmabtsbf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gbktijlzh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxihxcgxo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/ggnovhqli.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gzkkuujgg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.tarul.cn/Article/details/gszkxeqeq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.bbcook.cn/Article/details/gdjqhtrve.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gvcuenajl.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/ggnyxhyar.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gonhabszk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/gdtxjwlyf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gtsakurmy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gnuudfwrb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gybcrzlgp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/guxhbllyz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.yfazqb.com/Article/details/gdbcltpaw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gswzhlknw.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/gvrucyche.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/glypqgnki.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gavyzzder.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gtdjnkyxg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gfelowosn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/ggupvlymt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gqldykmhm.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gcgdlwock.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gpuvlckue.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gywtksfmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gxjoxtalh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.epnwcf.com/Article/details/gxtkcvusf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gnxoakxic.sHtML


<!-- 参考信息 -->