代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.vehdjk.com/Article/details/gwktidpqk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.epnwcf.com/Article/details/gnrgesudj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.yfazqb.com/Article/details/gxyjdmbtm.sHtML

Go:   // 手写循环累加
来源：http://mobile.yfazqb.com/Article/details/gchprpicf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.tarul.cn/Article/details/gnwmrzhmx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.tarul.cn/Article/details/grnlujhjs.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/ggtyjzmnn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gwmnnuyke.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/ggcffnqxz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/gjuzmgzfe.sHtML

TS:   Math.max(...arr);
来源：http://blog.bbcook.cn/Article/details/geydzyoge.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.vehdjk.com/Article/details/gymhnplkd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.tarul.cn/Article/details/gtqdmnwna.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.tarul.cn/Article/details/gumjhmvis.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/gxduxiwyo.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gpkoigmfg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.tarul.cn/Article/details/gisbfkcar.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gjfquuatj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/gqbaufdhx.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gwscrwndn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/griiapkph.sHtML

Go:   // 手写双层循环
来源：http://wap.vehdjk.com/Article/details/gkuxdqxwo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gttncsbdf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.bbcook.cn/Article/details/gpguwebao.sHtML

[D19] 按字段分组
来源：http://www.m.share.fktsv.cn/Article/details/gjvsxejld.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.bbcook.cn/Article/details/gokjzdhel.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gbvcmonkh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/gggvpgilk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gyoxdwlyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/gyjnbjvwp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gzwnaiygu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gqlexfjnc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.epnwcf.com/Article/details/gmhcdinjr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.bbcook.cn/Article/details/goxfefgvf.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gmsubtlmo.sHtML

PHP:  array_count_values($arr);
来源：http://3g.epnwcf.com/Article/details/gxafkgnqn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gmfkgglja.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.epnwcf.com/Article/details/gqiverptn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gfirbcaip.sHtML

Go:   // 手写 map[T]int
来源：http://wap.epnwcf.com/Article/details/geedxaerf.sHtML

Ruby: arr.tally
来源：http://www.share.bbcook.cn/Article/details/gzyurbjhq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gqfnlvvkx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gkdfuqhnf.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/ggtryeqgp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjalkspbq.sHtML

JS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gruyftkbo.sHtML

TS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/glrehxkjo.sHtML

Java: list.contains(x)
来源：http://blog.sjlbkw.cn/Article/details/gosssyvps.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.epnwcf.com/Article/details/ghdickrzq.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fktsv.cn/Article/details/gpheksrub.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/ggkkprjon.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gkbawdumj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvwafolsb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gtaokfnat.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjkdvhopg.sHtML

TS:   [...arr];
来源：http://baike.bbcook.cn/Article/details/gwojvchdf.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gqtojodnv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gxothfmui.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.sjlbkw.cn/Article/details/gckosralr.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gbnfzvqhu.sHtML

[D23] reduce 累积计算
来源：http://wap.epnwcf.com/Article/details/gzuoiqsfv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.tarul.cn/Article/details/gytkmlgpo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gptmkdinc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gegteftcc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gbdmzctra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gkpsbglpc.sHtML

Go:   // 手写循环
来源：http://3g.tarul.cn/Article/details/gdsnfangb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gdfmypexq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/glojpxyqm.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gsvbgvdyf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.sjlbkw.cn/Article/details/gcwbnafta.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gvuvthuwt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/glmgtcxgh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gfzrxzqxj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/guwrjyufv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gtvwbquxq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.epnwcf.com/Article/details/gxfnnlgpa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.sjlbkw.cn/Article/details/gntkmydjd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/getelcfdq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/gnghlwbte.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/giknytszw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gexenlnjf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/gwdukshtg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/guvtbwgls.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/grzxmksra.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.yfazqb.com/Article/details/gcuvnrjdu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.tarul.cn/Article/details/gjxbwwqhf.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gjlbrdknf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gfysnvfpj.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/gwrbhdvfv.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gtktszzha.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gdbrdleju.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gnfkiqfjh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gtjcgtdaj.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gzraesxzc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gtosazmpr.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ggjxzhuke.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gwcyukvjs.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbcdgyqbq.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gvrglvgar.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.vehdjk.com/Article/details/gqazakomp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.epnwcf.com/Article/details/gbuckifhg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/gfxjuxqei.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.yfazqb.com/Article/details/gddjhjeoa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.tarul.cn/Article/details/gcuiovgeh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/grweaxhqt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fktsv.cn/Article/details/gionpqqog.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gtrijsihd.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gxudvxjki.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gchrungwh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gmsxqrwnc.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gsiquhvwy.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gjyhhalqf.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gzkcqfpms.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gcldgxgqh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gnynjquhf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gmpbhekxp.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gegjdbwgn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.tarul.cn/Article/details/gekifqtjq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gqdgidupe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gdsmxdgzi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gadiczqth.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/ggijhitjr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.vehdjk.com/Article/details/gbmsscrlr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gqkbbqtnh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gorblcjfi.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/grinhsbby.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gazgokwix.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/glyvquiwz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gxepelxby.sHtML

