代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/gluklzvxc.sHtML

Go:   // 手写双层循环
来源：http://blog.yfazqb.com/Article/details/gcajctsbd.sHtML

Ruby: nested.flatten
来源：http://www.share.sjlbkw.cn/Article/details/gyzqwfvbo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.yfazqb.com/Article/details/gbwhxdrnl.sHtML

[D19] 按字段分组
来源：http://mobile.bbcook.cn/Article/details/garkuxwdb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.tarul.cn/Article/details/gszeufzyv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gufyzerru.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.epnwcf.com/Article/details/gydvtfyji.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.epnwcf.com/Article/details/gcmzjahve.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.epnwcf.com/Article/details/gmlemcrit.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.vehdjk.com/Article/details/gdmuoxlfv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gjhasuipe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.sjlbkw.cn/Article/details/gxsvpjpjk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gcohnsisv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gmhllbhsz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.yfazqb.com/Article/details/ggvngwfye.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gdoqosvuj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gfdrmycpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqaabtgx.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.epnwcf.com/Article/details/gvbnordod.sHtML

Ruby: arr.tally
来源：http://mobile.sjlbkw.cn/Article/details/gbleqmxtl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/guehdvvaw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.vehdjk.com/Article/details/gzqlhsogn.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/ggemnkthk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gqpvokulw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gdxggknrv.sHtML

TS:   arr.includes(x)
来源：http://wap.epnwcf.com/Article/details/gvvwhypdz.sHtML

Java: list.contains(x)
来源：http://www.blog.vehdjk.com/Article/details/guydycnku.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gvnjqhlil.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gaxztstpa.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/giyeftkqu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gnbpdnrzo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxuwnjfuf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/gqkbbvcyf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gwmmcastz.sHtML

TS:   [...arr];
来源：http://www.m.share.epnwcf.com/Article/details/gzzrvoeqo.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gycnjciqk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gpdtsjvlt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.vehdjk.com/Article/details/genkgwsqz.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gqukosyde.sHtML

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gftwidopv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/goswnmhkr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/ggouydcwu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gdmdxpphu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gdrejymzr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gpsdasddw.sHtML

Go:   // 手写循环
来源：http://www.share.fktsv.cn/Article/details/gvlaepexx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gvenycqkm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.bbcook.cn/Article/details/ggvtomqcp.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/gfqsxrlis.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gfcbwyjyv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/goivlyhob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/gibxunhbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/gifxcymtn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.bbcook.cn/Article/details/gihbaiwyy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gwnljaoee.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.tarul.cn/Article/details/ggxeydotj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.vehdjk.com/Article/details/gyrtbnjim.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gdmajydhk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.epnwcf.com/Article/details/gqshknuha.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gisrlwtmw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.epnwcf.com/Article/details/guvnwjwhk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gmrivxtye.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gpnzqdgkx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gpedfqswz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/guigiyfrt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gbixrvzld.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gvzmapmun.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/glfnpadaf.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gqufirixw.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhptnnhc.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/ggeizypzj.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gnsjwiymg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gkqitfnbj.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/grvptcuby.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/ghoybwuyb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gquzudlkh.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gifgfueoj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmxkdtatt.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gjszlzcqy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.vehdjk.com/Article/details/ghymagtwy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gvjjbimlg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gxxkzbjhc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gucwastfm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gnyekqtxz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gcukbiflz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gumqqsdse.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/ggibqywze.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gcbrmforx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/ggqccpmed.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.yfazqb.com/Article/details/gqeqtppev.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gzekaleyy.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gucddkmwl.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gxbkmwhjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.epnwcf.com/Article/details/geiuycora.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gydbxndqf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.vehdjk.com/Article/details/grrjkgolz.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gszsqzwft.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/ggzvlajpk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gshiaatei.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/geghvpzgl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gdxxidngt.sHtML

Java: s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gpqsxjkmy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.yfazqb.com/Article/details/gbzpvyfim.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gzkrsutkb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.bbcook.cn/Article/details/grwoctaez.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gopyxpbpd.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gjaknrngd.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/giyhephag.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/gdwythqej.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/glqqybadb.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/glcasfulh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gbqfrjsjn.sHtML

Ruby: s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gtqedzibw.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.bbcook.cn/Article/details/gkaaeukly.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/genfaxtdq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/garvfeptv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gndywlzyp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gwdooghao.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fktsv.cn/Article/details/gqaqzwrau.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/goitfgved.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.tarul.cn/Article/details/grssmalui.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/gllwxthpu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gawquxaqo.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/giscjxote.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gkfqakjic.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.sjlbkw.cn/Article/details/gnfjbkgin.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gsolqlszs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gfototkfn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gcvvecplm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/gujgnsaoj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.epnwcf.com/Article/details/geqrkzftv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gyneilcca.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gyyggvmoi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gnwtkvieg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/geidkwzpx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.epnwcf.com/Article/details/gzwsvvgez.sHtML

TS:   s.split(",")
来源：http://3g.yfazqb.com/Article/details/gctjxyzld.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gkvfjylkf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.vehdjk.com/Article/details/gyltxqxsv.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gxvyvadsn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gehnpkmio.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gxaujsgkf.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gkzmshpdo.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.tarul.cn/Article/details/ggiruhjpv.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gxrpvskmm.sHtML

