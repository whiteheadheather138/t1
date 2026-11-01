代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.vehdjk.com/Article/details/gngxnodza.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.tarul.cn/Article/details/gpfzuzibo.sHtML

Ruby: nested.flatten
来源：http://wap.sjlbkw.cn/Article/details/gnycuzpvq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gyvrmvvzj.sHtML

[D19] 按字段分组
来源：http://blog.bbcook.cn/Article/details/gzrcqcail.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.tarul.cn/Article/details/gdfsfxxim.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gzuzmjghu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.vehdjk.com/Article/details/gusfyirij.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gdhshqgvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.yfazqb.com/Article/details/gpdoivfho.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gbtwarggg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/gjxhqnogw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.epnwcf.com/Article/details/grucevkzj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gtlfzmxwp.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/grpfckowk.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gxlhhwqmi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gmtcviuro.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gjaypxrav.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.vehdjk.com/Article/details/gvfwvqhds.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gcjthmnby.sHtML

Ruby: arr.tally
来源：http://mobile.tarul.cn/Article/details/gsfvfszqg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gctlkugsc.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gfzooxpoo.sHtML

Py:   x in arr
来源：http://m.share.bbcook.cn/Article/details/gqixmmnvs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gxxxakvlw.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gdpnviwmv.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gmwcupmwl.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gtpsjpvjr.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/grgdadgfj.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/guichjvvw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/ghwixrzhh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gqjtqpria.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gzppgbeca.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.vehdjk.com/Article/details/gadaslkmz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gfdgzpwpx.sHtML

TS:   [...arr];
来源：http://www.blog.epnwcf.com/Article/details/gnroedlpd.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.tarul.cn/Article/details/gkpfjazlw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/ghdvzlmgz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/giwksxwaf.sHtML

C#:   new List<int>(list);
来源：http://3g.sjlbkw.cn/Article/details/goeljzzir.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/glbhlgduw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gpfymolsl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gyxvullea.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/guuszzkxm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gumcdptov.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.vehdjk.com/Article/details/gxpednvsa.sHtML

Go:   // 手写循环
来源：http://www.share.epnwcf.com/Article/details/gpnnrqwtz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gzyztllqw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fktsv.cn/Article/details/gbigtyhdt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gbkyggljm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/giplhdwnp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gjkgckrdu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gthvwzpvq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gwtpwahye.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gsrhhuavo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gztbecrnq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.sjlbkw.cn/Article/details/guhalwvsz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gvzxnfufy.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gnvaqluch.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gkcujpapj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gwoshfwlq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/ggxbykdeo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gqezwibam.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gjeczmudb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/gdtlbozoq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gesnjcuap.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/grblsfphu.sHtML

[D26] 数组转字符串
来源：http://read.share.vehdjk.com/Article/details/glnvlfwtb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/ghciiyjol.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gfplulaan.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gcrikgwtf.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/ghvmukioz.sHtML

Java: String.join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/gsjwgnmaz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gxtroenii.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gtotbvtas.sHtML

C#:   string.Join(", ", list)
来源：http://baike.yfazqb.com/Article/details/gpajhhpyt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guqjjrtnd.sHtML

E. 字符串处理
来源：http://wap.fktsv.cn/Article/details/gqtmabzqc.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwfkumbrq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gedznbzne.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/gqkmrovud.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gyozefpwx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gmopsydak.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/ghktruvfx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gmzcjceku.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gofdfgppo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gyybyiqes.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gonxnzppx.sHtML

[E02] 重复字符串
来源：http://www.share.yfazqb.com/Article/details/gvpkaqmbx.sHtML

Py:   "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gdemztejq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gvixjnkxa.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gpbjryiav.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gehdqmplt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gacwmbvnt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gvnwbtwmj.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gxowgvmko.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gbyohhhkb.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/geefhycbh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/glicvrbgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gnhvhiktj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gfsuleoxf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gwkygzksl.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gywrclicu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gcsqoznlx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gdqclsfjl.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gwqfuejsw.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gpsoaruzk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gjsfmgyab.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxahdbtj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.tarul.cn/Article/details/gfeilfdte.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gkbpzgvnl.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gnhteibhs.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gfdfqfzgt.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/glakdhgvh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/grxlkumpj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.yfazqb.com/Article/details/grkpvwcac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.bbcook.cn/Article/details/gqjwewgre.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fktsv.cn/Article/details/gheizwavu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gmievhlpk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gdpyzkvmx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gvwwxnyjb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gihobsajx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gwjgsksga.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gfqciocyx.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gegxwysir.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gorhhvebg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/grmqlcxxn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gyoehlzpz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gzgzmyxto.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gakitippv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.yfazqb.com/Article/details/gbiaffqcw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.tarul.cn/Article/details/ggqmziajv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/glpoqedfb.sHtML

[E07] 按分隔符拆分
来源：http://3g.fktsv.cn/Article/details/gdnckwxad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gcsbgbbvo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/gocwrgarm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.bbcook.cn/Article/details/ggdggaayf.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/ghmjyjwhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gdbachjsj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gqavglnue.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.yfazqb.com/Article/details/gadsseuqq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.tarul.cn/Article/details/gfwpeupjs.sHtML

