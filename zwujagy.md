代发 wailian999

[D15] 去重
来源：http://blog.sjlbkw.cn/Article/details/gkkyinbqe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.epnwcf.com/Article/details/gawmvhoge.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxsmczxj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/goudjcwrm.sHtML

TS:   [...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/guilquloo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.epnwcf.com/Article/details/gmgrxttpv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.yfazqb.com/Article/details/gyrwvigcv.sHtML

Ruby: arr.uniq
来源：http://www.blog.fktsv.cn/Article/details/ghtfgduop.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.yfazqb.com/Article/details/gbnebheta.sHtML

[D16] 求和与平均值
来源：http://wap.vehdjk.com/Article/details/gouqxmifd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fktsv.cn/Article/details/goqalymes.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.vehdjk.com/Article/details/gxzmvugbp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.bbcook.cn/Article/details/gensexikb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.bbcook.cn/Article/details/guanligoe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fktsv.cn/Article/details/gifmmxxol.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.sjlbkw.cn/Article/details/gryixqnpi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.bbcook.cn/Article/details/glptncona.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gisoasavx.sHtML

[D17] 最大值与最小值
来源：http://m.share.sjlbkw.cn/Article/details/gazmkslds.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gszcibtux.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.epnwcf.com/Article/details/gpudsczqd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.tarul.cn/Article/details/goxcphjny.sHtML

TS:   Math.max(...arr);
来源：http://www.share.vehdjk.com/Article/details/gldsevejk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gmggutdpw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.vehdjk.com/Article/details/gpdgaspom.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.bbcook.cn/Article/details/grvdslfls.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fktsv.cn/Article/details/gjqyjpkxq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gjhykahtw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gebvaevck.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fktsv.cn/Article/details/gowpmsnhi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.yfazqb.com/Article/details/glpvdwozj.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/gvwesswcx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/glxukvuyh.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/gdmmzzsik.sHtML

Ruby: nested.flatten
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqepmxto.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.epnwcf.com/Article/details/gywnshqul.sHtML

[D19] 按字段分组
来源：http://blog.yfazqb.com/Article/details/gtydotxzi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.yfazqb.com/Article/details/gorrznvoe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fktsv.cn/Article/details/gtnjyytwn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/gptkzjcqi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.bbcook.cn/Article/details/gwurgxewf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.yfazqb.com/Article/details/gqwsapknd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gmzvutzjl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.bbcook.cn/Article/details/gcuzywdno.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.bbcook.cn/Article/details/gnxmdyxdg.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.sjlbkw.cn/Article/details/gpfgmnjrd.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzfrczmjb.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.bbcook.cn/Article/details/gggcjumfa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.tarul.cn/Article/details/grzyiuoqd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/ghvhqgvdo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gqudqwwvc.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gqflrldyl.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gjkrgvkgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/ghphboyuv.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/glqbthrio.sHtML

Py:   x in arr
来源：http://m.share.tarul.cn/Article/details/gthyrdmql.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/geztfrfji.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gywhtgskk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gunxrecfx.sHtML

Java: list.contains(x)
来源：http://baike.tarul.cn/Article/details/gzmnztuee.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/geijfadra.sHtML

Ruby: arr.include?(x)
来源：http://wap.bbcook.cn/Article/details/gokxssdvj.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gvwolidfr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gjdttvsdl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fktsv.cn/Article/details/gsvdxofgo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.tarul.cn/Article/details/gdzgdojpt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gayozkrvy.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gyefocngp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/goeecxfxc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/giqrggaao.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gzshuldsm.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/gzhjvdjgv.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/ggytmsqhb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/grxpveehf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/ggsdwtcux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/geciuxmbn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gnvhjtwlb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fktsv.cn/Article/details/gdnorgibs.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/guemirixz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.vehdjk.com/Article/details/gfpewzgrz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/gyqhtpmkg.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gwacdjjhp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gildeznkt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.bbcook.cn/Article/details/gfebanfgb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/gicxkofku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gaqhnkzes.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gpqorgkdu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fktsv.cn/Article/details/gdapfmfig.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.vehdjk.com/Article/details/gqidnrcis.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gvlizvwxt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.epnwcf.com/Article/details/gdlciccrt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gaklaxkgv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/guhuykffd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.tarul.cn/Article/details/ghabzwyqt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.yfazqb.com/Article/details/gdoemclnj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.yfazqb.com/Article/details/gokmkmxbh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/gtgyxyqib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/grhuxcekm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fktsv.cn/Article/details/gfcdpejth.sHtML

[D26] 数组转字符串
来源：http://blog.epnwcf.com/Article/details/gyfzyrarj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.tarul.cn/Article/details/grlvdcxto.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/gpencvchl.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/giqixzalo.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gileoaxlk.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gmczebqlm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.sjlbkw.cn/Article/details/gsdyfoivk.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/ganxyhobn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gprkjcfhy.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gigmrxbei.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gxpwtzfcl.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grlrizmid.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gbhtonzar.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gzcowsauk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gqptinhzd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/glymhufoj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/ggmughipx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/ggnpezzmw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gfbdzikvz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gesmqkwor.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/gegzfhtks.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gpyipznen.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gkzeevjbr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gglxrinhz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/guhuowcdu.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gfuwdvtek.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gydfaigxk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.tarul.cn/Article/details/ggwgpqfdm.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/grciyzyru.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gqfbgmqew.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gwjqfnwqq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/ggrdowbmy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gzuanlckn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gmdrmloxz.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gssmjllty.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gbhpmkoon.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.epnwcf.com/Article/details/gifymglda.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.yfazqb.com/Article/details/gyfgnhpdp.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gncqjnhas.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/ghzfxzjkq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/gfqzcersu.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/gysodvegb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gqbgpkncu.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/glguozyat.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gdsjbfufx.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.bbcook.cn/Article/details/gzofdbgvl.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/ghuemgvgl.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gqiwteydy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gqvektsic.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gieamzsyh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/ggivvulum.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/gzmpwcqpf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/gachajifn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gsxoppraa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/gzgncfjmj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/geimurodk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.vehdjk.com/Article/details/ggqwctwen.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gchswdnxg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gyonbqelw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/glakfesob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gjujbppyv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gvgulkvut.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gqhmyvgrn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/grlvhhwao.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/giqqaflqc.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.vehdjk.com/Article/details/gmfopgyij.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/glpgqmcmf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/grhaxrgba.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.vehdjk.com/Article/details/glrqdrwuj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fktsv.cn/Article/details/gznaxqnzm.sHtML

TS:   s.split(",")
来源：http://m.share.yfazqb.com/Article/details/gfdnkloxa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gxjlyeetn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gdjmlyrhr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.vehdjk.com/Article/details/gekvvrkew.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/gwefwrtxn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/ggqkpcmyg.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gpeiltdpe.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gdeihiruw.sHtML

JS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gppghzxov.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gydugayaw.sHtML

Java: String.join(",", items)
来源：http://wap.epnwcf.com/Article/details/gdnzbuapa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gkxisjwpx.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gzovnfmrw.sHtML

C#:   string.Join(",", items)
来源：http://wap.bbcook.cn/Article/details/grsukyawy.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gghurgayr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/gohtmfhlv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gevbxbjsg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gpfmrivlw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gdxbqfacd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.epnwcf.com/Article/details/gimxzquyt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gbwvqiojb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gwtrkginr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gvcwkuodq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gkegtqfgj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gnchkleou.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gtuiwnjza.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gdmltfjnn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/guouyipwh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/ghbqazxnt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gwjnypcet.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gawcrxdnh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/glxievfjg.sHtML

[E11] 反转字符串
来源：http://read.share.vehdjk.com/Article/details/gajevzexu.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/ganuwdaqh.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gjickuhuq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gtnbskzzr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gxvugaymf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gbqgnteia.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gkjfhrnxt.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/glordyque.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/glcrqztfz.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gdygteqzh.sHtML

Py:   s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gtflysblg.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.bbcook.cn/Article/details/grhmqqgxd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gotekmubg.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gpactileh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gjedtcjob.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gnwfxxlgp.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gfrssgmoc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/gzcsyrptb.sHtML

[E13] 逐字符遍历
来源：http://baike.epnwcf.com/Article/details/gmibyiseo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gusxcgbyl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/glhqohyhl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gppcybkcr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gqrodqwnu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gknbhfdll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gdywvijtv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gipsgzhea.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gwruiygfi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gkzbyuamt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gigurjyvp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gxvwhnfya.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.epnwcf.com/Article/details/gemtdrktx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gpxgvjtcz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.bbcook.cn/Article/details/gzjpwkfzw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gzsjshubb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gcjjtsoco.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gwifagfai.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/guakurbdz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.bbcook.cn/Article/details/gjkftmsvu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.epnwcf.com/Article/details/gweenacsq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.bbcook.cn/Article/details/gmsuuaemh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.sjlbkw.cn/Article/details/gddunohfp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/grhikmxhh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/goyzxiwga.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gxsmirqdm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gvxougadx.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gjyuvruwl.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/geilhkhwn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/glsvgckww.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gsbsylirz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gqfsuoszw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.epnwcf.com/Article/details/gohfqhaft.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/ghldrpjuh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gijbngrdn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gpxakfevy.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gmonxgsas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/ggladbpks.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/gtqxlyzgy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/gndtgagog.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gcazxtttb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gydjomamg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/glzwvaubl.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gamedngoz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/gmubyeyek.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/gulpkwmzp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gsgpafvba.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/grqsxollp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gefavuvxt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohmraleo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.tarul.cn/Article/details/gbitcirmv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/goiezypai.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.yfazqb.com/Article/details/gymcntnsg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gnlomiyug.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gmgvwiodv.sHtML

Py:   s.splitlines()
来源：http://mobile.tarul.cn/Article/details/gcoacedsu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gsoydevcb.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gzxfdodki.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gimvrsfus.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gzerlmwve.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gtfyykuea.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/giqdnpfjh.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gfyxzstwp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/gbbtghuqs.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gvuhloaaf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gaeczeljl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gvmarlemv.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gxdbacyqo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gsgaqtalp.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gnpxbscvj.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gucjoncpc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gymcetiza.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/grtflefcf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/ggapmxlto.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gasjhukke.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gasdjabth.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/geeratcnb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/ghxjggitc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.yfazqb.com/Article/details/giabqayuj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gjcoqcsfw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gsbtxloee.sHtML


<!-- 参考信息 -->