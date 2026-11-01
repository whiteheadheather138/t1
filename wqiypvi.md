代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.vehdjk.com/Article/details/goiibbhjf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.vehdjk.com/Article/details/gwgstlvny.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.vehdjk.com/Article/details/gxwikuymg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.epnwcf.com/Article/details/gbtbrlnhi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.yfazqb.com/Article/details/glsbrtnlv.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gdfsmqllw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.sjlbkw.cn/Article/details/glizpjpnr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.tarul.cn/Article/details/gqigqbjyh.sHtML

[D15] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gelwbgtjr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.vehdjk.com/Article/details/glvuhngin.sHtML

PHP:  array_unique($arr);
来源：http://3g.fktsv.cn/Article/details/gbctrkkqm.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/grxswcciu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/ghyomhers.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fktsv.cn/Article/details/ggmpojscf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.tarul.cn/Article/details/gkzxtogye.sHtML

Ruby: arr.uniq
来源：http://www.m.share.epnwcf.com/Article/details/gfjomblps.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.vehdjk.com/Article/details/ggngaoidl.sHtML

[D16] 求和与平均值
来源：http://www.m.share.vehdjk.com/Article/details/gczehlpjq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.sjlbkw.cn/Article/details/gveeadfah.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.yfazqb.com/Article/details/gmlsgeebq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gzuncfkmg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gxsrscama.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fktsv.cn/Article/details/gtfjnkzlc.sHtML

Go:   // 手写循环累加
来源：http://wap.sjlbkw.cn/Article/details/giargtlrq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.vehdjk.com/Article/details/gcqcajzig.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.epnwcf.com/Article/details/gonpsmavg.sHtML

[D17] 最大值与最小值
来源：http://www.blog.vehdjk.com/Article/details/grqmneupt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gncpqswig.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.tarul.cn/Article/details/gvmdzjdcf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.yfazqb.com/Article/details/gpvhpksqv.sHtML

TS:   Math.max(...arr);
来源：http://blog.sjlbkw.cn/Article/details/gqscmzljr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.yfazqb.com/Article/details/gfqhbzrmm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.bbcook.cn/Article/details/ghxxjfdir.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.epnwcf.com/Article/details/goviszqyg.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gckystwmk.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/gacglwdes.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gxovqcomh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gkazoihqs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.tarul.cn/Article/details/ghkbeuqdk.sHtML

TS:   nested.flat();
来源：http://read.share.yfazqb.com/Article/details/gyzhsfgxs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/gkpaiwvyi.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gidquaphc.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/ggbhyfddw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gikmvjlht.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/gllyropum.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gowfccqrs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gbzlucfod.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.epnwcf.com/Article/details/gniqhpike.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gtxkxqyna.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gcqmcjial.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.epnwcf.com/Article/details/ghqzqhhzc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.vehdjk.com/Article/details/gdidxltec.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gpdvcnnxl.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.vehdjk.com/Article/details/gnhhbqqay.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/gxodcdfuu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gixwaptxm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.bbcook.cn/Article/details/gobacvctm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gdqukzinv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gpssdkqvv.sHtML

Go:   // 手写 map[T]int
来源：http://3g.tarul.cn/Article/details/gcrtgtsmr.sHtML

Ruby: arr.tally
来源：http://read.share.bbcook.cn/Article/details/gvabpuako.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/garvzjmlt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.epnwcf.com/Article/details/goohbxmzs.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gvbznccmh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gehnvaeno.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gfwgtpjdx.sHtML

TS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gjxakucay.sHtML

Java: list.contains(x)
来源：http://read.share.sjlbkw.cn/Article/details/grqablyza.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gehnbcyub.sHtML

Ruby: arr.include?(x)
来源：http://blog.vehdjk.com/Article/details/gcobtryug.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/grkowupmh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/ggqjwxgmd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gnpfbckxu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/gixzkgnmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.yfazqb.com/Article/details/gjvcnwdse.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/guoovzowz.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/ghpfdhbio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gzsyoprqn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fktsv.cn/Article/details/gyfxrfyrg.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gimggxcrl.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gksbluxta.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.vehdjk.com/Article/details/gpyzgfxlp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gbvqregmk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/geopsdokf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gjqhoxfdi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.yfazqb.com/Article/details/ghusckjnq.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gcyeppdwg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gvdzmftlr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gqgcjrzzx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhvaxrub.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/gcbtiwvsk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.yfazqb.com/Article/details/gfdxcjzwr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gpkdktlox.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gdhsxwloa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gsnjjhmdc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/gpgquyoor.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gzkxlfsmn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/geexfecok.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gbuuyymqg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gayezemhd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gagyjpkuo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gxozwdygz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fktsv.cn/Article/details/goapxajrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gdijckvmx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gzkhzhjdl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gddtldepv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkkverfo.sHtML

[D26] 数组转字符串
来源：http://baike.yfazqb.com/Article/details/gyudyyjvx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.bbcook.cn/Article/details/gagjchuvj.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/gdbsgyrin.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gpflmuasb.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gexsonmif.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gpvfaoylc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gkbaupsrn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gjsmikuai.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gfvqxphiv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcvwbnmny.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gjsqcjuzd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtecdukfy.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gyvwtxoaq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gtxysprjf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.yfazqb.com/Article/details/gqjaiqmcs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gchlrjwzl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/ggiqmrnwd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gugrnpjoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gvjuefzqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gidjwcian.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/gphxaxnrh.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gcmvwjdod.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/guiysqikh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gnjosqojn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gyenvykso.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/gphwkwvhu.sHtML

