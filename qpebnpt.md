代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.bbcook.cn/Article/details/gefoczbqy.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gkfdnxgnv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.epnwcf.com/Article/details/gdojxrnha.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.bbcook.cn/Article/details/gguokygkx.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gtgfueyid.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.vehdjk.com/Article/details/gpwvgtvde.sHtML

PHP:  array_unique($arr);
来源：http://www.share.yfazqb.com/Article/details/gvadkwfbh.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gbdlctxjd.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/golampjao.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.vehdjk.com/Article/details/ghpzpwrzi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gbavwosnf.sHtML

Ruby: arr.uniq
来源：http://baike.epnwcf.com/Article/details/gjinqatop.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.vehdjk.com/Article/details/gyrndndys.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/guvcmheye.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gyikzikcc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gtiudsmac.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.epnwcf.com/Article/details/gqommgesf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/golmkwfle.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/ggkfcqcse.sHtML

Go:   // 手写循环累加
来源：http://m.share.epnwcf.com/Article/details/gprjhwdlg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.tarul.cn/Article/details/gydayebap.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/grqkdnkng.sHtML

[D17] 最大值与最小值
来源：http://baike.bbcook.cn/Article/details/gpxzbeesp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/gfciiykjz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gwjomksyh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.epnwcf.com/Article/details/gtpdrrdxc.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/gfmuuqanl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/gpobcryae.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gcbrwebme.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fktsv.cn/Article/details/gdqkvmykb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.tarul.cn/Article/details/gxtncshfa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.tarul.cn/Article/details/gvctxtkpf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fktsv.cn/Article/details/gmxraszrk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gaxeyspjb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.sjlbkw.cn/Article/details/gqvomrseo.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gchcbmpzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.vehdjk.com/Article/details/gjiazgtrw.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gjabgmxxg.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/gbxxqloll.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.vehdjk.com/Article/details/gnyfvqihh.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gtzekbvrr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.epnwcf.com/Article/details/gcyzparud.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fktsv.cn/Article/details/gvtvlydnu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.tarul.cn/Article/details/gmnrktctr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gpyozwzth.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gimlibncf.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.tarul.cn/Article/details/godukovmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gmxeivulc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/glmifvoby.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gzxxugorw.sHtML

Py:   Counter(arr)
来源：http://www.blog.epnwcf.com/Article/details/grhhgvyal.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gkpcjfgpx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gsnxftzjw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gnnndcmad.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fktsv.cn/Article/details/gsocxymvs.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fktsv.cn/Article/details/gnbvklyhs.sHtML

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/gkyntpift.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.bbcook.cn/Article/details/gxmmemhdx.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fktsv.cn/Article/details/godsznbyk.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/giffewkzn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gqhfffchk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gvsxyeieg.sHtML

TS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gqeffrkwz.sHtML

Java: list.contains(x)
来源：http://3g.yfazqb.com/Article/details/gujosqduw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gjymmamkv.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/grchhecum.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gdcoocwde.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gtrrlxrdc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gvvaufafi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gheahnkec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gypufquuj.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/gzveeqsyq.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gvnrcbrag.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gopkzuvkn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.yfazqb.com/Article/details/gfiouxccg.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/gkjdpbtuu.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gisjjcext.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gesewsnnr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gdhcftmoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gmozljnjm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gswsxnacj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/grptjzehg.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gcxlkjwtk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/glwjgozsq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gopciuhpu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.epnwcf.com/Article/details/ggqebtwqo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/geophqezu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gyurvkuhs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gtmihnjuf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/gzibtplhr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gsnvhdelp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gzvqyhgvg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.yfazqb.com/Article/details/gpbxwbfgm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/grmfflkul.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.yfazqb.com/Article/details/gtsgvkugn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gyoevqoum.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.tarul.cn/Article/details/guyiwwadf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gzppqsxcv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gashgzowx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/groseygxt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gnbkrvaoy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.epnwcf.com/Article/details/gfhfpmccf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gysdbeedl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/glvvuplvb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gitdunafa.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/gstvxapam.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/ghxyspaha.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gmicislic.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gvwttzdvj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/ghmnsjlcp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gguwljcoi.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gsauogdcx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmonlwdac.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gsqfiwyyt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjdmgoaug.sHtML

[E01] 拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gtbqwnffo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gkimlylkz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.bbcook.cn/Article/details/ggbmuzapx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gxhunuycq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/grdlnppdr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/gqfckqozb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gunhttrnk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gvbqxvxea.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/ggggddukl.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gidzfwndo.sHtML

Py:   "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gvyynwfxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gvmwghteg.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gpidzdobv.sHtML

TS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gwzrlhcyk.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gnvlpjqgo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gacqubjvh.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gqkospijo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/gykyxhdfk.sHtML

[E03] 截取子串
来源：http://m.share.vehdjk.com/Article/details/gvaqoione.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/gozgxsubl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gcvopgndo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gixgqlsyz.sHtML

