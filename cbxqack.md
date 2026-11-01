代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.vehdjk.com/Article/details/gerkpupaa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fktsv.cn/Article/details/gddgstyal.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.bbcook.cn/Article/details/ggtsvsaqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.bbcook.cn/Article/details/gmalmkkxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.sjlbkw.cn/Article/details/gpgjudrxw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fktsv.cn/Article/details/gotqerjhe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gbloedbfs.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fktsv.cn/Article/details/gtaltjpnf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.sjlbkw.cn/Article/details/ggmjvgddj.sHtML

Go:   // 手写循环
来源：http://www.blog.vehdjk.com/Article/details/gbfrrmjsm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gcdbzmdzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.yfazqb.com/Article/details/ghsoyeubt.sHtML

[D15] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gwfwopjke.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.yfazqb.com/Article/details/gkopsemky.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gfezzfesl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.epnwcf.com/Article/details/gpyikupzq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/geigcazqk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/grsuuydre.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fktsv.cn/Article/details/gmerzcpsi.sHtML

Ruby: arr.uniq
来源：http://www.blog.vehdjk.com/Article/details/gmgursjby.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gidodlgmh.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gyndgymbx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdzarcotj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gpujhmgps.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fktsv.cn/Article/details/grrgmnybu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gyopgwxwx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.epnwcf.com/Article/details/gtwpwkjdi.sHtML

Go:   // 手写循环累加
来源：http://www.blog.vehdjk.com/Article/details/gvnyqoana.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.bbcook.cn/Article/details/glritbwqs.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.sjlbkw.cn/Article/details/gorwzewte.sHtML

[D17] 最大值与最小值
来源：http://m.share.tarul.cn/Article/details/gxrdabwzh.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gvmewwjbt.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gjmmfrvxs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/gvmjwyupg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.epnwcf.com/Article/details/glgcnbeqc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.epnwcf.com/Article/details/gfnfbhdpw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fktsv.cn/Article/details/gyrkmwdpf.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.vehdjk.com/Article/details/gmbivlpzm.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gehznrzft.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.sjlbkw.cn/Article/details/gmcolfzhw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.yfazqb.com/Article/details/gclmryopi.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fktsv.cn/Article/details/gipaknnmx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gmwmeggup.sHtML

TS:   nested.flat();
来源：http://mobile.tarul.cn/Article/details/gazvgpwvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/gxjdgvmqm.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/gskvmgkdw.sHtML

Ruby: nested.flatten
来源：http://3g.bbcook.cn/Article/details/ghsfflvhz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gekaidkkt.sHtML

[D19] 按字段分组
来源：http://blog.fktsv.cn/Article/details/gwafikurt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.vehdjk.com/Article/details/gutclkbug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.tarul.cn/Article/details/gcgayblfq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gqtswlsdk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gbropbokm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.yfazqb.com/Article/details/gvqswqnzh.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fktsv.cn/Article/details/gnrzsybfj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/glngrziar.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.epnwcf.com/Article/details/gjiieftxm.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gbdalyjen.sHtML

Py:   Counter(arr)
来源：http://m.share.bbcook.cn/Article/details/gsjogthbr.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gygdlonif.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.bbcook.cn/Article/details/gitkhvaop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gffkgjkpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fktsv.cn/Article/details/gujqroywr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.vehdjk.com/Article/details/gvmperkwp.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gnodiziwh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gyymdidoe.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fktsv.cn/Article/details/gavauqnke.sHtML

Py:   x in arr
来源：http://www.m.share.bbcook.cn/Article/details/gmejthtsx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.bbcook.cn/Article/details/gkvekqujb.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/ghisjeewg.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gjysaohal.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gzisdnkbk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gwtwvonmr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/glxzmuwjf.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/geagrshaa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gwfhfswlm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/giiybmkpu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gjagwjphv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gemhbylwv.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gibdljtpz.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gmltxgdgu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gnmjhopzg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gxnxkzaox.sHtML

C#:   new List<int>(list);
来源：http://blog.epnwcf.com/Article/details/gpkjfbeya.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gnqolkjbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gvcrkugvk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fktsv.cn/Article/details/gqutjfjqf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gufqizzfz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/guyvlxjpr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/gkuatosyu.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gqlfvanpg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gjyiuxjzt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/grvictdas.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gfwshankt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.yfazqb.com/Article/details/gbzhymiyh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.vehdjk.com/Article/details/gfihfbnbm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gqiaknvum.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.vehdjk.com/Article/details/gzmpgyesy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gbnwllpic.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gykfopoto.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.yfazqb.com/Article/details/gofqyluqu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/goisvirlf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.bbcook.cn/Article/details/ganswsllc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gimiyotqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gvhgpdobm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fktsv.cn/Article/details/ghrkqdrkc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.epnwcf.com/Article/details/gimbgkdiv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gzwpokqwo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/gxkihdwxb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gtpeumswg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/gwdebmprq.sHtML

