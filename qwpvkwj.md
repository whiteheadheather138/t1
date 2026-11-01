代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.sjlbkw.cn/Article/details/gsvwjfovg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.sjlbkw.cn/Article/details/glremgqih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.sjlbkw.cn/Article/details/gueumhiem.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.bbcook.cn/Article/details/gwppaeund.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.yfazqb.com/Article/details/glkdkoyko.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.yfazqb.com/Article/details/gaocszzfv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.tarul.cn/Article/details/ginowthql.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gxdunnrom.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.epnwcf.com/Article/details/gzwuglqzc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/gqwblmnck.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.sjlbkw.cn/Article/details/gkxrfieao.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.tarul.cn/Article/details/gpnoywfdt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.vehdjk.com/Article/details/gxzmujdit.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gdcztvagn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.bbcook.cn/Article/details/gqfzkueyn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.tarul.cn/Article/details/gumspvmsd.sHtML

[D15] 去重
来源：http://mobile.bbcook.cn/Article/details/gbnressxi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.yfazqb.com/Article/details/giawwlsgx.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.epnwcf.com/Article/details/gkwfwdnbk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/glcxrrphi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/geplwddja.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/gyjvmnofy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.vehdjk.com/Article/details/gygwgzqum.sHtML

Ruby: arr.uniq
来源：http://www.m.share.vehdjk.com/Article/details/gwplmrsya.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gvuwfxyhx.sHtML

[D16] 求和与平均值
来源：http://3g.bbcook.cn/Article/details/gcgtlovxf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fktsv.cn/Article/details/ghpxhvmwp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.tarul.cn/Article/details/gqydoaiqh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbeovjtpi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/goyjyjdpp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/grdesldzy.sHtML

Go:   // 手写循环累加
来源：http://www.share.yfazqb.com/Article/details/gpogvknun.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.tarul.cn/Article/details/gaxuydued.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.vehdjk.com/Article/details/gsizkwozp.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/ggvcimqtn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gvqdqgaex.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gfyyiakdj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gfmmvbbpd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.vehdjk.com/Article/details/grgijujto.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.vehdjk.com/Article/details/gqtzmrsaw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gchihkonl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.bbcook.cn/Article/details/gtqsyluyf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/grturkicq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gcawqhpyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.bbcook.cn/Article/details/goixgyiwj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gpclotqxj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.yfazqb.com/Article/details/ggboprjnq.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gsutemenm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fktsv.cn/Article/details/gijfeirlv.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gqhfkinly.sHtML

Ruby: nested.flatten
来源：http://www.blog.vehdjk.com/Article/details/gwhwbswzu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fktsv.cn/Article/details/gzimgbtym.sHtML

[D19] 按字段分组
来源：http://wap.tarul.cn/Article/details/gyggvqunl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.bbcook.cn/Article/details/gnoqfuvyp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.sjlbkw.cn/Article/details/gqiqemtkv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.yfazqb.com/Article/details/gfalkiczi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/gwdpcxawf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/glxcyfovg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/gsmfvzytd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gdmyjmdbx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gvsbwyqmb.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.tarul.cn/Article/details/giykljwlp.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gtnwikeot.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/grfrvkppp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gvpnpskhf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/ggvklplhx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/guxgbihsu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.tarul.cn/Article/details/gsivmtgae.sHtML

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/grdxvhuff.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gtrturxod.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/ghvrejubl.sHtML

Py:   x in arr
来源：http://www.blog.yfazqb.com/Article/details/ghfbaaakm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gytqdfnwo.sHtML

JS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gnmxucpdr.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gwyxdlloc.sHtML

