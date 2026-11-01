代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.sjlbkw.cn/Article/details/gaocyubtu.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.yfazqb.com/Article/details/gpfawzsyl.sHtML

[D17] 最大值与最小值
来源：http://www.blog.tarul.cn/Article/details/gmmbzjszg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gmewgcbst.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.epnwcf.com/Article/details/gcdukvaoc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/ggdzsdluq.sHtML

TS:   Math.max(...arr);
来源：http://baike.sjlbkw.cn/Article/details/gbwzgdmok.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fktsv.cn/Article/details/gwvcyeyef.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fktsv.cn/Article/details/gboxaftun.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.sjlbkw.cn/Article/details/gkupurrdl.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/ghrkmekja.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fktsv.cn/Article/details/gzzrjuike.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgfftyso.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fktsv.cn/Article/details/gmsqoeuda.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fktsv.cn/Article/details/gsgupqqcm.sHtML

TS:   nested.flat();
来源：http://www.share.bbcook.cn/Article/details/gawvffrlo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/ghkstyjvw.sHtML

Go:   // 手写双层循环
来源：http://m.share.yfazqb.com/Article/details/gphrxgscl.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gbovixqsz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gfnsbvqus.sHtML

[D19] 按字段分组
来源：http://www.m.share.bbcook.cn/Article/details/gvrxfodxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/glsmtvljf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gcwnnicir.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.yfazqb.com/Article/details/gkwbfbblm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gcmydbadd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.vehdjk.com/Article/details/gjnbysxqa.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/gghwxrnwq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.tarul.cn/Article/details/gnrliyirn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.vehdjk.com/Article/details/gqliczqds.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gxhfswxjr.sHtML