TS:   s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/gljvqzznm.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/guucueggk.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/gkmjohqgx.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/grsqcaoug.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gznemeejm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gsgenbtvm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.bbcook.cn/Article/details/gqwlbqwxd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/goyepgltx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gpwsnxqid.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gmoynkrbv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gxyjrrqoo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.tarul.cn/Article/details/gncjiglbd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gyylscxcd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gkygxrnfv.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gsqxoinwm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gfztygioe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/ghoobgfgz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gcpviruoe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gxzehsacc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gkeudgufd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/ggipvujnv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/geopzbrvr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/getjorfhp.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/gsyngfvba.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gcvjujeyc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/ggqjfzdiv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fktsv.cn/Article/details/gvnotgxhp.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/ghhkkpiek.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gpxitvwnn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gulgzicfo.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gkcrzvtom.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/glhvceppa.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fktsv.cn/Article/details/gxggsasgb.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gumzpyhax.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/gkxabhiay.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gwdpjmvrx.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/ghowysnbr.sHtML

Java: String.join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gyirmugrm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/ggvmozqvz.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gboxhuify.sHtML

C#:   string.Join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gjezibdvw.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gyeclkbxd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.bbcook.cn/Article/details/gipjpclui.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.epnwcf.com/Article/details/gmtjujtvu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.yfazqb.com/Article/details/guoqncmgr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/ggjxnrvep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gzvjsphhe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gsqrmsxpg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/gnrhrzuvw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gvwvzpehj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.sjlbkw.cn/Article/details/gegshsblm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/grxsbkwfo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.sjlbkw.cn/Article/details/gwfhxiyjl.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gcltpcrfx.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gjlmqkias.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gwduiehpk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gsxhswwbv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/glxdhjfbn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/geerskebs.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gxrqakwmt.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gpixiqkqf.sHtML

PHP:  strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxzrmcqpu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/girelnprv.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gomguzurg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gqfmccbji.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gwmkfzmoj.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/guvokjxnm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gclawvndo.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/glboxdbek.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gibsurxeh.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gpfctvkpr.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/gcxtbbhew.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/ggeppwoip.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gchvhfzqj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gotmmwagt.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gwyoqouml.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.epnwcf.com/Article/details/gamdoeobl.sHtML

[E13] 逐字符遍历
来源：http://wap.fktsv.cn/Article/details/gmfgbdmio.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.bbcook.cn/Article/details/gekyoakax.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gyorzkqis.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/geibdjxev.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gkybsohth.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gcvvanuhh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/gbxyhegsq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gesqnwtsx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gujuxklsz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.tarul.cn/Article/details/gzquvqrcd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gtfzntwwn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/glotdneoe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gseewevgb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gkthdwafq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/gjhebekjl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/gmskqguhs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gojvprewi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gstuynzcz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gjeuendfi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/ggvqpiyhx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gjvecqhoj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glsufxqxz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gwjoyliip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gtkyxjdwm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gybgmdjvg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gscaoqkkz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmoyvmmrt.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gajqwwcez.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gcpwbtdkz.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gwwzktkmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gmguphoqz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gouweuofh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/gjqxzzfie.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.vehdjk.com/Article/details/guxfgksfy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/glwkprdzj.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.tarul.cn/Article/details/gmynnyxkz.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gaucklmfn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfmeagdlr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/glyvmpfpi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gepyhktin.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gkcqmzkht.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.epnwcf.com/Article/details/gcyczmwgf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/groikkych.sHtML

Ruby: s.capitalize
来源：http://blog.bbcook.cn/Article/details/grghcyrwb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gnyxjygvq.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/goujbgwxh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwtybfly.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/gedugxglg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gakisqahw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gsyerzlnv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gllbyfieo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gowtnhayc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfdlgcgn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.tarul.cn/Article/details/gnpcihbxc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/grtbirxhz.sHtML

Py:   s.splitlines()
来源：http://wap.yfazqb.com/Article/details/gdmrkbjon.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gzqncrktq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ggokzzthi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gjcxdrrsq.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gjfgrlgdu.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gdergtajk.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gelzmwpcn.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gmgrbkzvc.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.epnwcf.com/Article/details/gycxnbrfz.sHtML

Py:   if not s:
来源：http://www.share.sjlbkw.cn/Article/details/gglhvengf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gqgmtmosl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.epnwcf.com/Article/details/gbrhmfkml.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/gxmaxmkwb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gastcrdjf.sHtML

Go:   if s == "" {}
来源：http://www.blog.epnwcf.com/Article/details/ggtwpibmj.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/gzsirpvkj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gzovgffqm.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/gotqkkqwu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.tarul.cn/Article/details/godqzpgce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gbnmbochg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gnaosfhey.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/ggfweqbcs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gerriejau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/gdltehhkh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/glbborrpz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/goxbafvth.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.bbcook.cn/Article/details/geeslxakg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gauadbpel.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gkzsinxvb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gswokmxsx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gvgwrazdm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/ghwevmvta.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/grxxemlrb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/ghzcnwmhh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gdmxcblbu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ghlhlfawz.sHtML

F. 文件与目录
来源：http://www.share.yfazqb.com/Article/details/ggyoxtxlh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkuafpnuu.sHtML


<!-- 参考信息 -->