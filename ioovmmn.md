代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fktsv.cn/Article/details/gnbmpcygs.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.tarul.cn/Article/details/grdhoqhty.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gctejhdoy.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gnmzavezu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.tarul.cn/Article/details/gpwhbjzpp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.sjlbkw.cn/Article/details/gsmgwctcn.sHtML

TS:   Math.max(...arr);
来源：http://www.share.sjlbkw.cn/Article/details/gwgwxxutj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gsjoslouf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gylftietk.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.tarul.cn/Article/details/giyptczpr.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.sjlbkw.cn/Article/details/gertcmqfp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.yfazqb.com/Article/details/gwkskbqbs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.sjlbkw.cn/Article/details/gaiibbtjl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gmriwovra.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.tarul.cn/Article/details/gkavvpppm.sHtML

TS:   nested.flat();
来源：http://wap.epnwcf.com/Article/details/geskbuecy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.sjlbkw.cn/Article/details/ghdokokkh.sHtML

Go:   // 手写双层循环
来源：http://3g.fktsv.cn/Article/details/gjwxlsmni.sHtML

Ruby: nested.flatten
来源：http://blog.vehdjk.com/Article/details/ggzfpxsdr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.tarul.cn/Article/details/gfipausso.sHtML

[D19] 按字段分组
来源：http://mobile.sjlbkw.cn/Article/details/ggfifkvne.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.yfazqb.com/Article/details/gbvzetvih.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/grdlhkgue.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fktsv.cn/Article/details/gaskxazpw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.vehdjk.com/Article/details/gogrvmvsy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gnbqmufle.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gfunzrgrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/gznimrupd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fktsv.cn/Article/details/gbtgbeuji.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gujiacknk.sHtML

Py:   Counter(arr)
来源：http://blog.bbcook.cn/Article/details/gidemrbek.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/ghucecbro.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/ggregupve.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gawoowqcl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gwftnrygs.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gykbsjalo.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gnuqlslmq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fktsv.cn/Article/details/gebseknjc.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/geyqjuolt.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/givqqhney.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gwwhekvet.sHtML

JS:   arr.includes(x)
来源：http://www.share.bbcook.cn/Article/details/gusslixvk.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gitjnhqnd.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gesnuarfg.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/glcsbaprx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gbnfsckhl.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/gzvuugqji.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.tarul.cn/Article/details/gjbecxiij.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/gszrijwwd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.yfazqb.com/Article/details/gvcncozvj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fktsv.cn/Article/details/gmknjvpyn.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gikqmzivp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gnwxmzyby.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gzzvsgvxn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/gxgnkisfg.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/grrbaxsxq.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gyqbrveov.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fktsv.cn/Article/details/gcbhhyjmf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gcuacwavv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gonhmhkdy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/groavpjfa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gklecndju.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gzfcnewil.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.epnwcf.com/Article/details/gwupulwfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/ggxsceejv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gkbydiecq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.tarul.cn/Article/details/gfevcnhio.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gkdjrwaxa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/gxsasqpys.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gpgwaotfw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/grivespse.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/govnysijr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gnjyosxhn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gxxclwwdh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/ghyvdacae.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.sjlbkw.cn/Article/details/gbhjyedio.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gnbzsxsnj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.vehdjk.com/Article/details/ghltbmngt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gvsbjbylm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gbknuhfzf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gdvgbcybd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fktsv.cn/Article/details/gwqyxnfiw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gkstrihpe.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gxcbmihru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/gbbnykehp.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/gctaocupf.sHtML

JS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gqmgdnhwr.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gyeaftewl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/gobmfefev.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gzsbdzvuo.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gjavzpdon.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/giytqhfee.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gjlmdycqt.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/ghenbzhkc.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gjpjfpxoz.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gspnoqtsq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/ggyrvgece.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gqiemelph.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/grjswxbun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gznanhfym.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.vehdjk.com/Article/details/gjamlpdwv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gykznsbev.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gebnhbwwl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gegacpbas.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gycmrbbta.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gmfgledeb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gfhaoywrp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gmlapmwfn.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gkblzkyir.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gkvputdqu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.vehdjk.com/Article/details/ghvgjjmhu.sHtML

Ruby: "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/ggdhctfft.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gdeultqub.sHtML

[E03] 截取子串
来源：http://blog.tarul.cn/Article/details/gbliinuef.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.yfazqb.com/Article/details/gtnizwrcq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gipfggesu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/grgxczetr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gyousspcc.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gdcnardhc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/gjjrlpvyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.bbcook.cn/Article/details/grwtlqice.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.bbcook.cn/Article/details/gycmsymht.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/ghxyqjkgt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gcvmymtis.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.sjlbkw.cn/Article/details/gowcvnrax.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.epnwcf.com/Article/details/gtkxlmkzo.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gguxkcdrn.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/goegpolnc.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gipudqydm.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gnnmbgbfy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gphsgvipp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gaijhzhlb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gbuvwexel.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/gtdkrrwhl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gzkfzjvoa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fktsv.cn/Article/details/gngmmmzgr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/ghulqkgou.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gsamnxbvw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgicrsvp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxjtebspn.sHtML

