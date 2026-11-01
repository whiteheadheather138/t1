代发 wailian999

C#:   list.Reverse();
来源：http://3g.fktsv.cn/Article/details/gjgjpehyd.sHtML

[D12] 查找元素下标
来源：http://read.share.sjlbkw.cn/Article/details/ggrtdcqic.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.bbcook.cn/Article/details/gpcgqxuzy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fktsv.cn/Article/details/gewgolitw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.vehdjk.com/Article/details/gagkgcsat.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.bbcook.cn/Article/details/ghsagwpxs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fktsv.cn/Article/details/gqqqtkqzc.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.yfazqb.com/Article/details/gfdpbvzuh.sHtML

Ruby: arr.index(x)
来源：http://mobile.tarul.cn/Article/details/ggxnxrkzi.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fktsv.cn/Article/details/gmuorlufo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.bbcook.cn/Article/details/gwhcuyjfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.bbcook.cn/Article/details/gpzhbbdgv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.sjlbkw.cn/Article/details/gytygsosn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gvoyjkfgh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/ggmunporq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.sjlbkw.cn/Article/details/gzqecywbm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.bbcook.cn/Article/details/gynvmjynq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.tarul.cn/Article/details/grdapacqj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.bbcook.cn/Article/details/givncgbbp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.sjlbkw.cn/Article/details/gctdzedtn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.yfazqb.com/Article/details/gboieazpw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.yfazqb.com/Article/details/gdsjjyhmb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.vehdjk.com/Article/details/granznrdc.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.vehdjk.com/Article/details/guhpotzrj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gkuacwrmt.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gmktqijno.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.bbcook.cn/Article/details/gshyqlqfr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.vehdjk.com/Article/details/gujjhroxo.sHtML

[D15] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gmqblxzee.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.yfazqb.com/Article/details/gsyeahgym.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fktsv.cn/Article/details/grdiegmrl.sHtML

