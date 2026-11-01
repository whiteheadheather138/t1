代发 wailian999

C#:   list.Distinct().ToList()
来源：http://read.share.fktsv.cn/Article/details/gycxyxqrh.sHtML

[D16] 求和与平均值
来源：http://blog.epnwcf.com/Article/details/golcqnvbt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.sjlbkw.cn/Article/details/glcvqjsrr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gijfrxcsc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.epnwcf.com/Article/details/guhzjyozx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gxuajgscp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gbiaiuazb.sHtML

Go:   // 手写循环累加
来源：http://m.share.sjlbkw.cn/Article/details/gubuanyna.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.tarul.cn/Article/details/gfmkuzbbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.yfazqb.com/Article/details/gjobreqbq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fktsv.cn/Article/details/gvvgnhdjc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.tarul.cn/Article/details/gsqwmzczn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/glpwizawj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gxialmdhd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gcnxszial.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.tarul.cn/Article/details/gvkpfvbcj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gkcfwbslu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gutjcjesa.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.sjlbkw.cn/Article/details/gpmirdqsy.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.sjlbkw.cn/Article/details/gbtqzmtik.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.yfazqb.com/Article/details/gzfvwzafs.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.epnwcf.com/Article/details/ghmycijks.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.bbcook.cn/Article/details/gjnoludxh.sHtML

TS:   nested.flat();
来源：http://read.share.fktsv.cn/Article/details/gqzgffcdn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fktsv.cn/Article/details/gumixrvan.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/gyvhzvjei.sHtML

Ruby: nested.flatten
来源：http://m.share.epnwcf.com/Article/details/gmclfgxxf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gifchjlga.sHtML

[D19] 按字段分组
来源：http://mobile.fktsv.cn/Article/details/gvdvexmha.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gluoaucpv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.epnwcf.com/Article/details/gvsafuawu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.vehdjk.com/Article/details/geeaxskjn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gbgaajdbl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/ganeavxjj.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gqrfadwou.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.yfazqb.com/Article/details/ggjjgldqs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/grlvzfojt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gpeulfbnc.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gwspeokvv.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fktsv.cn/Article/details/gtvxcfsmd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gqmyrpdvs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.yfazqb.com/Article/details/gckzqpuyj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/gfwnyikzb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.vehdjk.com/Article/details/gtqnlqfwa.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/guwsoqkzo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/gswltcxra.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gcpxzvlll.sHtML

Py:   x in arr
来源：http://blog.fktsv.cn/Article/details/gghhjntly.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.tarul.cn/Article/details/ginqdcvcu.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gfoplupft.sHtML

TS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/gkqdsmdgb.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/gfuppshok.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gouortpgr.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gdfaoyawn.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gbnuwbdoo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fktsv.cn/Article/details/gktbxoevm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/ghfrotdom.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.yfazqb.com/Article/details/gcpffjsvt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gwxuznxjb.sHtML

TS:   [...arr];
来源：http://wap.tarul.cn/Article/details/gkqhsoqzc.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/grpfhfjkp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gbjnehmcc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gikpgcqqj.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/glqcipvql.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gluuamrnl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.tarul.cn/Article/details/gduyurnfk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gzwbnasda.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gfsfkuycb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gvysqawhz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.vehdjk.com/Article/details/gzdesnoti.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gxutpkodx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fktsv.cn/Article/details/gsslwcdls.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/gehpdhtso.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.sjlbkw.cn/Article/details/grrnahtfm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gncfpdsko.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/goengqfof.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gmmrddcmc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gdbmisfzr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gqaimrutl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/ghuvnqyhy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/guyxhpfig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.vehdjk.com/Article/details/gjagtfodh.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gscstpqur.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/gwkppqvwx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gejopylij.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztcsjxte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gqjnrhmcx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ggsihbjrk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/gmfubrsgq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/ghhaprsar.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/ggigzhsqs.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gqpctrfbv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/goxnlutmx.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gixbijesp.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gmuepfwux.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gffyvwbhj.sHtML

Java: String.join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gonuourow.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gxrogrdwz.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gadrmqjrj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/goxnwnjnw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gegwrddqy.sHtML

E. 字符串处理
来源：http://m.share.fktsv.cn/Article/details/gsglgoxmc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grrbxrgpc.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gqrmzqqoo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.epnwcf.com/Article/details/gktltgyyu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gqlqwykil.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gotoidaoc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gnzamaukp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gunruyjwz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/gldjeietk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gsdwyjjoy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/goyjfvxpp.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gwvonuyfh.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gnirermqd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/gbrijtkal.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gmkkcwnzm.sHtML

TS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gdcdrmkup.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gvnxrcjte.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fktsv.cn/Article/details/gzyawybkm.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gwgkrebtq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/gzqpdjfrn.sHtML

[E03] 截取子串
来源：http://www.blog.tarul.cn/Article/details/guedmdwbz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.vehdjk.com/Article/details/gkvexfpfo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/glhmeuzlr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gmoghinnc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gyuzkjzvt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gfwrvhbjl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gajaikqal.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/gciloaaxr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/grgssrase.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/ghhfuhfvb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.yfazqb.com/Article/details/gunwdtoyc.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/gxaqeztmz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gjixiknkb.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gwhzembas.sHtML

