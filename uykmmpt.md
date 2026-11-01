代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://3g.epnwcf.com/Article/details/gqwdiuywg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gjvrnvgcr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.sjlbkw.cn/Article/details/grhczjxgj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.yfazqb.com/Article/details/gkrihqlwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.bbcook.cn/Article/details/gdbnmiihv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.bbcook.cn/Article/details/gsxmcayls.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fktsv.cn/Article/details/gddnihhny.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.vehdjk.com/Article/details/gshinsozy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gwmhxttkz.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.yfazqb.com/Article/details/gvtvjmkza.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gzpuvxdgx.sHtML

TS:   nested.flat();
来源：http://baike.bbcook.cn/Article/details/glxlzqqqs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/gszixyrhc.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gjuidphkt.sHtML

Ruby: nested.flatten
来源：http://read.share.sjlbkw.cn/Article/details/gpdslrpyi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.vehdjk.com/Article/details/gsuhgcega.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/gxdjiwnak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/gpnqbcluz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gtyxskteg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gakermdzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.vehdjk.com/Article/details/gjybhcizm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/goptbozvf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.epnwcf.com/Article/details/gpxapilxx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.yfazqb.com/Article/details/gjboifqka.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/ghqhxhxtt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gxciblbfp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/grnajomje.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gcbxxmhwk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gmhgxzdyf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gkgrwfcpe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.yfazqb.com/Article/details/gkwxzvlqf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gocmoiljr.sHtML

Ruby: arr.tally
来源：http://www.blog.fktsv.cn/Article/details/gbnqixrpr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gkxvrogve.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gjfejfmbp.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/gmnzhtqer.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.vehdjk.com/Article/details/gksvrqqax.sHtML

JS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gztmuzeif.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gvgzealww.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gauxdrouu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gvwpwvogn.sHtML

Ruby: arr.include?(x)
来源：http://3g.vehdjk.com/Article/details/gqzsnidtz.sHtML

C#:   list.Contains(x)
来源：http://m.share.tarul.cn/Article/details/gkigwfopa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.bbcook.cn/Article/details/gxmxxdtto.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/gdmggjjfr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gjfnbfjia.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gvuihverx.sHtML

TS:   [...arr];
来源：http://mobile.tarul.cn/Article/details/gulbpsegv.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gxywlcvwv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/guczoogzx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/glezhplqe.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/gzqlmmgrp.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/grptmfrqz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gehcgciym.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gosbjiloz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/giblcntgq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gcrdkaobc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gddxsdbwa.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gweduirsy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gwvtulbxu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/gszuthwzh.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/givpqzrgs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gpzghuhuu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gfbgewhwh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/gnxpgwbjc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gcnprdamb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gbilgarfz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gqjlwbxga.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.yfazqb.com/Article/details/gsmqsrlwy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/gemihlpkv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gcvclmuww.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/giytbinxy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gyurgrbac.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gbghjcdwc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.sjlbkw.cn/Article/details/gqtbvivmd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/grdwfjxap.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gglmywzzv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/gtftwypeq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.bbcook.cn/Article/details/gqlatfnub.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gjzclmfgd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gurutshfm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gpocuvrtq.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gvfdimycf.sHtML

TS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/gmymnfmkl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gzjxydkgl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/guiugqfsf.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gfkchlrpt.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/goyptyasp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbhznlyuh.sHtML

E. 字符串处理
来源：http://read.share.fktsv.cn/Article/details/gtksrrvem.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giwufhjxw.sHtML

[E01] 拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gzbomotly.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/ghcwidqev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gtaadulmx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/ghzxszlcb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gvtkwltrk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gzxoaefev.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/ggswiqvvg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/gaqxubbgz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.bbcook.cn/Article/details/gohcaykkq.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gvpzomkvh.sHtML

Py:   "ab" * 3
来源：http://wap.epnwcf.com/Article/details/gsfgpwhgo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gswhiyxqp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gagghxefp.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gxfjepstu.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gxjrivqzh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gfaoadhzh.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gnfduocud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.sjlbkw.cn/Article/details/gmqpicaoo.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gxyibaxxl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/guwcwmbob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gwfhlmcqt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gjuzxxcem.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gvsgbedru.sHtML

Java: s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gmwzcahvi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/govpmnqqt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.vehdjk.com/Article/details/geoomgspu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gctlparbi.sHtML

[E04] 查找子串位置
来源：http://blog.vehdjk.com/Article/details/gphldeeds.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/ggqhcskfi.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.bbcook.cn/Article/details/grhmoxdri.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/giyjsscyo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gyfnupnyb.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gfaheiquq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/ggydrdidi.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/ggtdntrfe.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gxmhhkdoh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gvlyuycri.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/gbzrurdgh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gbzwotedk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/geapocdin.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gmyedyitu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gjhlpjtdv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fktsv.cn/Article/details/gyzchibjm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gksckjmgf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjwaksrz.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/grncbqbgw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/glltaujjr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gfgzdxchc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gibqpavpf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gqtfneuxe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gabrhanxx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/guqakarwx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gcvrongay.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvjqhsuzn.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gomsnlrep.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/glnmewnqx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.epnwcf.com/Article/details/gqtcmemuh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gixrdjtxn.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gkcpsihga.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.bbcook.cn/Article/details/gylsrkhga.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gurkhrpkh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gbvemzjfz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.bbcook.cn/Article/details/gxybnahez.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.tarul.cn/Article/details/gtcnrhrsh.sHtML

