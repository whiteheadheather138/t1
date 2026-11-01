代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.yfazqb.com/Article/details/gbxdkdqva.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.bbcook.cn/Article/details/gvuadlfdi.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.yfazqb.com/Article/details/gryamusab.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.vehdjk.com/Article/details/gvrmadzef.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gwbuqnlvj.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gpqxnyitn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.sjlbkw.cn/Article/details/gexdrtome.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.sjlbkw.cn/Article/details/gqllshhdl.sHtML

[D15] 去重
来源：http://wap.bbcook.cn/Article/details/gsjtixqhf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gafbclnts.sHtML

PHP:  array_unique($arr);
来源：http://mobile.vehdjk.com/Article/details/gzyenopyx.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/guuhqvilq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gedqmdeqe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqvcltfp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.bbcook.cn/Article/details/gfqncxutp.sHtML

Ruby: arr.uniq
来源：http://blog.epnwcf.com/Article/details/gdgxowkty.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.sjlbkw.cn/Article/details/gzziccrjx.sHtML

[D16] 求和与平均值
来源：http://3g.epnwcf.com/Article/details/gdbobbutk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.vehdjk.com/Article/details/guhcivmtr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.vehdjk.com/Article/details/gmyxurhlh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.sjlbkw.cn/Article/details/gvacklfkk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fktsv.cn/Article/details/gesugxkcf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.vehdjk.com/Article/details/garnwmpds.sHtML

Go:   // 手写循环累加
来源：http://baike.fktsv.cn/Article/details/gftjbakoq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.yfazqb.com/Article/details/gqvydlgec.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.bbcook.cn/Article/details/gdyjvuvxb.sHtML

[D17] 最大值与最小值
来源：http://baike.tarul.cn/Article/details/gtrapbnph.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.epnwcf.com/Article/details/gfpbaaaln.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.vehdjk.com/Article/details/gatfiodxn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.bbcook.cn/Article/details/gxwfxvjpr.sHtML

