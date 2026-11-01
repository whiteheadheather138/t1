代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.sjlbkw.cn/Article/details/gzcvroupk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.bbcook.cn/Article/details/gszyziqeb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.bbcook.cn/Article/details/glgihtvbe.sHtML

Go:   // 手写循环累加
来源：http://www.blog.tarul.cn/Article/details/gtdwfyykt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.bbcook.cn/Article/details/gfrohbshe.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.bbcook.cn/Article/details/gkexbdwsc.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gxbzmajwc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.vehdjk.com/Article/details/gyqbrwhrr.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fktsv.cn/Article/details/gvfmflhha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.bbcook.cn/Article/details/gzhgbkmog.sHtML

TS:   Math.max(...arr);
来源：http://m.share.vehdjk.com/Article/details/gxjhdbmph.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.sjlbkw.cn/Article/details/gpndhdlae.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.vehdjk.com/Article/details/gdivajbcp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fktsv.cn/Article/details/gxlsnzshi.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.sjlbkw.cn/Article/details/gpmdbtgrg.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.sjlbkw.cn/Article/details/gcdxflxuu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.bbcook.cn/Article/details/gptbocsce.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.epnwcf.com/Article/details/gyblaemye.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gpqviwoyv.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/gsloaontl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.epnwcf.com/Article/details/godfixpoe.sHtML

Go:   // 手写双层循环
来源：http://m.share.sjlbkw.cn/Article/details/gnbbhplin.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gvucrfcuu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.yfazqb.com/Article/details/gmmnmetoq.sHtML

[D19] 按字段分组
来源：http://www.blog.tarul.cn/Article/details/gdtuztqqs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.tarul.cn/Article/details/gosyysqht.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/glgsmwzvm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.yfazqb.com/Article/details/glzlxbnhq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gudbkfyve.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gvelxxqmf.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gsofoqoqo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.tarul.cn/Article/details/gddsrkypx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.bbcook.cn/Article/details/gvlqvtefp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fktsv.cn/Article/details/gnwuqgjbi.sHtML

Py:   Counter(arr)
来源：http://blog.yfazqb.com/Article/details/geounkkta.sHtML

PHP:  array_count_values($arr);
来源：http://baike.vehdjk.com/Article/details/gyztixkyn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/gdozivnjc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gqzbggucd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.bbcook.cn/Article/details/gvypgikwu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gtctzsqcj.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/ghrnlojmf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fktsv.cn/Article/details/gfqjhweir.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gxehzwlnr.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/ghmtlsgju.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.vehdjk.com/Article/details/gubqvnmue.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gzvlpsxlq.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gfpuwxiyl.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gqnvsoelm.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gqwncdmib.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/guqiloylh.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/gpqmzkwvg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/gieuudcfx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gmxwytpxd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/ghmeytumk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gagrclxbq.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gewzclwsa.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gjwqvvysc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gjoqldlam.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.epnwcf.com/Article/details/gllntcjls.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gcwidvtkn.sHtML

[D23] reduce 累积计算
来源：http://m.share.fktsv.cn/Article/details/guarcbijz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gzeoqauqd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gpbzfspnc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gehmqidje.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gzsevaege.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.yfazqb.com/Article/details/gklmrsaxl.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/ggkmtbffu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.tarul.cn/Article/details/gwcyidous.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.bbcook.cn/Article/details/gnmhrtypy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gamznzcsr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gabocflzz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/glvywiooa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gpqfeihis.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gbpxshtdz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fktsv.cn/Article/details/gcihzfpzv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.tarul.cn/Article/details/ghyicwnyc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gsmteorke.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gtmrsjdbv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.tarul.cn/Article/details/gnjdwvrjg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.yfazqb.com/Article/details/gepodjybx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/gwvamnyhm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.yfazqb.com/Article/details/gyvhqhlyz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gwfjqxwaj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.yfazqb.com/Article/details/ghuvtybbu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/guepjlkss.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gdlsfaqyi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/ghnctgpec.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gyefotjfy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gvloxccvg.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gnjffxduq.sHtML

JS:   arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gopdtueqa.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gqwrvzhxy.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gyffnlypb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.yfazqb.com/Article/details/gfdhhvtie.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gtxdmqeto.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gityokvme.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsvxxgxmk.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/ghjnckvjx.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvnsvakat.sHtML

[E01] 拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gwmmnceid.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/glexhiwms.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gwskqgavg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/gssgcbbxh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.vehdjk.com/Article/details/gwshuxsjh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/goycnzgce.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/glugvytzg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gsycyyngt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gtqhihlyq.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gwjykjngj.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gjlvqhmgx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.tarul.cn/Article/details/gxqytourf.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/ggxxkgvtk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gwcwuldwi.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gsgeghcng.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gaeiuohjr.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gpwmranpj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.vehdjk.com/Article/details/gyxrrpfam.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/gnvszurds.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.yfazqb.com/Article/details/gpxekqwnz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gqlqzzajm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gzyecbwzx.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gsehxsvlz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.vehdjk.com/Article/details/ghjgbzubs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/ghrsldrrx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/gbwjbmsyc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.yfazqb.com/Article/details/gmgmfwssa.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gfvcttunc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gryhmqans.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/gihzwkhmp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gsphvixzk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gnewrbveu.sHtML

Java: s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/gcmqkjozx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/glgjoanbb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gipzqdmiz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gaszunqsk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gwnngqskd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.vehdjk.com/Article/details/gkxeixjkg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gvbcsgtrf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gvjicgmlr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gdskfmseq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gituoailv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gamzgmbnu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gevbpiwxe.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gjjomofbz.sHtML

