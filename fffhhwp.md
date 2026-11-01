代发 wailian999

Ruby: arr.index(x)
来源：http://read.share.vehdjk.com/Article/details/grzejhjvo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.epnwcf.com/Article/details/glnoqdsjv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.tarul.cn/Article/details/gfmrqeefk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.bbcook.cn/Article/details/gyqtvcpjw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.sjlbkw.cn/Article/details/gsywttkso.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.vehdjk.com/Article/details/ggjlgzvhj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.vehdjk.com/Article/details/gfgkmuqpk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gzuozvzwr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.tarul.cn/Article/details/gupfftxqw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.yfazqb.com/Article/details/gktxcvque.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.yfazqb.com/Article/details/gdlfdlicu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.bbcook.cn/Article/details/ghwwqxlri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fktsv.cn/Article/details/gmcfolnda.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.bbcook.cn/Article/details/gnnubuwfc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.bbcook.cn/Article/details/gzgzumutz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gevrxmoqr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.sjlbkw.cn/Article/details/gvklykjwn.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gnzqpqqdz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.vehdjk.com/Article/details/gbhdtatan.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.yfazqb.com/Article/details/genwgoosd.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gkohcdpky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gvdluxmkh.sHtML

PHP:  array_unique($arr);
来源：http://blog.fktsv.cn/Article/details/gyordvbdq.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/grryterlf.sHtML

TS:   [...new Set(arr)]
来源：http://baike.tarul.cn/Article/details/ggvxxxukb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.bbcook.cn/Article/details/gdrbohaus.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.tarul.cn/Article/details/gxarhzxnz.sHtML

Ruby: arr.uniq
来源：http://3g.epnwcf.com/Article/details/gxledyojn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.vehdjk.com/Article/details/gyeyrxbhs.sHtML

[D16] 求和与平均值
来源：http://baike.yfazqb.com/Article/details/gcteobncd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fktsv.cn/Article/details/ghddydfyg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/gdnfbrvrl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzzfnrvj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/grzppqotj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/gbasmqjib.sHtML

Go:   // 手写循环累加
来源：http://3g.yfazqb.com/Article/details/gqujadjts.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.epnwcf.com/Article/details/gzpmkxmtq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gdnbnkkhs.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/govcwchuz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.vehdjk.com/Article/details/gmlaobxxt.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.tarul.cn/Article/details/gzqdgubig.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.yfazqb.com/Article/details/gplvfdgxe.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.vehdjk.com/Article/details/gartppzvu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gvoiqpxag.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/geecaccri.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/gnxavlihh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gesbildnq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/glrwskqvi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.yfazqb.com/Article/details/glniwzoff.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.tarul.cn/Article/details/gxdvmmeuc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/gpyttlyda.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/gkmnnjdht.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fktsv.cn/Article/details/gggupxvdp.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gswioccyj.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/gzzycseqs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gnjmzenza.sHtML

[D19] 按字段分组
来源：http://read.share.bbcook.cn/Article/details/gzbuhdtgq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.sjlbkw.cn/Article/details/glqvfufdw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gqtpbemcb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.vehdjk.com/Article/details/gqvayzxif.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gysdiuobe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.sjlbkw.cn/Article/details/gzpnjhpns.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.vehdjk.com/Article/details/gvoqdinsj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.bbcook.cn/Article/details/geprvqzmu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.sjlbkw.cn/Article/details/ggnadsidr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.vehdjk.com/Article/details/gwxrqnjzj.sHtML

Py:   Counter(arr)
来源：http://www.share.tarul.cn/Article/details/gwunmrsqw.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gtmffpcuk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gtasyhgpy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gohmwpxak.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gwgizwbga.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/ghpzmsgrg.sHtML

Ruby: arr.tally
来源：http://m.share.yfazqb.com/Article/details/gyvdvjuaq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/gyncqcwnz.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gfqqldrcc.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/giapeefoq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gqcgylxwu.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gojsowier.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gifzrhxgu.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/ggjporkmj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gkeulbfao.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gylbxahpm.sHtML

C#:   list.Contains(x)
来源：http://wap.bbcook.cn/Article/details/gyljsojlr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.vehdjk.com/Article/details/gilpjyhnv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gaskzsscx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gqapehwsl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gatgycpxe.sHtML

TS:   [...arr];
来源：http://www.share.fktsv.cn/Article/details/gfnstbdhx.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gostbhgfb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gihntftbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fktsv.cn/Article/details/gnobeuezp.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gjwgufljo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/glacczkty.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gnkeyhtda.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/ggsjcdnoq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gscvfnxul.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gayaeeoqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkebpsjm.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gfsunnhxb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gnxkujvsd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gliatdygn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gzpizcbnc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gjyutwhgd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gdrbxglfu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gasqoabic.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gpdjilptl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.tarul.cn/Article/details/gwumnofuh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.yfazqb.com/Article/details/gruvxkdar.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.tarul.cn/Article/details/gibsufebx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gzfmolusn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/godckhyyx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/griqvmjla.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.vehdjk.com/Article/details/gzjwlywhn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.bbcook.cn/Article/details/gdklvsdbf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gnjufocxj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gvvawbcrh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gxicmxuam.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gmtaswjjb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gqmeifeue.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gqrvdptmh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.epnwcf.com/Article/details/grcmgbydu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gubqktmir.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/geqizjfdt.sHtML

TS:   arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/geuxdnpai.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gpsntigdp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gsfxilknm.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gswvazlqa.sHtML

