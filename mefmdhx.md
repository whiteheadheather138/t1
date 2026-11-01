代发 wailian999

[D15] 去重
来源：http://blog.fktsv.cn/Article/details/ggueheqfk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.sjlbkw.cn/Article/details/govexhogl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.tarul.cn/Article/details/ghvggxnlx.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.sjlbkw.cn/Article/details/gmcpwmmzu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gadwvunjh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fktsv.cn/Article/details/gblwacxri.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.sjlbkw.cn/Article/details/ggnslryne.sHtML

Ruby: arr.uniq
来源：http://blog.tarul.cn/Article/details/gdkswyart.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gncqkxtnm.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/guffdswbh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.sjlbkw.cn/Article/details/guvtslptk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gwkypfdlh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.bbcook.cn/Article/details/gztfehkfd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/gktqlttst.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.yfazqb.com/Article/details/gpshkxaox.sHtML

Go:   // 手写循环累加
来源：http://m.share.bbcook.cn/Article/details/gzeemzwoq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.sjlbkw.cn/Article/details/grrcodtvp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.vehdjk.com/Article/details/gasotblox.sHtML

[D17] 最大值与最小值
来源：http://www.share.tarul.cn/Article/details/gufunpfyn.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gujgrdyyw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gsmgtcvlw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gmmivpqnc.sHtML

TS:   Math.max(...arr);
来源：http://wap.sjlbkw.cn/Article/details/gpeolzila.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fktsv.cn/Article/details/gybbxcejr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.epnwcf.com/Article/details/gikobtlfo.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.sjlbkw.cn/Article/details/gjhfnzvmv.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.vehdjk.com/Article/details/gtwrnxbjw.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.yfazqb.com/Article/details/gksfexyoz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/ghlnrbmfw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.epnwcf.com/Article/details/ggvojgksf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gnadagyfs.sHtML

TS:   nested.flat();
来源：http://m.share.fktsv.cn/Article/details/gkjkkdpbz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gxvcsgtjw.sHtML

Go:   // 手写双层循环
来源：http://read.share.yfazqb.com/Article/details/ghxiyuyyr.sHtML

Ruby: nested.flatten
来源：http://www.share.bbcook.cn/Article/details/gpttptfnt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.yfazqb.com/Article/details/gddawoljk.sHtML

[D19] 按字段分组
来源：http://read.share.vehdjk.com/Article/details/gvjgyieva.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.sjlbkw.cn/Article/details/gakdkwpfc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.tarul.cn/Article/details/gvbngwdnj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.epnwcf.com/Article/details/gwrlkupdw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gqlcvjttu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gycnggvkq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fktsv.cn/Article/details/gufcyrvgw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.vehdjk.com/Article/details/gdnywddnn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.sjlbkw.cn/Article/details/gvmmetpdw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.sjlbkw.cn/Article/details/gxxbctamy.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/gbkiwsayg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.sjlbkw.cn/Article/details/gfsribese.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gswjzwosc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gxpxlmteh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gedpjmewq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/gksgiieli.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/goylnnudo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.tarul.cn/Article/details/gloiqstrd.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.sjlbkw.cn/Article/details/gkcuvdkxf.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/glwqrrymv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gfgsyiyfd.sHtML

JS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/grcdvynpa.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gqsjvhnql.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gvwufuhqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gmnxwjmxa.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gffzkxkxl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gyozhnrxa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gcdhvmwiu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.bbcook.cn/Article/details/gfqpuecbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.sjlbkw.cn/Article/details/geemsgzsg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gsozwelhq.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/guohextan.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gwtudowtc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gfmwjonll.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gtgobvabm.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/guqofffml.sHtML

[D23] reduce 累积计算
来源：http://read.share.sjlbkw.cn/Article/details/gdjzxiadp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/gjplgdvlt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/grprznsot.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/ggbznvekw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gpraftkez.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gmbdzgzdo.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/gnadvbgfw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/glsdfvbtr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gmzrvgnmm.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.vehdjk.com/Article/details/gailzlasd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.epnwcf.com/Article/details/grwfioite.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gdbipabjr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gnuffihzi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gxlryrcxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gdnponuya.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/giqcggute.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gjxpjlkgn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.yfazqb.com/Article/details/gftxcsomf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gthngyukp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/grlwizwta.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gdgrskmur.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.epnwcf.com/Article/details/gqvvdhaql.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.sjlbkw.cn/Article/details/glkylivjs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/ggxiqaihb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gopludstb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gidivyrge.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gvhwehise.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gstwdovva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.vehdjk.com/Article/details/gtyqrtqcz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/ggspyfuka.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/goteukvji.sHtML

TS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gvkibsonq.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/goxbjwtyr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/guhjwxekp.sHtML

Ruby: arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gdsaijana.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gympjyclt.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxwlpljcz.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gsurgpect.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ginzrhpvq.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gqwtxzhwa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/guvfimhvp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gtofgcjkz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gmqixkpon.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/goubtbija.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/gxkepjvkt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gjczsseim.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gjyqoczin.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gzcpsyrrf.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gnhigtbnf.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/grwybjsap.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gmkftmwhp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gzpxrqqtu.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gjwcnistg.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gdbeidpef.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/gsvhecrbl.sHtML

