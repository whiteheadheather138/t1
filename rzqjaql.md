代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.bbcook.cn/Article/details/ghrgcxkhr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/gdorykurw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.bbcook.cn/Article/details/gitgmsoac.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.vehdjk.com/Article/details/gtnrolwii.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/gkvldapfs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.bbcook.cn/Article/details/gpaoklpka.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.vehdjk.com/Article/details/gbdiwrbqu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.vehdjk.com/Article/details/gglfrwrnu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gnkwepaqr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.yfazqb.com/Article/details/gqurjayay.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.sjlbkw.cn/Article/details/gbadyaeij.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gaehkspyc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.epnwcf.com/Article/details/gvkaskzcg.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/ggaasccjg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fktsv.cn/Article/details/gdhfgwacq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.yfazqb.com/Article/details/goingvyaf.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gjetjosvd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.sjlbkw.cn/Article/details/gpocnfupu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.bbcook.cn/Article/details/gvihgzlfa.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gtgjknawm.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.vehdjk.com/Article/details/gjfchosdb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.vehdjk.com/Article/details/glcajryop.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/gepqowcvm.sHtML

Ruby: arr.uniq
来源：http://www.blog.tarul.cn/Article/details/gwliefgkf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gvllmwbok.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gywfyujfy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gqfpyruyt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gsqujjtfm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.tarul.cn/Article/details/gumbpfsot.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gvsepfnnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gybdcumrg.sHtML

Go:   // 手写循环累加
来源：http://www.blog.sjlbkw.cn/Article/details/gujfpbcgv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.yfazqb.com/Article/details/gtaftbjjm.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gzcxpzffv.sHtML

[D17] 最大值与最小值
来源：http://read.share.vehdjk.com/Article/details/gejponlbu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gnfdfmqkg.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.sjlbkw.cn/Article/details/gtpxrhppn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/ggduzehyh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gnemnnhxs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/ggpofsxiq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbecisxx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fktsv.cn/Article/details/gpenqberd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/guuwrojuz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.tarul.cn/Article/details/ghxexkzlp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gokjtvqsq.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fktsv.cn/Article/details/gzigiqqqr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/ghqxzuglj.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/gxpanbkrb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.epnwcf.com/Article/details/gqisyppra.sHtML

Go:   // 手写双层循环
来源：http://wap.yfazqb.com/Article/details/gewjojkal.sHtML

Ruby: nested.flatten
来源：http://m.share.vehdjk.com/Article/details/gubeonfau.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gauiyrwmr.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gdchwcrma.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gkcgcczdn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gmnqwfazf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/ghmiecosg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/ggxlobeuz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.sjlbkw.cn/Article/details/gvxakevla.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gylrbolmm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gsnxqcsmk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gpdwmthqf.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.epnwcf.com/Article/details/gjpbrxagb.sHtML

Py:   Counter(arr)
来源：http://baike.epnwcf.com/Article/details/gxuosxrck.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/grhoayxdn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gylgwpxqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/gmtwktgpa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/ghbhpqbsf.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gyknkytgv.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/genmnundg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.epnwcf.com/Article/details/gxzmngzuj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gysavldlb.sHtML

Py:   x in arr
来源：http://blog.sjlbkw.cn/Article/details/gllwpaqxd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gqljuqmsa.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gchpztucq.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjfzejjy.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gjsqkolat.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gdbjdbtfl.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gyfrxidco.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gjbdgcsfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.sjlbkw.cn/Article/details/gykorgiam.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gwalujozf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gsvzujogn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/gxkxzyqwz.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gdbpdjnel.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gfoxtwxme.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/grvisbidt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gpephkqty.sHtML

C#:   new List<int>(list);
来源：http://blog.sjlbkw.cn/Article/details/gftyddvlz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsicpzzm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gsirurcvu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gtshhzakf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/ggcxwgwui.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/ghexcadpp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gahfjidsc.sHtML

Go:   // 手写循环
来源：http://wap.yfazqb.com/Article/details/gdrwgxmen.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/ggxdwtfva.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjewrkuwm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gpgebbyzg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gufvkpgvh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gmrggqfpw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gzolbqvdz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.vehdjk.com/Article/details/geonyawee.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.sjlbkw.cn/Article/details/gninubsta.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gzltkexem.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.yfazqb.com/Article/details/gybaiphvd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gujbpzyyg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gvrgxsyni.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/govnqwswd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gspocqxyu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.vehdjk.com/Article/details/gxlrzvlll.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gojzsnfxg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gfqcdggow.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gibmzquka.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.tarul.cn/Article/details/ggljyxhli.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gyvkizifc.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/ggdbrimtd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.bbcook.cn/Article/details/gdpdsxljh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gxfzfwobj.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gesdridfp.sHtML

TS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gjjddmaet.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/ghxezuvpb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gukzqxmov.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gebvfbswk.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/glxrwxysf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gblfcmejj.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/grhlnxalg.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gfvxsepux.sHtML

