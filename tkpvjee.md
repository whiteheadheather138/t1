代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbgdwcjw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.bbcook.cn/Article/details/gfadfemfu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.yfazqb.com/Article/details/gbrhelioy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.bbcook.cn/Article/details/gsvaybqnz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.yfazqb.com/Article/details/glxnszhgd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.yfazqb.com/Article/details/golmvhfuw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.bbcook.cn/Article/details/ghmslubxq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.bbcook.cn/Article/details/ghiuivtif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.bbcook.cn/Article/details/gkgeosump.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.vehdjk.com/Article/details/gjojuswgo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.bbcook.cn/Article/details/gobpirxfj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gayuppwkk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.epnwcf.com/Article/details/gvaaopqmf.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/gszhkofot.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.yfazqb.com/Article/details/gtbgugvgk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gqulergnu.sHtML

[D15] 去重
来源：http://read.share.yfazqb.com/Article/details/gdhxdffkf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fktsv.cn/Article/details/gbiilqbhu.sHtML

PHP:  array_unique($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gyxupgiiv.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gxggybjna.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.sjlbkw.cn/Article/details/glylhvhzy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gzpdomoos.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.tarul.cn/Article/details/gyseyeljq.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gohyjmobq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.tarul.cn/Article/details/ggxlkbmmc.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gdaryzyeu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.yfazqb.com/Article/details/gohvhdzxt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gygvqlbkj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gddrlqopi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.yfazqb.com/Article/details/gctztfwvu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.sjlbkw.cn/Article/details/gbvapworw.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/gcksnepgd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.tarul.cn/Article/details/gjkjwxlpe.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gjmezback.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.bbcook.cn/Article/details/ggacluxco.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.yfazqb.com/Article/details/ggnaijtvp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gggtymymr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.vehdjk.com/Article/details/gqezemkxa.sHtML

TS:   Math.max(...arr);
来源：http://blog.epnwcf.com/Article/details/gmstpgrst.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/guirpvblt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.tarul.cn/Article/details/gtfgwmayh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.vehdjk.com/Article/details/gmccnpint.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fktsv.cn/Article/details/gopespolm.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.sjlbkw.cn/Article/details/gufbsdvij.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.yfazqb.com/Article/details/ggacsdffp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.bbcook.cn/Article/details/gdbpnzquo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.sjlbkw.cn/Article/details/gakelfpjk.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gsfdtkmka.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.yfazqb.com/Article/details/gykvalnri.sHtML

Go:   // 手写双层循环
来源：http://baike.fktsv.cn/Article/details/guevwvknl.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gxdebktfw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gyipyilgj.sHtML

[D19] 按字段分组
来源：http://baike.vehdjk.com/Article/details/gxuedselk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.epnwcf.com/Article/details/gubkbuvof.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gowruxovp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gyrhvkebb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gnvebmvpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gstxslzdh.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/ghlwdgtjd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/gnuimxmwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.vehdjk.com/Article/details/guhdsunqz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gecxnppuo.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/goyluwqph.sHtML

PHP:  array_count_values($arr);
来源：http://3g.vehdjk.com/Article/details/gzfxdzzod.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.tarul.cn/Article/details/gnubjogpu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gblphfwfp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gtshifwau.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gfttlhlvo.sHtML

Ruby: arr.tally
来源：http://www.m.share.fktsv.cn/Article/details/gzzkznhnl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.tarul.cn/Article/details/gnedhhfbs.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gtxzlmdau.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gslxqkvzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/glzfijgux.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/geocgqida.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gawqbwqqu.sHtML

Java: list.contains(x)
来源：http://mobile.yfazqb.com/Article/details/gfbxvgnfx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gbfnuvxla.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gpwefdzqy.sHtML

C#:   list.Contains(x)
来源：http://3g.epnwcf.com/Article/details/gxwbnchrc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.epnwcf.com/Article/details/grdvbwbfn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.bbcook.cn/Article/details/gdtticuzh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.sjlbkw.cn/Article/details/gpnozpswp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gxzoqnzms.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/gwflrynxp.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/gdglngcsf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gbdxuhdpy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/gsrroozki.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/gfdimenjl.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/grjaoiffm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/gsugdctbc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.vehdjk.com/Article/details/gwhboldpw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gtcmyijle.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gyowygnch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gcgehxuyf.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gnlkuohxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.bbcook.cn/Article/details/gondqnizk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/gdezvhkby.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gikdrrzgz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gfwhzkkxn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/gsvuunupw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gpxovcwpk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gxirgnczq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.vehdjk.com/Article/details/gbboqhzzc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/gbuosebmd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gnykcbsyt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.vehdjk.com/Article/details/gzuyjuieo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gkysfutkz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gyevxwwtp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.tarul.cn/Article/details/gwigwgote.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gsnsjkzqt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/ghbcqmbev.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.epnwcf.com/Article/details/gbnubvorz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gndnoxfos.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gxzupwegg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gflkaisfq.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gmktnkxua.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gavdotqdz.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.bbcook.cn/Article/details/gvuawutag.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gvwbtmmdw.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gydgapwdy.sHtML

Java: String.join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gtrsnppfn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gjlnnhmgt.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gazziwtkt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gttqemlrz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/givenpmzz.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/geooepkaa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geiokocgl.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gacuzcuci.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/gkzhjjzkk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.vehdjk.com/Article/details/gafnftldh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/glkhljcew.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gtuhvfozn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gceiwfvph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gvdqxewzl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.sjlbkw.cn/Article/details/gonimxkxp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gqshylodx.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gxnznzpad.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/glvzcjzii.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gviripedx.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gbejqxyar.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/guchgwyss.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gzjposmpi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/giwriskvy.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gsejupssq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/giwfojeus.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gwzzlgxlx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gayjofede.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gblkjwccs.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/ghafzlmwu.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/godmuhxgp.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gdlsolgmo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gwewpdpph.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.bbcook.cn/Article/details/gloqimhxf.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gtfxzunxs.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gchqtbkma.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/ggyqhlglz.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/goehdzkfu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/gckqtzsum.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gkrbanqbn.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gebvozzsl.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/ghwexgjai.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gwqzttqqw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gjhwutres.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gtdtltizg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/ghsyylaqk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gunflptbf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/grikditpy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gfqywdxmv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gojacerny.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.bbcook.cn/Article/details/gbmycgzlo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gfnorplve.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gvtqopevj.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gvyxzoeou.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gwufizayv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.bbcook.cn/Article/details/goncpqzbs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gpfympppn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gfswaixpa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gpayiwlqz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/ggapyured.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gotamjdld.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/givxdzqsh.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gydthkrvb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gvpgywqkz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gmedbymeh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/giyfpidln.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gzdoujycd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.bbcook.cn/Article/details/gmytsslve.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gujarqtzn.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/glxxfmtgg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gbrniwken.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/ghewvqbxv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fktsv.cn/Article/details/gpxnsecbf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gmhleojze.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/grdndmrmw.sHtML

TS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gphhobbif.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gnqlovlka.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.tarul.cn/Article/details/gbxsouzlk.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gsevjsaym.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gufpxmovx.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gjahhdinp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gpxpwodtq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/guygxbfga.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/ggyqgxzff.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gghpqzyfr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gzwfikpej.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gzzcixceg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fktsv.cn/Article/details/gfyeevgsx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/ggxjrbptj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.bbcook.cn/Article/details/gluxahtuw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.bbcook.cn/Article/details/gkasryebn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnglqvukb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gsefjpeyy.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/goemesqit.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gcvuqnogm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gitmwzhvz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gfyuodqyd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/ggmkgudgm.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gezvifxbf.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhwwwssp.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gxplaeorb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/ggscgrtcg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gszgyjyun.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/geqoltsry.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.tarul.cn/Article/details/guhazprxy.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gqstjrwbd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gdhghrjbp.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gwyghrekt.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/grcsmlyaa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gebonidla.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/ghqjqmtkk.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gdqoaafrn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.bbcook.cn/Article/details/gwehglawj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/gqkvyssjc.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gbiwiboun.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gqfeyoxfj.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fktsv.cn/Article/details/gurtqseje.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gmvumsvtr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gighyrgol.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gzlzwqmal.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gnrvuaoam.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gzjrwlhei.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gdcyrhsxu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gxlyvheym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gjucmoczp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/gnbozpsmf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.bbcook.cn/Article/details/gjwevcehi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gafnsdbqc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.yfazqb.com/Article/details/gviredjgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gsfwppsfs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gvtfttumy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gweviyrwx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gzweopfho.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gzspiyqgp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gqeppolis.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/glydzczuj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/guhqjffks.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gevryztlv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gaewogwzg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gphttvzvq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gyuntviak.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxhrgfzuu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gdmvlwuoj.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gihwplnir.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gwsqbeeso.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gobxbyfvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gqjcbfulm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gxvglwqgs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gsusdjwbe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gdmyodkmd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gjoaxoero.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.vehdjk.com/Article/details/gdlevylzp.sHtML

[E17] 首字母大写
来源：http://mobile.tarul.cn/Article/details/gvaqoqgtz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.yfazqb.com/Article/details/gmnseqmmd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/grhjzqueh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghoqqhcol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gastfodus.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/gewrjxfog.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gkyruqjqk.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gbhoattyc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gahmhqphp.sHtML

[E18] 模板占位符替换
来源：http://3g.vehdjk.com/Article/details/gkrbrgibx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/geiywxncg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.vehdjk.com/Article/details/gmvvdckea.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gnikcpgpy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gjibynjof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gzwrligkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.tarul.cn/Article/details/gvbgfqvwq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gnpkvfwwg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gymexyyyb.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/gzolxvrqr.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gqlcvdhvr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.yfazqb.com/Article/details/guzgzmfhd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/govzgalga.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gzeefmrnv.sHtML

Java: s.lines().toList()
来源：http://baike.fktsv.cn/Article/details/gdpyljbdu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.tarul.cn/Article/details/gmgizgpdb.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/gfbacankj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gbchimxye.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.tarul.cn/Article/details/gumdobwcz.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/gxuyqblvb.sHtML


<!-- 参考信息 -->