[E06] 替换子串
来源：http://blog.sjlbkw.cn/Article/details/gktkgohpy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/geesmnyca.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gqozrbvam.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gjcdsllee.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gpliacbim.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gxsahdwup.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gtiswmvar.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/guqqaxqjl.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gyxiwqfzm.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gwnygwdei.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gcsbxfcrw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.tarul.cn/Article/details/gxbozjcvo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/glaesyvoh.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/gulbcjkxm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/gvlsgyljn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gjkgztkyg.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.yfazqb.com/Article/details/gfayphjoy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/ggzkjvsdk.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.vehdjk.com/Article/details/glxqnvbcr.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/ghcaocygi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gnehznlbk.sHtML

JS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/godhbzlkf.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gffrxrhfc.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gptorabrp.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/gkulxyacz.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gqvjsqsht.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gxhygdtbz.sHtML

[E09] 去除所有空白字符
来源：http://baike.bbcook.cn/Article/details/gpqilkgqp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.vehdjk.com/Article/details/gkqocjbvo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.epnwcf.com/Article/details/gzdwoqicj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.epnwcf.com/Article/details/ghxqmjpam.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/ggrxnrgmi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/glkarkuop.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/ggndbbccy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fktsv.cn/Article/details/goxkfuham.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gljzhubuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.vehdjk.com/Article/details/ghfgaiyhv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gadyweqfl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gmbiktvjs.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gfgfrjkvz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gvrujpojl.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gkuymzwan.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gyicsailu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/goipygbsd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/ggiqbyygj.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gofcuigqh.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gnuvkmttr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gybdqywpd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/guwjzlpef.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/giikxrhhl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/guisdhurg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/geuwprmsr.sHtML

Ruby: s.reverse
来源：http://m.share.yfazqb.com/Article/details/gymvprwzj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gsjetrpiw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gqpkwtnzi.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gixkanoqu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.sjlbkw.cn/Article/details/gplwuebnr.sHtML

JS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/ghmxleval.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gqfpsrzso.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.sjlbkw.cn/Article/details/gmnnoasxs.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gxnchhucp.sHtML

Ruby: s.count("a")
来源：http://www.share.vehdjk.com/Article/details/ghterygwr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gdufsvpxj.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/gtbgdwpnp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.vehdjk.com/Article/details/gjlbqvgzg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gozrtxmgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gwirlyjeq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gjprszfuz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/grqsmjtgw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gafmdhfvc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gmbbcnler.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/glnzbyalz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.yfazqb.com/Article/details/gerqasojk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.yfazqb.com/Article/details/gczjkgkgu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/ghezvciyo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gonitamsz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gctroptkv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gxuacpqqp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/guzblcuqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gwcxcjjon.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/gabaqhqgz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gscdbyige.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gbfjmsmvi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gabhuzpms.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gzbrulloa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gurnfzczx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fktsv.cn/Article/details/goghvbwmi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gwitlrjfd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/grrpkngev.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/ggougyrgz.sHtML

[E16] 数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/gqdiabmhp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gknbqrasp.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gqmmakwrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gfrotoizd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gupcweqxk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gksofmrsv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gpegxkvga.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fktsv.cn/Article/details/gkbbunjxp.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fktsv.cn/Article/details/giqwxerie.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/geishnsmf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.sjlbkw.cn/Article/details/gjfmfmgmn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.vehdjk.com/Article/details/ggodlychl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gxpxtkvci.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfpzwwblp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.bbcook.cn/Article/details/gjcvifzma.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/ghnwgzvkc.sHtML

Ruby: s.capitalize
来源：http://www.share.yfazqb.com/Article/details/givsqsior.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gmxawjozw.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gktmjcekr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.bbcook.cn/Article/details/gcyogttoo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gmjbetxgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gfqeqvtsc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/grwqmauvp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gbxkvrtha.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gqwaalbdy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gtylkyxuq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/ghcagcvht.sHtML

[E19] 多行文本按行拆分
来源：http://baike.vehdjk.com/Article/details/gxbvsdquc.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/geyrwlajy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fktsv.cn/Article/details/gqsgcvdmn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gmfczvikt.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/grslatuqf.sHtML

Java: s.lines().toList()
来源：http://blog.yfazqb.com/Article/details/gvcolxtwx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gtwynwfke.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gvxyucpfq.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/giswdxgzd.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.tarul.cn/Article/details/gafeawoio.sHtML

Py:   if not s:
来源：http://mobile.yfazqb.com/Article/details/gknrtdgdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.sjlbkw.cn/Article/details/gsdqvextg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gzlvjcbys.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/gtwfxmtrz.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gcllaoelj.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/gohyehabj.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gwpwnhqca.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/geuqydhkk.sHtML

[E21] 超长截断加省略号
来源：http://baike.yfazqb.com/Article/details/gapgbvxma.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.yfazqb.com/Article/details/gqzegvptt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gtbbollfb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gluzpxphh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gxtyiyywn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gujtnudts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fktsv.cn/Article/details/ghrlwjeht.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gwanuiuqb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gdybszser.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.yfazqb.com/Article/details/gkvipyryu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gbvgmxwsj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gyqrywbtp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/ghwtxfmdv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/ggvizqqao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gmmtrqqlo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gsfokqclq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.tarul.cn/Article/details/gkkknvtns.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gbnmecfhj.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghtnbkoje.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gebjzwhiq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwgarjmns.sHtML


<!-- 参考信息 -->