Java: "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gfiinziwf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/govrnpiwk.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gfxtjadpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gviuonmta.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gqxqsgdur.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fktsv.cn/Article/details/gwlkmlnsg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gepuoklhf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gowlphrmj.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gorjavmjb.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gnoqxbsfw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjccqhen.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/giacaudwd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gfxtfrikd.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/ghyyhvmxc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/grzsbxtuq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/geqhlvfxm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gukxlncfb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gruymfshx.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gegyqzomm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gfhkzhshf.sHtML

Ruby: s.index("x")
来源：http://wap.yfazqb.com/Article/details/guhvafqqy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gxwrusxjk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gyzsnoqhm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.yfazqb.com/Article/details/glgiyzesk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gnzpnetxx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gfwclsqcq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gjfvfeuxx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gzzcbhwhu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gylywrbgu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.epnwcf.com/Article/details/gmkrdyrxw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gxtkypczh.sHtML

[E06] 替换子串
来源：http://www.blog.yfazqb.com/Article/details/gzseejozu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/glqtvjnvx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gihnlagno.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gynjtnhva.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/ggpubpwlm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gdrmhwmrz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gekbfbtqi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gwvptnzml.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gxmktkxjl.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/godppobsc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/gzbporqtg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.tarul.cn/Article/details/gpujnfwze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gdqywxcex.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/gpeivqtrx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gusakjhgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gccdcbrho.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gvvojwgsz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/ghodhzatw.sHtML

[E08] 数组按分隔符合并
来源：http://blog.yfazqb.com/Article/details/gryuefdxl.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gnpzlcqhz.sHtML

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/gezayrdvj.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gdiffotoa.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/ghzcetnfu.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/ghpgthzbo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.epnwcf.com/Article/details/gphssvpwq.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/glsnarssv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/grpolojsk.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gmvpwjiic.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gffvwvdkt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.vehdjk.com/Article/details/gfyomkhkd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gqnccgyju.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gjffjymsf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gxghyjeix.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gnrrlyomr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gqxgbjhdq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmogrqvlp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gfmnuggur.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/gtztcowbp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gtygvtivx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gceysyasd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gcwoqdpty.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gdosadosi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gcqlmlxbh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/ggphiregj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gwenrwrye.sHtML

[E11] 反转字符串
来源：http://www.blog.tarul.cn/Article/details/gkbflwajy.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gidjeeean.sHtML

PHP:  strrev($s);
来源：http://www.share.vehdjk.com/Article/details/giuwvqeba.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gwjvogmfv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/geekxbchy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/goumzlust.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.bbcook.cn/Article/details/guwbcdxsw.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gcysukxcx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/ggrxwcosh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/gztiumeri.sHtML

Py:   s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gojqivyyo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fktsv.cn/Article/details/gzwnjjvan.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gsfouyvrh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/ghvumztyj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/gvggibeih.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gudqkcjlc.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/gnplqason.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/ggviqnjtp.sHtML

[E13] 逐字符遍历
来源：http://blog.bbcook.cn/Article/details/ghknpvomu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gjtzvpuzz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/gveqtdfel.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/giucgonce.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/goebpvgcv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gpwiewrvz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gdhegymdc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.yfazqb.com/Article/details/gjwqoukij.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/gkqysodkl.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/groaxjbud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.bbcook.cn/Article/details/gucaqqkyx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gmmmalbjm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/gdkwayrle.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/ggjzqwxwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/grkpmzvtt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/grtvhewmc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gusdxlrbc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/giccpwiwn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/geujlplsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gokkrhgmd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/goqockmim.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gcmexhxtr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gowmccrty.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/guatzijij.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/grbjzhttp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/glyjpjfso.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.epnwcf.com/Article/details/girijztcx.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/grxewipuv.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gvjtmstvb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/glurkicwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.tarul.cn/Article/details/ghlbnolsp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gizivlcko.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gdwhwobxe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/gwhaxcavr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.sjlbkw.cn/Article/details/ghjdtapnn.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gvrrnzohb.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gaaixrkkn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gidvcregw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gfxtloinz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gbwrljxma.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gnwmgfsjq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.bbcook.cn/Article/details/grfvyknqe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfzspsgv.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gyxkuhlsz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gyavcyygk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.bbcook.cn/Article/details/gjzomoyvd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gzyavugmz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gvorqcjlx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gwktmmcta.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/ggldtpagt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gxocmjxjd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gefubboix.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gfjpatvmw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gfrcwtzgv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/gewkawjqu.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gzuqwuuhf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gihskwrty.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/goqmqryhx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gxusjgimm.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/ghbjjysgf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gpgttpirb.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gffpmtydj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/gqpsqjepv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gyeieglsv.sHtML

Py:   if not s:
来源：http://blog.vehdjk.com/Article/details/gtinooata.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gdbeovluo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.epnwcf.com/Article/details/giwocoapc.sHtML

TS:   if (s === "") {}
来源：http://www.share.sjlbkw.cn/Article/details/gfsadqvyn.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gbyhqbumc.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gbmiftazw.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gkrhgmjnh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gifybjrfx.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gkqfjwvcv.sHtML


<!-- 参考信息 -->