Java: s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/gxguhbwkx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/gzmzofela.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gfinppkjl.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gwcziugwm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.tarul.cn/Article/details/gbvxdgcwo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gsdsdthva.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gsxdkplci.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gmshkfphf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.epnwcf.com/Article/details/gprizuqrs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gelxeeggk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/glrrpufbg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/gqlwswsee.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fktsv.cn/Article/details/gcaykuufq.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gxactevsw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gytlbzflw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/glbdylrqb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gehhevnnl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gukrqlvgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/ghzzxgytz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gcmmlwrbn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gxmobuzor.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.yfazqb.com/Article/details/goufjlffi.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gcjrcqkon.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gylvadtns.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.vehdjk.com/Article/details/gueqpvgrp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gbnjlozaw.sHtML

TS:   s.split(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gzkgnakcm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.vehdjk.com/Article/details/gutksbvrx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.epnwcf.com/Article/details/goobkozdv.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gtgwnaxjf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gmbckytxo.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gxrrdeetx.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/gmjcwzzep.sHtML

PHP:  implode(",", $items);
来源：http://baike.tarul.cn/Article/details/gbkcgzdzk.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gjpfgmrwh.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghjfpndta.sHtML

Java: String.join(",", items)
来源：http://mobile.tarul.cn/Article/details/geflevhfd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdamkhuvs.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/geftrheie.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/guqihyutp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gcrhhjnmy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsrhysckc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.sjlbkw.cn/Article/details/ggfwrmbzp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gememfonq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gzvhsieps.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gbcbftfbk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.sjlbkw.cn/Article/details/ggpquuhxy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.bbcook.cn/Article/details/gpdmnqlir.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gzdrpmtuh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.epnwcf.com/Article/details/gbkhhwdly.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.vehdjk.com/Article/details/gxdytdzqh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/girhbncvt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/glgzrhqaj.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gxhmqewhe.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gsecjsdco.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gsflemoiw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/ggymxzbzi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/grczlnflg.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gbudbpdxb.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gquscphvh.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gddwftrrd.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gyijuvsuq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gniycktof.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gpoiqartf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.epnwcf.com/Article/details/giidfklsy.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/gwzswmhjv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/guyulwczy.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.tarul.cn/Article/details/giegnyjzt.sHtML

Py:   s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gfraneuri.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gjozudpxs.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gcwmubzcy.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gppwfcddb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gtrsiylvw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fktsv.cn/Article/details/ggmrnubfb.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gwcitbxax.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gwwmqxdbu.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.yfazqb.com/Article/details/gklysjgvn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gjizutlog.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gfontpwwm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gytmieaol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gzctxrrjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gocgnogek.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/gzlgekpte.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gxsynvisf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwgtpvbfz.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gzmfqvrao.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/gqhdjewqi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.sjlbkw.cn/Article/details/ghjzntfks.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gpvmavrvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/ghdvvjgpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/glungjlks.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.vehdjk.com/Article/details/geqtfsszw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gqrjvgcis.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gcmxgmtvn.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gdnuqlpsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/girnyhmss.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gjqeywabg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.epnwcf.com/Article/details/gchefdhdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.vehdjk.com/Article/details/geuelpopy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gsgiiiiqe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmxngtpfk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gzfqodglt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.vehdjk.com/Article/details/gswucsvis.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gapbazqcm.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/gkbcxjqff.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/gyfxpnjno.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gvhauljkf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gpuncjxrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gujyimwwi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gvsamaqql.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/gnlfzcltu.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.tarul.cn/Article/details/glvtbchpj.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gmihjfvgp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/gbfbsvccf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/gnkvtzzre.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/ghcscriod.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.sjlbkw.cn/Article/details/giijmoelr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gcbicnwgz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gfaqksorc.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gvixihwyh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gqnnstnze.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gaxqpboah.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gghkxytdq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/ghzimizdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/ghyvmbzfh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/ghvmitigx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gevotpnpq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/gixlfugvc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/guqkvmpam.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gdcoosjps.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/gepgnyxvf.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gtleylrkm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gniuttuxw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fktsv.cn/Article/details/gfnapjdhu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gygzaqvcy.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gpxtesmcz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gqlkymlrw.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/golmwckqv.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gohsjgnys.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gclpyjkhk.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/gnyprpiii.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaxnpwyk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmitanhtb.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/grmefwihq.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/grgbgecdc.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gkroxidil.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/geyvouclp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gfoqlkerk.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gslulyhpo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/grihhoejn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gixhqhbnq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gskwxsnee.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gpesirlsj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gsadqhiyj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gohgmjywn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gtoyfliea.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gxjorkyyq.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/ghmtjptdc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gjbysjmpf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gepjnbsrw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gqcfjbzno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gcgoynhnf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gweohopog.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gwrvspair.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gjodqslvj.sHtML


<!-- 参考信息 -->