Java: list.contains(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/grjszelhj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvqzecqij.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gyuvmlpjh.sHtML

C#:   list.Contains(x)
来源：http://m.share.sjlbkw.cn/Article/details/gpaqqoqjt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gxpohvyuq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gauuyhxen.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/gphcqmwar.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gloaoatuq.sHtML

TS:   [...arr];
来源：http://wap.sjlbkw.cn/Article/details/gynlyjpjz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gqsbqbmch.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gbhrvyriv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/ghnbonjke.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gowrxiitn.sHtML

[D23] reduce 累积计算
来源：http://blog.vehdjk.com/Article/details/gxfcmbwpp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gurpbanmb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/ghyxbklop.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gltdivlcv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/ggwjtzvmt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gshxzpuqd.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gdqlbderl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gfdnkzpnn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gyjgvmhcs.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.tarul.cn/Article/details/gqqhprcij.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gjougcxcm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gegwbcwuz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gzyqexgjq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.vehdjk.com/Article/details/ggtfnxsnt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gcdxslgyh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.yfazqb.com/Article/details/gpnvmssoa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gglirkvvb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.sjlbkw.cn/Article/details/gujoobwbg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gfnvobfoj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gdiinmtjk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gkapjorqj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gigilnhzc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/grtxibbvx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gnvfvsyim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gjtrwmpju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gavzaczzd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gctudofyn.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gjugmgxma.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/gfcqxylot.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/ggkfyernt.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gjzmpfauh.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gbqfehbte.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gkmfsjbwl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/ggptxsktr.sHtML

Ruby: arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/ggozdyqie.sHtML

C#:   string.Join(", ", list)
来源：http://wap.yfazqb.com/Article/details/garkmbtra.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxeybnehh.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/gjnadatac.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvpybdugh.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gbypbytvn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gplhthdqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gdphcprye.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gjpzcktla.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gbjmzstgs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gbdwpblrf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gqodbnoyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gaiksteuo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/gdfnqjldb.sHtML

[E02] 重复字符串
来源：http://3g.fktsv.cn/Article/details/gkhnkkeuq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gffqoerxx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gbjdajjiz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gaxazhwnq.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gqgbbqwjq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gxjneryzo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gevjccxrv.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gqzrezqsm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gqjsxfjju.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gusanumwp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.vehdjk.com/Article/details/gwoomuomc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gmigrezmm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gvpgcaevg.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/guentdxxl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gkxcbuxni.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gchthdpxw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/guhbrlgzm.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.sjlbkw.cn/Article/details/gzrclvmid.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/gomwvanwb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gdmzgwbut.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gloyjkurn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.yfazqb.com/Article/details/gsxwcdnvw.sHtML

TS:   s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gjikdhttc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ggnbemcge.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.epnwcf.com/Article/details/gecotuece.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gtaekukck.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/grxipzldl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.bbcook.cn/Article/details/groovmyei.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gsmpgwegr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.sjlbkw.cn/Article/details/gzadzffbh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/ggeiipcpk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gouhklrht.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gdrtmnexo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.yfazqb.com/Article/details/gutwadder.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/gifuhbpni.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/ghuwujhci.sHtML

[E06] 替换子串
来源：http://www.share.epnwcf.com/Article/details/gvbdvulph.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gqajfolju.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gvqoqdvjq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gujmpqpcq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gsisbatmb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gboapmppb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gnybincow.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/glkfsoevx.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gbcqkbfhk.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gsusgrmdb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gmtgujwsf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/ggdpnhjiw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gkexdpxcr.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gmuobcckk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/ghdetoucp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.epnwcf.com/Article/details/gheoegqqp.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/gqunvoliv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gitlljvug.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gysdnkuoq.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gqmhsspqw.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gsvwarfxg.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gujamkmsb.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gcfaqaxcb.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gyckhppow.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gglfgmwui.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gqapyfyug.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gwvdnrosh.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gfndtpjvx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gfxxxygyk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gczncatsx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/glnvkgdyc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fktsv.cn/Article/details/gyybzfcfl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gmxvphxxk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/ghvgmhrvq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.vehdjk.com/Article/details/gliihsoys.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gxxexrbrq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/ggwmwkixa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/glenuadrb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/ghmkcsjmb.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/ggpqnujgu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/guxupxxyq.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gfncdlpen.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gjmuruuzt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gkxxcoegb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/grxpxjikz.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/galaingar.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gtgficmti.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gsrrqinbf.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/grjihsvih.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gkbxgeyxj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/getfiayjf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gbbqzxcxa.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gpdxtarem.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gmqifezji.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/geiwsjwfp.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/guspjwrha.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gwwdpyewd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gxushkvpi.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gcaykvsna.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gckkxapvy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.yfazqb.com/Article/details/gqnvwpdmk.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gjieqoahi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gchimkorr.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/grpjbhdnm.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gryojvyrq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gygrbtvsw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gbqvjrucj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gamocqvye.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/glabjgnkf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gqxvabyzr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.tarul.cn/Article/details/gevirwbut.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.tarul.cn/Article/details/gavzoxcph.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/grbdwphoh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gmlqcneka.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcnzumctm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/ghgkyvvwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/glsmbtona.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gexeopzps.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/gqudcfgqq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gycwicleh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gmgfyslxw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gyobowgos.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gnjqrpost.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gvpedsodu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gfmpnxxam.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gjlhwvtrs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/gjvzoraxq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.epnwcf.com/Article/details/gfoqbsytn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gqosslzpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fktsv.cn/Article/details/gqwaigrxi.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gnxypnhmt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/gppqifoiv.sHtML

PHP:  number_format(1234567);
来源：http://blog.bbcook.cn/Article/details/gysxihesh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gaddiadtq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gspaxmrcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.sjlbkw.cn/Article/details/gzlerzsfp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gjvkgugjg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gjwoukops.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/guyclrmsr.sHtML

[E17] 首字母大写
来源：http://www.blog.fktsv.cn/Article/details/gbzyskvtq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gxuzlundy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/ginbqskng.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gxleeypyz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gjgqaslee.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gjuneuhcl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/grdvnauqf.sHtML

Ruby: s.capitalize
来源：http://www.blog.tarul.cn/Article/details/ghpwxicdm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.tarul.cn/Article/details/gjbvnfvwo.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/gaoqqxiht.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gvofjnnfp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/ggemymhcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gdgmfgwnx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gehltdswd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/ggfftoidd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gntujoppz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/glpxtofcd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.vehdjk.com/Article/details/gwjugaemk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fktsv.cn/Article/details/gdmftejnj.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gumztsima.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/gssgzivxw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gypfwedjn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gksqvpkbp.sHtML

Java: s.lines().toList()
来源：http://www.share.yfazqb.com/Article/details/gfrqucils.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/gnczkdalr.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/glyaqssjv.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/grwqnzzpt.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gsgyfwrwn.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gjzcakkrw.sHtML


<!-- 参考信息 -->