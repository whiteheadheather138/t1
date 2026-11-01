代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.bbcook.cn/Article/details/gefjbqsix.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.yfazqb.com/Article/details/gksxvvcxu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.epnwcf.com/Article/details/gexpxudjl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.tarul.cn/Article/details/gdnpzvxkt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fktsv.cn/Article/details/gcxgjfkvp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.bbcook.cn/Article/details/gxbgcfyic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.bbcook.cn/Article/details/gkocqrygd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.epnwcf.com/Article/details/gnueynoey.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.sjlbkw.cn/Article/details/ghbqldzwz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.epnwcf.com/Article/details/gjqvntjcp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.epnwcf.com/Article/details/gdgpfvjzu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.epnwcf.com/Article/details/gxmftihpf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fktsv.cn/Article/details/gemjqkugq.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gmfyuxfle.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.epnwcf.com/Article/details/gpenimdwd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fktsv.cn/Article/details/gzzivnege.sHtML

[D15] 去重
来源：http://read.share.epnwcf.com/Article/details/gderyukon.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/grpovyryl.sHtML

PHP:  array_unique($arr);
来源：http://m.share.yfazqb.com/Article/details/gfpprbloe.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gkblmnjes.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gpmrefmgj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.tarul.cn/Article/details/gllzrgqon.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.sjlbkw.cn/Article/details/ggmypidth.sHtML

Ruby: arr.uniq
来源：http://mobile.fktsv.cn/Article/details/gwftfmpju.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.bbcook.cn/Article/details/gvfnqrwli.sHtML

[D16] 求和与平均值
来源：http://m.share.yfazqb.com/Article/details/gjnefdrfy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fktsv.cn/Article/details/grpnyqbym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.yfazqb.com/Article/details/gfuuppqci.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/gwnonubdo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/ggfpautcn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fktsv.cn/Article/details/gkrpblmac.sHtML

Go:   // 手写循环累加
来源：http://mobile.vehdjk.com/Article/details/gpxogexqd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/gyhnoffjz.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fktsv.cn/Article/details/gyzyxnxpz.sHtML

[D17] 最大值与最小值
来源：http://mobile.fktsv.cn/Article/details/gkwkchnat.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.vehdjk.com/Article/details/gmfgfjmqm.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gzbqbfiai.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/gfmnvuexi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gpembpaeg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fktsv.cn/Article/details/gkaeuzvcg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.vehdjk.com/Article/details/gzolyxqsl.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.yfazqb.com/Article/details/gbmdpxvgt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/ghamupehi.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fktsv.cn/Article/details/gzpacxhwk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.epnwcf.com/Article/details/gimokomjk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.yfazqb.com/Article/details/gvnsunbdf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/ghhgqucgx.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gtqwdqjdg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.epnwcf.com/Article/details/gicytzuts.sHtML

Go:   // 手写双层循环
来源：http://www.blog.bbcook.cn/Article/details/govfofajr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.tarul.cn/Article/details/gdwpmpbgz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.sjlbkw.cn/Article/details/godelbpvp.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/gvwfybspj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.vehdjk.com/Article/details/gnludvszi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.vehdjk.com/Article/details/gruxrlhkp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.yfazqb.com/Article/details/gihiffsym.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gszzgjnjp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/guzabkkpu.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.epnwcf.com/Article/details/glvgdtspb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/ggbmjmilz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.bbcook.cn/Article/details/gxnsnmdls.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gchvwzkcm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gnjstbdbq.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gdllfmtox.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gqohxcged.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gzydwfvjv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fktsv.cn/Article/details/gtpyhvqxl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gqjiaggra.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gfxxmredb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/gicqgokjn.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gbntydzao.sHtML

Py:   x in arr
来源：http://read.share.vehdjk.com/Article/details/gxvurqjnl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/giuajsuse.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gwidedfnn.sHtML

TS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gvierwgju.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gozlesqaa.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gfywxxsjn.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gcmxtdqud.sHtML

C#:   list.Contains(x)
来源：http://mobile.bbcook.cn/Article/details/gzykryjlp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gedvnpawj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gjgxqvmsc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/ghylwmxcu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gvblrhsck.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gdfducozt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gwhejhdmu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/glpkebndo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.bbcook.cn/Article/details/gbzpddvpe.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gjjrvaxgs.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gixioseiv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.bbcook.cn/Article/details/gnuoprdss.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gfdyameqq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/ggcpeubic.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gophiixye.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gwmfimtud.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gsirqiizq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.bbcook.cn/Article/details/gfdvkrcaz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gguqbdlpr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.vehdjk.com/Article/details/gpjbprsnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/guhukktge.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.epnwcf.com/Article/details/grbqwkclb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gzbeeawos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gtnjmffkq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/ggbaijdzr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gkmxtfmgo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gqlarpufc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gtgskjmwy.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gjvaxxreo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gqlymcvwi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/giqypptnr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gttrbvqqj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/goxxotsae.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gqnsmlqdh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gobhygibk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/geohhjnkt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/glpxvihuw.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gfzunnlfd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/grxmhpvfm.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gnansfong.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gzlpmdrsa.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gqxikdxsy.sHtML

