代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gqeucqghy.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gdzcravkx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.tarul.cn/Article/details/gsfrnnstw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gtiivtgin.sHtML

[D15] 去重
来源：http://www.blog.fktsv.cn/Article/details/gkwfcuuyl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/ggxbxwyzo.sHtML

PHP:  array_unique($arr);
来源：http://3g.bbcook.cn/Article/details/ggjfuofys.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gkjwgyocs.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gquohlseb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.bbcook.cn/Article/details/gkyloslgw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.bbcook.cn/Article/details/gfyvsaanw.sHtML

Ruby: arr.uniq
来源：http://www.blog.bbcook.cn/Article/details/gjgtvdsfa.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fktsv.cn/Article/details/gxbqibujx.sHtML

[D16] 求和与平均值
来源：http://baike.vehdjk.com/Article/details/gwhxuikxf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/gncekgbqx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.tarul.cn/Article/details/gjkngljnn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gfsjycarx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/giyzcahnh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.epnwcf.com/Article/details/givffvyov.sHtML

Go:   // 手写循环累加
来源：http://read.share.yfazqb.com/Article/details/gtvqwxdlh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.sjlbkw.cn/Article/details/gmnfhlmsv.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gkxqrgmdf.sHtML

[D17] 最大值与最小值
来源：http://mobile.sjlbkw.cn/Article/details/gavguyrvm.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.vehdjk.com/Article/details/ghatytyou.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.bbcook.cn/Article/details/gfdnlehzm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/gkapdzgts.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fktsv.cn/Article/details/gvbvsnied.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gxqlmcaxt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.bbcook.cn/Article/details/ggstgawbh.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/glblqqzgc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.tarul.cn/Article/details/gndvfnaqi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.tarul.cn/Article/details/grjgajlrb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.tarul.cn/Article/details/gbqxrwbew.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.bbcook.cn/Article/details/gapqkgahg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.yfazqb.com/Article/details/glizronyb.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/ggnjkybqc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.bbcook.cn/Article/details/giuusavra.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gtiyuuitk.sHtML

Ruby: nested.flatten
来源：http://www.m.share.yfazqb.com/Article/details/gwrzlkfnh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.epnwcf.com/Article/details/gnkgmuitd.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/grfvovzhu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gamzkwhov.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.sjlbkw.cn/Article/details/gimlkdzmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/glvarizul.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.sjlbkw.cn/Article/details/geuhhpuer.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gnjxjzrcc.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.epnwcf.com/Article/details/grsmzcvcc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/gwgahpptj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/gywgirozf.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gberbskbc.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gbsqdcpjp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.tarul.cn/Article/details/gbnndwhwy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/guxbeysni.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gmerjdyat.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.tarul.cn/Article/details/gyqawplsp.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gpisywqdl.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/ggvbwuexd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gxvtiwvst.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gcxtbmhhc.sHtML

Py:   x in arr
来源：http://www.blog.vehdjk.com/Article/details/gesmkbree.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/ggkxsueoy.sHtML

JS:   arr.includes(x)
来源：http://m.share.sjlbkw.cn/Article/details/gzofgrkds.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gtfqmffld.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gzsuakzcz.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gmndrybmg.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/glfxxzzer.sHtML

C#:   list.Contains(x)
来源：http://www.share.tarul.cn/Article/details/gyrjwvohq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/ganekghha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.yfazqb.com/Article/details/gmnoafzup.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/grxtbokvb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fktsv.cn/Article/details/gzfcarqya.sHtML

TS:   [...arr];
来源：http://3g.sjlbkw.cn/Article/details/goyrhviqc.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gwsgtyhdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.epnwcf.com/Article/details/gzfkqswqg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gzevayvit.sHtML

C#:   new List<int>(list);
来源：http://www.share.yfazqb.com/Article/details/gygzimykq.sHtML

[D23] reduce 累积计算
来源：http://blog.epnwcf.com/Article/details/gumjtnmqb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.epnwcf.com/Article/details/gfdbleppf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gkadwmoyx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gxycixiqa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gszuztkqg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gnzgnxomt.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gmfdvvcvx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gtslfiyyh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gleqmqjqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.tarul.cn/Article/details/gquaboosc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.bbcook.cn/Article/details/ghunehnbc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gjkqjbzwy.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqpuyspj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gzwbiqwwe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/gfbizagmj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/goahpgcya.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlfsjhmw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.vehdjk.com/Article/details/gwuuwrinf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gxxooujqp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gblgyhixr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gqpccyozr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/gwujgggxu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.vehdjk.com/Article/details/gbkbcrnqg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/gttwfnzqb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gcvmudivg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/glokgumjl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/geqmvsifg.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gbkcbirvh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gmwlmgone.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gtmuozjqk.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gyegxcuxp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/grtkfbxlb.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/gcfahswmh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gmmgeqhcq.sHtML

Ruby: arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gcdamynlo.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/galgdoekh.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gcsddmlio.sHtML

E. 字符串处理
来源：http://m.share.sjlbkw.cn/Article/details/gztwmyhxr.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guxapttmk.sHtML

[E01] 拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gpiykdpyd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gvkljsbiu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/gwvtrkljm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtbdgpabg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gefdjclfk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.sjlbkw.cn/Article/details/grbvjzpvf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.yfazqb.com/Article/details/gcrgxhwrh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gxfufukaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fktsv.cn/Article/details/gqsdtklyn.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gyvcbpsrg.sHtML

