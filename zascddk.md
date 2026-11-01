代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.sjlbkw.cn/Article/details/gdyfhtqan.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.bbcook.cn/Article/details/gwbcquike.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/gcpczelqg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fktsv.cn/Article/details/gzakzptym.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.yfazqb.com/Article/details/garrqrunn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.epnwcf.com/Article/details/gqfjghzte.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gcjkdxzjh.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.tarul.cn/Article/details/gxxtdtglu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/gnrjracdb.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/guobqkjnc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.vehdjk.com/Article/details/gfdfcfteq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.yfazqb.com/Article/details/gvamqgnci.sHtML

[D15] 去重
来源：http://baike.fktsv.cn/Article/details/ggnjgkpkr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gzgxxbzvl.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gowmqqwta.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gligqejlw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/grblpbogy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gofnzpnvh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.bbcook.cn/Article/details/gkselnvck.sHtML

Ruby: arr.uniq
来源：http://m.share.epnwcf.com/Article/details/gjobdlhds.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.yfazqb.com/Article/details/gamgznley.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fktsv.cn/Article/details/gvrlskgys.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.epnwcf.com/Article/details/grqbrdltl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.tarul.cn/Article/details/gmeuuosrp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.tarul.cn/Article/details/guwtpuduc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/gcchijqmq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.bbcook.cn/Article/details/gcqiiuxum.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.yfazqb.com/Article/details/gzdsiqszv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.epnwcf.com/Article/details/ghsvpaddn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gywljbcxu.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gtjnaslrg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.yfazqb.com/Article/details/gckzabbsi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gkkvqmdsz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.epnwcf.com/Article/details/guxztagxm.sHtML

TS:   Math.max(...arr);
来源：http://3g.vehdjk.com/Article/details/gpbmbsacm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.epnwcf.com/Article/details/glmdfgfed.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/gvvzytnin.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.epnwcf.com/Article/details/gmgotmbvy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gjcnlyszn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/glyacfjgs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gyscuvvkk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhhdlcpt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gbvfutmrl.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/ggkbkjiyq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gaiokdcgz.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gzvsyaekv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfywhwff.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gxcxnqbyp.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gxktdcfvc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/gfvqsiade.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gzeadmrtb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.yfazqb.com/Article/details/gcqiiqswy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.yfazqb.com/Article/details/gxebrwlyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/gplbelunz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gteiuyvki.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/gosfhzkqs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gjgvnwlvb.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.yfazqb.com/Article/details/gfxqxisxh.sHtML

Py:   Counter(arr)
来源：http://read.share.epnwcf.com/Article/details/gynixdusn.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/gtawjfmai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gkpolignf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gslrmziap.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/ghouzvmqh.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gmskzagfx.sHtML

Ruby: arr.tally
来源：http://baike.tarul.cn/Article/details/gkhucmwjd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.yfazqb.com/Article/details/gqvqfxypb.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gfevktjkx.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/glpmgooyn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gdkkehipm.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gdhqiwoac.sHtML

TS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gyrzdxujy.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/gtmleqegs.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gmvrdinqg.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gqdwipksu.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/glcfjqxfk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fktsv.cn/Article/details/gspuhdkha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/ggkrxwgzw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gqipdfbij.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gzvbebrkl.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvuwbajqw.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrgcxxdi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.bbcook.cn/Article/details/guqsxzwuh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/grhuyzgrz.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gwuvkyvcm.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/glgxlqjeu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/ggoernobo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gcncfmdna.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gcewpfmbf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gntytyhlf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gjlhtghmg.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gzcamfbik.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gpeqlgizu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gbxbgofab.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gdxgidbxu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/ggxvvdlye.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.epnwcf.com/Article/details/gtqwcmglo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gfdcwcnoy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.bbcook.cn/Article/details/gcrgfbciy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/guzupdnmv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/gllicuhel.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gvqjtiomk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gjjksvrih.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gfdasxyda.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gqmdrrflv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gafbifvbq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gntmteknk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gimuuimtp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gfdkvqqfk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gewourjlg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gdragmzea.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gqqzjvgqz.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gyapaovwm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gmswrliuv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/glqxcfvca.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gknjobbqy.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/grnhidiwm.sHtML

Java: String.join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gefajglvt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gfhbiceom.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gvtacnshr.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gkxriohdr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gytppeqvs.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gosuiscph.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvuccsgum.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gnjjnvdpi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fktsv.cn/Article/details/gmbijeolj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fktsv.cn/Article/details/gsquvsatl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gtclwjcqp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gngxzkepk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.yfazqb.com/Article/details/gpnhvbxos.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/ghgkpyuud.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.vehdjk.com/Article/details/gfwqyncmp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gyzfduosj.sHtML

[E02] 重复字符串
来源：http://www.share.fktsv.cn/Article/details/giuyyckhd.sHtML

Py:   "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gkpiwqpwp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gzrgoxcwu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gkxxoncyw.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gofioqqcb.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gdxoqcspa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gnbtoloom.sHtML

