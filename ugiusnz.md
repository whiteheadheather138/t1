代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gyhqktgir.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.epnwcf.com/Article/details/gdnwbenlp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/gvsrwuqkw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.sjlbkw.cn/Article/details/glijslqcn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.vehdjk.com/Article/details/gdzekcwaq.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gnynpppjo.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gcxkpdavo.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gybnnhtno.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gdrxeevhi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gmrxidomz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.bbcook.cn/Article/details/gakxtjpkk.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.vehdjk.com/Article/details/gqorueexi.sHtML

Ruby: arr.tally
来源：http://m.share.sjlbkw.cn/Article/details/gxrrsbajm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gxolbsgjx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/grcyrpujo.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gffhukdru.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.vehdjk.com/Article/details/gewdpbphq.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/ghpbtpwki.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/ghwnwffuw.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gtymtwewg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.epnwcf.com/Article/details/guntyhfxo.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gihwmuvec.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gisugfnzk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gwfpqkmyk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gkxhlycqf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.tarul.cn/Article/details/gjhjrpyqv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gchxedmbp.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/gcumbamau.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.bbcook.cn/Article/details/gusjckbbi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/ggiqasltc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/gyatpesax.sHtML

C#:   new List<int>(list);
来源：http://wap.tarul.cn/Article/details/gqrknfxdl.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gyfvlnpae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/gdkvcdhaj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gavxuftnv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gzbfjumvi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.vehdjk.com/Article/details/gxjdlgobx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/gopbyumzr.sHtML

Go:   // 手写循环
来源：http://baike.tarul.cn/Article/details/gfrxrrurb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/gapldnonm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.vehdjk.com/Article/details/ghuwclzqx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gzhkoaftu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gqsdqrmzy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.sjlbkw.cn/Article/details/gjfrukten.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.epnwcf.com/Article/details/gzbocbhft.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/gsplgcdra.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/ghbxlysbu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.epnwcf.com/Article/details/gmbqpdlom.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.vehdjk.com/Article/details/gnzdywvay.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.bbcook.cn/Article/details/gblsdktwq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/gxscpslal.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.tarul.cn/Article/details/gvdkgcqpp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.bbcook.cn/Article/details/ggjepmntb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gvadvwhvq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gtipwuhjt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gwcwctnvx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.tarul.cn/Article/details/gqgzebpdn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.bbcook.cn/Article/details/gscbldqxp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/gzvmtausg.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/ginbxkapp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/gfejjagvv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gaglnckys.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gdgiqagqw.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gwpebrrbg.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gbjqrwumy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/gznocueym.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gqgalampo.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gjooewbtm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gtnyqtmrj.sHtML

E. 字符串处理
来源：http://www.blog.fktsv.cn/Article/details/gxexavabm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gsxipqskj.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gpvvnbjtm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/gdeofhtlm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gqajsjibv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gakslyjrv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gnwoyltdu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/glvhmalwx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gkabllltn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gumjnncqk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gxkprnrjq.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gsibjxkst.sHtML

Py:   "ab" * 3
来源：http://www.share.tarul.cn/Article/details/gwguzuiyc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gmwprewip.sHtML

JS:   "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gudnfxbzw.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gullitjhd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gvfntxzyi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.vehdjk.com/Article/details/gzqzcgghn.sHtML

Ruby: "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gtpmblyqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.bbcook.cn/Article/details/gbaqomsdw.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/goadtatts.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/grwwkonkk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gbeyaagpu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gghjyfotm.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gbqgezrhf.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/ggoqeomyq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/glugcogok.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gtatwazzh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gvcuczwzz.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gsrlfvjnr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gikxxpizl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gziybylzk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.bbcook.cn/Article/details/gsiurkltt.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gzxekuwal.sHtML

Java: s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gzcwomqar.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.tarul.cn/Article/details/gzagkklzy.sHtML

Ruby: s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gntjsvlty.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/ghisglhut.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gcjykckrr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.epnwcf.com/Article/details/gbcdqbczq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/guorshqyz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/grxfewuvt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/glswxmccf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gfdtqtjpb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gdhpwungm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/ggkxkuukw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gpoqajoxm.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gmcoxwtxg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fktsv.cn/Article/details/gqvtopkab.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gmfbhgdbx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gqnekdzoz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gkseosvkr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/giiiybvbs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gogrcrcwz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gycwojzvj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gfxvjekfz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.yfazqb.com/Article/details/gfecgvjgv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.sjlbkw.cn/Article/details/gnyydkuxy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gcbkbjcga.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/grdrwqsri.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gafwznnde.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.vehdjk.com/Article/details/grxymqqdl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.tarul.cn/Article/details/gwnzekqec.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.tarul.cn/Article/details/gwyxbkqad.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.vehdjk.com/Article/details/glpxutfqz.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.epnwcf.com/Article/details/gujrefkif.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gbnzmompn.sHtML

PHP:  implode(",", $items);
来源：http://baike.sjlbkw.cn/Article/details/grphknyjd.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gojzdtivl.sHtML

TS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gomccjyze.sHtML

Java: String.join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gsrkbbntg.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gauyimliz.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gqafhxyiu.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gqvwyzped.sHtML