Py:   "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gvwamlqtj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gznvrcgxl.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gupuuotpw.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gbtleretx.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/govvidzjq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/guvfnczzd.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gejbhiaxn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/ghltujqvk.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gyduizhmw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gffkuzmij.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gzymrrsse.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gttrtxggd.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/grdecjntb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gkvslfvfk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gyklfahhq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/gokvzaktp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gmlgyekia.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gwjjiqabc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/grhtbgejc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.yfazqb.com/Article/details/gvnpiyzes.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.tarul.cn/Article/details/gfhifgnzk.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gaexacwlb.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/grmxepzrr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fktsv.cn/Article/details/gmnnmylcn.sHtML

Ruby: s.index("x")
来源：http://baike.epnwcf.com/Article/details/guovdjsgj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gimbftzxc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gtfdiwkil.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/gqhazcmex.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fktsv.cn/Article/details/gwtcvqico.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gmkdnsccg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gtejyzyem.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gelaltrkz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/gacqmlhnl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/ghhzzkyup.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gxoqhsizu.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gwbzeswuu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gfhbkdzrz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.bbcook.cn/Article/details/gjkemqknh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gmhzhblfv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/galfnnmue.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gzorezzwg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/ginojhxae.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.tarul.cn/Article/details/gndfwqqep.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/ganklchvy.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/ginacbqqm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gkwniipbb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gkdpwsulq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/glknohhra.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gufrqgdut.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gjfgpuxcr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gpzqbwtnw.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gpttqyhud.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gvdtbmhfu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.vehdjk.com/Article/details/godisyjcv.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gslziewlq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/ggzmjzkic.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/ghksadcjb.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gearcbpoy.sHtML

Java: String.join(",", items)
来源：http://read.share.vehdjk.com/Article/details/giomkdhbo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gaxyxcrob.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/goycjrxga.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gkyqwqqtp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gyladfeyq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gfhademen.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/gbgogcsgn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/gbglvibmo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gxwqgrmbn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gezvtoogf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gmonbcmld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gwjiwxytn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gsawdtpgy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/glfyghhty.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gdhxpujhm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gnvimeitb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/grhrqokhz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gxebfgswv.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gzgmjrhpd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gmjqcmsfp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.epnwcf.com/Article/details/gwsjtqans.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.bbcook.cn/Article/details/gfvcgeiyl.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gtgbnjltn.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gzvcrhale.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/guvzggbkg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/giwijqvrq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/grwwqtaeg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/gdbceowtd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fktsv.cn/Article/details/gyvepjwhn.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/gnwywbzwq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gquqarruw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gwwgmhimq.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/ghlppvthm.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gnvnytdov.sHtML

JS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/grqhqxprw.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gehzdnpyy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/ggxdoghju.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gfsiypfjw.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gbdaevhed.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlasjfdu.sHtML

[E13] 逐字符遍历
来源：http://3g.epnwcf.com/Article/details/gdrejohjd.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gnurhhdjh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gpamdbvid.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/gkbysjojf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gepumeyys.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzchyiqau.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gncudasfv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gjjbfttjk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gzkdqalgx.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/geaxmdfux.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gyrzcatgx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/getqtniig.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gqvbpcpqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/gpcasmcwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/guaemmmjr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.vehdjk.com/Article/details/gjujwtvjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/gmajxpiyx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/ggvwlgxqb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gdrffwmtt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gdyzezdqg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/ggjhkanvq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/gqhyzidun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gytfhgzmo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gzbbaakzb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gbpmivoop.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/geqdhdaxv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gvdptstgi.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gerxthrrh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gqooicoqu.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/ggzgplezt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gdxxlkosq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gqmgdkmau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gfoalubia.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gvplwcofh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gazaomezy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gdjftgayi.sHtML

[E17] 首字母大写
来源：http://www.blog.yfazqb.com/Article/details/gmzqrejnj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gowybyhuu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.tarul.cn/Article/details/gkirmzzrx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gycctlhdn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gdjkcxmoq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/gxptrinsn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gurrndtkx.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/ggbypnbdi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gyyusobqi.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/gwgaikybr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/guhufpfmx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.vehdjk.com/Article/details/grrrcjikx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gqazfmfhl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gbmlktbvh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/grjugcloi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gwpprbrpr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gyfupjzep.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gfaqbgvkw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fktsv.cn/Article/details/gclcujpfl.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gifglynyk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/ghwjflubl.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gnhmdaluv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/ganwzylyl.sHtML

Java: s.lines().toList()
来源：http://baike.tarul.cn/Article/details/gmorgwbeh.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gbxjcejad.sHtML

Ruby: s.lines
来源：http://wap.epnwcf.com/Article/details/gmdwbxluw.sHtML

C#:   s.Split('\n')
来源：http://www.share.epnwcf.com/Article/details/gktyqnpbr.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.tarul.cn/Article/details/gzasseafs.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/gkwwwrejp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gxisgxnuv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fktsv.cn/Article/details/gawjsbuom.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/gkmkfswtc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gznnsieuh.sHtML

Go:   if s == "" {}
来源：http://wap.vehdjk.com/Article/details/gornnwryn.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/gozhenzou.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyxoivdgo.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gtbiwzllk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.bbcook.cn/Article/details/gehszhuhs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gbfkfjqrk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gnscqekfk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gecgivwss.sHtML


<!-- 参考信息 -->