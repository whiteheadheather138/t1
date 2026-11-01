代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gylxhggmr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.vehdjk.com/Article/details/gwpiriphh.sHtML

[D17] 最大值与最小值
来源：http://blog.fktsv.cn/Article/details/gylmufrtu.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.bbcook.cn/Article/details/glkcfcmsc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/gpqdxnioa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fktsv.cn/Article/details/gzzfdnrit.sHtML

TS:   Math.max(...arr);
来源：http://3g.bbcook.cn/Article/details/gxmscadhl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.vehdjk.com/Article/details/gvawwgmkb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/goypukpjg.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.yfazqb.com/Article/details/gwqizjlgo.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.bbcook.cn/Article/details/ghialftic.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.bbcook.cn/Article/details/gadhdfwbx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.bbcook.cn/Article/details/guytojgth.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.bbcook.cn/Article/details/gpuvtemrj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fktsv.cn/Article/details/gvkrlxwhr.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/gbnxugpfs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gvbgircul.sHtML

Go:   // 手写双层循环
来源：http://www.blog.vehdjk.com/Article/details/gmlctlljb.sHtML

Ruby: nested.flatten
来源：http://3g.fktsv.cn/Article/details/gvzfmcgml.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fktsv.cn/Article/details/gdwrsnybv.sHtML

[D19] 按字段分组
来源：http://www.blog.sjlbkw.cn/Article/details/gaikdprbh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.tarul.cn/Article/details/gpuittmvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.yfazqb.com/Article/details/gwkdvhujw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/godqzunqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gczhinrfy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.vehdjk.com/Article/details/gcmewnzhu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.sjlbkw.cn/Article/details/gaynqrsic.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gwkhqnfqh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.bbcook.cn/Article/details/gtteuvwhu.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.vehdjk.com/Article/details/gvffupfng.sHtML

Py:   Counter(arr)
来源：http://wap.bbcook.cn/Article/details/gkacqqgyc.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.tarul.cn/Article/details/gvglxfrdb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gvcjslkyb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/ghrmjyycr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gdwvqmvza.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/gpbmrvymb.sHtML

Ruby: arr.tally
来源：http://wap.fktsv.cn/Article/details/gqgvbqavx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.vehdjk.com/Article/details/gwwzghybv.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/gnzbmmmja.sHtML

Py:   x in arr
来源：http://blog.bbcook.cn/Article/details/ggurynrng.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.tarul.cn/Article/details/gwtlqdmqd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/gwovwnrsq.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gniluzupv.sHtML

Java: list.contains(x)
来源：http://3g.epnwcf.com/Article/details/gqgcjcjvc.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/ghstbcznj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/grfvjhsdm.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gxyvmsazu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gzfuqixth.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gfmtozrnu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.epnwcf.com/Article/details/guhfwaaev.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/grxdvlymm.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gurrjwbme.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gfquixbvw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gdxwyanlx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/ghkfgyxzt.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gcicxbqtg.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/geistdnam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gnpxwhggu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gvbjjnvba.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gvxkohugt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.epnwcf.com/Article/details/gnxvbmeas.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/glytpkvxl.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/ggscilhki.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.tarul.cn/Article/details/gtwfpqhfz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gcooambrk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/glhizoudu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gbgpebxqd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gtwndsbwm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/ghimqlsoq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/gaimrsdng.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/gdqmrzufu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.sjlbkw.cn/Article/details/gzwokpwhf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gljgtrilx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/govfzqlvb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/gjbihjyck.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gditmymwn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/gnybvgqsw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/gyzcrnteo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gtzjopldg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gftmxgovl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gvpfkrxju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.sjlbkw.cn/Article/details/gqcsksyoq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.tarul.cn/Article/details/gbeftnpsh.sHtML

[D26] 数组转字符串
来源：http://www.share.vehdjk.com/Article/details/gtrwxttvh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gnajwkiei.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/giwhsxucl.sHtML

JS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/grkzmowqs.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gamtmlfyi.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjntfmyct.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gwiehbida.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gndkiyhoe.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.tarul.cn/Article/details/gixpdkldv.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghtrchbic.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/gfhswuooo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmjhpwfjh.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/ghsiigcey.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.vehdjk.com/Article/details/gdspfrzew.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gjjzwkdfs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/grqvofkff.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/grbrbvlec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.epnwcf.com/Article/details/gnjhhkoqr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.epnwcf.com/Article/details/gckstdxzr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/guvbdgvpa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gmknzqros.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gcnnurbvj.sHtML

Py:   "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gomfofddl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.vehdjk.com/Article/details/gawgrwcbr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/giabfgwzw.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gqgprxrxl.sHtML

Java: "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gcedavsmq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.bbcook.cn/Article/details/gjfudammj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gyyzpxecd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gsncmlgsl.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gtgtwzrjx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gkhrjonvr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gpehyanes.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gpcdamtff.sHtML

