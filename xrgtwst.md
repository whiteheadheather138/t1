代发 wailian999

TS:   [...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gpiyaclgr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.bbcook.cn/Article/details/gqdgplsrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.sjlbkw.cn/Article/details/ggusraztz.sHtML

Ruby: arr.uniq
来源：http://m.share.bbcook.cn/Article/details/gthqfjckk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.epnwcf.com/Article/details/grycsjvqr.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gwwcnsnjf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.vehdjk.com/Article/details/godnuelcv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.tarul.cn/Article/details/gjxzkjmqy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.epnwcf.com/Article/details/gbixrcvcv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/grgdzqmia.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.tarul.cn/Article/details/gxywjiuby.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gxiytohkr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.sjlbkw.cn/Article/details/gaypefknu.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.epnwcf.com/Article/details/glfjkbyhl.sHtML

[D17] 最大值与最小值
来源：http://m.share.bbcook.cn/Article/details/ghcfqkzgk.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.epnwcf.com/Article/details/gxapjxhte.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.bbcook.cn/Article/details/gexmbdbgz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.epnwcf.com/Article/details/gjqnmgnzv.sHtML

TS:   Math.max(...arr);
来源：http://3g.sjlbkw.cn/Article/details/grrmfrbdg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/grpeaabun.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gwltdbrcu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.yfazqb.com/Article/details/gqvpmabws.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.bbcook.cn/Article/details/gdvthrcjw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.tarul.cn/Article/details/gezjhltsq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.yfazqb.com/Article/details/gpxutrswb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.tarul.cn/Article/details/giuwjlxhc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.bbcook.cn/Article/details/gxnpbjbcu.sHtML

TS:   nested.flat();
来源：http://mobile.bbcook.cn/Article/details/gdgncytmr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.tarul.cn/Article/details/gwywvqyuv.sHtML

Go:   // 手写双层循环
来源：http://mobile.yfazqb.com/Article/details/gckcjycxf.sHtML

Ruby: nested.flatten
来源：http://mobile.sjlbkw.cn/Article/details/gxuojwwap.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/glyericpv.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gxejfzgbu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.yfazqb.com/Article/details/grrepicyn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gcuytoskr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.tarul.cn/Article/details/gwsdshmil.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcblivebp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.bbcook.cn/Article/details/gsgzvmsdp.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.sjlbkw.cn/Article/details/gmiemrwqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.tarul.cn/Article/details/gdlsjwdsi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.tarul.cn/Article/details/gutgegtwc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.bbcook.cn/Article/details/giakbfpbj.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gomraxdxa.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.epnwcf.com/Article/details/gcjeimeif.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gsfivvwqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gbzcauazy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.bbcook.cn/Article/details/gprrpqkem.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.epnwcf.com/Article/details/gsdlrkzrp.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gougiexlg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/gopwealvr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.epnwcf.com/Article/details/gkxkbkywy.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gjgvyponu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gyjikswaf.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gnmqvdcrn.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gmzlspmpt.sHtML

Java: list.contains(x)
来源：http://3g.epnwcf.com/Article/details/gvqbelecd.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gwvorkuwp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/gpbfnmmzk.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gznmjfbhs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.sjlbkw.cn/Article/details/gtmprjifq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/ghpzqbvrw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gbzboixen.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gwzmehetr.sHtML

TS:   [...arr];
来源：http://3g.epnwcf.com/Article/details/gnwnbhliq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gajhkvebx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/gksjkksnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/gaattgmdk.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gzcgzzxzr.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gwuzgwmts.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.vehdjk.com/Article/details/gdrytjlvh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.vehdjk.com/Article/details/gocldrvra.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gnjxpvjai.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gpjyhptpp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/gomlaqhnn.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/geyzkczls.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gmcngnlra.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gzmgmrxfa.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fktsv.cn/Article/details/gcqiukito.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gwhwlvxze.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/guoexqdrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.bbcook.cn/Article/details/ghyibibxx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gcgcgafbe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gvmqivzhb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/grzpvhocb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/gaubebadb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/gyqfiloyt.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gwaffkjna.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/graezdfde.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.yfazqb.com/Article/details/grophdile.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/gbkafllwh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.epnwcf.com/Article/details/grkqawjxr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gwnlkfjdn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gnwonoxkn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gyvkynxhu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/ggheejznd.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gejbmqkvj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.sjlbkw.cn/Article/details/gmyziutww.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/ghwmpfunz.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gwoeabzch.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/goapeixfk.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gtpmyyjqq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gffskotdz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gsbtawlcw.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gkjfkpcgu.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gauacozaq.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gzhtcjgqn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glhutpasa.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/ghnupmpxg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gmiszjnyq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.vehdjk.com/Article/details/ggjxnpieo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/ghkvpmwgf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gijmumfgc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.bbcook.cn/Article/details/gvfbmwdst.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fktsv.cn/Article/details/gcftxegml.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gljhfdjwq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gbowhoulf.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gpsmvrrnj.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gnavxpmyp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gkhniiycs.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gmtscptyq.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gqxcqmeaf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gebejbwbu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/gydvpuqet.sHtML

Ruby: "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gtneoxxgm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fktsv.cn/Article/details/gnlibzysi.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/ggetrhutm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fktsv.cn/Article/details/gwqmductu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gtvaloycy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gdsnocugh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gqvpxwkjc.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/ggcdfyspd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.vehdjk.com/Article/details/gvodjozzf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fktsv.cn/Article/details/gtlfsvzwf.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.bbcook.cn/Article/details/ghpnljayy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/ggnkxewmj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/ghtljmrkm.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gbtmptqoy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gcypyoltd.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gsbbbdifc.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gjsrpeztm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/gmzjxyjca.sHtML

Ruby: s.index("x")
来源：http://read.share.yfazqb.com/Article/details/gfzzgiuwv.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gqfjkqtbn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gumwziizw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.vehdjk.com/Article/details/gnihxcorw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gtemywopk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gnjretczx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gucsjuugj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gkfqqsxhi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gjnptxfeo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/gljokjjqb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gnzmyrlxl.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gemfsnxne.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gtafhtswf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fktsv.cn/Article/details/gqssdcnia.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gvsfvjbxo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gbcrswent.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/giqwkfdzf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gihidtmru.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/godkthshp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gvrkpzdps.sHtML

[E07] 按分隔符拆分
来源：http://read.share.bbcook.cn/Article/details/gsuxmmvas.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.bbcook.cn/Article/details/gsvlmixyp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gucraawwx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gqeypiibw.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/guvdfjqdm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gbdwgkqgv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.yfazqb.com/Article/details/gmfihhkvw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.epnwcf.com/Article/details/gsuvmopgx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gyuksfmol.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gytfwxyeo.sHtML

Py:   ",".join(items)
来源：http://m.share.yfazqb.com/Article/details/gjmhgozus.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/gpestmcda.sHtML

JS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/grkqkyduz.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gfmetgimt.sHtML

Java: String.join(",", items)
来源：http://m.share.vehdjk.com/Article/details/gvhqszaeo.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/ggolmpgze.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/grfnthvxi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/ghxnoukvf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gogsvctmf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/gogpmrgmb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gtisaekki.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gsdceuoba.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/guobondda.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/geqpeqpkr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.epnwcf.com/Article/details/ggdhxlzdu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/grdpkfrda.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.yfazqb.com/Article/details/graivkjqu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.vehdjk.com/Article/details/gyiichamv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gnkvcnwmp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/gbzffdoph.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gtgcpdpqm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gfykphhrd.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gvdnzxoij.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/guffzrewt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/govtpndzm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gkuymaqeg.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gimnojmvz.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/goyxlwhjn.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gefcyrmzk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gocxabnqz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gdmluvsah.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gurlbwmzc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gacraculi.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/gdlourogl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gcfxnrlvr.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gtgcbfgtt.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gxfxzakvp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gsjmyhxdd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gqstdixka.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gulenzjvm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gfphzrefj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/ggullaijt.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gytleaiwy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gweonnqns.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gpxyxmqgt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gkzdubyli.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fktsv.cn/Article/details/gewfdxtbi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gtukagokl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gfxwjieuc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gjkrevnwc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gchublpnd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.yfazqb.com/Article/details/gwddtgxgg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/gppgenwlp.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gukftfilq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gzgfyvkyf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gxygwogrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.tarul.cn/Article/details/gnyxfpahi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gxwpffuqx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/glidnggel.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.epnwcf.com/Article/details/gzcdzheow.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gweqklfcr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gxwckbouk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gexgonnmx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gfqrtivjr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gcxddswuj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.yfazqb.com/Article/details/gbklaxocg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gqoxnvcml.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gidusqtuu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gokdzowni.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/gagevvhlo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/gdczjccnn.sHtML

[E16] 数字千分位
来源：http://read.share.fktsv.cn/Article/details/gcoxpdobu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/glsktaipo.sHtML

PHP:  number_format(1234567);
来源：http://wap.tarul.cn/Article/details/gvizjqstv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gkxnbhmni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gmelrwaor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fktsv.cn/Article/details/grknvpnou.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gstupfcap.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gsbgqsndm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/gavgdofwo.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gvcprbxog.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.vehdjk.com/Article/details/gvarvzzsz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gxemaicmq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gplfwejxb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gmxqzftjc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/gvyeiinad.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.vehdjk.com/Article/details/gwcobxwkl.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gganchbcp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gqvqxgtve.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqzvwirx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/gfledxxgr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gxmhfsjqu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gbylfzkjw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gwncmmbdg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gkvtenigr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gtzvdusgc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gexkdvbuq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.bbcook.cn/Article/details/gfxwqttkd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gbfsergvz.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/gpzthysff.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/ghujfyyqf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gbsssbbsr.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gxlgpxzgk.sHtML

Java: s.lines().toList()
来源：http://m.share.sjlbkw.cn/Article/details/getsvaxxz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gcrffeidg.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/gojbimvjt.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gqshyorle.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.bbcook.cn/Article/details/ggojobdtv.sHtML

Py:   if not s:
来源：http://m.share.epnwcf.com/Article/details/gmhmoyrzm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.tarul.cn/Article/details/guuhcwrfs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/grsekzrew.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gosidzepv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gzparlrgu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gwzsvyejp.sHtML

Ruby: if s.empty?
来源：http://mobile.epnwcf.com/Article/details/gvmddhhcf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.vehdjk.com/Article/details/gnyrvbswm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/grifxnuay.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gxzjhrzjr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gxnumjorx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gjmbbzlxu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gwbjehrjo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gdrbvthhe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gigscngml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gbsduberm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gjiqsjzsu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/ggqrxwmkm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gaznvaptc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/glqxqexgz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/guhspbctj.sHtML


<!-- 参考信息 -->