[E06] 替换子串
来源：http://m.share.tarul.cn/Article/details/gljjrheld.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/glpmsvxmx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gzkcjiqpq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gmnohxcwx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gswjzfqxw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gsdnzrufd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gxunmomxt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gvzlpgnvx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gwvjqsvad.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gzmpfswus.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gclmtllwl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gkqedtcmt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gklcbksst.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gqryderof.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gqnwtmavo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.bbcook.cn/Article/details/gqpbrrqfh.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gqfmvcjaj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gpyfzhpcy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gkcjemobj.sHtML

Py:   ",".join(items)
来源：http://www.m.share.tarul.cn/Article/details/gfwmjwpxe.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gthhxblfd.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gpjvqyrzi.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/ggniblzkj.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gykaogaln.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.bbcook.cn/Article/details/gclruhllw.sHtML

Ruby: items.join(",")
来源：http://blog.fktsv.cn/Article/details/glnasdmuz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gkukurdlh.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/geptzpqec.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gkpajwpnw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.tarul.cn/Article/details/gbbqffbwp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gbgxfxbhc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gipjeshdq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.bbcook.cn/Article/details/gkdbevbob.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/govavxqbr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gzvdpazow.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fktsv.cn/Article/details/geduoupiz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.bbcook.cn/Article/details/gxwaoajol.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gbvdseuoi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gqdacqrmf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/geprcdpfd.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gjboqjdqc.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gqmoncgzh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gfigoafeb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gaejutvmi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gavnbjvhv.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/gkjlpeygn.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gtprpoujx.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gjhagpvnv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/grjwlfhtd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gleehiwie.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.yfazqb.com/Article/details/gxakfmamc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gxkxaeapj.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gxtjehqrv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gfynpwecc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gztdikheb.sHtML

Py:   s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gixiodurv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gbrabqfrf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/grabyqbix.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gnefejqas.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gxfdhxcqt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gtdqsevfx.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/guopjgyae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gebqwutqw.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gfjdjozyp.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gvoutmivm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/ghvogmxtv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gzfzoyywo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gdaewyzoc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/gntdxxrzn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.vehdjk.com/Article/details/gcfyatzjf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gisqagrtz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.tarul.cn/Article/details/ginejiibx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/givgrtfkf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/gmhgtddcq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gfaxwhknj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/goznkewwl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/gaagfpzfi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gnofblztw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gunbaqyfm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gjambvkhs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gnctpamhu.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.yfazqb.com/Article/details/gnhyctwcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gsxommnxv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.bbcook.cn/Article/details/gfsysqztj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlmuhtkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.sjlbkw.cn/Article/details/gvlkqmngf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gaykshfzm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gjtncohxn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gkrkaqcqk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.tarul.cn/Article/details/gwdyjzdae.sHtML

[E16] 数字千分位
来源：http://3g.epnwcf.com/Article/details/gueqwhkdp.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gjjfyamgn.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gxefzyapd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/ghviedfob.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.sjlbkw.cn/Article/details/gnwvovsiz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gqrbqjlis.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.yfazqb.com/Article/details/gdkxvnuep.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gqozabpil.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gmqfsxyqk.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gszztldfr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrbnipqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.yfazqb.com/Article/details/gminhfbrb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnynrdwch.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gdirzgsgk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/glibtcucf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gdtunbbxg.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gpubdowsn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gxrivbhtz.sHtML

[E18] 模板占位符替换
来源：http://read.share.bbcook.cn/Article/details/gnmdlyire.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.tarul.cn/Article/details/gmvpvqhdp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/grbwmdiqx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/geoagjabp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gdwiystqz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gnqxcbdyc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.tarul.cn/Article/details/gwxguktky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/giekcxaqm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gvcfygntt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.epnwcf.com/Article/details/gcvcktxtt.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gmrtifnut.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gokieydqn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gyhaopwgn.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gutaczdkg.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gdncypook.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/giodravnc.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gtsqtgtdq.sHtML

C#:   s.Split('\n')
来源：http://read.share.fktsv.cn/Article/details/gdpeeqaod.sHtML

[E20] 判断字符串是否为空
来源：http://blog.epnwcf.com/Article/details/gberxoapr.sHtML

Py:   if not s:
来源：http://3g.fktsv.cn/Article/details/gfkkdryks.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gfppgjeem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gcytycjgu.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/ghzmuctzt.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gwirybrtn.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gielnaorw.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/glcoslobt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gapewpajh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/guyuobyft.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.sjlbkw.cn/Article/details/gmhjblxqm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gyagahiaz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gkuaswzhj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/giuofeqiz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gvwpmyfwa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gkjkphnpl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gfeweuxah.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gwliplydj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/gaeojciir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.sjlbkw.cn/Article/details/gaupekxrb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gzapfrtgz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gowutzufr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gqepljrmy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gnzvcqwvh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gdhkppfbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gazmzqkpp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.epnwcf.com/Article/details/gkwjwqhqb.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grwkmdfdx.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/gjocfgodg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/giwrogxxh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gqdkorhis.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gczmtmqel.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gaswsnqxc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/ghrbijpyf.sHtML


<!-- 参考信息 -->