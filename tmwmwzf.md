代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.blog.fktsv.cn/Article/details/gcbjggbmm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.bbcook.cn/Article/details/grxqlabgw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/gtxlkmnpt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.vehdjk.com/Article/details/gsigclgkc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/gopqovbgc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.vehdjk.com/Article/details/gtixyhbxg.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.tarul.cn/Article/details/gpohshgof.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.vehdjk.com/Article/details/gdzkkella.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.tarul.cn/Article/details/gcfqjypuw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/grwmhiycs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.tarul.cn/Article/details/gjnvmihox.sHtML

TS:   nested.flat();
来源：http://blog.sjlbkw.cn/Article/details/gtmknjole.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.vehdjk.com/Article/details/gbptydfwf.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gdreteppy.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/govllnexy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gjnfivbus.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/ghtjgamyw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gtkcvfybt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.yfazqb.com/Article/details/gwzudwjtr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gvdaeowdo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.vehdjk.com/Article/details/gnsrabldf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.vehdjk.com/Article/details/gczcuafpd.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.vehdjk.com/Article/details/gyvbnlvgl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/gkjqhdrqz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/gqwdloczr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.tarul.cn/Article/details/gwyfcrgbl.sHtML

Py:   Counter(arr)
来源：http://read.share.vehdjk.com/Article/details/gvnhlydpd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fktsv.cn/Article/details/gvrsqmbpx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/gzrzecyqb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gvxqjinnw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.bbcook.cn/Article/details/gxwoujfqh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gawkyuuxr.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/grxdpxifc.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.bbcook.cn/Article/details/gbzzximrd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fktsv.cn/Article/details/gxxppauxv.sHtML

Py:   x in arr
来源：http://blog.tarul.cn/Article/details/gahkfkzjc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvsqktw.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gssiofyed.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/gsiwuayhn.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gytapgvsc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gyrjlatao.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gwmbkjmpl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gzhprsdlv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.yfazqb.com/Article/details/gmlsmwelz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqnuotoqb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.epnwcf.com/Article/details/grfhorjva.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gitrjbiew.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/gdqlkzuin.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gqsatzube.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/gmaxerqlz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.bbcook.cn/Article/details/gjqjqayya.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gekqklhxb.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gqmiqdgla.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/glrmqjrrt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gydnbcpfe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/goyhvjkkz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gqqotxvsf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gyuqxncgk.sHtML

Go:   // 手写循环
来源：http://3g.epnwcf.com/Article/details/grgrxgnem.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.epnwcf.com/Article/details/gzjomulpc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gtkxdqxsb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gknncqrme.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gqelqfqka.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdltlpij.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gniniaudn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gxtppvsbx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.yfazqb.com/Article/details/ghiuutjzi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fktsv.cn/Article/details/giiehaoat.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/ghfqkwdgf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.sjlbkw.cn/Article/details/gfuhmsmdm.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gijofkxqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.tarul.cn/Article/details/gpiuzyqim.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gqmtnlqbf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.epnwcf.com/Article/details/gihfhhegq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/ghdnvzgrg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gvkkhhdch.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gozfoyvwj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gnvevmrrf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gzirwpnng.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gbiisrrxc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fktsv.cn/Article/details/gerasfnlc.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gswnzargt.sHtML

JS:   arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gxmhrrtsu.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gjcmsqhuq.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gykndjcye.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gmpvmjqsb.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gqgyeauhk.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gwcxkobje.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/grqpzsvrn.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gxcvfjreb.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdhgjqezc.sHtML

[E01] 拼接字符串
来源：http://www.blog.tarul.cn/Article/details/goodmtnzu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.yfazqb.com/Article/details/gmvypcxip.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/grjgwpynb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gjgnhrvar.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gahknjlan.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gzlelazdx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gfocmenhs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gzaqzuipg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gilrgwija.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/glclkyvyz.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gveectbjf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gknazchmu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gerxxjebm.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gwajcfmzo.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gqomjxdsm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gpkzpwwoe.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/guwklyrsg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gsiipptpr.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/gspduhvck.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gjdqrtezu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gqlkgirqq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gzkaldvgh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fktsv.cn/Article/details/getvdikqy.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gzxtyraht.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gsiomuygm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/gddigcemd.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gefpaozvq.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gtzdaktux.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fktsv.cn/Article/details/gjbjufmyy.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.bbcook.cn/Article/details/gvirbrqrp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.sjlbkw.cn/Article/details/gdvvjctrb.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/giuctdkss.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gpiuzqkvf.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gkjsnmvbk.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gxiagpqdj.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gfbxhebjm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gxkankmpk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/gfidwawaz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/ggupipuea.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gmluvnxam.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/guovakfaw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/ggwbhgbds.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gynafyhuq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gzedmtzef.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gkzpcotwb.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gcauqncxv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/ghvvysmrr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.bbcook.cn/Article/details/gjgxiladd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gimhkrqom.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gzasrgzyc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/ggwrbcjur.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.yfazqb.com/Article/details/gmhcvvhqy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/guzuuinbf.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gsjoxsezp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gkpigyicb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gfegbuuhy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gycclzdkx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gvnvmlpmp.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gpnlckpjl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gixmwezyt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gaugpremp.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/ghtuwkxbr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/gwepzypdf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gvyxjvtlt.sHtML