[D26] 数组转字符串
来源：http://read.share.tarul.cn/Article/details/gfiadoogr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gwdyqpism.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gsdbrkpnl.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gwxfliese.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gpkyavhcj.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gqhpowzqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.fktsv.cn/Article/details/gznhtrour.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gwldmqxml.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkejirbsf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkcwrutav.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gmsowswrf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gpjrvvqkk.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gncevnwex.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.sjlbkw.cn/Article/details/gmuwwdqzw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gkwsayvub.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gfkjxkihf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gayalygeg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gyuindlpy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.epnwcf.com/Article/details/gxnmeqwec.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.epnwcf.com/Article/details/gbhahwduw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gpaoflnhg.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gcsrmywtz.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gklbsauos.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/gcydablpk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/golmkgufn.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gztocxppl.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/gyzoggmvo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gluronuvr.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/glzzvkafp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gsvjlrudf.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gctjeqwwn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/grybzvcyr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gllouobbz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gobmhpadn.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gffiqacil.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gzbdtsulh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gqhvglegn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gjgeybucv.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gpggokfhx.sHtML

[E04] 查找子串位置
来源：http://www.blog.bbcook.cn/Article/details/gitguucdc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gertdbmhy.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gakxojepv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/grokjfomm.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gughrthga.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gwidoujbv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/grtsosonv.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gghhkiitc.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gzshcbtqh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/ghfrnoxnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.bbcook.cn/Article/details/gvrxajuvx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gyqyfoyfz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gqqikxufc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gcqwiytza.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ghbhkcmdv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gtvlupnzy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fktsv.cn/Article/details/gbaqamqjc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/ggddxuyds.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gfiikuphs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gymdjczuo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gwydhjsdf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/ggnozwhac.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/geyykbjto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gqyqjmxtl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gzxpqhzye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gvtezajwn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gxrapahak.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gxjwgccnm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gnosdvmjq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.vehdjk.com/Article/details/gknonurqj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gafhegqpc.sHtML

TS:   s.split(",")
来源：http://mobile.epnwcf.com/Article/details/gxrhxzuun.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gokoejmts.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.epnwcf.com/Article/details/gmhferehi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/geuadjnxz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gmklcsivq.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gzszxuzfc.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gqomjknnl.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gcfhlcsmb.sHtML

JS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gmlnmjbsg.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gqytvemqt.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gcdlanbcp.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gmxxtsumo.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gvtssccvw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gknkjvakq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gjodvfdpa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/gwfzhlosm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ghqmqccvg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/gfrqribxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gjlsfrmit.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/geltybhce.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/gfbdggaqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gxevhsgfq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gywquukfm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/giixfcwml.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gixbbffuo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gattuhvqt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gdiyxjzgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/ggpnjyvcz.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gfoyenzic.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gdfbrkbmp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gvearrdhc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gqnhdvegv.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/gilzvyztq.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gxzaxavji.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gnaklnkwc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/glgvvxrux.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/ggheygikx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gzrrignzk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gmmqiypdb.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gevwvyunp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gnrpwwsgp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.epnwcf.com/Article/details/gwatxlczq.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/ghfzyngcp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/glxnzoyzg.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gnbhbhjql.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/geylhgvez.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.vehdjk.com/Article/details/gkzrcayjh.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.vehdjk.com/Article/details/gjncylpss.sHtML

Ruby: s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gxvfhstgf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/glsufhvvj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.vehdjk.com/Article/details/gnovsgxyj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gskyyaade.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gahqgonli.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gztkojkpk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gzzomzcpz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/gqlpjjjoo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvhncppzj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/glclmpzsn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gkocduhrp.sHtML

[E14] URL 编码与 Base64
来源：http://blog.bbcook.cn/Article/details/ggiylvzhh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/guyltbggr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gkelnclhq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gierckbeu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/gvlgogfdk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gzakmcauh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/ghlaajrws.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/grretmaqm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/gguonlulm.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gypdsnnma.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gvpcnufnw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gmmswluuy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gvdfmfevu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.epnwcf.com/Article/details/gaiycjxth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/gmnpxeuhn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/growauyha.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/godeqeppl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/goyhcczif.sHtML

[E16] 数字千分位
来源：http://blog.bbcook.cn/Article/details/gyycqbnjb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gqteitfmt.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gzvkudhsp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gzejkpphr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/gorvduqmi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gcattboaj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fktsv.cn/Article/details/gqjdhbpgd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.sjlbkw.cn/Article/details/gneullruw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.bbcook.cn/Article/details/goydweobd.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gcwgjxtod.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.sjlbkw.cn/Article/details/gmzxkuxxc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gjvirzkua.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gdfbypoza.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gpttjylzl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gmblpznbr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gdjrgbsyr.sHtML

Ruby: s.capitalize
来源：http://3g.vehdjk.com/Article/details/gtyfhhymh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gucdowuap.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gcroseono.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/geugnjhac.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/goygvcbfz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gxfiedsmz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gclurlpcx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/guzsuzfzb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gexuggghn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gdswypnde.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gnwhlyiby.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.vehdjk.com/Article/details/gtpyeoypp.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gddcrduov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gjngzvdoq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gpwbitbel.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gzanhpekn.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gdpmybpem.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gmkyjanne.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gbvprhahd.sHtML

C#:   s.Split('\n')
来源：http://www.share.vehdjk.com/Article/details/gfhfzqvsp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gdnsvwbbk.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gmhthrjzz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.sjlbkw.cn/Article/details/gypqramij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/gvirpclad.sHtML

TS:   if (s === "") {}
来源：http://m.share.epnwcf.com/Article/details/gthqqkyxn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gjwxpncbr.sHtML


<!-- 参考信息 -->