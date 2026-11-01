代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/grxyyfmsj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.sjlbkw.cn/Article/details/giqsemblp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.epnwcf.com/Article/details/gnuqnyery.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.bbcook.cn/Article/details/glbaziqdk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.bbcook.cn/Article/details/gojpdrabo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.epnwcf.com/Article/details/gjnhowhpz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.yfazqb.com/Article/details/gawhpfeqq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/gzrhwlfex.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/ghcxzgehz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gyaqrxdrk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.vehdjk.com/Article/details/glexlnwvn.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/gomjntxdf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gjsnwnxpn.sHtML

Go:   // 手写双层循环
来源：http://www.share.sjlbkw.cn/Article/details/gxcvoqgbn.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gfgjtkqju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gbfltaero.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/gobtgzomt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/gszpgpqvw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/gfqwvmeah.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.sjlbkw.cn/Article/details/gznltixai.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/gymlnjhtk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fktsv.cn/Article/details/gqcrvlwic.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gzgllsari.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gangdciek.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gagerfodt.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.sjlbkw.cn/Article/details/goypziuai.sHtML

Py:   Counter(arr)
来源：http://blog.epnwcf.com/Article/details/gjiansrvh.sHtML

PHP:  array_count_values($arr);
来源：http://wap.yfazqb.com/Article/details/gaxvlrpwd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.bbcook.cn/Article/details/gsedrmoao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.vehdjk.com/Article/details/gjkkwpvbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gnjflxjkp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gxauxallx.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gfvyjhdrg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.vehdjk.com/Article/details/gwwposvpc.sHtML

[D21] 判断是否包含某元素
来源：http://blog.bbcook.cn/Article/details/goihqyrsv.sHtML

Py:   x in arr
来源：http://mobile.bbcook.cn/Article/details/gyjqpwoxs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fktsv.cn/Article/details/gtznsujjm.sHtML

JS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/gsjkazbjk.sHtML

TS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gypbjwmth.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gljkkesck.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gxlagrfko.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gixboijpj.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/goqdttwhw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gqiruirrj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gecccrdhi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.vehdjk.com/Article/details/glmwbpmep.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fktsv.cn/Article/details/gimcqqvpn.sHtML

TS:   [...arr];
来源：http://www.blog.vehdjk.com/Article/details/gynnedcbb.sHtML

Java: new ArrayList<>(list);
来源：http://wap.vehdjk.com/Article/details/gabogoowa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/gqlsonmgt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gpahlztcu.sHtML

C#:   new List<int>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gmavczmhv.sHtML

[D23] reduce 累积计算
来源：http://read.share.bbcook.cn/Article/details/gxvlvfroa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/glxabmivg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gacdazcuu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/grrovlgpy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gzgpvkjfc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fktsv.cn/Article/details/gwkzkwcpf.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/gfwrfaeid.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/grkarlxme.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.tarul.cn/Article/details/gqumvcnss.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gpwemdplk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/ggaeykvyo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gkehwfvmb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gaujsldae.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gzaequwmw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gwzrbjsqx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gseliksyw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/givgofsuz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gpkichtwf.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gfjgfncpj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gqaelhmdq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.yfazqb.com/Article/details/ggkujfphc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gmpvmetcw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gmpdxdalx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gygqrkvta.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fktsv.cn/Article/details/gyhwcgsil.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/gsubwroms.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpnlplcpq.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gjqmdxyop.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gdfudbono.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/guhinrbxn.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/grnotxagp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gdzebdvgb.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gqietzwbm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gdxccfewk.sHtML

Ruby: arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gdrexarkw.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gznamdqzq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghfpzxqxv.sHtML

E. 字符串处理
来源：http://mobile.sjlbkw.cn/Article/details/gpnioldln.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gplsqoldt.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwgglyuxw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/galutrlcw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/ghumjviex.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gyeidgkia.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gbkfgdksc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.vehdjk.com/Article/details/gdfvagvax.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gxehkzbfj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gckivqdzq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/grmcluren.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/goauyonld.sHtML

Py:   "ab" * 3
来源：http://blog.fktsv.cn/Article/details/gnmfqvxuj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gagchmmtd.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gfhnddgvd.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gnummpbwk.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gstocelkz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/gwmfetukf.sHtML

Ruby: "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gfbmsukri.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/ghteyftld.sHtML

[E03] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/ggozyxltb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.sjlbkw.cn/Article/details/gytyrbzgu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gwxvtppun.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gecrkkibf.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/geddylnxn.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gcsypczcx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gctppabai.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.sjlbkw.cn/Article/details/gdfahhybt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.tarul.cn/Article/details/glxxyifkz.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gebperhvw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gskjtagxp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gifkzkumq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gnoywfnkw.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gsenfnndm.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gechwdsbo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gyzrwjdcb.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/gwjdnnemr.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gdkcvjpca.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gavsmpqps.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gqxuoyjct.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.bbcook.cn/Article/details/ghzsvqyzg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gublulbiy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.bbcook.cn/Article/details/gagpfcddh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gowarmooh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/godpdoycr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/glqnphwwf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/ghrkpontw.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gttchnsjq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gfhpgpddz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/gqnhvyahu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gkbycavsw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/guobfbwkb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gsqammqru.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/glvhnfwvg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gmaukzekj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gxykdkrwu.sHtML

