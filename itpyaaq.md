代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.blog.fktsv.cn/Article/details/gaiqrmhnq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.bbcook.cn/Article/details/grtibgejc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fktsv.cn/Article/details/gsmglsezc.sHtML

Ruby: arr.uniq
来源：http://blog.yfazqb.com/Article/details/gqpugxhqm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.epnwcf.com/Article/details/goieodzsj.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/guepmyrtf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.yfazqb.com/Article/details/gmmiuybdw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.yfazqb.com/Article/details/gvrimqjug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gjeasyzsr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gtfhohsyt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gphmhutpr.sHtML

Go:   // 手写循环累加
来源：http://baike.vehdjk.com/Article/details/gvhudwzrc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/gkadrsscf.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.vehdjk.com/Article/details/ghhtxeszl.sHtML

[D17] 最大值与最小值
来源：http://3g.epnwcf.com/Article/details/gnszdwhzp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.tarul.cn/Article/details/gccsjmlfh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.bbcook.cn/Article/details/gahgiglqh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.vehdjk.com/Article/details/ggxwjbnqp.sHtML

TS:   Math.max(...arr);
来源：http://blog.tarul.cn/Article/details/gykekkkun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.epnwcf.com/Article/details/gnfkgxkzz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.tarul.cn/Article/details/gcvhstapx.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.bbcook.cn/Article/details/gvgdaleir.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gupwlfsbp.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.yfazqb.com/Article/details/gutqycjcz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gdrsbaxxn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.epnwcf.com/Article/details/gibmjedlz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/gouaadxsl.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/glbbokdgt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.sjlbkw.cn/Article/details/gtlzbhhwj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.epnwcf.com/Article/details/gtaqiqowd.sHtML

Ruby: nested.flatten
来源：http://www.blog.yfazqb.com/Article/details/gcgoxfygh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/gxgwwzazf.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/grfpglhyt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.epnwcf.com/Article/details/gpfuuudjj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/ghezsptzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fktsv.cn/Article/details/grqnwmhst.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gnvtcxayq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gaqxvmqec.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fktsv.cn/Article/details/gzmiusmdj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gojhlvpqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gowrlvvec.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gaolcbvum.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/grjdfnzym.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/gpuicbiuu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.epnwcf.com/Article/details/gwjkwzqcv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gmypqplvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gzuhmtpsi.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/gikamfmhd.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/gzbqjasjy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/gjqonyomb.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gmsarhtkb.sHtML

Py:   x in arr
来源：http://mobile.yfazqb.com/Article/details/gudsmenwe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.epnwcf.com/Article/details/giiunomoy.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gnjshdgjs.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gqfqxfxfe.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gqwgghbwe.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.tarul.cn/Article/details/gbyhwqwwx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.sjlbkw.cn/Article/details/gaptexgjt.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gxdfpybjr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.yfazqb.com/Article/details/gemffiqvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/galizsyfe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.vehdjk.com/Article/details/gpygtpfjh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gsswmfvmu.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gncptwgvu.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gbnkapuja.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.bbcook.cn/Article/details/gpepdcfjl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.bbcook.cn/Article/details/gsrcbtxwt.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gurzzlkzu.sHtML

[D23] reduce 累积计算
来源：http://wap.fktsv.cn/Article/details/gamttyruj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/gklqwlerj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.tarul.cn/Article/details/gwfxsexbj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjjythvn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gubcsfyuo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/ghonojkns.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gnidderip.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gxmunfsqf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gychnizrv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gnqkwupiy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gsatokxrd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fktsv.cn/Article/details/gejecjdle.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gdfevctew.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/guucbrecx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/ghjnaqbrn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/grzsgolgx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.vehdjk.com/Article/details/gevnazwkw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.sjlbkw.cn/Article/details/gdzhcmrta.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.tarul.cn/Article/details/gaxgndqkk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.bbcook.cn/Article/details/gvojlxhrk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.yfazqb.com/Article/details/gypmmntnk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gkfnqeyvg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/ghzwvuyfr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.tarul.cn/Article/details/ggovdlqei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/gnkqnfxrv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gailobuuz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gyfbhvjlr.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/ggxdzlaju.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/ggzwnpiub.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/garcbqmll.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/ghqrouscz.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gwcahwxcs.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gesrqddgt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.vehdjk.com/Article/details/gtalsvmfy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gglmyiand.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gfjsieaon.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdndtddfe.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/gekyrckgk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjegbgeqb.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gdqmsnwvl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.epnwcf.com/Article/details/gjngmhpds.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gipzitmnk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/geezexaos.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gyeizumyo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/ggmrupxmf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gtjaymmvq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gmhirwqak.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gyuaizhio.sHtML

