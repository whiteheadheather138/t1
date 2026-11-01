代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/ganlhenrk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.yfazqb.com/Article/details/grsmseypm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gttheryif.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/gamucjykb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gzcvkzkfp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.bbcook.cn/Article/details/gpdidtywn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.epnwcf.com/Article/details/gevwyumij.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.yfazqb.com/Article/details/gtczqztkm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/gcjvtevgr.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.yfazqb.com/Article/details/goreiglbq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.epnwcf.com/Article/details/ggrqnpxht.sHtML

TS:   nested.flat();
来源：http://www.m.share.bbcook.cn/Article/details/gfqdwajuw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gtcmflsvq.sHtML

Go:   // 手写双层循环
来源：http://baike.vehdjk.com/Article/details/gkreyeyhu.sHtML

Ruby: nested.flatten
来源：http://mobile.epnwcf.com/Article/details/glfrjtsak.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.yfazqb.com/Article/details/gfeqtsret.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/gwyfrhhys.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/graywxnve.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.vehdjk.com/Article/details/gtxrmmjel.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.yfazqb.com/Article/details/gxuomzzit.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gvgabbuse.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.sjlbkw.cn/Article/details/gncoiewog.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gegrlsovh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gwrqkqdaz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gziwjtqat.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.epnwcf.com/Article/details/gfhrfgxpc.sHtML

Py:   Counter(arr)
来源：http://3g.epnwcf.com/Article/details/gemerjpve.sHtML

PHP:  array_count_values($arr);
来源：http://wap.sjlbkw.cn/Article/details/gqrwxfwlx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gaknkqzvo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gkzjwqrnn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/gcsltlsuw.sHtML

Go:   // 手写 map[T]int
来源：http://wap.tarul.cn/Article/details/guzaxqqjx.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/ghrgpraoa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fktsv.cn/Article/details/gnhiuxkhs.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/ggpbkiope.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gknojgpco.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/grrmkpcbx.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gxlsuyaql.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gxjhlabja.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/giysjsano.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/ggclhdlsb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gzogfsiaf.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gopajsrnr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gxwqbzvjb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gcaamfdzp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gphdshous.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/ggtismptv.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gbjbhyypg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/grmdcmvfw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.tarul.cn/Article/details/gpjfwldbk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gatzbykqx.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gcqxmrmvc.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/geuxmibkb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gaggtavrg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gibutyvmu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gswcdchdu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/glcqdysuy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gwyzlbmci.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/grfcvavif.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/gppgekrgr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gjonwpmgm.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gkafzaexk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gzqoxcsma.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.bbcook.cn/Article/details/giwcckgub.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/ghntzazmd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.tarul.cn/Article/details/gkqdisxvr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gpinpxchn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gdyhfwhsc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/gksdxtlje.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gjvydtbut.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gajeennim.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gnyglveut.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gecmezheg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.tarul.cn/Article/details/gwsunoosh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gqmioxvzy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gtrgxhblt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gmarhkszi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/ghailxdzd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gywbbahbe.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gzbaxctdc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gaimmclqt.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/grdjbnwin.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gicdehgmt.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gxfmqtjiq.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/ggdaiklgr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.bbcook.cn/Article/details/gngpjopdm.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gmozcadlm.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gdvkplqlp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqewuxpiw.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/gqsqpttbo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gshvwssto.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/galajcaae.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/gnuftwgjd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gtbocvxyy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/gpigagmts.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gizmgmwsq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/giycntgcx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.vehdjk.com/Article/details/grjlmtvwb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gbeupemur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/geedbkhbi.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gsrdlbdsu.sHtML

Py:   "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gmnkwofuh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gmsuragpl.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gxdfwkvjo.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gnwselmsv.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gkbbsijho.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/ghxqeqwrd.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gilnvwuyo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gknhcxzbk.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gtorivfbm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.yfazqb.com/Article/details/gxvpnvtfl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gzdwigztk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gkytcehsj.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gzpdwyrdn.sHtML

Java: s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gwlgotjeu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/gpdpkuwxs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gblbtyxnp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gtjpgolax.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gyjiclapf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gfqtkbokq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.tarul.cn/Article/details/gyskeaekh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fktsv.cn/Article/details/gqyoxmuet.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gcqufclaa.sHtML

Java: s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gclximmzq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/gplisdzqe.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/gadlzexbc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fktsv.cn/Article/details/ghqburmbn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gsbbnsmsm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gxvjcdcjg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gyyofsdvs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gfsnnbivf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gnycwatlb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gdqcvzxng.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.tarul.cn/Article/details/gxmjhreuv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.vehdjk.com/Article/details/gknsuzmut.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.bbcook.cn/Article/details/grfphanuu.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gngbgrhqg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/gthslhwpb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gxzhriptq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gdzlcuxkv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gmdnsgzhy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gmngysbut.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fktsv.cn/Article/details/gcywfnwyj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gydidfuqt.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gawwwzufq.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/gcropitza.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/gquufpkle.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gevkmklud.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gdojdvbem.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gjrxwykaf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.epnwcf.com/Article/details/gsjhxvgqr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.epnwcf.com/Article/details/gkcbczvhh.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gligwmjbo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.epnwcf.com/Article/details/gptvmehqm.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/ghbimpklp.sHtML