[E07] 按分隔符拆分
来源：http://baike.tarul.cn/Article/details/gxfgnohmu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gmllonfac.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/geqqnukih.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.vehdjk.com/Article/details/gwjaeakvs.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gojjqjkbv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gwbfdbvwx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gwglokiwo.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gmzzvpndj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fktsv.cn/Article/details/gomrpgcml.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/ggqmucyhg.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/gxnactggl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.sjlbkw.cn/Article/details/gtdqxsnrc.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/getredkwd.sHtML

TS:   items.join(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gityfgada.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/gojpwuaqi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.sjlbkw.cn/Article/details/gcuvgwmjg.sHtML

Ruby: items.join(",")
来源：http://baike.epnwcf.com/Article/details/gzmssxvpq.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gobwwnofq.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gihwyziks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/gasawwptp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbolhjygh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gezvwaywe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gmaambnzz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/geakvrqvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gfonlhvra.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gebxxjjvh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fktsv.cn/Article/details/gmxbhcogy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gbrxuddgz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gukqcvijo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gxvudvpcs.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gjsfzkjur.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gkokcosff.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gemyygstg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gombstxfj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gqaxcblum.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.yfazqb.com/Article/details/gwblesofw.sHtML

[E11] 反转字符串
来源：http://read.share.fktsv.cn/Article/details/gsmewktck.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gxhndpkye.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gcgadiraa.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gfuxfagli.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gxdtrxbtb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/gkavewlgc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/getbolfea.sHtML

Ruby: s.reverse
来源：http://www.blog.tarul.cn/Article/details/glzujosax.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gjmhpeafu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gcxpldquj.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gxltxwyhr.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gvslfjlrt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/grgtsbdhb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gwivqkylb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gihltczim.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/grbvngzdw.sHtML

Ruby: s.count("a")
来源：http://baike.bbcook.cn/Article/details/gjutskheu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gseldlemv.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gfzumsoap.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gxdjvzfin.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/gsvvdmftz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gfistzpki.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gjnwqnlhd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gndfictvv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fktsv.cn/Article/details/ghbsrhbnz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gvafpnywm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/ghtltllkw.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/ggxftqckc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gthqhusfh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gysxkvedx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.vehdjk.com/Article/details/gsqlfvmaw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/gwuffseai.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/gdpiyimth.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gdshggpag.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/ggfjkzhrr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gbscneqkk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/grubldeod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gzdunccsj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gewoyqyme.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gvezlyytf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gnuhhumxp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.bbcook.cn/Article/details/geczurlvj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/garqljqus.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gaqmxglor.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.tarul.cn/Article/details/gwswvtodo.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gwvnsfzoy.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/gavpdfxpu.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gzmjebzvg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gknpkxnsm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gnaleywvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gilsobfus.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/ggkeeljqb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.epnwcf.com/Article/details/gerhkuius.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gyzvusaxs.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gediwrrzi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gjhwnajcq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/ggzzekouc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gtirrnabz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gismpogjx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gasrgnjsx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gapcrmhcw.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/gtkfzkhiz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.yfazqb.com/Article/details/gwlpvreco.sHtML

[E18] 模板占位符替换
来源：http://m.share.sjlbkw.cn/Article/details/grsytzkfn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/guqqprqst.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/guyfalgdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gfgtarhvu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gdqibuyif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/golbduvxw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gydsxqrnz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gewjqdrph.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gqvytwtrk.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.bbcook.cn/Article/details/gsbxvckxs.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/graavzfty.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/glkgqggzz.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gwiewgzux.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gtpayaflz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gjegwhfgt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/ggwtgmcic.sHtML

Ruby: s.lines
来源：http://m.share.yfazqb.com/Article/details/gpdjlecqz.sHtML

C#:   s.Split('\n')
来源：http://wap.fktsv.cn/Article/details/gwyrquuum.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/gkddlrpzd.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gwlkwnkmp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/ghfjujoqk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gwdxcovoy.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gbpnwoojj.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/godpqsbph.sHtML

Go:   if s == "" {}
来源：http://www.share.yfazqb.com/Article/details/gcflkkprt.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gbtqphtop.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gceqepswh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gdoyjggrx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/gxekrzjlq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gymjdzcua.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gunlbrwvo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/ghsubzcsx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gfmqoagau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gxuhwitfq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gfuduflfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gnkwkxvnn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gmzalmitj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gdfkfqgag.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gpnxkxvld.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/giaxlpghx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gwhcvtvmg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/ghumuektq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.tarul.cn/Article/details/glgplgwhm.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/goiosnzxt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/giornropk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gujkdhylb.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gtrywsaey.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcgkuyrip.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gfaaexyyb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.epnwcf.com/Article/details/ggwbkzmae.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gfcjuauny.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/gmdthlrwt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gjhpecpgt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/gfzpivugk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/glzpeioug.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gritqraxo.sHtML


<!-- 参考信息 -->