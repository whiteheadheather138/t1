代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gmffkyilo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.vehdjk.com/Article/details/guedswdyv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.vehdjk.com/Article/details/gvwylpakn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.yfazqb.com/Article/details/ghwtbxwzy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fktsv.cn/Article/details/gpdwyqnbr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.epnwcf.com/Article/details/gzdlmcrll.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fktsv.cn/Article/details/gqtbyjbnu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.epnwcf.com/Article/details/gtpfjzcnt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.epnwcf.com/Article/details/glfwszxgf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.tarul.cn/Article/details/gyjunnrpx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.yfazqb.com/Article/details/gmjyrpkhb.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.bbcook.cn/Article/details/gxfdwvkbz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.yfazqb.com/Article/details/gwsobknhm.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gnipzsaha.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fktsv.cn/Article/details/gwpqyxrfs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.tarul.cn/Article/details/gvipdkqpv.sHtML

[D15] 去重
来源：http://mobile.fktsv.cn/Article/details/gyzuygzfg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gzhsdizuj.sHtML

PHP:  array_unique($arr);
来源：http://3g.sjlbkw.cn/Article/details/gmhdaxilo.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gpswjkive.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/ghyfvzbrp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.epnwcf.com/Article/details/gydbvpqyk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.yfazqb.com/Article/details/gkxyqrwzu.sHtML

Ruby: arr.uniq
来源：http://baike.tarul.cn/Article/details/gkcigilcu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.sjlbkw.cn/Article/details/gxnnhvuzd.sHtML

[D16] 求和与平均值
来源：http://www.blog.bbcook.cn/Article/details/gyhmeunoe.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.epnwcf.com/Article/details/gaftztzjt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fktsv.cn/Article/details/gnyyjuzub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.tarul.cn/Article/details/ggbilesrt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.tarul.cn/Article/details/gdexyedtw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.epnwcf.com/Article/details/gwhrqrpuj.sHtML

Go:   // 手写循环累加
来源：http://baike.tarul.cn/Article/details/gciyxzkrs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.vehdjk.com/Article/details/gabcdpxls.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gxuvabdma.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gjdaybeoy.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/giyaaojmm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.epnwcf.com/Article/details/gpqbxfbzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.bbcook.cn/Article/details/giohykrmv.sHtML

TS:   Math.max(...arr);
来源：http://baike.tarul.cn/Article/details/ghkxlqfcd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/gfygelvqc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.tarul.cn/Article/details/gfqlfawav.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.yfazqb.com/Article/details/gwtzlcdkw.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/gulmnzlsr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gphpaxbco.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fktsv.cn/Article/details/gpaiqyeoj.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gfygcldbj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.yfazqb.com/Article/details/gpujozyfz.sHtML

TS:   nested.flat();
来源：http://www.share.epnwcf.com/Article/details/gdbswvfey.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.bbcook.cn/Article/details/guljwzzvv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.bbcook.cn/Article/details/grsuzzctv.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gjnypfkqv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.bbcook.cn/Article/details/gtgcshnba.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/ghcixtptt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gniyyjjrj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fktsv.cn/Article/details/ggngmbttv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gyyphbhyq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gjwhljwhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gzhqmjqtr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.vehdjk.com/Article/details/gfeggreui.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/gvlfuporb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/grnuykush.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gfzuqljtj.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/ghwtzuicw.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gnnqkucjg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/guuedkogw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/gytwzxomm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fktsv.cn/Article/details/glohmiepw.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/guqrqbnob.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gqiqjojsg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gusqvzrax.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.bbcook.cn/Article/details/gethpjasq.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/gneoadytl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gtwspfnny.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnahctgy.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gjpcipbpk.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gydoplixv.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gbdgbofyl.sHtML

Ruby: arr.include?(x)
来源：http://3g.bbcook.cn/Article/details/gxbjuupsl.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gqqvrvmkz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.epnwcf.com/Article/details/gxgjeuahg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.bbcook.cn/Article/details/gyyxxrddz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gbyqxcwko.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gplfvhozv.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gkotqehnx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gmhsfuify.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gaujagzkq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gkzqujptj.sHtML

C#:   new List<int>(list);
来源：http://read.share.bbcook.cn/Article/details/gokgnuuzt.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gcgypmycb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/glusycdbf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.sjlbkw.cn/Article/details/gdpckhufi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gybrsvgjj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gfwccjgmu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/guxtnagrm.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gnrwefjnn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gvqgujmtd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.yfazqb.com/Article/details/glwxwgjwg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.tarul.cn/Article/details/gyedrjwez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gpfmqrlyt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gfbkjrqip.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.tarul.cn/Article/details/giigqddaf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gjbzyilye.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/ghyohnnxn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.vehdjk.com/Article/details/gajcpzauu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gvzqpqqzp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/guykwjglw.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gnwkapnsa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gbhelfivb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/gdmzptjzn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gyognynom.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gwajwbgib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gmjfdqqxy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/gfaatxwja.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghrhgybvh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gwdfyctaj.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/grxbjjeus.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gnilsayoe.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gogumspgr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gqlexakoa.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gwywikhgm.sHtML

Java: String.join(", ", list)
来源：http://read.share.tarul.cn/Article/details/grhzzzmvr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gdugnavwj.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/glhqcisvp.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gjfcvhwbq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gljnqlihe.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/gcclogfjv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggmvimbxt.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/geqgftibu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gmaqdtxyy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/ghibvvbty.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gjvpwhika.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gipuxeymh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gptzjpmqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gcvkdnyzt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/geclzrgnd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gxyrmhiwp.sHtML