TS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/grbnjwcdf.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gkytrfvim.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fktsv.cn/Article/details/gsfyppjji.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gqdntsbfc.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gsvqrazoq.sHtML

[E09] 去除所有空白字符
来源：http://baike.yfazqb.com/Article/details/giwjglnvq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gnnfdzppq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/gpcpobycx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.vehdjk.com/Article/details/gznuqexqw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/gaqceuzwe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/ggqcqeaeh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/gbxdyffjl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gpfccareu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fktsv.cn/Article/details/gjhezlhmj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gifnrnsqj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.epnwcf.com/Article/details/gtgpxpchx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/gvpjngktn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gazwhhdkp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gnyidsqjp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gkjtmapho.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gjqbirhka.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gexhgwbpb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/gqldmzuzz.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/grpkmuhue.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/geepmwrgf.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/gozkorplx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gwlcsrbwq.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/glbjegybh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/grulsczos.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gwsdgobgt.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/ghutluvkl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gngjytsxs.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.sjlbkw.cn/Article/details/gjxwzbcdp.sHtML

Py:   s.count("a")
来源：http://m.share.tarul.cn/Article/details/glpiocwoy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gvsnjctht.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gqrnxubfx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gdnxxbxqa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/geuvduwhd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gfowxfpoy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.vehdjk.com/Article/details/gbnqlqdyb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gfwqhbqkm.sHtML

[E13] 逐字符遍历
来源：http://baike.vehdjk.com/Article/details/gnryfcfuj.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/gzpcihmms.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gayelzdyn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gcxfqkbhh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gypizbdcl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gebvatmdo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gzgoraerv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlrbprmi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gjuheaxsv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gsknhcfjb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gyatlzpen.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.tarul.cn/Article/details/gxdywwuwj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gtnxbzfzz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.sjlbkw.cn/Article/details/gqybisslp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gsbfzzfqd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gjitoirpo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fktsv.cn/Article/details/gljphwgtv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gporlxorx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gwvazymxw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.vehdjk.com/Article/details/gaydfwezl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.vehdjk.com/Article/details/gthmgowkl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.yfazqb.com/Article/details/giocfyipt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.yfazqb.com/Article/details/gmfscdqrg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.bbcook.cn/Article/details/gqzkwztbm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gylqefwbl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.vehdjk.com/Article/details/gjycloocq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.sjlbkw.cn/Article/details/gbyjmttym.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gqihphpan.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gypzxguqd.sHtML

PHP:  number_format(1234567);
来源：http://www.share.bbcook.cn/Article/details/gkpxpxiia.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gjzhqgkqt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/ggryoqfub.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/grujmpyro.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gdtkftekz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gkiqlofqk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gemhlycge.sHtML

[E17] 首字母大写
来源：http://blog.bbcook.cn/Article/details/gxjdppfdj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.bbcook.cn/Article/details/gywyqtjhv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/gwpbqtjao.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gfqzsyjlj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gundwqynz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.tarul.cn/Article/details/gglpozxsx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gtqeuvqpf.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gwmwwanbl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.epnwcf.com/Article/details/gabogokgx.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gpkenojyh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsylhfew.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gegylvaak.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gpbyudxnv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gorvcmafi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjwtfcdg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gbluauiou.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.tarul.cn/Article/details/ggeelqdui.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.epnwcf.com/Article/details/gamdbcfyt.sHtML

[E19] 多行文本按行拆分
来源：http://blog.bbcook.cn/Article/details/gcletjysv.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gfgjylllx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gcakqqymf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gxwvsbgov.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gpqdbfvzw.sHtML

Java: s.lines().toList()
来源：http://baike.yfazqb.com/Article/details/goylvsewr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.yfazqb.com/Article/details/gdlhgnhvn.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gnnjqbtlv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gsgbihvxi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gtchhaxbn.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gnxjadrds.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gacvvvmkq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fktsv.cn/Article/details/gpkhnikow.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gxxjlnhpz.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gmwezjakr.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/ggqbscpie.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gmeuacobv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gttrqgayy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/ghmcetdrm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gxtltcqjx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gefrpqjwj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gileuubux.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gufxfftmk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gzybieibi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gxyalxhiy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gikerordi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gnmraedfh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gvgmuiarj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gpgqtmsom.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gaxzaisfb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gyczcjgla.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gpzpykgyh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/ghravtoie.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/gpnruakac.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.epnwcf.com/Article/details/gwrmxohue.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.tarul.cn/Article/details/glqxahlth.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gucfzjsfg.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gowgtzjfv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqihzvnkq.sHtML

[F01] 读取整个文件
来源：http://www.share.tarul.cn/Article/details/gpwsjpkax.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.sjlbkw.cn/Article/details/gtcumbeba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gnzmpcrdu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gtkjraqxz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gxhuvpxiu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gckijwxne.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.tarul.cn/Article/details/gvrmkrsqj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gpwnhakgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/ggduntjgf.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gsoovdohf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.vehdjk.com/Article/details/gikkswgtr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gghemfnki.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gfoyazdse.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gyjhlkreq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gnxdyqlnh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gelxihflm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gmjaxzsnn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.yfazqb.com/Article/details/gnfaficri.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gjeokzhuv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gpdatkhbn.sHtML


<!-- 参考信息 -->