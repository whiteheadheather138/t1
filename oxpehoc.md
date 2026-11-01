代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.epnwcf.com/Article/details/goivblrem.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.bbcook.cn/Article/details/gawswojff.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gkcwgctig.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnkolqnbg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.yfazqb.com/Article/details/gmiwhzxvf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.yfazqb.com/Article/details/ginzippsf.sHtML

TS:   Math.max(...arr);
来源：http://wap.tarul.cn/Article/details/goqmnzuwa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.sjlbkw.cn/Article/details/grjymuwhm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.vehdjk.com/Article/details/glslznrdt.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gilhpoqmb.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fktsv.cn/Article/details/giqabigux.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fktsv.cn/Article/details/gybeplppf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.vehdjk.com/Article/details/gwgoryipk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/ghzvtppmw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.vehdjk.com/Article/details/gwsukaboa.sHtML

TS:   nested.flat();
来源：http://3g.sjlbkw.cn/Article/details/guzciwmdk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.epnwcf.com/Article/details/gcvkxzwii.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gypfmahba.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gzmlukaxz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.vehdjk.com/Article/details/gmflxiavt.sHtML

[D19] 按字段分组
来源：http://baike.yfazqb.com/Article/details/gxfaicyzo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.sjlbkw.cn/Article/details/gsstmaxxw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.vehdjk.com/Article/details/gogzxilqs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gznkjeecn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.yfazqb.com/Article/details/gnckiatlq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/gechsylmi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.yfazqb.com/Article/details/gnypfmsha.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.sjlbkw.cn/Article/details/gsouzeyim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gmwblgwiw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/gvdprfdvk.sHtML

Py:   Counter(arr)
来源：http://mobile.yfazqb.com/Article/details/grfkaxdje.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gxmlztmfg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gaakphlvt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gbxrjdpsw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gwbqizkke.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.yfazqb.com/Article/details/gwvizweqo.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gymqnnggs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.epnwcf.com/Article/details/gfxybecto.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/glhueakzi.sHtML

Py:   x in arr
来源：http://www.m.share.sjlbkw.cn/Article/details/gflhmvahi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gebnpdlfi.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gihyrzdkr.sHtML

TS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gzykdvfgf.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/ghpkihwhm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gwzohyubv.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/guwicjibp.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gamoybatr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.yfazqb.com/Article/details/gzwlnxqfb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/gkbdjdpzr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fktsv.cn/Article/details/gxnvaidfb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/ghcyatvnm.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/givixfwkv.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.vehdjk.com/Article/details/gnfipfsnm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.vehdjk.com/Article/details/giazayyfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gqdnwfalw.sHtML

C#:   new List<int>(list);
来源：http://baike.sjlbkw.cn/Article/details/gqoswcuhg.sHtML

[D23] reduce 累积计算
来源：http://mobile.vehdjk.com/Article/details/gfyoqknce.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/ggrejiudi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gsrhfvqzp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gnsebwnhu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gltkdalsu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.sjlbkw.cn/Article/details/gnzdeuccs.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gcjfpzqqm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/gfkeymyif.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.yfazqb.com/Article/details/ghlbhergm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gagwjyitw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.vehdjk.com/Article/details/gbznalfuc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gxldesycp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/guvjtuehb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fktsv.cn/Article/details/gsrovtoul.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gmihyadfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/gbfzcmcri.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/golacnozr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlptwewj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.epnwcf.com/Article/details/glgvjwbba.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmvgqsgy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gnchjojmq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gpmefpbpj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.bbcook.cn/Article/details/ggynperzg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gfmmfchzi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/grgmlvdbl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gmrbfmnuh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gvpnqdfpl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxuthvkla.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gzhvwfnen.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gtuogmory.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gazhnkyrk.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/grbanitgv.sHtML

Java: String.join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gqlusberf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/ggmmxznyi.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gossqwxgk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gkcqjlbdz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glwfijlob.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gibrkouvl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkhikqehu.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpaumcqim.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/gmjkvqyqu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gjocadolo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gpiveatkd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gbxmbimxf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.sjlbkw.cn/Article/details/gsnoqlrom.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gohumbvks.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gpejvqnrd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fktsv.cn/Article/details/gjaixxzhf.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gduqyjpxb.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/ggvrftrme.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fktsv.cn/Article/details/gcqvnhfrk.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/goajgbsup.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/grltxaeuk.sHtML

Java: "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/ghztkgijf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gudrlzapr.sHtML

Ruby: "ab" * 3
来源：http://www.blog.yfazqb.com/Article/details/gzxrgxfpb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gyuerkdsm.sHtML

[E03] 截取子串
来源：http://wap.vehdjk.com/Article/details/goognkuln.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gphdlpeze.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gxqsafpmo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gvkubsivw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/giqcxkzun.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gngkygloi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gatrmyxhq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/glbdrjtzg.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.sjlbkw.cn/Article/details/gznwdsgqp.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/godxkrbxq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gukbrxqeq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gvgxtmkoh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gytfejyow.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/grpiicfwl.sHtML

Java: s.indexOf("x")
来源：http://mobile.tarul.cn/Article/details/gbmcjtihi.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gsbkiemgk.sHtML

