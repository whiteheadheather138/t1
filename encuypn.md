代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gccozymtf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.bbcook.cn/Article/details/ghsaamidi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/gonrenoam.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fktsv.cn/Article/details/gsrelcvks.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.tarul.cn/Article/details/gijhfinqs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gjstfincz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.tarul.cn/Article/details/gufoohgnl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gheccoblp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.vehdjk.com/Article/details/gynmhbhad.sHtML

Go:   // 手写循环
来源：http://wap.tarul.cn/Article/details/goaummnxi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.yfazqb.com/Article/details/gzoqapffa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gjcvjajde.sHtML

[D15] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gqjiimipn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gfjoaocyu.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.tarul.cn/Article/details/gifyrimoi.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.vehdjk.com/Article/details/gzqdvhjom.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gtcjccdyb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.epnwcf.com/Article/details/gqyivwxdp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/ghqbotplh.sHtML

Ruby: arr.uniq
来源：http://wap.epnwcf.com/Article/details/giejqbaeo.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.epnwcf.com/Article/details/gpuypeoke.sHtML

[D16] 求和与平均值
来源：http://www.m.share.yfazqb.com/Article/details/gskxagpih.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.epnwcf.com/Article/details/gklxgxcvn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.epnwcf.com/Article/details/guemslksb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gvcuuljed.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gtjfcaphv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.sjlbkw.cn/Article/details/gnyxqymdd.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gvwywlhmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.vehdjk.com/Article/details/gvgkjeaqq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fktsv.cn/Article/details/gsprjiovq.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/glxqywuvw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fktsv.cn/Article/details/gnetpnhqo.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gqxmmgvzj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gscqszina.sHtML

TS:   Math.max(...arr);
来源：http://blog.vehdjk.com/Article/details/gptpcahgj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.sjlbkw.cn/Article/details/ggzdfzvxd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.sjlbkw.cn/Article/details/gwchczozm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.vehdjk.com/Article/details/gjjygkrsn.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.tarul.cn/Article/details/gdnqvxjov.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gkjjsbiln.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.sjlbkw.cn/Article/details/gpherthbd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/gkixpcyit.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.sjlbkw.cn/Article/details/gchtkyzux.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/ggbcnxqrs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.yfazqb.com/Article/details/gqsjxwvlg.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gawbepjoq.sHtML

Ruby: nested.flatten
来源：http://baike.sjlbkw.cn/Article/details/gexryvxoe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gnhcfcrsm.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/gbwukksgi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/gxkpdfdvc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gjeibgwwf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gmyptuzqq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/grarhrapb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gawhdpplo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.yfazqb.com/Article/details/grkixnuma.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gpesispcn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gryugkopj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gxbwsxlus.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gudxcuarx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gmamkvzfm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/ggsvfnupw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gmlkamhso.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.tarul.cn/Article/details/gpfhfbeqb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/gamxdnzze.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/gollstvpu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/grsshxzqb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gkwqxazoj.sHtML

Py:   x in arr
来源：http://read.share.epnwcf.com/Article/details/ggvhmiqxo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fktsv.cn/Article/details/gwzudehxy.sHtML

JS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gklvsxqfy.sHtML

TS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/ghfyddfjt.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/giopvcghe.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gqgyfeacs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.sjlbkw.cn/Article/details/gkrhuylpp.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gqpraaszb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gqwywuiki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gouiisvzy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.epnwcf.com/Article/details/gflmiobmu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmroxxpkx.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gqqkwgbgx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gunjvsshx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gbvbvotfq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoboerzf.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/guiovqpqt.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gwbqztcql.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gfezyckaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/geubghynb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gumftzgmz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gcypedtkw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/gjntkaqkk.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gwoyadrnj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gweyddtmy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.yfazqb.com/Article/details/gyhwwsqcu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/glsalinye.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.bbcook.cn/Article/details/germcqrtg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gtlclsgzq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/gqeijibyc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwdbmonxk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gtfbuhuiu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/ghgxnfebx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fktsv.cn/Article/details/guputktkr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gfgmdbgnq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gsmoneesu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gccviphnq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/ghwdqtyln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.vehdjk.com/Article/details/ggitklffc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gojqpynvs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/gldgjemfg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gxllxlxvc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gmvmgqjby.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvejrbmme.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gtudrbbbv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/grymjwbka.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fktsv.cn/Article/details/ghngrktsg.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gxaizfvhp.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gmjctneck.sHtML