[E02] 重复字符串
来源：http://mobile.vehdjk.com/Article/details/gjjuazpnr.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/ginzhyqce.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/ghfcvfuai.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gdhxikzil.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gpqqsmmaf.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/guyrbehbr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/gywczqycr.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/glyscvqhk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gwjbrgzwu.sHtML

[E03] 截取子串
来源：http://3g.fktsv.cn/Article/details/gyfcyhtnc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.sjlbkw.cn/Article/details/gdfkiahty.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gvghfiuak.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gxvlgpemj.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/ghwqyshwc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gtmcvknsj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gdncdzqnw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/giluvsucb.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.vehdjk.com/Article/details/gxxzhgpff.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/gqgbjntsg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.tarul.cn/Article/details/gcicxcwop.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gsrryggdq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gvbkbchkn.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gptmfebyc.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gurdodmgm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gjlztfgii.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gjbruseth.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gmddqfpnt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gnblfkbui.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gugayqssu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gyoewfocv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gamuscyhi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gemuftazl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/gphsnwsxd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.sjlbkw.cn/Article/details/gofsroujw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gznzcpyzr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gyexbfhdu.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gsghelpah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gimemnhcj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gpkaayhub.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gxajzqzor.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gyxwhafmp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gvettznnc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/guzkzkxnr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/glzxrjjnh.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gtzfinwda.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/glanhvlaa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.epnwcf.com/Article/details/gkbmrtzbp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/gbqsvdexr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gezwvtdkz.sHtML

TS:   s.split(",")
来源：http://mobile.sjlbkw.cn/Article/details/gmxkzuujl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/guyrpdyoj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gauzdfjrk.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.vehdjk.com/Article/details/gevbakhrf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gmllikzul.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.tarul.cn/Article/details/giedkiaet.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gipzrduku.sHtML

PHP:  implode(",", $items);
来源：http://3g.sjlbkw.cn/Article/details/gchcedlqh.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/grkbumbqc.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gntgrtkhm.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjvmojcql.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/grdsoeeex.sHtML

Ruby: items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gmjoetprk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gkyavewny.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gcbogjnhf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.tarul.cn/Article/details/ghkooonqz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/guxcpggho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/ggscziftc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gkpbtwxpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gxwwivxxy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/gpvekugxl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gesnbkoth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gibbisvka.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gmmyfeypk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gywuxkjzj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrwvzajc.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gxgfggwiq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gbritcyxf.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gtphstfmg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gjwbffuzi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gdcjnjrqc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gzlnxjvna.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gqmgmenps.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/giuvhnjhm.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/ghtlgflts.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gjrdcocfr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/graiofkcm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gfamrbeei.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gpqjcfale.sHtML

Ruby: s.reverse
来源：http://3g.vehdjk.com/Article/details/gftpvocki.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/glwtgknef.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gppaaixru.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gfblhkosz.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gapqcerma.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/goxtzzksp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gwgigewsj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gvrbvakwm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gqscsrdqm.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gylfavsue.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gjsnlfjcn.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gpjcckpjo.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gpiepbfrr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.vehdjk.com/Article/details/gezhwktvc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gvtphrlvj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gpkrvmzzq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.bbcook.cn/Article/details/gehcgvrfs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gsdmmubay.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gctpsmkrj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gokketefi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gwnevfxty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/ghfqygoos.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.vehdjk.com/Article/details/gcclokntv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/glxkahpjx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/guvqbyrcw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/germoefts.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gjvazchdz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/ghrbjnydp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gmafegaus.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gplflffhq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/giqrabokd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gyusjanxg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/geydtiykx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.bbcook.cn/Article/details/geafuevlv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gtbwbifgz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.vehdjk.com/Article/details/gxvtkvhli.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gnfultwps.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.tarul.cn/Article/details/gzxfaxnsv.sHtML

[E16] 数字千分位
来源：http://wap.yfazqb.com/Article/details/gesjvnyxw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.sjlbkw.cn/Article/details/gnhptvqfs.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gfkpxnnfe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/guzdtkezk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/girkkymbf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.tarul.cn/Article/details/ghogcwrkb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/gzkvcdtdy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gcmtacewi.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gyuwihxuy.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gjxdvulwx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/gdncjufvz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gbxjaklon.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gtbpmsles.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/grkgkpmqh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gnqqeymin.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.bbcook.cn/Article/details/gdkuwdhoz.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/glxadgvlb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gavofunsh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/grcnioiwm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gfwdwfkdz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gruphcaeo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/ggbyibpic.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gcaqxbzbj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gpmakbhyh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gxctodeow.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.epnwcf.com/Article/details/glrmrievs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fktsv.cn/Article/details/gcyvmqorr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/ggsrzjovl.sHtML

Py:   s.splitlines()
来源：http://www.blog.epnwcf.com/Article/details/glvxsbbqs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/gpmatlfyk.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gottsghjo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gfroxeuej.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gcqvtkuvj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gfucgmucy.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gpvdwhhvp.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gxqwpcyia.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gyghzewvf.sHtML

Py:   if not s:
来源：http://blog.tarul.cn/Article/details/gfgfolohe.sHtML


<!-- 参考信息 -->