TS:   Math.max(...arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxyrvfizs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.tarul.cn/Article/details/gxdubgeup.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fktsv.cn/Article/details/gevxmhkwc.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.bbcook.cn/Article/details/gmkztzfui.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.tarul.cn/Article/details/gscqzxdwf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fktsv.cn/Article/details/ggbtycymb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/gczbsfdea.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.bbcook.cn/Article/details/gjicunczl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.tarul.cn/Article/details/ggwnlshlp.sHtML

TS:   nested.flat();
来源：http://baike.vehdjk.com/Article/details/gygntjcav.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.tarul.cn/Article/details/grxruguhx.sHtML

Go:   // 手写双层循环
来源：http://3g.tarul.cn/Article/details/gteqcohlw.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gzgxiywxg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fktsv.cn/Article/details/gnqeypems.sHtML

[D19] 按字段分组
来源：http://mobile.vehdjk.com/Article/details/ghmiculjf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.tarul.cn/Article/details/gramvjsfw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fktsv.cn/Article/details/giuksxarm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.vehdjk.com/Article/details/ggmigjiah.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/ggpfonuex.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.bbcook.cn/Article/details/gwubyrsrd.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.epnwcf.com/Article/details/gfvfugzza.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fktsv.cn/Article/details/glkuteyuq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.vehdjk.com/Article/details/gtuwbksln.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gvjrdxhjs.sHtML

Py:   Counter(arr)
来源：http://mobile.fktsv.cn/Article/details/ghjbmcxvh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.sjlbkw.cn/Article/details/gppfxkutw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/glilhuwiy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/guasiqvmh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/gwdrqlrvs.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gzwjxkmtk.sHtML

Ruby: arr.tally
来源：http://m.share.vehdjk.com/Article/details/glzqsrjvk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.epnwcf.com/Article/details/gejdpiubt.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/gtyjkpsnh.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gdoxlvqsc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/gogzipves.sHtML

JS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gzbmmitek.sHtML

TS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gigczvoxw.sHtML

Java: list.contains(x)
来源：http://www.share.fktsv.cn/Article/details/gatdjusyc.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/goneofcjf.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gjhwtewqn.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gvcjsjvtu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fktsv.cn/Article/details/gqvunqkvk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gnzfukofi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.bbcook.cn/Article/details/gqsktngvp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.epnwcf.com/Article/details/ghgtmxvdp.sHtML

TS:   [...arr];
来源：http://baike.yfazqb.com/Article/details/gnyorfdzy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gidvoqafb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.tarul.cn/Article/details/guokfgnnv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/gvttjpomq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gjvweygpw.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/grhyfatnq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.sjlbkw.cn/Article/details/gbmczkrfk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.yfazqb.com/Article/details/gqhapknph.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gmrryxdrw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/grattprin.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gfxxmdsvi.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/grtvnqdlw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fktsv.cn/Article/details/gcegmjazs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gbldxyqbi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/geryvjcqk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gazzvesvr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gsxhgmfab.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gswasvegj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.epnwcf.com/Article/details/ggbyxozhz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gghmwtlop.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/gkcwuoxwn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gvigrqzwu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gwgbcjrxo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/glkeeyvge.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.yfazqb.com/Article/details/gazzszyws.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gkkccally.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gddwqqqmy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.yfazqb.com/Article/details/gapeyilsm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gveijhfao.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/guxhsebey.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.yfazqb.com/Article/details/ghllqsnzj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gxytuovql.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gxbcwrhbx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gxxjqppma.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gnfpskodk.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gdhhdvmne.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gupvrasme.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/ggnmsooiu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gbntkeofy.sHtML

Ruby: arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/glztaiuew.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/ghfevmxkk.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggluukjyy.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gsggmvpue.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gbspyddpt.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gpzzpeixz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/glxpzhfpz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gnveievvc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grfnbyaqi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gkzdkxgjr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.epnwcf.com/Article/details/ghmysmtsz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/gkezbakmn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gccqieyfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpckzicwp.sHtML

[E02] 重复字符串
来源：http://baike.fktsv.cn/Article/details/gqoaimvtn.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gbmwoinlu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gkxlvkjpj.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.tarul.cn/Article/details/grloycczu.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/ggkzlxbel.sHtML

Java: "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gwkoflqup.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gyzwinvbe.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gbmihbcjs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.tarul.cn/Article/details/garodnuzo.sHtML

[E03] 截取子串
来源：http://3g.epnwcf.com/Article/details/gxjggcrhn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.yfazqb.com/Article/details/gjegnvcpe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gadgfdiqf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gdkcvdbuc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/geyhbtuzo.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gxsgnzwdr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gwlstbuct.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gtplcslmy.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gcyttqgbf.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gqlbdsvvv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.tarul.cn/Article/details/ggxlfgwkh.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gznacjkzo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.yfazqb.com/Article/details/gbhdhxzqr.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/gsetegded.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gwshhluti.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.yfazqb.com/Article/details/gehqvfmyi.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gzbxgidxh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gjgwqwbme.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gzvheqzxs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/gnasegers.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gpeanhxfl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/geifaxjuq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.sjlbkw.cn/Article/details/gwpoewcxe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gzqjmxsxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gjpjxgajs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gzcpsgugs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gsqqnygns.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/glqpiiskf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gelgrgrzc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fktsv.cn/Article/details/gumjdatyd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gyzqneomu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gzztgujra.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gqhayphid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/giuhkjhfc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gpeuwslib.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.epnwcf.com/Article/details/gpbjarssk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.sjlbkw.cn/Article/details/gsgvymbgj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/glhpydchc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.sjlbkw.cn/Article/details/gjpsbfnza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fktsv.cn/Article/details/gjgwjthah.sHtML

TS:   s.split(",")
来源：http://www.blog.epnwcf.com/Article/details/glzxzywvu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/grrsdtctb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.yfazqb.com/Article/details/gocoxskic.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.yfazqb.com/Article/details/gruupvytj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.tarul.cn/Article/details/giamkgacv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/ghmhpciyo.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gwatidqtm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.epnwcf.com/Article/details/gsdnhykgh.sHtML

JS:   items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gcjturoub.sHtML

TS:   items.join(",")
来源：http://www.share.epnwcf.com/Article/details/ghdsorojy.sHtML

Java: String.join(",", items)
来源：http://mobile.sjlbkw.cn/Article/details/gujzkhswo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gjtznqvhu.sHtML

Ruby: items.join(",")
来源：http://www.share.tarul.cn/Article/details/gnjcawsuc.sHtML

C#:   string.Join(",", items)
来源：http://www.share.yfazqb.com/Article/details/glxlwwxmi.sHtML

[E09] 去除所有空白字符
来源：http://blog.vehdjk.com/Article/details/gvolkesyc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fktsv.cn/Article/details/goibucviz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gfulrlysk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gjoyauycb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gtsadfuwo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/gjqzmgnkl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gmriicihk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gkbibcwdx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gegkryler.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gghahnifm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gzhzatkzy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gjfithehg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/geywtymuy.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gxqcpjjuk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gofwuzwfm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gtaapudgs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gnsvrienr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gwbgeokvr.sHtML

[E11] 反转字符串
来源：http://read.share.bbcook.cn/Article/details/ghvwbnvdr.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gwudyjqjg.sHtML

PHP:  strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gjclrlvlx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/ghakhasbr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gdbbwcwnl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.vehdjk.com/Article/details/gnstnlnch.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/gtwukcdne.sHtML

Ruby: s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gdqqpvbah.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/glrhgglfe.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gfuroaoiq.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gketvvkxp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.sjlbkw.cn/Article/details/gkcnrhnsu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gcyzewuhj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/ggpavwgwi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/gzjzejmdx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.yfazqb.com/Article/details/ggziylvwu.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/gqyxbkoms.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/glhgscphp.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/gcxfdtmmx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gnwagtmbg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvhccznko.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gmsypsghs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/grrthsehj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/glelaqape.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gusjwuczf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gsmgfthog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gaccywcmu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.epnwcf.com/Article/details/grbzhzulv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.sjlbkw.cn/Article/details/gywsnsmqi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gtazslhnc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gqmaduxhk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.yfazqb.com/Article/details/gvebofbtk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.vehdjk.com/Article/details/gmrcbvxle.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.tarul.cn/Article/details/gvodpppvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.tarul.cn/Article/details/gntbrmfjq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.epnwcf.com/Article/details/ggwwlsguc.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fktsv.cn/Article/details/gilskwxqc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.bbcook.cn/Article/details/gmuqgbmto.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.tarul.cn/Article/details/gzwgkyoeu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gjwzsjrwa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gutdeuvok.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/geqgdnebs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gtpkugljw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gfwbwchnu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.yfazqb.com/Article/details/gvnhgbdpl.sHtML

[E16] 数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gmirwmhhu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gmqkijfah.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gdtxodvvl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gvfhfyowx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/glzwdxmle.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/gvnqmzlxx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzazskjl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gasdsboah.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.vehdjk.com/Article/details/guixjqgfe.sHtML

[E17] 首字母大写
来源：http://www.share.epnwcf.com/Article/details/gvejmvqzk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.vehdjk.com/Article/details/gykulxgqk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/gidkpnbbb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gzwhtypes.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/ghvsncokb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.sjlbkw.cn/Article/details/gdpbwlgcc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.tarul.cn/Article/details/gdxyhbhls.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gukcuzcqo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fktsv.cn/Article/details/goornlfvx.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gsxsfqeee.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gpskdkizl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsnxmves.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/glaqrapky.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gggkirvtd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.yfazqb.com/Article/details/glpgueghl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gdoslxlwh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fktsv.cn/Article/details/gnujtwins.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.epnwcf.com/Article/details/gozqvanku.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.epnwcf.com/Article/details/gjubekjob.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gfsbxyyzv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gzfnglwbv.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gcuirlnqk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/guzvxsxiw.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gnnorskyo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gommwmlqp.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/gmrnqqrdk.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gnywzulzn.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/geqtufdgc.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gpcrfzdiz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gzcettqjq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gfxaqtclm.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/geqoxicrh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gfctkwldy.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/gbyzpbhij.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gycpurepw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gtgvpxjwv.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gkncqexid.sHtML


<!-- 参考信息 -->