Java: String.join(", ", list)
来源：http://m.share.bbcook.cn/Article/details/gsypmhuiu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/giodswkkt.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gkkouicee.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gqcqprabx.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gacfyofmy.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/googyfgpm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gotmhnnsv.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gulmnpucp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gwqpwaubd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gdyjjyrli.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gtcpdovau.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/glucxyzjn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gdkmzffyc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gczyfxwlt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.tarul.cn/Article/details/gnpualuqp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gicgsbpsr.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/gagvrgjts.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gawdbtfbo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gmikamukx.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gpsjjwnvo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gsbsefqgl.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gmyoypkdz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fktsv.cn/Article/details/glsspmlpg.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gcqrznxkr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gowicetfg.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gzystylvz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gkdrgocml.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gimjwqecc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gfpmvcvvk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gkkqoziys.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/giqydzokk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.yfazqb.com/Article/details/gvvfkrhha.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gryvihdpa.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/grurwfnnv.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gbhwjzwsq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gljhhoaav.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.yfazqb.com/Article/details/gmpcrbuat.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gaairpdkd.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gfzwcafie.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gmmkfwdpd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gflafzwyk.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gfsecbbog.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gpkhajgjn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.tarul.cn/Article/details/goozbmmpl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gfwuijhca.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.tarul.cn/Article/details/geeivtofj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gwkfimlgz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gtztgmnnt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gpcesllla.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gimqvkoct.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gbzkqeece.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gjybumbkn.sHtML

[E06] 替换子串
来源：http://baike.bbcook.cn/Article/details/gdmsgvspb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gxxwywify.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/goyrnsunn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gvyysmyse.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gocxlzjiu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyljyiohy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gyxvhnucb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gehtcqahb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gdtymadeg.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gylglpzhz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/ggnrktwnd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/ggxarudng.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gzezyuful.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/grotbckwo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.tarul.cn/Article/details/gsgfscvbm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gvexzhmwq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/glysocvxt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gaglrvpkx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/gehbqkudh.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gcxkmcxpg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.epnwcf.com/Article/details/gdkjganzz.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gdecyoiqq.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gteqgaqkb.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/grsrzwfvu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gvnfcckzy.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnyxhadtd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/ghuutnyih.sHtML

[E09] 去除所有空白字符
来源：http://mobile.bbcook.cn/Article/details/gmyqdtljy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/ghbxvjpfb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gxbbfpiab.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gmdrdoeng.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gqswgobuu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.epnwcf.com/Article/details/gmjmisiwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gxshnftdt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/ghlwsigzp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/goltqmxkh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gyphsopux.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/golbplsch.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gyvrqawfb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gqjjvrvlz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gcieaahxh.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gxxhagdfr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/ggyapivew.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/grdutxpyg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gretelghd.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/guwnnaeux.sHtML

Py:   s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gibmggmuu.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gygjiqtth.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gpgablooy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gqglwrrbf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/gwkwfzwbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gzraovqkn.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gqfvoxfqp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gzbzmybit.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gojmbrclb.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/glzcjklab.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.yfazqb.com/Article/details/gaqlgbkwf.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gryoqlqfj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.bbcook.cn/Article/details/guclocchx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwiuluhk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.yfazqb.com/Article/details/gmeblbtbp.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gmggdadgb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/guvvmherk.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gqyspdsny.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.sjlbkw.cn/Article/details/gdoouwjgy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/gfmjdrvgs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gywwivuvu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fktsv.cn/Article/details/gprrsbqat.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gsyymwgal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gawtsjklu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gqmvsomqk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/ggxxjbcza.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gkgaryufx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/ghzpvowad.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/gbknpreil.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/goffzlqcb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/gsbjmgucv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/gjejmxxgr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/gvzijexyi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/geltpolfw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gcsnxezma.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gahsfmsvb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gdqlyktyp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gwezfchro.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gkidxnvkr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.yfazqb.com/Article/details/gjrbfuwfn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gxbjbowop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gkzyrioaj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gbxdjblop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gqsnsooat.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gxmqqjlbn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gxjhfcvgb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gbtstvjdn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gxzqukbqp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/guhgpsiyd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gndiykrtn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gjymfrysc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gejbkqizx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gtjedesbk.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gfvhwgkpv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/glqwucply.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gjasfcazz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gtaftsbyc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/geccfwhbj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gwfipzlvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/gqgywhcni.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gadvcyxuo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/gufpykcxw.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/ghwrvnqkx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gknxvdzar.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/geejzgslu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gnybvxjbo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gipxfhfvm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gcmbpomwo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.yfazqb.com/Article/details/gviklnebv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.vehdjk.com/Article/details/gqqtsfaxe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/glecpesgw.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/grngwljid.sHtML

Py:   s.splitlines()
来源：http://3g.vehdjk.com/Article/details/gtlicmswm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gsgmoqfor.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gfkasceiu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gmgahlcfb.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gxupzkncg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gooblupka.sHtML

Ruby: s.lines
来源：http://3g.tarul.cn/Article/details/gvwvvirom.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gvlirpxow.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.yfazqb.com/Article/details/gtnvpgdwm.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/gghsmoqhr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gtwgiitqv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/gxttazwye.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/gffgrewxk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/ggcfpnbnh.sHtML


<!-- 参考信息 -->