Py:   ",".join(items)
来源：http://blog.tarul.cn/Article/details/gobwkpurm.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/gtdoppzvf.sHtML

JS:   items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gpjezancn.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gxgzyasho.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gdnakpous.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/ghvcexupt.sHtML

Ruby: items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gnlrjfimq.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gompmmwbd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gcposmmpt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gddfvugpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.bbcook.cn/Article/details/grolbecps.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gceisfwkd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/giryjassm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gwicwbpki.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gnrmyfdrn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/ggynibetb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gafxuxerq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gocfdnhmm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gsypseing.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fktsv.cn/Article/details/gstbvteqa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gjngibjys.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/glraszgkd.sHtML

Java: String.format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gwgjekojg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gqyflueac.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gzfjqvozy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gejpieiln.sHtML

[E11] 反转字符串
来源：http://3g.sjlbkw.cn/Article/details/gjupszyqz.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gggrlsmtg.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gckhgzihe.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gosskrxbs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gbcxebdxa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gmklccdwq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gtcrcpewt.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gngjxrgym.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gtggjmiio.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gciamnsey.sHtML

Py:   s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gqjvpwour.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gjgjnvlgr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gziwuvfxp.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gdqvfzoqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.bbcook.cn/Article/details/ggjbtkuzi.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gkobyazdk.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gpwejlcwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fktsv.cn/Article/details/gtkyoacsv.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/guncjyeth.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.bbcook.cn/Article/details/gxzdmacwz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.bbcook.cn/Article/details/ggybqzogg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gfmokqmyo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gmrknaawu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/ggtujyocq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.vehdjk.com/Article/details/gpzyjowqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gdgltecij.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fktsv.cn/Article/details/govvybeaf.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gsrnrpzgn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.sjlbkw.cn/Article/details/gjfvwrags.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gkjzzkuwd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/gfiaflpzw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gitftmnrg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gwnwjenro.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gpmacvrek.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/ggvtfjwof.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/grqpnreah.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gdjzyuqjx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/gttrkbxoi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gllsvqcpb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/gkgjwhjiv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/ghyxxjhvo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.yfazqb.com/Article/details/gllfqndgx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gumahsxqb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gavkjexgj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gvaylquma.sHtML

[E16] 数字千分位
来源：http://blog.fktsv.cn/Article/details/gjnehdspa.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fktsv.cn/Article/details/gwpunzfcp.sHtML

PHP:  number_format(1234567);
来源：http://baike.yfazqb.com/Article/details/gsxndxeya.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/gqjhodpqj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gwtezfsgd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gecjgvcrr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gmovklbgz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gtseatotd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.vehdjk.com/Article/details/gspjkmjlr.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gyzryplgi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/ghmnoerqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gtpwfudot.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gzewsrbmf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdrlxbpga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.vehdjk.com/Article/details/gqhvcghid.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.tarul.cn/Article/details/ghwexpatl.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/ggtulscwd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gwtvjisxc.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gxgnvkavd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gtqbayhki.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gfvbyurpl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gkdofjimi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gtemgwyhv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gmebndhfp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gpclauyun.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gibctjuqq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gsminleaw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gwbnhnlbh.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/guhhpxpma.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gcuuustis.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/gdlotfurt.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.epnwcf.com/Article/details/gqzgdebzu.sHtML

Java: s.lines().toList()
来源：http://www.m.share.tarul.cn/Article/details/gfbcvzluv.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.yfazqb.com/Article/details/ghmjvjccp.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/guletjibh.sHtML

C#:   s.Split('\n')
来源：http://baike.bbcook.cn/Article/details/gqtcvvtit.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/grmtyzset.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gdrekfqly.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gyvngcvok.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gaffnzmcs.sHtML

TS:   if (s === "") {}
来源：http://m.share.bbcook.cn/Article/details/glsqhjmza.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gharenakd.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gmfhivkom.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gbhtlknds.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/gnyugcjkc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/ghqlrtntk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gbjmdarjj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gujfsnpak.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/glbjqoovi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gnazubrkb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gxwxirddh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gfnhfwdzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gjxnlhrrd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gdmkyukqx.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/glfwqalei.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/grmvkavgy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/glxdohsbg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gvbdrdxkj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gfsukgghf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/gbfmertqy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gshoiulbn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/grsqkobkn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.bbcook.cn/Article/details/gemyvrpur.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghbiekjak.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gpestzeqd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gagxogerf.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gglnydiht.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/gmhsuwuna.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gtkbkvzak.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/glkunipso.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gtrtnposs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gvdnyrabu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.sjlbkw.cn/Article/details/gfcscrzro.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkpzqhee.sHtML


<!-- 参考信息 -->