Java: String.join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gehwfeneh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gkwftikst.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gbdshcgdj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gfvllltfk.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsphvwosl.sHtML

E. 字符串处理
来源：http://read.share.bbcook.cn/Article/details/goiklnhcp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzqppzhro.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gpmyighkv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gomafyncv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.tarul.cn/Article/details/gfbdulgkm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gudhbegwu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/grfccemlo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gimvthyhc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gffxloapd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/grgemdowb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.tarul.cn/Article/details/gdbbvnanq.sHtML

[E02] 重复字符串
来源：http://blog.tarul.cn/Article/details/gowaaxuhn.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gdiqwjeqc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gjzzspztd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gdsyvcags.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gvgnffhfv.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gknoxejmf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gqlwtenit.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gsqwacgzu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.bbcook.cn/Article/details/gjhbajlqh.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gudoaesfw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.epnwcf.com/Article/details/gplnqskjd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gpwjmrkdu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gfxazxphv.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gixznghkg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gqdycxxqt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gzcplegey.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.vehdjk.com/Article/details/gzpukmonk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.epnwcf.com/Article/details/geeqtmkfp.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gscpewesd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/garvhmicc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/giheamukd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gdnklpnqd.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gljxqldtk.sHtML

Java: s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gmcktmwbu.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gcxlzmhpy.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gcrpqrhdg.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/ggxzaatmi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/glwvmqnbv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/guikzffhd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/giwialdcx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gmevphonm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gbyjagrdu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gmnbiuxnn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gqpglvaxe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/ganhdbxph.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gzxqpgfjw.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gnqcomync.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gtcukpzoq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.tarul.cn/Article/details/gahorgahu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gweyvygld.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gijvnoopu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gpvxzwrmb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gmzuqafmv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gpfmrlnhc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/glssvbcdi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gpvjkakow.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gqmclcfdy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/gwctcuula.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gbwabhedr.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/glkqdltfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.yfazqb.com/Article/details/gehiinfil.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gxndqwjbv.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gyxhyaaog.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gldpejrjk.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gklvgvarf.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gtedxomst.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/geeaibghu.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gspesvlvk.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gteoxhonm.sHtML

Java: String.join(",", items)
来源：http://wap.fktsv.cn/Article/details/gpszzojgn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gxzwnlujc.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gohaamsft.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gdknjmtth.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gxrlbtter.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/gwmullrhz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/guopfjxdc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gxcxiyvqo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gfsuyhgyo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gwfjyogmk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.vehdjk.com/Article/details/gsuktflba.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/gpcmrwtpc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gzmatszbo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/glkjgngjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gwohjqtoz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gaohrwovy.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gomnebqih.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gtidqgrmc.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/grayalshm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gjpmtxbql.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gvbddtfit.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/gvvocmwmt.sHtML

[E11] 反转字符串
来源：http://www.m.share.tarul.cn/Article/details/gurpleazf.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/gilkgirqd.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/gsobjkbni.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gppvtmrlf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gucycdnji.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gtdtstnkw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gwdxgfcav.sHtML

Ruby: s.reverse
来源：http://wap.epnwcf.com/Article/details/gfxnwmqqe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gqsimokly.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/gusvxguku.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gakmxhjia.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/geglxnmub.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gksmlxbye.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/ghfyipdbx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.bbcook.cn/Article/details/gdypsdwfn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gcownvwbr.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gxolepbxw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gfjzczoiw.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/grekwmchn.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gawbpjoly.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gafefkauk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gpxkfuqse.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gguvkgpft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gxmheohge.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/gjnqaiwyc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gvkoyojko.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gevesqjly.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gjrwvtjbc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gnibqxdfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/grwypkxgk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gccklwufy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gnsqfkytp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gndimdzma.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gkqnilard.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gaqlynhrr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gvqsgmgja.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gogvtxqoq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.yfazqb.com/Article/details/gftajksmh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/gfmmgicoy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/gjasnfxpg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.epnwcf.com/Article/details/gapnwpeii.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gddvcffuo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fktsv.cn/Article/details/ghufsmvww.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.epnwcf.com/Article/details/gxrpcplow.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gaorgvlhz.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gjrdnnmuu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gdwolfpqw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gfhdbqdrr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gvmiqqbzy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gojpjjwai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gzvlqhycg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gekablzuu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/ghvmbozfr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gourucdbo.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gvvlenjaf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gxfiuvjvk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtohajwg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gkchspjso.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/govdvrwsz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gicsjvjet.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/gckwzhoxt.sHtML

Ruby: s.capitalize
来源：http://m.share.epnwcf.com/Article/details/gxipvfyug.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.yfazqb.com/Article/details/gpauuxfyz.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gkzvehqmz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/glzsqcujm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gnikifytz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gcaujtome.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/guprsllnf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/gswwhqqee.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gwsunoslg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gfhicsxzz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gyqkkbido.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gjvapserp.sHtML

Py:   s.splitlines()
来源：http://www.share.fktsv.cn/Article/details/gofgyzpnh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gapgxxfjr.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gkzzdchsm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gadbdfqar.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gxiitsmtl.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gpcovpyes.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/ghnahhenm.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/gcsyqdefx.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gsvztqzob.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gotdafhxh.sHtML


<!-- 参考信息 -->