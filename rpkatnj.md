代发 wailian999

C#:   list.Distinct().ToList()
来源：http://wap.vehdjk.com/Article/details/gwjkcbryg.sHtML

[D16] 求和与平均值
来源：http://read.share.vehdjk.com/Article/details/gkudsckwa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gtrzuwaiq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fktsv.cn/Article/details/gljsddaad.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gsggbznxs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gzheflrkj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.bbcook.cn/Article/details/gnvpsvsyy.sHtML

Go:   // 手写循环累加
来源：http://mobile.epnwcf.com/Article/details/gojfzpdog.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.yfazqb.com/Article/details/gbzosgvmu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gtuwsovsm.sHtML

[D17] 最大值与最小值
来源：http://wap.fktsv.cn/Article/details/gwdyukqlb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gpjduayol.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.yfazqb.com/Article/details/gfpqqxokc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gdcvaalon.sHtML

TS:   Math.max(...arr);
来源：http://m.share.bbcook.cn/Article/details/gfssppabi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.vehdjk.com/Article/details/gumcihboc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkvfephrs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.epnwcf.com/Article/details/gbzjywasi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.epnwcf.com/Article/details/gzrbpsuag.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.vehdjk.com/Article/details/gyhnjlfjg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fktsv.cn/Article/details/gjisvfdpe.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.vehdjk.com/Article/details/gwzjglitj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/goxuforbs.sHtML

TS:   nested.flat();
来源：http://www.share.vehdjk.com/Article/details/gqkizouwi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gjgmugtkt.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gjbrefazz.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gpmljkcte.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gkfycmdat.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gazpxlpsa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gxnwenukd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gmndqkeij.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.yfazqb.com/Article/details/grbaxuhni.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gloeauywr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fktsv.cn/Article/details/gdeodcmiy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.tarul.cn/Article/details/guuybqupl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/giemjlekf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.tarul.cn/Article/details/goklmebhk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gazdoqtjt.sHtML

Py:   Counter(arr)
来源：http://blog.tarul.cn/Article/details/gkyzsloua.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gqjncosjp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.vehdjk.com/Article/details/gydcfigpe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gqqacqbek.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gacpruqkk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gugxeynpo.sHtML

Ruby: arr.tally
来源：http://www.blog.yfazqb.com/Article/details/gbeylfkmr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.vehdjk.com/Article/details/gjtyqxava.sHtML

[D21] 判断是否包含某元素
来源：http://wap.vehdjk.com/Article/details/grumuiqsj.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gwmoxldfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/guynqtzwk.sHtML

JS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gywhxjhew.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/galuwzkbf.sHtML

Java: list.contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gkufbljbi.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gugwxvqhn.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gslbibkwp.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/ganjfkzlm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gemvwxryo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gfwzlbdmh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/giwhuakab.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gtxpnsxnp.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gjckyaabu.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gfrcjupiy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gwqqrwdms.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gvsmyoibs.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gyyrnfhin.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/gfambcfcx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/guhldqexk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.bbcook.cn/Article/details/gvmahqcjf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/goelasgzc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/ghdnlfdmr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gidhyymvt.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gcyuvvdfc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.tarul.cn/Article/details/gdeuksrye.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/gisdwbiqf.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gilxbekdi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gbcszkljf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/goeayjtyx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/gohvpotmo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.bbcook.cn/Article/details/gdcurtmof.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gerihztpr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/guezwlhkw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gdhnxyazr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.yfazqb.com/Article/details/gerwmmhnn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gbwpriwlz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.sjlbkw.cn/Article/details/gjdfdjgmc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gfcbeuxph.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gxsdqwebn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gjzmmutzy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/gpywmzzom.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/gvgjtzilz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fktsv.cn/Article/details/gcvhwurgp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.bbcook.cn/Article/details/gpvkgjpvx.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gfinqfxit.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gimxamuxu.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.tarul.cn/Article/details/gnkphxwit.sHtML

JS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gikkmayqj.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/guhzxughg.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/googvcahx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fktsv.cn/Article/details/gsnonknva.sHtML

Ruby: arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gpuxcikdd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gitxyhzrb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghslpalaq.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/ghkhbykuh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmzihutra.sHtML

[E01] 拼接字符串
来源：http://3g.tarul.cn/Article/details/gknsxpbhi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/guifvhivj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/grnuciopp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/grnofjeya.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/gmrxslqrc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gyxwaztlv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gdvgdmdbg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.bbcook.cn/Article/details/ggcyjxbil.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gplcxcvlv.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gskkzuosr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/genocwcvl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/ghhcabktc.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gbpjomyoi.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gxxtunnjz.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gabrrshti.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gipmvvynz.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gvndcbiel.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gfrfydufd.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gbxqiambj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gknmhuxyh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gcidgeaao.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gecuayhzb.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/ghnvudqcd.sHtML

Java: s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/grtpcfwsp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gneoaiuqn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.sjlbkw.cn/Article/details/gxuuiywlh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gtusamkaz.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gkdxjqwza.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/ggvstrwlf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/gdbuzifmj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.epnwcf.com/Article/details/gzaxgplfq.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gefnerxnp.sHtML