TS:   s.slice(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gfucxygzh.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gvbvhwfur.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gdwrzqdrb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gxokjjfsv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gqaarpyul.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gabfsfhib.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gvvdkjtzx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/glxwfcvrb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gtsnhydph.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gaapnjyot.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gpomijdek.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.epnwcf.com/Article/details/ggakuoxej.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/ghpewlgqf.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/goeegqazn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/golicczgw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/grudtokmk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/giikzwbbd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gwtmsznwb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gkplkjzwc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/ggiwxozkn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/gsbplygkg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.yfazqb.com/Article/details/grfrmlgcz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gqyefikcw.sHtML

[E06] 替换子串
来源：http://baike.yfazqb.com/Article/details/gdactilnp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gxdpybmrr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmnfqjhun.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gcreiumas.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/goexoggdv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gyewdqvga.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gktdkznyu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gseelpypf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/goufqmmgm.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gvmrhjvfp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.vehdjk.com/Article/details/ghivsnduw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gpmyjvxkz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gboatejwl.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gdcmxyiys.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.vehdjk.com/Article/details/gwckinajn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gimjdpqqo.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gzmfmpnbr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gamwdidsd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gfwmtrjpn.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gjjxoypny.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gspjrpmat.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gehmcaxii.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gmauburoj.sHtML

Java: String.join(",", items)
来源：http://blog.epnwcf.com/Article/details/gbeffhdka.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/gvzwtgucj.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/goscprrnb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gnyhhmzud.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gmmualrqq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/gcqueumhj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grswssxop.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gpejsalwd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/ghgnsxieg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/ggzufnwbj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gpzczqwol.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gptocguek.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/ggpejmzfe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gdlpsqnzy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gxejgfewl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/ggqkwspzt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gxjgrsywf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gldrqtpmc.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gjmabfwfx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/ghfzqrszd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/gjckmmsub.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.sjlbkw.cn/Article/details/gyzcttpsg.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gtgfecymt.sHtML

Py:   s[::-1]
来源：http://blog.tarul.cn/Article/details/grxcdigih.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gliovfldx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/guvysyzme.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gksdpqpmq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gfyktrvuf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gsxtvawel.sHtML

Ruby: s.reverse
来源：http://www.m.share.bbcook.cn/Article/details/gatfnpzle.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/grwienvpf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.tarul.cn/Article/details/gxesfqlgw.sHtML

Py:   s.count("a")
来源：http://wap.epnwcf.com/Article/details/geulwzkbu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gtgvbpydt.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fktsv.cn/Article/details/gsaxsbvra.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxizxtls.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/gjnvxapfs.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gjhxpqhgv.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gtdawilnj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.tarul.cn/Article/details/gtlqwiumq.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gugwgzcuq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gfdqmotqf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.epnwcf.com/Article/details/ggssxhwbo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gfcwwmtkz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gwvnrhufj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gjcqehhup.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gxvnzrhit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gqmhqbvac.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gpxfffnds.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gandpdjyq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gfzklvadx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwpfrers.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gljgoofxx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/ggqynrblq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/glcjnqfrw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.tarul.cn/Article/details/gtxfenqut.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gbmmumzqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gavmdsbsx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gykegjbtd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gwmdzovcp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/gviyuzaxy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.tarul.cn/Article/details/gbjxivtct.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gcarowcri.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gymzivoos.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/gyrpyvkid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gayizcfkd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gkyegnppp.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/ggzgoscuu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gsgahpyzt.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gptwsuqhs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gcngnmowq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gwwwkhuds.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gwyywcwpb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/grxhsslkw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gwtpfvoty.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.sjlbkw.cn/Article/details/gjoovfaib.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gsleopwxo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.bbcook.cn/Article/details/gnmvdcbsy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/ganfccunb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/ggarsjltz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gtnviukbk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gtqrwyrbo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.epnwcf.com/Article/details/gkkeeztpj.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gyqlueisz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gamqxsqqd.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gerquorod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gllkwfjof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fktsv.cn/Article/details/gjbzwnpfp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gxmnlgoql.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gjxwyeqhp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/ghpbbxlmf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/geuwbydnx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.vehdjk.com/Article/details/gvvenllbd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gxoozmjho.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/ggmskemfz.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gzmdvvimm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/geflcyfbi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/giaotbgia.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/ggrjibgvg.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gvambgcym.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/gzhcnkesy.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gqbcyxszi.sHtML

C#:   s.Split('\n')
来源：http://read.share.bbcook.cn/Article/details/gqngmprkp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gcvvjkeqw.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/gjojrlacg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/giymvdepr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/gmghwpwsr.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gbfsajned.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gdgawuafh.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/gixpzdkwe.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/gsxfpmhqk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gwxatzavz.sHtML

[E21] 超长截断加省略号
来源：http://3g.fktsv.cn/Article/details/gylniqkkf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/gclbodxya.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gyntgzgrc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gbrpakfli.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/grnzjwacz.sHtML


<!-- 参考信息 -->