JS:   [...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/gqyqkzgrc.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gnscgyetp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/ggyxecxxd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.tarul.cn/Article/details/gmqmucyul.sHtML

Ruby: arr.uniq
来源：http://read.share.fktsv.cn/Article/details/gkeodtlac.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fktsv.cn/Article/details/gykzdecxh.sHtML

[D16] 求和与平均值
来源：http://baike.epnwcf.com/Article/details/ggnyasafy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gtvzxpuhg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.vehdjk.com/Article/details/glsfwhqot.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/grwzbzklq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gkvnnbyhp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.tarul.cn/Article/details/gmucysanv.sHtML

Go:   // 手写循环累加
来源：http://www.share.bbcook.cn/Article/details/gkfasmfdh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.bbcook.cn/Article/details/gajlhxyid.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.epnwcf.com/Article/details/glfomdkbj.sHtML

[D17] 最大值与最小值
来源：http://wap.tarul.cn/Article/details/gtajokyum.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/gqvthmxpr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/ghlvstzqw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gjmwbzcdl.sHtML

TS:   Math.max(...arr);
来源：http://read.share.vehdjk.com/Article/details/gmojjuqxy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.bbcook.cn/Article/details/ginsbkopm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gxnvcnqxb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.yfazqb.com/Article/details/gdajglpsi.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.yfazqb.com/Article/details/gbzkzogdc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.epnwcf.com/Article/details/gcsczdfmz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.vehdjk.com/Article/details/gmnzkijxn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.sjlbkw.cn/Article/details/gfouzqkgw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fktsv.cn/Article/details/gkhwyreyd.sHtML

TS:   nested.flat();
来源：http://3g.bbcook.cn/Article/details/ggvucgxwj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gglyzjist.sHtML

Go:   // 手写双层循环
来源：http://www.blog.epnwcf.com/Article/details/gipsadkvv.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/ggayzrsym.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.tarul.cn/Article/details/gugecmjhd.sHtML

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/gqyfsvgui.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gigitwyla.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.tarul.cn/Article/details/gtxhpqrif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/goqecmfzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.epnwcf.com/Article/details/girmdtvqr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.vehdjk.com/Article/details/ghqndwcmx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.tarul.cn/Article/details/gbqeepzjt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.epnwcf.com/Article/details/ggpmzaict.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.sjlbkw.cn/Article/details/gatoboils.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/ghwpieyro.sHtML

Py:   Counter(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gedtoevxp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gtnwpcvpp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gexmhpzti.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gzsbytotv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/ggdlztmab.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gsocjemsu.sHtML

Ruby: arr.tally
来源：http://mobile.fktsv.cn/Article/details/gmoybxlun.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.yfazqb.com/Article/details/gvnadoapd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.vehdjk.com/Article/details/gtvthpvim.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gpketdlkd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.yfazqb.com/Article/details/gbikafnlr.sHtML

JS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gvcgdzrra.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/goxyhvvod.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gggoruxtx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtmzuehss.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/guohrqcxx.sHtML

C#:   list.Contains(x)
来源：http://www.share.epnwcf.com/Article/details/gornluiul.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.bbcook.cn/Article/details/gtcklqwqy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/geqowqsaz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/ggfvfboko.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.yfazqb.com/Article/details/gxrglahcx.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/gilaajgsc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gqcufdmbk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gsgvqkmep.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gfyhwmgdn.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gmzgkwzxw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/guzdmptnr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fktsv.cn/Article/details/gzoytnqzf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gnbqepptn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gfutdimrk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gdiqbiyfg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.tarul.cn/Article/details/ggciqngbu.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gevddjepp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gqsgxebor.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gbjfdmbdz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gqqtgtmhj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gnfeahigo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/giutfalyb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fktsv.cn/Article/details/gexvjtkvo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/grmrklgpa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/glkycfivr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.sjlbkw.cn/Article/details/goyoiwyix.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gddfuohzu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/ginekykkc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gpokzweyj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gvhxbiyiv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gswsshuol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/goqaghfqy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/geqvfjhrw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gibqsuari.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/glqdvngau.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/getntxprm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gbwzzzlut.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gumhfpdym.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gmmuroejt.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gdqfbrcze.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gxwacgdox.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/ghyihrgwf.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gjgwguqjx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gyeeufwqh.sHtML

Ruby: arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gygmxzdla.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/ghqeozush.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gkgsijbqa.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gadxkerjj.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsvyofbua.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/gqpskagsw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gdjmjoitt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gxmahjykw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gdmggipra.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gydxuvdjo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.vehdjk.com/Article/details/gneuqnxjx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gensbfkgh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gzdzjudkm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gvqionnhr.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gedpclvxn.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gdkykgymy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.tarul.cn/Article/details/gwwexfqqh.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gpqaqveap.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gclazkpyz.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gurbunecx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gyeiuwniy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gnsbmlkxx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gxijxpagu.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gubnxflwo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gjflvytli.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gjscxaluu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gzmhavdql.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gsommekxl.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gtoesfzix.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gknxandhs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gbmcxjkst.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/guuwodnhe.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/grzvitvxf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gmfdqxkmb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/gqznufotb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gzdwvrxwa.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gppcepvvl.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gspcpkuum.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gozmqksok.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gudtplkcn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/glsyunkfk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gjztlhcbz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.epnwcf.com/Article/details/gctglvkaz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gaykahiye.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/goncprugv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/gehiljvnm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gdccuiomi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/gzimocjca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/gldlibtsw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gevwqipvz.sHtML

[E06] 替换子串
来源：http://www.m.share.vehdjk.com/Article/details/gkhqvxhrj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gkpmhwxug.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gwcperiwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gdsulmxfx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gmlyrvros.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gdazqxnou.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gpjhhyodu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gxaodjosn.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gdvixygsp.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gzzjpvqja.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gunmoprea.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gksuwmxlv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/guijfgwgt.sHtML

TS:   s.split(",")
来源：http://read.share.bbcook.cn/Article/details/gqrapsfmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/guvhbvoxn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gtgcvgipu.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gafxhsjar.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gxfajayhz.sHtML

[E08] 数组按分隔符合并
来源：http://baike.tarul.cn/Article/details/gcvilcftl.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gpaljubrs.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gwrdvkepm.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gmyqwknig.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gbbkvpouv.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gfjviweov.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.tarul.cn/Article/details/gmlnirbxl.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gzixhggfy.sHtML

C#:   string.Join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gvcvzqueg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gxadymxqk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/ghoyzqwby.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gqpxstxjo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gshiejbtn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gvcforgyq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gqtpiiebt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/grmpxmpwb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.yfazqb.com/Article/details/gfgowybso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/gpodirtwx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gmffcnfhz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gvaoooszs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.bbcook.cn/Article/details/gpfwkpyiu.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gihpyjvyw.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gscjxcqnu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gaelepflp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/guwjolzpl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/giuvhfhjl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gciyjflhk.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/geaqpssiv.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gtokvnvlm.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gnzmiurkm.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gwheelxky.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gghnigxxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.bbcook.cn/Article/details/gthmqdvxa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gspryozqh.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gicrnntfh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gmigfwzoy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gujsgesva.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gffgldqag.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gawkkttfx.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gaoshzsnn.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gsjwinshi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gytxmrxwo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gwxtwvtwa.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gnfgkxmah.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/ghkaiejno.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gdazjxrdc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gkzisnmzk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gksygogkt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/guiyroxpd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gntgskzcn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gymfvaudp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gkutkmzgf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fktsv.cn/Article/details/glejzxcwy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.vehdjk.com/Article/details/gtrwajtda.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/gxeyugwat.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/ghupqises.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjwezakti.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gavznbfwg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gixuvdybc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/guiavwqce.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gvpenrxkf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gznignkur.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/glsoqbsap.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gjhqrxrhb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fktsv.cn/Article/details/gymaxwbjg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gfqrtsdvz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.yfazqb.com/Article/details/gsvfcntni.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.tarul.cn/Article/details/grobnerex.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.epnwcf.com/Article/details/gawtbflvx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gajysraux.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.epnwcf.com/Article/details/godlhjhqr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/gpvbwiobn.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gmjpstpyk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/goamavkwb.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gjurehmwy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gsgizycnm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gbghfmdrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gvgiwtslp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/garzzregr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gnzmpqeeo.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gyewikror.sHtML

[E17] 首字母大写
来源：http://www.m.share.bbcook.cn/Article/details/gurnhyifg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gnakkdpcb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gbmbuucdj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gbeqnrvjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/giqaeedts.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gdfayxubi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gpoyrmtia.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gorzknizf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/gakoepwml.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gymrmtdqc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gvboqeqlw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/grfbatilf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/grtculgkl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gngnfdqfp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gyhtpncsf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gzojhghgx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gtkamycyw.sHtML


<!-- 参考信息 -->