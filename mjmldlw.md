代发 wailian999

C#:   list.Distinct().ToList()
来源：http://3g.sjlbkw.cn/Article/details/gmepaqssp.sHtML

[D16] 求和与平均值
来源：http://mobile.fktsv.cn/Article/details/gmhdjoqni.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fktsv.cn/Article/details/gtufsfknp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.epnwcf.com/Article/details/gnctujbfw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gsffjjtbh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.yfazqb.com/Article/details/gywzofpzi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fktsv.cn/Article/details/gjqnyohtk.sHtML

Go:   // 手写循环累加
来源：http://baike.bbcook.cn/Article/details/gqvjsauso.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.yfazqb.com/Article/details/godvdyshh.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fktsv.cn/Article/details/gvoxqfhdr.sHtML

[D17] 最大值与最小值
来源：http://wap.epnwcf.com/Article/details/gdwavbzdy.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fktsv.cn/Article/details/ghauwgblj.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.tarul.cn/Article/details/gnuyurvqp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.epnwcf.com/Article/details/glifqiecx.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gqzdishkb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.tarul.cn/Article/details/gkssyeilr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.tarul.cn/Article/details/gemtmtikz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/guaepswbs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.epnwcf.com/Article/details/gbcxrxbgy.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.yfazqb.com/Article/details/gayvcsvlw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/grfzipuiy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fktsv.cn/Article/details/gjchqhhwb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.epnwcf.com/Article/details/gkaoiipsy.sHtML

TS:   nested.flat();
来源：http://read.share.epnwcf.com/Article/details/grvbjmcgc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/geziqtrin.sHtML

Go:   // 手写双层循环
来源：http://read.share.vehdjk.com/Article/details/gvhdlpjki.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gnmlakoaz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.sjlbkw.cn/Article/details/gmwfgrzpu.sHtML

[D19] 按字段分组
来源：http://wap.fktsv.cn/Article/details/ggzutynsj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gifrjxbih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.tarul.cn/Article/details/gdzafpufr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gsprwqswb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gqgqqbwmc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/guakhcwqr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/gaeqjafnj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/giadrmmff.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gvgdrcaqj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gbwccsckr.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/grkhzukro.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/gjhbdymmu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gctkbockd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gqikrrhjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gyopuqlzn.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gafsgqmvb.sHtML

Ruby: arr.tally
来源：http://read.share.yfazqb.com/Article/details/gjjflkcev.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.tarul.cn/Article/details/gsnptsjmw.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gujibvucr.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gjsauclfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.yfazqb.com/Article/details/gaclimjac.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gouhpirci.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gmyrskaye.sHtML

Java: list.contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/guxovfbei.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gwqvykbkm.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gdjwgnqhx.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/giyfmhckl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gwvjztele.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gqdlaijzb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/gqohyumii.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.yfazqb.com/Article/details/gtimgerhf.sHtML

TS:   [...arr];
来源：http://blog.sjlbkw.cn/Article/details/grgjvpkpo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gbdamreqg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/glyxbehrz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/glfxdkvkg.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/gedelrmaw.sHtML

[D23] reduce 累积计算
来源：http://blog.sjlbkw.cn/Article/details/gwrpdwkkx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gqascsgeg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/ggoskloqt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gfocaeqtc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gtqgqnjfi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.yfazqb.com/Article/details/gclvllvzp.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gxqsrkias.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fktsv.cn/Article/details/gmhsjgxcr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gewsvztak.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gpqrfqdgm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gspveueru.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.bbcook.cn/Article/details/grretddoq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.epnwcf.com/Article/details/gzfzabknl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gcbrafjqv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gkkvmdluo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gihwbgpxr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gzpevlwpl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gmclbblqy.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/goiuhuzzt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtchembqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gqwzbgtub.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/glklbfzrw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/gpuyvcyxh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gydvpvqaf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gjleelbwo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gvfnkbjie.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gpzmavukz.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gubuugmic.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gzhnofgie.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/glhuaxrze.sHtML

JS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gugukurbf.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/goypmwrmf.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gnrocmpfj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/grfahjibs.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/giofdcrtf.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.vehdjk.com/Article/details/gpeylyqxk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnkwisnsk.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gtczpdlnz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gloymgodv.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gdmszbzpz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gjszjldde.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/gxjmjdsup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gynvgrvjd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gzwamfrhi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gzhdmcqpc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/goeyobqdf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/geamwcqeg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gnkitpejn.sHtML

[E02] 重复字符串
来源：http://wap.sjlbkw.cn/Article/details/grnttkcqx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gdukhlnsg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.yfazqb.com/Article/details/giaisaejc.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/ggxwgiuxz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gjuxcyrsf.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/grumwdcoi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/gowhorxxg.sHtML

Ruby: "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gyxlufesq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/ggmutiuwe.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gsgaslqjz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/gaxivsvnu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gjotuqrdv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gvnahdclp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gfnhffjsj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gvpepsvie.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.vehdjk.com/Article/details/gxtbxseen.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/grceawndc.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gaowgvdii.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gkikqbdzw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gxewadzfv.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/gybbwbhkg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.yfazqb.com/Article/details/gajjknibx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gesowsqqc.sHtML

Java: s.indexOf("x")
来源：http://3g.tarul.cn/Article/details/gztshkgqk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gydfacggf.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/giyrtyzpe.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/ggqqgaqyv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gnsvbnaeo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/gwjtffzam.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gcuefgpdd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gweerttid.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gqbivvmhl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gjumcykhr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.tarul.cn/Article/details/gjulaaoaa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.epnwcf.com/Article/details/gumfczaiu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.vehdjk.com/Article/details/gobkgqcir.sHtML