[E09] 去除所有空白字符
来源：http://3g.fktsv.cn/Article/details/gwoqpyohx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gwddgmcrd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.vehdjk.com/Article/details/gawedkngv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gkbfwkvxm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gvlahkcja.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gzirpfzow.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gpinlbimf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gxdetfppp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/ggkrdkpta.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.yfazqb.com/Article/details/gkxhemkde.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.tarul.cn/Article/details/gqttbmwjp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fktsv.cn/Article/details/gobfkbnha.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gsztjdbmo.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/giqtrkugk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/ghmzdtxbm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/geyyszqpm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gvmokinsp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/ghblsdpem.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/gkjafdphu.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gvjmxqkma.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gdpbhzfwx.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gqtqimaqc.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/glowwoxkz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/giggxnspt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.bbcook.cn/Article/details/gktphowxv.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gbjmnwthz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/ggqigrfhc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.vehdjk.com/Article/details/gvxemlfgl.sHtML

Py:   s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gcjzwtbkb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gadtsdxuc.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/grsixtalm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gbmakfomg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.tarul.cn/Article/details/ggxxiwbfb.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gyxmugsyn.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gmalbjfdo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/gcqbdxtri.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gzyrvgbus.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/gorebwfbc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.bbcook.cn/Article/details/gdqzkbdgh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/grrqpenih.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gsyhezamg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/gfhucsvfn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gmsuftmeq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gfjqsjeji.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gslkdbanm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/ggcrcuwmx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.vehdjk.com/Article/details/gvzjnamaf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gfofefwmr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gbkftvmud.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gepeygvid.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.yfazqb.com/Article/details/gcrlelvrv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/grtbfhgbo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gcvoeibib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.tarul.cn/Article/details/gjoixywql.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gigweexvr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gdwudahpc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gfimpyuki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gbwtrfrdn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.bbcook.cn/Article/details/gsxkguxfu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gvspckrkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gyykgtuux.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gzexudrww.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gujrvkmpz.sHtML

[E16] 数字千分位
来源：http://m.share.epnwcf.com/Article/details/gdcnpucqs.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fktsv.cn/Article/details/gwphxelek.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/gdfdzgzjd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gfjrgifsi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gblmfzljc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.bbcook.cn/Article/details/gubuugkxc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/gypbzikrj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.epnwcf.com/Article/details/gajedqryl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.sjlbkw.cn/Article/details/gagmbrhfe.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/glhqeaqjn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.vehdjk.com/Article/details/goebssjrn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gjluepmgu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxcwqowih.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gckaqlouq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gprmqnttc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.yfazqb.com/Article/details/gtdeupewg.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gadvhdwgf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/ggrscjapu.sHtML

[E18] 模板占位符替换
来源：http://blog.bbcook.cn/Article/details/gdhkbagam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.yfazqb.com/Article/details/gcpxyorut.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/ghdqurvfj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gjawtnmkc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/ghqelqukg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/glgjgkxdg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/grosumewf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/ghlhnigrp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.yfazqb.com/Article/details/gbegrhmyf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/ghmaqmxuq.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gptememgx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.epnwcf.com/Article/details/gyxelpnlz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gotuafhmw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/grxhggjnj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/glpzorolo.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.vehdjk.com/Article/details/gpgmfzfef.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gknxssfto.sHtML

C#:   s.Split('\n')
来源：http://3g.sjlbkw.cn/Article/details/gzstsasnp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.tarul.cn/Article/details/gphgtntoo.sHtML

Py:   if not s:
来源：http://wap.yfazqb.com/Article/details/gjidptqja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gegzzwdng.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/givsbbeph.sHtML

TS:   if (s === "") {}
来源：http://baike.bbcook.cn/Article/details/gldrocumw.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gmwzozaji.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gcijmiute.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/gwlspzyfo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.bbcook.cn/Article/details/gdfsswldq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gnfgejafu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gaegxvsum.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/ggrzngxdd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gmgybjvrl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/getlfehoa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gltfedase.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gzckvhtcs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gfkimkvew.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gjlbbashe.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/grvlgjbur.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gdxvdxmmk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/glgxtiiad.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/gructcbsd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gqovdnwkf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fktsv.cn/Article/details/grhdzdyyx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.sjlbkw.cn/Article/details/gszbpuizm.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/gozpybnht.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gwbkhpgmq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guiohahay.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gbdocvqux.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gfoaizuni.sHtML

[F01] 读取整个文件
来源：http://mobile.sjlbkw.cn/Article/details/gygqkhjvi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.vehdjk.com/Article/details/gsmuybkmg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ggwzmjgul.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fktsv.cn/Article/details/gahpdbums.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gelpsmzre.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gaecxpovc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gukgdybld.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxchdntzb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.tarul.cn/Article/details/gcinhtpmo.sHtML

[F02] 逐行读取文件
来源：http://blog.fktsv.cn/Article/details/ghbjppfit.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/givsbdcym.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.bbcook.cn/Article/details/ghrwwlxkc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/giiadloux.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gtgovvdnl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gjogopzii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.epnwcf.com/Article/details/gchwvntef.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gxzpyvxdg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/gpxyqrpxw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gdxnaiayg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/gbqrpvotn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.yfazqb.com/Article/details/gbdjvaklz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fktsv.cn/Article/details/gavjbhyuj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gllycxxtw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/gecdxxppr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.tarul.cn/Article/details/gewzrkloi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/gjfxznqds.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.sjlbkw.cn/Article/details/gwfoahtyl.sHtML

[F04] 追加写入文件
来源：http://blog.bbcook.cn/Article/details/gklkqdgsb.sHtML


<!-- 参考信息 -->