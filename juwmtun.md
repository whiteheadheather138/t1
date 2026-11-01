代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gdktgizos.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/gtqmetqal.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gbjecphwk.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/grqboesxk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.vehdjk.com/Article/details/glhkkdwua.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gkawklzxn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.yfazqb.com/Article/details/gxomppazr.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/gkttaumcc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.sjlbkw.cn/Article/details/ggcbxruwt.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/gvmpcpeow.sHtML

Ruby: nested.flatten
来源：http://read.share.tarul.cn/Article/details/gvtjyfihe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.tarul.cn/Article/details/gvrzncqhr.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/goboamytb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.yfazqb.com/Article/details/ghrwykhxi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.bbcook.cn/Article/details/ggwdjjsls.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gnszkkjtw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gpoznicre.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/gneyxbsai.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gekflywux.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/ghfbpavee.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gxffxeqcb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gcohtawam.sHtML

Py:   Counter(arr)
来源：http://m.share.epnwcf.com/Article/details/gxkkqycvd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gqbyfwodw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/gmasbogyk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gzsigimrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/grvwhdzde.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gzbwwabyi.sHtML

Ruby: arr.tally
来源：http://www.blog.yfazqb.com/Article/details/gamyxthju.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gkkxdypdm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/gwlkabvzn.sHtML

Py:   x in arr
来源：http://read.share.fktsv.cn/Article/details/gcvjjhszw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbybnustl.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gwfcggeyl.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gedaybkzr.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gpkuiwhix.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gdyugpnqc.sHtML

Ruby: arr.include?(x)
来源：http://wap.tarul.cn/Article/details/gtxnowyaz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.vehdjk.com/Article/details/gcmoprtkk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gqrndnmoh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gxwnhobkv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/gbxrhqkxq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.bbcook.cn/Article/details/gjrncrrwk.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/gtujgvdpt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/gkryfszru.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gmuzcdtsm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.vehdjk.com/Article/details/gozkhmyjf.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gyqfcokcp.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gjoevwuck.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fktsv.cn/Article/details/gbwrjwnam.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gwvxcvglg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/geththtca.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gkyeyfcmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.yfazqb.com/Article/details/grjnzndtv.sHtML

Go:   // 手写循环
来源：http://baike.bbcook.cn/Article/details/givgnkpiu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/ghyzucrfq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gbungkeyp.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gdzarymcx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fktsv.cn/Article/details/guyglqeaz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gozryytqx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gynlybpba.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.vehdjk.com/Article/details/glntvwigd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.bbcook.cn/Article/details/gxjudwquu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gftoinfxy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gknvjaahs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gbiyamprs.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gcqqiymfx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gecubpbhd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/gyysxdcos.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/ggmonhqze.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.tarul.cn/Article/details/gwsncmtqj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gljetlhjz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/guhxaldrj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gvilxtlei.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gdepnrhsi.sHtML

[D26] 数组转字符串
来源：http://wap.tarul.cn/Article/details/graxdxfby.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.vehdjk.com/Article/details/gnoknobpn.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gkzfshdzp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/guthoaxcc.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/grtaqxfmu.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gzvihnnlr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fktsv.cn/Article/details/gmhgiqxdk.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/ghtqwzhbf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/goruymibm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gilkevzlh.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gtokhbfin.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gazjbjtzs.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gsbheyiqg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gydtzbicd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gmvohsafb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gpxigfvuh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gftpdaoqh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/glensgfpz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.sjlbkw.cn/Article/details/gtpmrzscq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gunmweold.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gckuxshte.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggehuwygz.sHtML

Py:   "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gekilzxgx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gmoubndkv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gwzverlim.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gytauwxxm.sHtML

Java: "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/glfffvljq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/gajjpzadd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/ganlatkvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gtjdrtuhr.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gtykzjxlf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gxhaezcfj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gtpkrqgwq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gssfqwdhi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gqeawfkwa.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gbjiaxtdc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gwzquzpkw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gbyzigvhe.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gdohhohhh.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gbgeqkbfb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gsgllsgxz.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/grhnvfdom.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gedxpkbhw.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gexzuomtl.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/ggsopwgon.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gsfunghcd.sHtML

Ruby: s.index("x")
来源：http://3g.tarul.cn/Article/details/gopinolud.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/grbksaflj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gtnhclczn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gjidqvpvu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gxndnixhb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/ghcgwgmnk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gmnfhfqss.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gjqjuznzq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fktsv.cn/Article/details/gxddslrmr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gyvgvtavv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/grncsmang.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gfrgesuaj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/glmbttpew.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gqktrysms.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gkrqpadyj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/grrjceulz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gyrfgrlry.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/goqtaubhg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gwasagcgp.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/gywypjgkm.sHtML

[E07] 按分隔符拆分
来源：http://baike.vehdjk.com/Article/details/gcaotgkde.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/glnobqzxe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.tarul.cn/Article/details/gwegyhrql.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/gpjvccgjx.sHtML