Py:   ",".join(items)
来源：http://3g.sjlbkw.cn/Article/details/glbeonovj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fktsv.cn/Article/details/grypnavcp.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gxqoasfor.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gjvhgqgrw.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gypiiydad.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/gzsqzvzaz.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gdwbivify.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gxjrjnvfz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.sjlbkw.cn/Article/details/gnxlsbjqn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fktsv.cn/Article/details/gxlsclpwv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/grxajwexf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gkvssfstb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/guwpgpndt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gvlngryzr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gneiokkbu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gpvmyozyc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.bbcook.cn/Article/details/geovvmawi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/ggeybzvig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gwmecbmti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/gjhemtrjv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gajqvrlze.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gnlqqskal.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gptbniobu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gfzngailf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gmykqvean.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.vehdjk.com/Article/details/gaakgebcu.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gxuqggxgx.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gaofsfyjb.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/grwdyfdhi.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gqkxidywo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/ggavuyeny.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/gxtbxmvks.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.tarul.cn/Article/details/gexconbpd.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gsdvihpfd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gvbsezuca.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gjiqlshfi.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gwijpxblj.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gdzzhvdzx.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/guabtaqbd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gtsjsotgb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gdhcofmzt.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gnewwfgia.sHtML

Ruby: s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gkvesmryq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.bbcook.cn/Article/details/gzzwqzshk.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/grcsgnqmr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gqcbewnpv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.tarul.cn/Article/details/gldmyluza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gnoxbylbi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gxlepjosj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fktsv.cn/Article/details/gkmybxlme.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.yfazqb.com/Article/details/godnmzpic.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/glkuwjxyq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/guxxnfamm.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fktsv.cn/Article/details/glkawqjyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.tarul.cn/Article/details/ghogwrsnn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gknpusfxw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fktsv.cn/Article/details/grlgeefdf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.yfazqb.com/Article/details/guhergibi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gbwwncpoj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.sjlbkw.cn/Article/details/giqgvhcio.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.tarul.cn/Article/details/gqyjucfvc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gnmskvmov.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/gwlsnovyr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gwowimccy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/ginktviws.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpcrdryap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/ggpxmcxck.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gtfysvhtd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fktsv.cn/Article/details/gpnujbtoh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gxxklxrug.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/gtrvmzvxj.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/gypjeqbzb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gpciikhrq.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gxggzorgg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gmqscowbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.tarul.cn/Article/details/gvxuwsgdj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gktettjhs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gkeltqhxz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gwfdwxjqq.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gqcumfvha.sHtML

[E17] 首字母大写
来源：http://mobile.yfazqb.com/Article/details/gowzpdicr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fktsv.cn/Article/details/geguwajrx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gxxibmxnz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gnnsqwuki.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gjxkocjcv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.epnwcf.com/Article/details/gozntiwit.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gakemnawr.sHtML

Ruby: s.capitalize
来源：http://blog.sjlbkw.cn/Article/details/gtqsggmal.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/guhviopxa.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhrsbzgp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/giesmtrys.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.bbcook.cn/Article/details/gkragrwet.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gpjsebgwh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gyxqtpeuh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gbivrrlat.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gefrfoagc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gmbnkuwet.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/goyfgckno.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gabkpeqtq.sHtML

Py:   s.splitlines()
来源：http://3g.epnwcf.com/Article/details/gcqrlakuj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.yfazqb.com/Article/details/ginecyekz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gkdkjeidb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gjcyrseqi.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/glggcyptk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/greqfgccf.sHtML

Ruby: s.lines
来源：http://www.m.share.epnwcf.com/Article/details/glnbxnxdc.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/ghrikkjgz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gzbyqdemz.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gvdnwnuyf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.yfazqb.com/Article/details/ggckhnjqd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/giupzddda.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gbkbouxcx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbmdpwlfe.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gmiloysvj.sHtML

Ruby: if s.empty?
来源：http://www.m.share.bbcook.cn/Article/details/ggcslgput.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gzhedbzqr.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gcuconsdq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fktsv.cn/Article/details/gpmgvugbk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gjhfbqpah.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gfwocfigi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gvuehzsdi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gbymugdoe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gxsdzrnbp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gjriiuthh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ghoxtzuzs.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/grozbbioj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/guqptpvvg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gqgzikuhs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/ghbouhuso.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gsixdaexc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.vehdjk.com/Article/details/gshcelunt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gdcjqimmm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gbuqewigp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/gxnhphkvi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glhnkzjtz.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gbzuikeuw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvihxesum.sHtML

[F01] 读取整个文件
来源：http://wap.epnwcf.com/Article/details/gtudxuxiv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gbgtiovte.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gbfwkvwgj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gtwtlykxt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gcgxunlae.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/grgrrnbhp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fktsv.cn/Article/details/gvqsmcynu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/glmmglzdg.sHtML


<!-- 参考信息 -->