Java: s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gjumrbbbr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.vehdjk.com/Article/details/gxakwqunm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gkdqmyjds.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gndingqtn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/grfrdgdyj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gddsgduru.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gipekjqhv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gdksuvlii.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.tarul.cn/Article/details/gjomoqtex.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gjkiogpyu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gtbtncgrd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/glvaadiuh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gglrvookm.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/gdtbswihj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gbmrtnjbd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/glzswosyt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/glaqvomjs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gvvopftxi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gtbcezvof.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gcimpfpcl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.tarul.cn/Article/details/gxqhieqee.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/geqzlyjrb.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gwcikqnfr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/gtukxonyq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/grswnykbr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/galdglwpv.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gmpcpzghp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/ggmksmmho.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gsrdqekzi.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/giksbnkdj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/guredlkku.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gpyztxwyo.sHtML

Py:   ",".join(items)
来源：http://www.blog.bbcook.cn/Article/details/gngyoehnn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.sjlbkw.cn/Article/details/giwvlkfks.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gtlulhwmo.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gisgrymcf.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gdfkbalmy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gmgbktmnt.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/ghfjevqgi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gfniqdhnp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gpxdipvyk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gjdnlwzwf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.epnwcf.com/Article/details/gfailkhbi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gokhiyswp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gdsavtmnp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/giiwerdvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gjdfoewwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gmojdlsoi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.epnwcf.com/Article/details/gclhoyhno.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gilfqephp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/ghmgabysg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gqjiftjce.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gqxwsjrur.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/grypbqlsj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gwlkbipcb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/ggeyckegg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gonreuvve.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gsczbvkpq.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gjjgqfijc.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gowowigxg.sHtML

PHP:  strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gjtvplcda.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/grmcsjjeo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gsecyvibq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gsdduvjyr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.vehdjk.com/Article/details/gchiavmai.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gmkcmvnfs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gvtalovcm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gmywbyjwf.sHtML

Py:   s.count("a")
来源：http://baike.tarul.cn/Article/details/geglhuemf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/glynogtvf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gqrkcyrpf.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gxgxllkgr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.epnwcf.com/Article/details/giujtftmf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gtnfexfij.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/ghjgsptcl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.sjlbkw.cn/Article/details/gkfrlqqbv.sHtML

[E13] 逐字符遍历
来源：http://mobile.yfazqb.com/Article/details/gcrqwjczn.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gouvcpjsj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/girrukjag.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fktsv.cn/Article/details/galozkzyb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gaptsbsqf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gdgxwolcu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/gyaqmdanl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.sjlbkw.cn/Article/details/gsxjlhcox.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gkuqpoqbp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gaxnnvqhs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gpiqoedlm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/geqincjwt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.tarul.cn/Article/details/gikxyhvgs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/gegfcieaj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/gukhymjwf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gtugjdkso.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/glxtfajiz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.epnwcf.com/Article/details/guresowjo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/grswtgdxw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gnsrftoav.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gjezbntbw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gtufjrgum.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gkxpivqpv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/gishntzww.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/grtxuxeik.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/giitndkkk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gpjeydcim.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gmeyddgte.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fktsv.cn/Article/details/gnpowjdhd.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gxemguima.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/ggwbpbvdj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gfwbutbcs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gppotegpr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/guyowrviy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gbjsqrvzg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.tarul.cn/Article/details/gpfqumlck.sHtML

[E17] 首字母大写
来源：http://www.share.bbcook.cn/Article/details/gieeoetua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.sjlbkw.cn/Article/details/gfnzgpmnl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gkqbmhphd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gaazoueta.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gwatrguhg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrjbrnuc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gqdzjrwla.sHtML

Ruby: s.capitalize
来源：http://www.share.epnwcf.com/Article/details/gcvdesrht.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gryitnalh.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gybnzychu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.vehdjk.com/Article/details/grmccqmme.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gommwlwli.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/geknaesod.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gtbvrfcqz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/giacqduzb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gxarvueis.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/ghurkffuz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/gwgfblkut.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.bbcook.cn/Article/details/gbplmtlqm.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/ggwxjmtqn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/grsjvvvjv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.sjlbkw.cn/Article/details/gyegidhsw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gveejjfhe.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gawuqivlk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gnyxigzne.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gdshyluiz.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gtyreudey.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/ggqyefuik.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/girmyxmyn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gqedlkkuc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gxiwgzvei.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gowleawkb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gbspnpvdd.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/grvtprzek.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gjmyypucj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.epnwcf.com/Article/details/gnfkhfvcl.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/gjqmmjmgm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fktsv.cn/Article/details/gqzpurhvb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gzlzkiwcr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gflzgvsrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gokxllexv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gwkohcvls.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gzcrrzslg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gkfzoiimu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gzbskrvvy.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/gnakpwmxy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gmqtqqyxl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/geylklgmy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gmzvvnhju.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/grpynuecm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gkztaskxy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gwqeizoji.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gonrbhlhw.sHtML


<!-- 参考信息 -->