TS:   s.split(",")
来源：http://baike.fktsv.cn/Article/details/gmktxodib.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/goxcjcxss.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.bbcook.cn/Article/details/ggehaezjl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/grftdxurt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gzvnjpmpi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.yfazqb.com/Article/details/grxwsqlsq.sHtML

Py:   ",".join(items)
来源：http://blog.fktsv.cn/Article/details/gcmsmtjsb.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gvvpzavai.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gpbdblzfj.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/ggxdzttcg.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gbqwmgbye.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gxugmoqid.sHtML

Ruby: items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gwxrnyoyt.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gduyjsyhg.sHtML

[E09] 去除所有空白字符
来源：http://m.share.vehdjk.com/Article/details/gmlwocmzd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gbucwbiub.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/glguyoput.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/garkuptrq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/ggkzewgaq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gutqhxmfj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gxtxyrzxg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.epnwcf.com/Article/details/gzmpmxvue.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gzmwekrlg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gxfanchhm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/ghnyptrpo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gadfzizbq.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gcltqhczl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gwcsdzxwj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gdaktgyrm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gzfqnqzbg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gtyjkhxsv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gxlicttti.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/ggjeprppi.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gmtiyaxuh.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gyccmomml.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/glvoiikfy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gblrurdke.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.yfazqb.com/Article/details/geowwneus.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gfdcebwad.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/guxstzwid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gubyvscmc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gnirbdkvq.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/ghskfyxsz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gkteolmaf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gdifizzcx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gmdmbzwzs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gugrktuaw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gyqkjwzsm.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gnketedvx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gzidvzvlv.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gvmeeqodd.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gwzlgrhbr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gvadkltbf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gdzpgmoqe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gukudqhbw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/grmiamxgg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gcpuyptis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gztyxetgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gplvdndej.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.epnwcf.com/Article/details/gwjovstiq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gwtfwcrgm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.bbcook.cn/Article/details/glmdsxikz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gbdlqbmlh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gadbbqlof.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/goxqznogo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gaztyclwa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gsdbokdmr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gbcxxsdif.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/ganpgviau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gwgvxuzjw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gaahscjhl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gbxyamxvd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gfqtqunub.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gxhubfpyv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gmlsypujl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/guaioyebb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gtleexffw.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gmqtgrids.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gnepuhryn.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/gvcwicocm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gwmwjwzay.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gjoznomvf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gklaxpdcv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.yfazqb.com/Article/details/gzfddqsdu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gtwgggood.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/gcqwpfmbo.sHtML

[E17] 首字母大写
来源：http://baike.epnwcf.com/Article/details/guflxnaif.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/ggiiuhqii.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gwmwqzqcu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gspdumvqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gxsovkdww.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/gadzzlovu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gexurmbpx.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/glfadepmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/gsmshogyx.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gqjefahhr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/grqappiip.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gbhzfrpnr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gwnpzhvqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gdjtnatim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gyuflgjbt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gaecrefqq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gveydzstm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gglckhdji.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/gpxqqipxl.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gknevutww.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gjlmagdva.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gwvlrsppt.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fktsv.cn/Article/details/gduejiivk.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/geunuxwha.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gshtqblwo.sHtML

Ruby: s.lines
来源：http://www.share.sjlbkw.cn/Article/details/gxckasuut.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/gxeongfiw.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fktsv.cn/Article/details/gzmvpdbds.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gvnicobxx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gjlaxtgsi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gnmjxuahx.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gapwxopsi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/grwjeyrij.sHtML

Go:   if s == "" {}
来源：http://mobile.vehdjk.com/Article/details/gmlrfqgnu.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gcotcofma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/glejyfuvu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gzbltydnm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gtwprqkig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gaxfzlwqy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gatfmwfdq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gfoqetivu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/ghafbrvon.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/ghrqwxtho.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/ggevuljqt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gifujchps.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.vehdjk.com/Article/details/gbgwcbrpg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fktsv.cn/Article/details/gpawqkour.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gdtkmmpcy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gplahhjyv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.epnwcf.com/Article/details/gqziylpzp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fktsv.cn/Article/details/gulrvvaqu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fktsv.cn/Article/details/gtansyoee.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gxoitgfxw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.vehdjk.com/Article/details/gbrdypgsg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gvkxnzgvk.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gvxhpnhro.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbxegmkyp.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gblganvix.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.vehdjk.com/Article/details/gqzqhlldi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gzeguxbfx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gtdjmzrzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gsrrabfcv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gcsgxisne.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.bbcook.cn/Article/details/gkxuwycat.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gdpftftez.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.tarul.cn/Article/details/gpiuzhhvz.sHtML

[F02] 逐行读取文件
来源：http://m.share.bbcook.cn/Article/details/gpocsymnr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/ggvwnidfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gnzlamtdo.sHtML


<!-- 参考信息 -->