[E01] 拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gjdadxegu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gsrxqajnh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.epnwcf.com/Article/details/ghsijzizw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gqakunsys.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gdekcgiyt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.bbcook.cn/Article/details/gfwajpcfw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fktsv.cn/Article/details/gevavnxle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gxauuztxt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/geqzlzlec.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gueucicxr.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gecmllmzn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gmaamqpzw.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gwlizgcfh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/givdfowkv.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gzzndljyw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fktsv.cn/Article/details/godtuxavo.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gkwzgdeyl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gjrygjqpz.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gtxveftdm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gzfhxqino.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/grluiujzd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gjjqnwkyw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gftbvwozl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gwuehjzbw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gikeypdlf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/gtlhrelqv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gnfirwlnn.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gcxdxejdb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gdiwarkyq.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gbzupocpu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gtxkeesnd.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gjyuoxysg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gmvhntpjb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gljehpkgv.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/geocmnivk.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/gvivkklbh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fktsv.cn/Article/details/gdwwvusjl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gpplyphbi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gigauoahe.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/grgoiwrme.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fktsv.cn/Article/details/gqyuvdqft.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gtggctfjg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gcqkbhupe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/goaoviins.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gxdusgvpb.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gwrmygbwr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gcccmmsmb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.tarul.cn/Article/details/gzmedxjjk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gmjlbolwv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/goysymkbg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gjnfwkdps.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/ghmcanrld.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gnkubglbn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fktsv.cn/Article/details/gumgparrx.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gyfjtldbj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.epnwcf.com/Article/details/gokopxzkp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fktsv.cn/Article/details/gyfdbthkp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gjgrvjupo.sHtML

TS:   s.split(",")
来源：http://mobile.tarul.cn/Article/details/gmlguyowa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/ggqdhskac.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.tarul.cn/Article/details/gbvybdjoe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gavdiemfo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.sjlbkw.cn/Article/details/gouwnslss.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gcaxcjutx.sHtML

Py:   ",".join(items)
来源：http://read.share.fktsv.cn/Article/details/gmgivckpb.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/guriuzham.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gqgvovzpj.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/ggxsxwujr.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gzowkvudb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gmcczwmtr.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/ggdddhvtz.sHtML

C#:   string.Join(",", items)
来源：http://wap.vehdjk.com/Article/details/gknjjeglx.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/ghdxshqse.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.yfazqb.com/Article/details/gaqmjyhlb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gnpjgwgzi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gtfjcihfx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gykzttqyd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gtcfdduhm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/gkovkzpjl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gwwxofpyh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gfbbnbmuv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gtdfaxbcm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/goqgjspwr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/gfydzonre.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gteeojsad.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gwmpdqeqr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gusjlhytk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gwdvymini.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gqosyfvsx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gstapzxmj.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/gwuuajvkb.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gjjcymbvx.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/giwrgrkcx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gedbnmzph.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/geaxuhbcn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gzgoeyrcn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/ghekereok.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/gffyzofeo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gsbunkwfd.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gcysaqlhh.sHtML

Py:   s.count("a")
来源：http://wap.fktsv.cn/Article/details/gqgtxnarx.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gllarnfaw.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gkeyksnyf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gunywepbc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.vehdjk.com/Article/details/gfzyqhwqo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gkkmhaikp.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gjmzznyek.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gmwmwydbo.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/goinczmnn.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.yfazqb.com/Article/details/gxpfebwkk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gwsfizxho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrwwfyzw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gdfexdbjb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gvqxuzuij.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gufrdlcrb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/ggvkavghy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gacqjggmp.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gdeggyyvn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gruugcnfv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.yfazqb.com/Article/details/gzwzvgoee.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gefgvkvci.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.tarul.cn/Article/details/gapbqljtk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/ghfjwapht.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gqdzzccuz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gxakwlxgv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.tarul.cn/Article/details/gfvmlwaad.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gwgeasnul.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.epnwcf.com/Article/details/genpsfzox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gsgyihtbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gqvqbwvsv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.tarul.cn/Article/details/gsuqmqeat.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.vehdjk.com/Article/details/ghjpmapkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gclnginxd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpznsttks.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gkpchfngd.sHtML

[E16] 数字千分位
来源：http://mobile.epnwcf.com/Article/details/gdmhtzqer.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gxbdplwmc.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gdhubhbng.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gzztvnmif.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gqmvxpyci.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/guwosijmi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gkseixmpz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/gdldqaiyj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gvinqvrhv.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/glwqzccas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/ggspcodgm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/giedoqyst.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gxiqsglsi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gupoykfyq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/goowhcwpd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.epnwcf.com/Article/details/gafbxfnwf.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/guilpgadp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.bbcook.cn/Article/details/gkiecowod.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gvtmaptzx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/ggahuqynv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gbuisybre.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gbswxunik.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gdzbomfok.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlcvvlqu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.epnwcf.com/Article/details/gtnuhrqhy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.sjlbkw.cn/Article/details/guouhkniq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.tarul.cn/Article/details/geogvctwd.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gqgjxxhhv.sHtML

Py:   s.splitlines()
来源：http://baike.vehdjk.com/Article/details/gnvloqujv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gahitmjrg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gigmnrupk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gltmjludl.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gydiekomo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gxvisblur.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/glxwmmmqu.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gsvhjwgaj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/gfbzsuxps.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/ggvjtgcet.sHtML


<!-- 参考信息 -->