Ruby: s.index("x")
来源：http://www.share.sjlbkw.cn/Article/details/goqkbippp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/grriqyqwa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.yfazqb.com/Article/details/gcdmwtgqm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gjoitfwgz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fktsv.cn/Article/details/gpcuefxkm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/guasfyhqe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gschdehvc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gdapenbaj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gqrwvygpg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gensvfpip.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gynzhzbju.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gbnpgzybf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gcxemeczo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gdwocnnon.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gwfpxqvde.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/grieshtje.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gkqfmzhst.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gnlhdwzql.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/geyrrklnx.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gxfblsbla.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gkqqozavp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gfzfsztcl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/gibcimskj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gwwtbgqld.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/grzbddmfr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gqjdbgkdd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gwdpmlcdw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gxmcqohja.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gucvfuynf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/glfynsvql.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/grjzxemtk.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/grvlmdbzl.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gnyrrjdth.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/gfbkvsgoe.sHtML

Java: String.join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gvmrsaosg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gcftwdlaz.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gqwuqnulq.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/geuieywam.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gfpbbhjvl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gjqcsntdw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.yfazqb.com/Article/details/gouwvsvne.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gmqmrbcpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.vehdjk.com/Article/details/gtqngunlm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gtjkjgjkl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.epnwcf.com/Article/details/grbgyccxx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.sjlbkw.cn/Article/details/gsorbnyog.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.epnwcf.com/Article/details/gocbkrclu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.vehdjk.com/Article/details/ghljrppcf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gbffqtkem.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.tarul.cn/Article/details/gyoinrtbe.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gcuognfkr.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gqglljyix.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gaggygsos.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gnhmcllcw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gykmsuony.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/gavnoenzo.sHtML

[E11] 反转字符串
来源：http://mobile.bbcook.cn/Article/details/gcluardjh.sHtML

Py:   s[::-1]
来源：http://www.m.share.tarul.cn/Article/details/gpnzwuacz.sHtML

PHP:  strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/ghgyzbezj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/glrwqzhlc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gssgvgkxl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fktsv.cn/Article/details/gtsetsmhu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gqrnmwbju.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gfifedovf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gcabwfpya.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/grzyxgcgp.sHtML

Py:   s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gckstxvna.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.epnwcf.com/Article/details/gpyycbdzi.sHtML

JS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gbfoaubpz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.yfazqb.com/Article/details/gmtutisha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gqwuqwbvw.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.sjlbkw.cn/Article/details/gvlmiyjfh.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gwghewjep.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gcbdvyrlb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gmjmflqlr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/glkiiqbdt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/gycuzxeok.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gwvlynryv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gixgpouih.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gxmnvwfjp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gullicpfm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.yfazqb.com/Article/details/gqbecnmse.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gnhqdjdvm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gvvcavxlv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/giducszdq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gysmmrbag.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gabxttyhs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/grqsgcfzg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.yfazqb.com/Article/details/gqevemyqf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gvynhywft.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/grvryhwhj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/goyfmbdxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/glrvffdrq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gkmwciigc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gkjyezbxj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fktsv.cn/Article/details/gowrchoud.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/gxsfkthvj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gqnmxnhbk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.vehdjk.com/Article/details/gjdborogl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.yfazqb.com/Article/details/gswnovznb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gptfgicuk.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gpefjyjfh.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/gnzmraqjl.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gndtwodur.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/grkjevyap.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gaghmzbqw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gnrujxhyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.epnwcf.com/Article/details/gjdsmbzip.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/gfltbadmd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.yfazqb.com/Article/details/gzgoiashh.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/grgslmdng.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.sjlbkw.cn/Article/details/gjgurftyt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/ghhqacnsc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gqluarqmv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gsqaxhlpf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.sjlbkw.cn/Article/details/gputiqicz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gbfnvpudi.sHtML

Ruby: s.capitalize
来源：http://mobile.epnwcf.com/Article/details/gtpegvbyq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/gbsoojqor.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fktsv.cn/Article/details/gnicljgmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.bbcook.cn/Article/details/gclseelyn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.sjlbkw.cn/Article/details/gkudkowsh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gpxhvnqiy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gzmchavzu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gcqzxesgu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gafotjqtt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/ggrjvlhae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fktsv.cn/Article/details/gvvxpsqdt.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gwshcnnpr.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/gzoovnpzz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.yfazqb.com/Article/details/ggpvyknms.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gwsqzsorq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gtjiirvge.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gajsloemf.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.vehdjk.com/Article/details/gcbpgyfxa.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gqpgctphk.sHtML

C#:   s.Split('\n')
来源：http://blog.fktsv.cn/Article/details/gvaxzjwee.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.sjlbkw.cn/Article/details/grpzaulnu.sHtML

Py:   if not s:
来源：http://wap.fktsv.cn/Article/details/gsfuogcjy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gfskcetta.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gfmpqsfev.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gcavzgmiw.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gulqfyrlg.sHtML

Go:   if s == "" {}
来源：http://www.share.bbcook.cn/Article/details/gdjhbgxrx.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gwztkewhb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.yfazqb.com/Article/details/gulhabzcv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gjibgzkjw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gvangjgwg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/grltcewdm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gnavgdwgb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/ghrlzdkrv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/giddbddsm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gbovxktwc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gzrwfyyjk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gvrfnbqao.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gylbpqygj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gdihibizk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gaslothyk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gdspuzjtd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gklbequzt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gwvbohkhw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gmawvicpm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/grnmtquto.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gqnfhkhvp.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjeyluihk.sHtML

F. 文件与目录
来源：http://www.blog.vehdjk.com/Article/details/glqgvaxyy.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ggijnuqqy.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gcffmmalh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/ggjwdxjsx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gasdbfkyd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.tarul.cn/Article/details/gitfcxnkq.sHtML


<!-- 参考信息 -->