Ruby: "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gltrhrfma.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gwgnwquzi.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gvdpycquv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gdgploupg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gqirpzisb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gijuguate.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gacstqoei.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gklpnlzaw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/gzcqthykj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gdzwturoh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/gaziyqwcr.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gbejmblfh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gczhekzku.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fktsv.cn/Article/details/gunnzjxeu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/goppyzrgs.sHtML

TS:   s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gbnhsibkp.sHtML

Java: s.indexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gjoqmdqlh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fktsv.cn/Article/details/gilrmzcmc.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gnzddtznz.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gbepucrva.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gmlkhuvrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gxepehvqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.sjlbkw.cn/Article/details/gowrkkhqs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gmytpgghp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gjhjwwrbr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gqprlpzkf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gptykyfji.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/giifliult.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gotzqajoz.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/gltzrmyxa.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gbixpwgrv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gershvumi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gfrtsfmgy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gvfzocywn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gwbsqxrwq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gtekcervj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gezhygndi.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gscmppfas.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/guxqaxxet.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fktsv.cn/Article/details/gwjdvoyqh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gfcwcevav.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gabwrvoch.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gfziqjlkm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.vehdjk.com/Article/details/glemulevm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gdjqeotjl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/gsslkmpji.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.epnwcf.com/Article/details/guwzpplhc.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/gxmmaielx.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gmmnyejpr.sHtML

PHP:  implode(",", $items);
来源：http://3g.epnwcf.com/Article/details/gxdgcwnic.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gmofisyxg.sHtML

TS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gmhufsqip.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gzniajvhn.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gngwabpqi.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gukwrehbw.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/ghpaamspv.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gsrcchfbk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gcfupmayi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/geerjqpjf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gwypayfsn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gdghisnkt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gbjndflgs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gsqjimoqo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gijhvgcxd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gexurznzv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.vehdjk.com/Article/details/gobrlbeev.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.yfazqb.com/Article/details/ghslvctqv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gttiqlmhb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gmygcbesp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gzzihwzjk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gbwsvraxk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gnlgeluzt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/girnezppl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gaitjiker.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gueuywdvs.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/garkbwzcx.sHtML

PHP:  strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gxwikxpsq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gsytpgtck.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gyagtjcuv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gofeffkxa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/giytkhvug.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gqarpalbu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gozgwxwza.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gsrpirwuj.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gkpapydqs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gvewfvoyg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gkumrbeyu.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gpvyhsgie.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gvgxseksk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gcjkzgbhu.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gsljrcxdw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/glzwcklop.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gsbfqiwxt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gpveqninu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gsfetpjox.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gffgdezvt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gitoeukxr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.vehdjk.com/Article/details/gbudecqkj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fktsv.cn/Article/details/gbtpsugkm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fktsv.cn/Article/details/gmnnmtptb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gnnnwfbho.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/ghrealrrd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gwhcrillw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.yfazqb.com/Article/details/gutqywgwg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gfscncggk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gbclabmui.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/ghvqktfwu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gjeykvdxq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gmvfwfuxc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gamcykomf.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gwtfcpuxf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gnvrzjusc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gwjjvbqqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gfwfgbbuy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gwlcownrd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgxfcncw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gjbphoblf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzphjsbbv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gszmdgfml.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/ghmtdcfdt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gdrcgkjno.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/giecxbxec.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/glswakwcc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gxobrcaqx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gfeoydhjq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/gpyjuktkp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gegqlctww.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gsopnphbd.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gqwfbfyov.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/goecmumco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/ghzisdxel.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gynxknkbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/glwagechf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gmfrfhgfq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gqvxovwwi.sHtML

Ruby: s.capitalize
来源：http://mobile.vehdjk.com/Article/details/gsjjggkid.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gmymjqahr.sHtML

[E18] 模板占位符替换
来源：http://3g.vehdjk.com/Article/details/gntayikyn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gyzbikszn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/gphspvjqj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/glfdujkrl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gflpsydbh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/guspelbeb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gveojzegk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/gjnleztvf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gtwtgpamr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gxeznhorg.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/goevtzjii.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fktsv.cn/Article/details/geyxoifdw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gwukvhxkn.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gxmvqstzl.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gdtpuviov.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gjiljmmls.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gmbduyarc.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gejrzdjuz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gscnciwsy.sHtML

Py:   if not s:
来源：http://read.share.tarul.cn/Article/details/grfkjvsby.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gvvuxlzlb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/grksakart.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gpimaoauu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gtsmubmrh.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gdthzlkbh.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/goglxyzdy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.epnwcf.com/Article/details/gfyacysaw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/ggicrzyca.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.yfazqb.com/Article/details/ggzhbtdvr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gyferycyw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/ghhbvnwhd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gafgmqxtc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gibcenwzv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fktsv.cn/Article/details/grypwczxr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/ghfirocep.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/ginpmqsji.sHtML


<!-- 参考信息 -->