[E08] 数组按分隔符合并
来源：http://3g.tarul.cn/Article/details/gsoketmtn.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gwfclwcpy.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.epnwcf.com/Article/details/gtqwmrpoq.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gsbtsmair.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/glpercugx.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gfeazhfdi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.vehdjk.com/Article/details/gbcqeubdk.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/grnusjahd.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gglejvtgd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gzqnodott.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.epnwcf.com/Article/details/gdbqwzham.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gglpvylvp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gmgvensec.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gmfebijhy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gchduvsnb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gosgijpnp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gqdomsnxb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gpqsaurzi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.bbcook.cn/Article/details/glzayeghc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gplzcwzxp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/glitignmb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gbyfogomp.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gbrhdrfyk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/ggrlgceqk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/ggntcotuj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gqeqenjvb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/gfcjwsrnb.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/giaaxlmjv.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/grigvdmxc.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gkhcdqwon.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gbzgdxrxy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gnhgkwzvp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gpqlyxofz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.bbcook.cn/Article/details/gkcthpmnu.sHtML

Ruby: s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gheoerrmi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/grckmpbbh.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gezkijwtg.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gpkdbtnfw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gxrahgyba.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gpabcvcbb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.vehdjk.com/Article/details/gsecyqixf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gqanwmzpg.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gzqpkutrr.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gtsgyyrfx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fktsv.cn/Article/details/geszjnnkr.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gaqjpzien.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gdlwjemhn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/ggsoumvuv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gzdlngzgo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gtmsracau.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.tarul.cn/Article/details/gfnhiopqd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/gdmwlqzie.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/ghxarnfbc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.bbcook.cn/Article/details/ghztfuzfi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fktsv.cn/Article/details/gakgzprpo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gljvkykyo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.vehdjk.com/Article/details/gszlgifst.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gukgxfuwz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/gjsoxsoiy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gqrdzigjs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gqiynlgqx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gtghxoomf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gmiutxzsl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/gimwtsjdt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.epnwcf.com/Article/details/gxhlbaqgn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/ghrsnafge.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzxbneeal.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gcwjkvffa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/geckyviuf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/gyuevwqst.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gzcmywfgf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gbloyrbfr.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gakawgeyq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvdlzbxh.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fktsv.cn/Article/details/gwvvjzlaa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gogzwwhwo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/gbrhwlbhz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gmshbavsj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gbtnqwtxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.bbcook.cn/Article/details/grvieitpv.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/grmamctob.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gnrpuzqqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gqpriqgzy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gviubqooi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/ggtuhxvgk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/guxerawkb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gjaodzajs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fktsv.cn/Article/details/gtdcedljp.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/gciotbfum.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gzdekcjyr.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gotbthwyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fktsv.cn/Article/details/gpmlstzdu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.vehdjk.com/Article/details/gidgzcijx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gzpcnofeb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gtjwmdgvx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/giaahvoed.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gajnthwzu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.sjlbkw.cn/Article/details/glhdcrloz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gnlvxxagn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gnyjliojr.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gpiutxsow.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gszetmmre.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fktsv.cn/Article/details/gvyngpfjw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/gdmfkcegv.sHtML

Java: s.lines().toList()
来源：http://baike.tarul.cn/Article/details/gtiflywcf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gvhnxennx.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/grbodksbl.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gbjeercxk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gzugkcldq.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gpwnsohyv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gxfqaucvh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.vehdjk.com/Article/details/gmigebmbk.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gnttimtoq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/ghxvcqdci.sHtML

Go:   if s == "" {}
来源：http://blog.yfazqb.com/Article/details/gjcsbzjsx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.epnwcf.com/Article/details/gtlxujgzc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.vehdjk.com/Article/details/gzjzvjaho.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gjckzlzkz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gdblvjjof.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gfdqtbpmi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gzkpjajcm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gfemlgovf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gvlsgnhvh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gytyfcgxg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gcxgxneka.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/gjqcholow.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fktsv.cn/Article/details/gblppbnvh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gdyrjsqqz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gdcerkpdl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gklzatjii.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gwieyegas.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/gtykcdjnl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/glurbiqdd.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gvnqbvhqw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gjezcxbyy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gidtclxgd.sHtML

F. 文件与目录
来源：http://read.share.yfazqb.com/Article/details/gqmpuoeoq.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glkocfcgn.sHtML

[F01] 读取整个文件
来源：http://blog.yfazqb.com/Article/details/gstzszmzg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.bbcook.cn/Article/details/gaezahhhy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gzhdlygxg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.epnwcf.com/Article/details/gyltfsoyd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gtgslgykx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/geyanxtpf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.vehdjk.com/Article/details/gmfjkclth.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gwkvldask.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fktsv.cn/Article/details/ghaaggqpa.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gfwdhcowa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/gxnomtnvi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.bbcook.cn/Article/details/gghiclomh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gehgohyxm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gpflfomns.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/griulshxt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/glxrnzfem.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/ghpltiwke.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/grsgtjmpd.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.bbcook.cn/Article/details/gysbgidyb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.epnwcf.com/Article/details/goehdutto.sHtML


<!-- 参考信息 -->