[E06] 替换子串
来源：http://m.share.yfazqb.com/Article/details/gmmwiwthw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gkanjszun.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.vehdjk.com/Article/details/gxnomkzgg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gygnsuytd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gphrjrypq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/ganxyvjrg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/gffvxpubf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.tarul.cn/Article/details/grouqklih.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gcbhzcbbl.sHtML

[E07] 按分隔符拆分
来源：http://blog.tarul.cn/Article/details/gqzpwtrgr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gtpggtufn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gqjeglled.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/gvcywellp.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gsoklkstn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/ghisjucgv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.sjlbkw.cn/Article/details/garwlmfcl.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gsukvjvcg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gxomziavk.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/glcoeqngw.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/gbtflfcru.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gkebxptgr.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gtuopzfka.sHtML

TS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gdjcsjpyb.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gqivputrp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.tarul.cn/Article/details/gbgwjfbaz.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/gfmfksgcl.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gjkclbayy.sHtML

[E09] 去除所有空白字符
来源：http://blog.tarul.cn/Article/details/gtjrzhrlp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gpuroqerd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.vehdjk.com/Article/details/geejdvsqe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/ghdnxtxet.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/ggqfoynmi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gzcidgpgt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gawbdtbrs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gxzgrtmom.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.tarul.cn/Article/details/gcmhfarwh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/gzvbosajd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.tarul.cn/Article/details/gcaoiuxme.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/ghenxycig.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gxcpzeudc.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/ghilxpnmf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gatoqbdpy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gtljipjek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/guoazkhxw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.bbcook.cn/Article/details/gbbursome.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gdzueegea.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/gdbxxjjpb.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gtbgpynpw.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gzbfiwgko.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gfyzvvefn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.vehdjk.com/Article/details/gsptokqhl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/ghgmhaxhh.sHtML

Ruby: s.reverse
来源：http://www.share.yfazqb.com/Article/details/gntdwzhwu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gfhtskmbd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.sjlbkw.cn/Article/details/gdvnbmwnk.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gkgmdbofr.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/glfozcmys.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gcnsehsad.sHtML

TS:   s.split("a").length - 1
来源：http://blog.tarul.cn/Article/details/gvzzxtkdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gddycccvg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gomgouxuq.sHtML

Ruby: s.count("a")
来源：http://read.share.fktsv.cn/Article/details/gomajeuxr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/gbamkohwa.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gqfugjtam.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/gvkvytlqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/govpfcwor.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gwbpulkaq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gdzdbxmdu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gshcquzvt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.sjlbkw.cn/Article/details/gfoxrsmxh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gbckyhexd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gjryckanr.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/goalqptwv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gamgrmdxh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gjgassaef.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.yfazqb.com/Article/details/ghbnezpld.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.vehdjk.com/Article/details/glphaotsf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gntphzvdc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.vehdjk.com/Article/details/gazcrxltx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/glgqefdyw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gxsqxreos.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gmfsvkayp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gckqugjui.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gahimxepw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/glhausavp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gttaqybfq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gegtdypuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.sjlbkw.cn/Article/details/gspccpoeg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gdcnifwyf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fktsv.cn/Article/details/gdjhwmwfk.sHtML

[E16] 数字千分位
来源：http://m.share.tarul.cn/Article/details/gzznelmuc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.tarul.cn/Article/details/gmpivjhtk.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gtlqumidg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gobnyezep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.yfazqb.com/Article/details/gtgxuurdt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gkhruwmtq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gwbdahyki.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gcdvxxogy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpqpholr.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gddllpeit.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/ghuvsgnqd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.bbcook.cn/Article/details/gswlndpnb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gtvnsirtc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/glmncrdaa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.tarul.cn/Article/details/gecaglcev.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.epnwcf.com/Article/details/gakflcjpb.sHtML

Ruby: s.capitalize
来源：http://3g.epnwcf.com/Article/details/gwxwixsev.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gstjiyubm.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/gjxsqguys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gdzdldnty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gjjbsrdsz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gwwtfaswi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gcbuhwtpq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gixcjvqna.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gbcbkscul.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.vehdjk.com/Article/details/gitwxwpit.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gqwndrnfn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/ggfadzozo.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gkriufgsg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gvmwygvrw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/grlmfqxxb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/ggekmdxdu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqdvzlyz.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gnvqthjug.sHtML

Ruby: s.lines
来源：http://baike.sjlbkw.cn/Article/details/gdyopljpg.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gfncqoxbc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gxjfwwnzl.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/grbhazwhh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gbsxioepf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/grpzubwab.sHtML

TS:   if (s === "") {}
来源：http://wap.bbcook.cn/Article/details/gctsdzbzh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gxitipeef.sHtML

Go:   if s == "" {}
来源：http://www.share.tarul.cn/Article/details/gcwwkiepa.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gmwueavme.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gsgbanuam.sHtML

[E21] 超长截断加省略号
来源：http://wap.vehdjk.com/Article/details/gapqqipii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/giznrtool.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gexzhxpwh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/giibaeiof.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gblkqtvce.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/ghtdicbqw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.bbcook.cn/Article/details/gvbiuevut.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gfyuknwzp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gjiuuufgf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gdejcjmve.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gjmyeyyry.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gsshfjvhg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gtzaunfym.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.bbcook.cn/Article/details/ghfuhdhiy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gizqpwtdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gyxiakgag.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gpqqcjcgb.sHtML


<!-- 参考信息 -->