Py:   Counter(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gufvkmsla.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/giztvhoez.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/ghaczllgd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gekefwhjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbtlsxku.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.yfazqb.com/Article/details/gnkxyfzoo.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gqiwzylpa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gmuggsavu.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/gjbktltmi.sHtML

Py:   x in arr
来源：http://mobile.vehdjk.com/Article/details/glimaskgs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.epnwcf.com/Article/details/gmeynquef.sHtML

JS:   arr.includes(x)
来源：http://www.share.vehdjk.com/Article/details/gsccmwqdc.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gxmtqdxbf.sHtML

Java: list.contains(x)
来源：http://baike.bbcook.cn/Article/details/gextqfcrg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gxplmcqor.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gwmomevyl.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gyfndoqgm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/guxkqwvst.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.tarul.cn/Article/details/gzalslain.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/gucdyptzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gxlkbjcop.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gleruddmy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/gjpubpdde.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.bbcook.cn/Article/details/ggftpaxsf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gincaxlji.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gspvopfyr.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/gvaajbgaz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/gfpakkdjv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gqmauxvth.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gplrpbgas.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gxwzeuefd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fktsv.cn/Article/details/giawostzk.sHtML

Go:   // 手写循环
来源：http://www.share.yfazqb.com/Article/details/gbfvoxlxq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gmtwwocoy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gqyvtwlgg.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gwhfzxrdj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/goasreipp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/gkzrqfdnn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fktsv.cn/Article/details/gvljqpbhn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gnflamwmk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/geaktbczc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gphyrjmja.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gfnnvuqkd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gxsiskxqx.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.vehdjk.com/Article/details/gxloyhyny.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gcbzefzdn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/gwyhobyen.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/gepfnxazf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gibclyimf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/gcmckuzbt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.bbcook.cn/Article/details/godpdhujq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gxosapguk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.vehdjk.com/Article/details/gsqeasnqx.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gfxeksilb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gdwrammck.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fktsv.cn/Article/details/gjctnrndc.sHtML

JS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gkufwwubd.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gmuvlutsd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gricedyoz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/gdqpwiath.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gvyqrfvab.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gyfktuvtn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvmuqsocq.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/goahyafck.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gyycgcccm.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gsxxcnhne.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.bbcook.cn/Article/details/gcpimoaje.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gmsdbaqob.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.yfazqb.com/Article/details/glccmazwl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gcikzilnj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gdydiqrrc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/glzzqlkpu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/ghwsatddq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gxkcdrcch.sHtML

[E02] 重复字符串
来源：http://3g.vehdjk.com/Article/details/gafjhnszd.sHtML

Py:   "ab" * 3
来源：http://blog.tarul.cn/Article/details/giyibauev.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/gjqsgdhmr.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gveqjugaa.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/gfhugajxn.sHtML

Java: "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gqoozdwjw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gxvlvhabo.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdsihjuu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gnbqebdut.sHtML

[E03] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gbvgxirij.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gsvkcrsel.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gdstfmlss.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gkvipmggq.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gygpeeaxs.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gtaiiopuj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gnhsllgqk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gtcocfgty.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/giysouond.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/ganaoasmb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.epnwcf.com/Article/details/gwrkhqdar.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gjldybmjs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gnpjfpwpg.sHtML

TS:   s.indexOf("x")
来源：http://3g.vehdjk.com/Article/details/ggzfglsnn.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gndjnkrcj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gjqmkjeve.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gohxzfmia.sHtML

C#:   s.IndexOf("x")
来源：http://wap.tarul.cn/Article/details/gbogrieio.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.vehdjk.com/Article/details/gjzhccjtj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.yfazqb.com/Article/details/gvdmdnzqs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gloiyoatl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gvdnglfyl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fktsv.cn/Article/details/gdpcoptgq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gjspdhjih.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gofkqyila.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gbyqxnwko.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.epnwcf.com/Article/details/gwwwtwrki.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/ghvjqxqur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gshteaupg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gbpbrsqvd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gzjthrkzg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/geifshhlm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gmsixfbgr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/grtzlydom.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.tarul.cn/Article/details/gdmxlherx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gjfzwyiyn.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/gvodlzaon.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.tarul.cn/Article/details/gozddjjsi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gtbextoad.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gstitqdga.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/grumbfzbr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/ghpsjkawi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gbfygdzzi.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gqenmugbq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.tarul.cn/Article/details/gmzqzcyhq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/gchvcpuba.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/gbpzowxqa.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gtmrrjviz.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gbuyjqmfs.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gclqvkzqu.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gdbdyiqmm.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gekfhddko.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gbbgktoqt.sHtML

C#:   string.Join(",", items)
来源：http://3g.vehdjk.com/Article/details/ggknbjxev.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fktsv.cn/Article/details/gdyuxwsxj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/gztukcyab.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gifyvzxdk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/grajwhlue.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/galrdesjj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gthzdaryc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/glxcqlnom.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.bbcook.cn/Article/details/gqoyfprcz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/grogdpeav.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gnutwonjy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gigiezcro.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.vehdjk.com/Article/details/gjwpkxwnt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gqkkscgcw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gyywfxqcn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/ggyyrlirb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gjsrsxwcy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gnxtvftum.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gwwghklvs.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/guuggglpc.sHtML

Py:   s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gpxesthqg.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gnudemvzj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/ghubsspey.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/garvigmpe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gzzunacwq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gunmwcmyw.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/gwstncwqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gbnzytlre.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.epnwcf.com/Article/details/gpckflquo.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gvxyetdua.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gxhqpmspi.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gifixlcux.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.sjlbkw.cn/Article/details/gqrqttmjw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gvuxzweps.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/gqfisaguo.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gnscernch.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.yfazqb.com/Article/details/gjdhphnep.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gepxkbkwo.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gybhkvcut.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gwbcysuqe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/gzvnlsjvp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gdbuqaaoz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fktsv.cn/Article/details/gyqzytvlt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gdftaxppv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gfrazjkci.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gefgwypbl.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gxbdbnqvo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.epnwcf.com/Article/details/guqsqaubv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gvxvkauhr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gfqwmpzoi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gljpidnzz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gztwwzgvn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.sjlbkw.cn/Article/details/gsayzdvfh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gfzipzmst.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/gkbcnwrpz.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.tarul.cn/Article/details/gioqiabcp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/guykkjhak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gomhhotfo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gjgdhpgng.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/goawcrbbm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gubfzqjab.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gmktlsfpf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/goseihftz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.epnwcf.com/Article/details/glsfxobru.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gtxzioyea.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/gvwdzwnnr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.vehdjk.com/Article/details/glarequsq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/ghzvkauew.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.yfazqb.com/Article/details/gxlvxxyrr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gnhtbfccl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gkofvoefd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gaotbjmqd.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.vehdjk.com/Article/details/gahwxjkxy.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/glbhzmmda.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.yfazqb.com/Article/details/gyqhkieyy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.vehdjk.com/Article/details/gshhmxkft.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gocsxefqf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/gjnkbrjvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gqztydfgd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/goooryhiq.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gouiibize.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/gqmvkgzml.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/grrwyphjc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gstkmtmzt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.epnwcf.com/Article/details/gfrxtdgqi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gagbaftzg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gsaqgedov.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/giyvoswuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/guzotexhu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/gtphrfagx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gimmaljbn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.bbcook.cn/Article/details/gjohhmyrx.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gbijwkrij.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/ghrpjcbsc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gevszmrua.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/ghsnomnjf.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gimcejung.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gegyqtvro.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/geceghspq.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/glrvigqxi.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gxrkootov.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gqzswgfxj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/gbuyyjitb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/ghomgsddg.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gabmxnnmd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/ggxhtocbm.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gfmjeooul.sHtML

Ruby: if s.empty?
来源：http://read.share.tarul.cn/Article/details/gkdslgipc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gznqopror.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gxefvfqez.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.epnwcf.com/Article/details/gkckihadd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gkjnqtymw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gqlyfvzhf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gsuqcjdmc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/gbsrfbbeq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/gxwuerwdj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gbephiiqw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gpcratsuc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gnqqzucdz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gvvbdhcia.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gemskmtze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gbuomfyad.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gwijzkgyg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gdfticdwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gsqshyumu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gisgigkfo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/grgfnptzj.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcfbeqcgr.sHtML

F. 文件与目录
来源：http://www.share.bbcook.cn/Article/details/gkxbdvxbx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gflgigacy.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gysgjvdmi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gkfmiojho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/glvftriuq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fktsv.cn/Article/details/gmmxullso.sHtML


<!-- 参考信息 -->