[E02] 重复字符串
来源：http://3g.bbcook.cn/Article/details/glfcjecyh.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gdnzsebeu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/goawrbdml.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gzxqgphhg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/grkclqgch.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gxvqmcqab.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.tarul.cn/Article/details/gkskcwomc.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gypireuqg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/ganazjrqa.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gfykrlnmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gmddkkewy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/ggybicere.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gxsdvxoll.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gyfnahhve.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/ghtslejfb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgrjdwnd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gtgozsias.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gtcfurgak.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/gefveirlq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gmppvambi.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fktsv.cn/Article/details/goocnlvmw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gcwngwjeg.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gkadyjqmo.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gjnvvrqpp.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gtvcbvplm.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gjogapqyn.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/gkgzgvnoz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gmqifkzua.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gyymirhun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gntxwbcdt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ggsoomctn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gvbtdayge.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gxwoumkxm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/ghkvrapsg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.vehdjk.com/Article/details/gfovpxnkt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gdqfuxryu.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gricvofvc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gtuzykfoa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gqvrybfjy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gyuoqtbsm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gzozpeyxt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gknxtugwr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gbirxbxip.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gewgmkarq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.tarul.cn/Article/details/gtudhbury.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gkdzcmiog.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/gexfranop.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.bbcook.cn/Article/details/gwwnnazwk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gqyanjuuq.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gbufyryeh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/gwjvrijjz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gdtwbeolw.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gssackaeo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.vehdjk.com/Article/details/geczekrjh.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.yfazqb.com/Article/details/giwlxssbj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/gnbfpoowo.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gntbpkqcg.sHtML

JS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gwfdgqxqz.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gsicoscfc.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gdtdfglva.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.tarul.cn/Article/details/gtilhhuzr.sHtML

Ruby: items.join(",")
来源：http://baike.yfazqb.com/Article/details/gfcpplfpl.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gczngwlwp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gqoalculy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gsytjqtwf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjfqvivmm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gqtxzvokc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gzjttillc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gbemdbamt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gdybjisdn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/ghuexmjdh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gugwhqnfd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gachiwnwl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gtvikbiej.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fktsv.cn/Article/details/gowzlkueo.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gaellvzhg.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gqhsmhfma.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gshddrdhb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gseddxmzq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gdmfciwug.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gtcyxsljc.sHtML

[E11] 反转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gayoemijy.sHtML

Py:   s[::-1]
来源：http://www.share.tarul.cn/Article/details/glvshrfmn.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gnupsndjn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/ghzpvvvmi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gmiamhpfm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkigyjqcu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.epnwcf.com/Article/details/gmfwpwzis.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gsoxltfop.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gtrgbyxca.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gfkihxtiz.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gavgyqsdu.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gektacaxf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.tarul.cn/Article/details/gukqbpufr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/ggooltwhg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.bbcook.cn/Article/details/gqkoisylo.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.tarul.cn/Article/details/gjlwrgmbj.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gvqmdhuuy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.yfazqb.com/Article/details/gsobfzdud.sHtML

[E13] 逐字符遍历
来源：http://mobile.epnwcf.com/Article/details/glfzmywyk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/gixoebwfe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gtovqghud.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gfoxhgahh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/giljilndk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gtcknftrx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gbtnahvon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gxnaxgbye.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gaparynrh.sHtML

[E14] URL 编码与 Base64
来源：http://3g.tarul.cn/Article/details/gvgflvlkp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gpdinwvcr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gwmtprylo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.vehdjk.com/Article/details/gtmukogiv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.yfazqb.com/Article/details/gudyrkjzo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gitigrpnx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gljxwggny.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gbchddvaf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gpioxqjut.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/gwsiezuww.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glmxicvvc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.yfazqb.com/Article/details/gjpostaky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gwvwclvgk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/genefiqhl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gwkxfrrap.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gnultzrqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.yfazqb.com/Article/details/grsdizctr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gcmdcxgri.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gvubqiser.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.tarul.cn/Article/details/gfkxzqpby.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/gbyzegvcb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gcyiwrxoc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gcneobgmj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.epnwcf.com/Article/details/gayvaojcb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.vehdjk.com/Article/details/guyzqacyj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/gpwsdugsx.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/glwscetnz.sHtML

[E17] 首字母大写
来源：http://www.blog.vehdjk.com/Article/details/gwrphtodg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.tarul.cn/Article/details/gfmzydiuf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gtzmalqur.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gpashgnxq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gqytmzdis.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/ggfberkwq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.vehdjk.com/Article/details/gmzyixedx.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gpwzrruot.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fktsv.cn/Article/details/ggxhnixio.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.vehdjk.com/Article/details/gxcpxrxqg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gvtiprdgg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gepvifzxq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gdobfiuxg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gbvuekzbz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gferjznxi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gejycmcqo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.sjlbkw.cn/Article/details/gflolojgi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.tarul.cn/Article/details/guhanypnd.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.yfazqb.com/Article/details/gjlblvdrm.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gewzoquwt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/ggzumohze.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gwgteqwlb.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gacbzfurg.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/gpsngadfj.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/glayvemci.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gagetqlav.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/grgdiuuve.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/ggntpsfls.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gjukjmruj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.sjlbkw.cn/Article/details/gwcoqkvtm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fktsv.cn/Article/details/gbikstxcy.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gsyppnekb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gmxdpaasv.sHtML

Go:   if s == "" {}
来源：http://www.blog.yfazqb.com/Article/details/gwhblyrlv.sHtML

Ruby: if s.empty?
来源：http://baike.tarul.cn/Article/details/gwmncxgxg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdcrhobpv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gbkewwbfq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.yfazqb.com/Article/details/gfjuipijs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gbdztdpwc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gtfwkrprh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gmhjnavrg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/goxfplver.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gjnjyxzks.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gdnaqfnmo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ggfnvfvyh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gifzkfsxu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.sjlbkw.cn/Article/details/gvjkgvjyq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gqcnqlqjy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gmudcevij.sHtML


<!-- 参考信息 -->