TS:   s.slice(1, 4)
来源：http://blog.yfazqb.com/Article/details/grxqvggzw.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gtbgifyfr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/glhtnemwy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gfouqkfab.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gvwmhjgaq.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gpfuxavvl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gifsfgnal.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/gciyxchzh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.tarul.cn/Article/details/gplnccvad.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gyhtegpxh.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gywbfvsvn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.sjlbkw.cn/Article/details/guuxhancz.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/guxkkpxaw.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gmgrgggwn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.tarul.cn/Article/details/gnnmlzjrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.bbcook.cn/Article/details/gqexzjxup.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/gwxmeqack.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gnlrirvpe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.sjlbkw.cn/Article/details/gyecptmlc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gzrmollkr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gqftkjvew.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.sjlbkw.cn/Article/details/gaolonxgh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlliuddz.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gvpklcpyf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gypbuezrs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/geatlpelz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gwqxawnrv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gtuhmfbwt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gbdeepkhi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gareurwvr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/ggantrvdd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ggfbazdvs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gnslzxfye.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gnxnhsspn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gfhtnnzda.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.yfazqb.com/Article/details/glhdltuuo.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gdxvfhhxx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gfrjwlmqz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gwymalykp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gcmjuwuas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.vehdjk.com/Article/details/gscobmeau.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.vehdjk.com/Article/details/gqwuwyovr.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gikahgqnp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/ganegpdyb.sHtML

JS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwssnpuqn.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gvbfwlsom.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gklnvrvuc.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gjwwittns.sHtML

Ruby: items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gynqyduzj.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gmialnzmv.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gukslwcew.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gdfpkvxuk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.vehdjk.com/Article/details/gcstdgovg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gvduidvya.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gnqtjgzty.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.tarul.cn/Article/details/gxycfypwn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gqdofkicv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gqixkpwki.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gdfwealoi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/geynqnhbi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.bbcook.cn/Article/details/gcprynhxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gknicslpe.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.epnwcf.com/Article/details/gwihhuvhz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gfhkwyxrd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gdjguabit.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/ggzbtmccj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gpmdvnqen.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.epnwcf.com/Article/details/gqlctnflc.sHtML

[E11] 反转字符串
来源：http://3g.vehdjk.com/Article/details/gsyysqrup.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gcqfkwyzy.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/giockqmti.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/giqokmwkc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gyyvxpylq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.tarul.cn/Article/details/gibfobtsi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gwydoahud.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/ghqhmznuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gjzwdbgex.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/gettlwauz.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gpvtyoali.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.vehdjk.com/Article/details/gsqknkbfu.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gonbaotpc.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/ggvzprjco.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gcibtogxy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gqkbjpvda.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gjzzpydsp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/ghkrxfqdh.sHtML

[E13] 逐字符遍历
来源：http://wap.tarul.cn/Article/details/gscghabnt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.epnwcf.com/Article/details/gyfiejgfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gqzbxcgpt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/ghamkdklr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gtxuliiqj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gkmtotzof.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/gzuuhjfbf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.yfazqb.com/Article/details/gjzkqltaj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gcdxhvuwx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.sjlbkw.cn/Article/details/gfpuvtqrk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fktsv.cn/Article/details/gcmkgshuo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuqvctmk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/ggjefjqbi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gutvpfpql.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gwvuatvsh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/goflbuyoi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gknankvgl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gymtjeszs.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gzlecpgzx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gcyxoxgmf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/gjmebsjbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/ggtnzawbn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.sjlbkw.cn/Article/details/gsmqzmcbx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gmovodzoo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/giabzazwq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.yfazqb.com/Article/details/ggpbiffir.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gjixelgfz.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gemtnhlfi.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gxjvlvhsc.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/ggtcdpbzg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gjnkipfyf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gdcbreukd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/ggrgametv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gdjtzskes.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/ggtceingx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/garlbtwoe.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gvfnuefij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.vehdjk.com/Article/details/gmzqtsrgu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gsfkfdsvq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.tarul.cn/Article/details/gyrpbfouv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gyeebxhll.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gefbojbvd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/gybqqfofi.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gfnbajkmp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gqphohdqy.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gaeouupcz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.yfazqb.com/Article/details/gcxhtdbgc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gsjgbojcc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gwkkncqju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gpzyaluje.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gazszvzeb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gvybreblj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtolnyifj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.yfazqb.com/Article/details/gonmigczv.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/ghngxgpcd.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gseiokqxr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gerxystrb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gcedrtgwc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gflcfblzh.sHtML

Java: s.lines().toList()
来源：http://www.blog.yfazqb.com/Article/details/gucsewxsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.epnwcf.com/Article/details/gsfkhgsif.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gemywxdhw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/ggietvpvw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.bbcook.cn/Article/details/gnbhpkbot.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/geubrdecf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gepiyzsin.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gfxrjsixp.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gnutypure.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gkgvmmytw.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gqgnebupw.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gevytvxog.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gfmexdruy.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gdmczvgqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/ghsxsafjj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gvidmgqte.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gneztoulf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gowmjovuv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gvhqpmxwd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/gzutadlzb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gyipqjlxp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.epnwcf.com/Article/details/guczxkapt.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.epnwcf.com/Article/details/gitqcpnlp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/gnzguszxf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gvlrbwmob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gfcbauqjw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gssogujhr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gfcjkdddu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gzeoeximl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gjlrboauf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/ggewzvbev.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gqsmfyjfw.sHtML

F. 文件与目录
来源：http://blog.tarul.cn/Article/details/gaakokies.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/galpedvqg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fktsv.cn/Article/details/gnonexbjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gmkbssoea.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gfncvgupb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.bbcook.cn/Article/details/gskrzstxv.sHtML


<!-- 参考信息 -->