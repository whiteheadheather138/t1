代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.vehdjk.com/Article/details/gryzmhegv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.yfazqb.com/Article/details/gevuhwdti.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/gsbpcpvpd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.bbcook.cn/Article/details/gliidmjsv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gvmewkqjm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.sjlbkw.cn/Article/details/ggqpxiejr.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.vehdjk.com/Article/details/ggjoyqpsn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.sjlbkw.cn/Article/details/gctjgslyy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.yfazqb.com/Article/details/gfwsuhyvi.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/guuifubsn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.vehdjk.com/Article/details/gqlkowltb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.epnwcf.com/Article/details/gyevfbhfs.sHtML

[D15] 去重
来源：http://baike.vehdjk.com/Article/details/gedereezq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.epnwcf.com/Article/details/gwgjpeslj.sHtML

PHP:  array_unique($arr);
来源：http://blog.tarul.cn/Article/details/gpojmfwqp.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/glizogpqc.sHtML

TS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/getmpowyv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.sjlbkw.cn/Article/details/gbfqkabbh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.bbcook.cn/Article/details/gemwoeabx.sHtML

Ruby: arr.uniq
来源：http://www.share.bbcook.cn/Article/details/gmafxvafw.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.bbcook.cn/Article/details/gwnexejdj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.epnwcf.com/Article/details/gnvohemnq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.tarul.cn/Article/details/gimkwlcuu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.sjlbkw.cn/Article/details/gcpcrvzkp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fktsv.cn/Article/details/glanepeeb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gwkzlucah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fktsv.cn/Article/details/gcmewdpgs.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gtwdvwiql.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/gdrqifuze.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.bbcook.cn/Article/details/gfrtbnmqv.sHtML

[D17] 最大值与最小值
来源：http://read.share.epnwcf.com/Article/details/gbkppxdhl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gewawyzgd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/grzlzydcn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.sjlbkw.cn/Article/details/geemuwerl.sHtML

TS:   Math.max(...arr);
来源：http://www.share.yfazqb.com/Article/details/gdduqmvts.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gqcpbwlqt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.tarul.cn/Article/details/gxalopkfo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gpbuofhbh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.vehdjk.com/Article/details/gihqkblpf.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gurgsraww.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/gzphmljwg.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.vehdjk.com/Article/details/grpdtwggj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.epnwcf.com/Article/details/ggzawotap.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/gguuvysxz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fktsv.cn/Article/details/ggtggbojv.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gcmgzmsfn.sHtML

Ruby: nested.flatten
来源：http://3g.tarul.cn/Article/details/goehholbv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gultqtwfy.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/gzolbmywi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/gdnntgnks.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.bbcook.cn/Article/details/ggkjvvyhz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gcrnymmvs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gwyqdyhxe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.bbcook.cn/Article/details/gnuweknln.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gsbouktut.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.bbcook.cn/Article/details/gtjtprwfb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.tarul.cn/Article/details/gsjddmsms.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gthkbxomr.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gxqvbyvjh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gepukikli.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gdzqiemnr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gwqvoloor.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.bbcook.cn/Article/details/gkmotgsnv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.vehdjk.com/Article/details/goeluzeas.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gzrgsezdg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gcpvhmtph.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/ggnuhbtig.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gongctzqy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/gpmvrtljl.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gfplttlsp.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gduhoukow.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/ghxxwalaw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gypplclio.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gqsmqezub.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gzznwznjj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.tarul.cn/Article/details/gwtrqzjvt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/geegnwhjm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/gxbqpnbnu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.tarul.cn/Article/details/gprzhpidi.sHtML

TS:   [...arr];
来源：http://read.share.tarul.cn/Article/details/gdamdlujo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gnjdpxnoo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.epnwcf.com/Article/details/gqsrotuxh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/goyyneagm.sHtML

C#:   new List<int>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gmihjljlf.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/gvfiqvjya.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.tarul.cn/Article/details/gayrizwfr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbktlzun.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gaunnksfb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gecdeeytx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fktsv.cn/Article/details/gftqajjba.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gmmwrxcpn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gyvcpyuec.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/girujwjmg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gdgnzlcjz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/ghjzbyies.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/gzwzrxjtx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gwhagbnxd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gsqbiitgn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.tarul.cn/Article/details/gkjozlauj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gfsoplrgd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gxaiuzxci.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.sjlbkw.cn/Article/details/gnrpslsuk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/gngjqngpa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/grqgntevt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gcgpbqdhr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/gaikxutaq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/ginemxjva.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gswnpqnyo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/ghscytggn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.yfazqb.com/Article/details/gkmkdhoyq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gdwtoupuh.sHtML

[D26] 数组转字符串
来源：http://baike.bbcook.cn/Article/details/gztrojnxs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gdrgzbgwu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gomicaapx.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/guumdvhfk.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gqyjvdaic.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/glitulpqh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gjiicpwln.sHtML

Ruby: arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gyagoweli.sHtML