Ruby: "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gpqwoznkg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gtrzmfmzo.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gnswbhbic.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gcwumrvif.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gqqpxfpur.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gzoteosoj.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gfixjjjis.sHtML

Java: s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gyfovvxzs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/grlzzanjh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/glzddgcep.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gpzkajisi.sHtML

[E04] 查找子串位置
来源：http://blog.fktsv.cn/Article/details/greevzjms.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/gruuyavei.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gxdpxqsjq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gxuyuizza.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gwnjmcbuu.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gwhdteqbb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.tarul.cn/Article/details/gxrpnjnyo.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/ghpunhsxo.sHtML

C#:   s.IndexOf("x")
来源：http://blog.vehdjk.com/Article/details/gnptfpodl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.bbcook.cn/Article/details/gpvhoeeuk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gbdqeazhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gfdrrjqpc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/gyzbncfug.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/ggombmsmr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gujksyqkb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/gvjtfwdyn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/gkgibczoa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gmcqceyhi.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gzrziucup.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gxkcpidrt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.epnwcf.com/Article/details/ggzotdhtd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gxjkznjij.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeycptyz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gjxcxhjys.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/giryojzxb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.yfazqb.com/Article/details/geftjhuzq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/gjdoudovl.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gmjpsohab.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gfssiwixh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gqyfvnzoi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/gnxvcwdyh.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/ggzwzweht.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gyhubvnss.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gystihvgl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gyadnnbeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/gjsjiewwb.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/gedbcqnzf.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/ggriqsijt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gixokaghj.sHtML

JS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/glqvpfhmm.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gpjrnowxp.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/gwcgfaobm.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.bbcook.cn/Article/details/gnvohqbyi.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gdqnprdws.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gflrzysgq.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gqtlozxvw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gmyutwwam.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/grrzrybbr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gvcmokjci.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gjbwonpdl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gnuldcqzn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gjxdrlqzy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.vehdjk.com/Article/details/gtkasrtks.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/goyjroycj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/guhswpkbo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gwxegljta.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/geauvnbbn.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gxudgigni.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gauxpobcy.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/ggnujcyyh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gygfjkudh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/glmlhbxzt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/gurzedsmm.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gaspaggsv.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gexpklgtl.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gijyiaywq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gihoayusg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gyelozptc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gtvgjubsn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gqhscqiyz.sHtML

Ruby: s.reverse
来源：http://www.share.vehdjk.com/Article/details/glcbiskat.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gsqmfvgys.sHtML

[E12] 统计某字符出现次数
来源：http://baike.tarul.cn/Article/details/gxqajohzr.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/ggsirzljv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gtjcjosqj.sHtML

JS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gxuhuvwqn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.vehdjk.com/Article/details/gngksojfq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gibbndefp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.yfazqb.com/Article/details/gweoowmlo.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gwdfjiurf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fktsv.cn/Article/details/gjvueekrl.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gsubsxkfk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gcwqjnerf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gnxvjoidh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gcdcedtzu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gzrmaukyu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gmzkuqedz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gempozwzx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/gguhavmpx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gaierpdjd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gcfmoobnh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gntvxuqwy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gelgayrsj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/godjmscos.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gkgsehznn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/ggzchimjm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gvwfudlkh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.yfazqb.com/Article/details/gucutlzpv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gyxlrzgvl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gcpcqvqza.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gqwrymefj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gpkogtacs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/ggiueljdp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/gjtpyvfqv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gfbbfgczg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.yfazqb.com/Article/details/geroxommp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gytfwvied.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gormuqpjy.sHtML

[E16] 数字千分位
来源：http://www.blog.tarul.cn/Article/details/ghiamactb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gxzgipovi.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gjkjsrbyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/ggicwtcyk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gpddcoieb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/goyircvud.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.vehdjk.com/Article/details/gaidlfjpl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.sjlbkw.cn/Article/details/gdqujawcb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gzdfvessz.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gwnljanjw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gxsjupxns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gegnsmgai.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.epnwcf.com/Article/details/gypcagajn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gadktpivh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gxrjxupmp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gdxloqtvk.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/gwdcotstd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gnzbvntje.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gdplagrhu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gjpwagigz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.tarul.cn/Article/details/gzqokttxq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gioqjsjrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/geeojffoj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gmptumhfl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gapviucac.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/ghwgfyvyv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gwzivbtkp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gazaisujc.sHtML

Py:   s.splitlines()
来源：http://read.share.bbcook.cn/Article/details/gjluerpll.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gberizqlz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gitfklhmt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gyefkehkw.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gmimtiuob.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.tarul.cn/Article/details/gukvqshlz.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gvatnrotv.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gyhbvzjbt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/gisaqimxi.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/gbknwfwag.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.vehdjk.com/Article/details/gvigoejfl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/grlsisynd.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gjmqhxxsf.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gqcjcudnm.sHtML


<!-- 参考信息 -->