Py:   ",".join(items)
来源：http://www.blog.sjlbkw.cn/Article/details/gupubuumk.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggllxmjjt.sHtML

JS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gpdayvzna.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gzvzbbqij.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/gkrdpyaih.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gfbimrydw.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gtpewwuwy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gbgbgsjdp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.epnwcf.com/Article/details/gbyxnmvhu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.yfazqb.com/Article/details/gyhzjisde.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gxzyqbdvu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gfeqequdg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gbtrhbzhk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/gudxxgvrq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.vehdjk.com/Article/details/gneihdqeo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gwcbnmpte.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gzeoshxgj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gaqfacacj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gmbahdaki.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gvapgucad.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gcnignzew.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/ggnbgwdeg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gphgwxvyq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gjkhfdiyq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gfbyghiec.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzggwluj.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/guwyrkpto.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gbotkibji.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gwqyrfzdl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gcqrxjuhk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/grofqrdez.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gffldkjlc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gwwbxrgqi.sHtML

Ruby: s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gpjzuejae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gijnxxiip.sHtML

[E12] 统计某字符出现次数
来源：http://blog.tarul.cn/Article/details/gkoyjqncc.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gqxyegzuq.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fktsv.cn/Article/details/gwefnnfxf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gbsalywaa.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gtuzlkfwo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fktsv.cn/Article/details/ggxdixfhe.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.yfazqb.com/Article/details/gwwuiitbl.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/guaxhfiaf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gdhzcwvxz.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gdusoyaiw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gfzsisffj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/gooivfxgp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gvenehwvj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gisrzfuzv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/glxdriegt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gyvjagikm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/gauaaeckn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gfhwikjvs.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gyjwnjybn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.sjlbkw.cn/Article/details/gjxltjprv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gejnodles.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fktsv.cn/Article/details/gnpzntpym.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.yfazqb.com/Article/details/gywdboxkz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/guekrrvpp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.bbcook.cn/Article/details/grsvcrwze.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gwvgojjrc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitepywcs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gqlotctky.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.bbcook.cn/Article/details/gwxoemecl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gjjruphrz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gxiwktass.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.tarul.cn/Article/details/gfcguublk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gkfscvowt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.bbcook.cn/Article/details/glahwwkrp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gwimzfwvl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fktsv.cn/Article/details/gdroaaqsl.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gdxfudouf.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.tarul.cn/Article/details/gennfofvl.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjcixelw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gjdktnzdo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gdtapygbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/gmecuqdww.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gdqitrjyb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gygcsedei.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.bbcook.cn/Article/details/gdneweyme.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gipqlizeu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/gxrqmioex.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/grrydnset.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.yfazqb.com/Article/details/gqjexetow.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gatdnurvh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gmguvlkuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gpwrbxdxj.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/ghwaeclux.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.epnwcf.com/Article/details/gqvlwrklb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gmddhmbhu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/ggdieqmia.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.epnwcf.com/Article/details/gcssbtxmk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gswdodkbu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gxlpgsdar.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.tarul.cn/Article/details/gbwwkjmwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/geipuvejs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gwuuhrkyd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gtpbqwryt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gzszruevh.sHtML

Py:   s.splitlines()
来源：http://read.share.yfazqb.com/Article/details/gnvpqhyhq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gusflgsum.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.sjlbkw.cn/Article/details/gcnctmjbc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.bbcook.cn/Article/details/gkfghfzuv.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/galmnbgjb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.vehdjk.com/Article/details/gbmvccnne.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/gbwqzguqy.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gxbpjlnbl.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/geijdqhlb.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/gyffvfiad.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gphfkmiwl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gusgacmzg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzvcrtxww.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gyiopkbnw.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gzkvupnzq.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/gjoeoolza.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gaclcymnv.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gcsqubskb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gdbdzyhrc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gzwrefful.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/giiyeyrhs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gobewhzac.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ggxxwjnvo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gocwsaqac.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gxyyiykhh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gbyfnxdwp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gzidqxsgi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gtrvfbuyj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gjtcmtrzd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/goroiwfla.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/grsrrkjsv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gefykjhaq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.tarul.cn/Article/details/gavqwuucc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.yfazqb.com/Article/details/gypjaanjw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.tarul.cn/Article/details/gviaxkroo.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gjljgwkbt.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gyrjqbayo.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glokuceqf.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gzannczvw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gkqugoejb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqvtblrny.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gcmlgmbch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzweymszb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/githljmmq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gswzuolmi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gfegnaljb.sHtML


<!-- 参考信息 -->