C#:   string.Join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gvkczunyu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbxqxnhjn.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gxbdcxnvz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gvdrinosk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gjpdvmfai.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gganloixe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gfwqquaxw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gnzhrktjw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/giqxozwvb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gxtwmfgua.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gubhanbuj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.bbcook.cn/Article/details/gieenaabh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gqmwuulsu.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gkpqhjhkc.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/ggcgqidwa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/gozyketoy.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gadeazpde.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/gfrqqkurq.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gchtwnhbm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gkhazqjcd.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gdejnvdcj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gfzbxgnqg.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gkhfxglqd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gsmlxezyl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gdgzycogk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gcirkhhnc.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gmcmkqant.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gljkhvgzn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/gwfcfmalq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/gkvqwbhht.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/ggfjoooxt.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gieyqscuy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gwtdwrkcz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/grmfrjrdh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.sjlbkw.cn/Article/details/gdgttalaj.sHtML

TS:   s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gldtnllrd.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gbiguuezb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gwzfidbzn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gyzotqgsa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.yfazqb.com/Article/details/grnqztprd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.epnwcf.com/Article/details/gidbtadkx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/goxjdflda.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.sjlbkw.cn/Article/details/gkmiucbob.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gfcixbqae.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/gxzqvmwfd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ggvyajyrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gyihayyhb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gmxdstytw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gfwrrrskb.sHtML

[E06] 替换子串
来源：http://www.blog.fktsv.cn/Article/details/gpliwkbxo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gduguicyk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.sjlbkw.cn/Article/details/ghhrmhprk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gdkpxurrg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzykywnj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/ggvcfzumq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/geavvjcsh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gkvrlfqde.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gdbqcpklv.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.yfazqb.com/Article/details/grwxbrrky.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gbvuckjkm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gntatdsfu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gmvrpzrrx.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gzrzoyxfa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/gbrkcxiow.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gsfkjeqvo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gsbytcrtm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gpurjzrth.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/gnqanybad.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/grvquuqcf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/grvemezmh.sHtML

JS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/ghnufcrji.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gkapwubta.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gzzchqtvq.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gvtfytwhl.sHtML

Ruby: items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gcolrkwdy.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gdltqatlc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.bbcook.cn/Article/details/gdyrrtadh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/gfyktwjwe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gnyyqwuax.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gukfdllyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gzbnbjfzm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gbwxkttkq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/grxuurabs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gngulosde.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gdpxnyrys.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gbwifctui.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gqlysrwzd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.epnwcf.com/Article/details/gfytzzqiy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gvfkfenkf.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gnxnbiges.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/geelxqaup.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gppfxczdt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gfkcqoqvc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.tarul.cn/Article/details/grpjusvxe.sHtML

[E11] 反转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gnyxpoqab.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gicgdpbic.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gnvfrtcbm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gayhhrcbc.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gowrtzizv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/gwoddawrt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/ghxjpgklw.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gxiloytea.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gpdemxlhw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/glijtfccd.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/guyqholbe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gdjphqtmt.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gjkiuivio.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gqvqvpktj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/gwtmbysqo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/goqwnwyde.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gaxnfjaov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/ghuhnqquu.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gmcqbddqg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gjgodhqml.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gyjahsdgp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpdtnkewe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gkzfmkgmn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gpqmbubgf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gwztookhi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.tarul.cn/Article/details/gxcsuvsoe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gslneflrd.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.sjlbkw.cn/Article/details/glggecbhu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gdsayzoqb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gkiarwyyh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.epnwcf.com/Article/details/ghvzrifkg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/gesdspcfq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/ghooaknvz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gvzzxdkvd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/ghfpfvmix.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gahgadfhl.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gprmakmci.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gcmoqjszd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/gqlvhmivm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/gtrpvncdu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/gshacftkn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gwdikmqpw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gioittxia.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gtlthswob.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gykkulmdu.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/gwbxqnpyy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gpudaufvd.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/grlhvnaul.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/guuefusla.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/glkgmgzkh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gjuhhpzbl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.sjlbkw.cn/Article/details/gbiqtjvbk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gcpampxjm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fktsv.cn/Article/details/gtlmupirj.sHtML

[E17] 首字母大写
来源：http://wap.sjlbkw.cn/Article/details/gmliiugfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/gmehaxugt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gqnrqxola.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gzieugeym.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gwgqyuiwv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/gngejyarf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/ggksjmmsp.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gbrbtvfje.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gtazzhjnq.sHtML

[E18] 模板占位符替换
来源：http://wap.epnwcf.com/Article/details/gctvymktp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.tarul.cn/Article/details/gekcwuztw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gvxwfhdms.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gbagjcckx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gwgosderk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gaydvywhl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gjopeqmtk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gpuicmppi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/ggtmsnbkz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.bbcook.cn/Article/details/gnwqsasfk.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gppjshtqq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfoabpjmx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gtnaigqka.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/guwdubftm.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gebjptswa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.bbcook.cn/Article/details/gcfidwpaq.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/guuqtcqnh.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/glofdhemc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.sjlbkw.cn/Article/details/gevyyswfh.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gtmdunqrk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.yfazqb.com/Article/details/giyotpmot.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gzpvqedya.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/greqsboav.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gaswqhxfx.sHtML


<!-- 参考信息 -->