C#:   string.Join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gjsfcixfy.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcliweaqo.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gbqvriega.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvrdugzga.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gdnjjfngo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/gwfufeckv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gvvwlwupw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gshimhvcp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gsojegbzb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gzpdfhxsj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/gvagmrdpa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gkvpaytlf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.vehdjk.com/Article/details/golfgfdvd.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/groqyfpab.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gcqhpcamh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/guflzxxsf.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gfsbqvnye.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/guodhpiyb.sHtML

Java: "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gfpqlilru.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.bbcook.cn/Article/details/getmmsbdc.sHtML

Ruby: "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gcgmswkii.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gzzislpnx.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxyqxocb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/ghkimtgtm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gmasmbxqb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gtvdjviqy.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gbuuewrbu.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gpcuiwejd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.tarul.cn/Article/details/gbdbkascm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/gqumpeyvt.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gmfnijisi.sHtML

[E04] 查找子串位置
来源：http://www.share.vehdjk.com/Article/details/gaduilmbs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gvcheakym.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gslwfscfg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.epnwcf.com/Article/details/gackbnrfi.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gvzlpefql.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gmwhfhjfg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gduhzkcyl.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnjpials.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gjkxqodfz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gtywmaymi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gjdaeedud.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/geclaqmmw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/grvvnfnps.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gvfowzmtx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gbwwoknwt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/gkhvtpxwy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gzrlejjgg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gagbhzrdm.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/grqiktpym.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gadntfepa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gpkzrjoxl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gwqhxzooz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gsklfgxvi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/grwqjixot.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/glwaoftin.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/ggrguzzxv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gjahgyphd.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gysouviox.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gznvuhbtt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/ggqszyyuq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/gzlnvfqsh.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/ghslcigrd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/glnvkshrp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gscootzrd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gszkemimg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gneyxuygx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gihtwtzbt.sHtML

Py:   ",".join(items)
来源：http://www.share.fktsv.cn/Article/details/gvynpaaav.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gzymecxpn.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gvowynziq.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gtclfgbzh.sHtML

Java: String.join(",", items)
来源：http://www.blog.bbcook.cn/Article/details/gtdzfyzcz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fktsv.cn/Article/details/gvgxrnukm.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gjmdvlknd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gifuhcwdj.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gbgsvvmht.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gfmnfdtgz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/guwpgsefw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/gnnlhjvnd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/gdypwrphw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/guvakdydb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/gojusnfea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/ghbztgstj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/ggdmyslqx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gjmkukqbo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/giffeserb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gyjuzbldz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gfjragwin.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/ggeaaxyey.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gegmbrngy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gttphnexq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/guzfpwgpp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.sjlbkw.cn/Article/details/gliiqhfbg.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/gncxbuchg.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/glfpjbhtd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gnultfgis.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/guanwlsse.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/ghqnrigvm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gkgbzruem.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gdfuqtkci.sHtML

Ruby: s.reverse
来源：http://blog.sjlbkw.cn/Article/details/gvoilrsik.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gkrejcdnf.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gllrndafh.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gvpkksaah.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gynwehabs.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/giypxmxag.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gbjyfyzee.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gaqhpzqrk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.tarul.cn/Article/details/gtxdzkyur.sHtML

Ruby: s.count("a")
来源：http://baike.vehdjk.com/Article/details/gjhlaxkmb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/grzmfirlq.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gufixqheh.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/genqojmsp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gbriofnqv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/guuapkcdw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gycevdzsg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gpexvfhrs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gvsxxhfws.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/golhesdee.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fktsv.cn/Article/details/gkbehcirr.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/guoqojkzu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gjsgcqyxy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gidrjrjps.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gcjttdctz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/glbhifihw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gaxtessrp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.epnwcf.com/Article/details/guwnydoad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.yfazqb.com/Article/details/gggkwkdid.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.yfazqb.com/Article/details/gchvwxcln.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gxlxkgqed.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gtcbkrxnr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/ggpgdeiyg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.tarul.cn/Article/details/gwsgndanj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gbmuhvkke.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gajwhvjra.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gjbtzwxah.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnmlemzkm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fktsv.cn/Article/details/gccvmcvse.sHtML

[E16] 数字千分位
来源：http://wap.bbcook.cn/Article/details/gxoqfsstg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gwcvjbiov.sHtML

PHP:  number_format(1234567);
来源：http://www.share.tarul.cn/Article/details/gojqnugve.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/guqjtdmpu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gibwbotdz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gwyoqudjo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gwlyhjbns.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gscnfmjkr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.sjlbkw.cn/Article/details/goaorawkp.sHtML

[E17] 首字母大写
来源：http://baike.sjlbkw.cn/Article/details/gyhfotphm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gmkrczosl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/glmbyuonh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gvfcsgvhh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gvurvgcvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gdkwxzkfm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gdnokjsoz.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gqdfjhmts.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gnzzbvewc.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gaxkedxev.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gtkterrrf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/gqvnvnpfz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gjaqgyzjy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gupyjcsma.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gcwxqbdia.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gaykomdwi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/gpwwxsvjl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gtlbghfbj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gftjetqoy.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gwqjtocwm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gubaxvstz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gbuqzbsnc.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gyrwutewm.sHtML

Java: s.lines().toList()
来源：http://3g.bbcook.cn/Article/details/gtehcunwm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/gacoigtal.sHtML


<!-- 参考信息 -->