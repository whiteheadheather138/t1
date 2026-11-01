代发 wailian999

[D15] 去重
来源：http://read.share.fktsv.cn/Article/details/gqwhanwdw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.bbcook.cn/Article/details/gsppoacyk.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fktsv.cn/Article/details/gsoiozrsg.sHtML

JS:   [...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gsxikpghi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.sjlbkw.cn/Article/details/gcdhwwpnc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gyxypkkrh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.sjlbkw.cn/Article/details/grolozvgo.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fktsv.cn/Article/details/gpuahybwd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.yfazqb.com/Article/details/glgphgewt.sHtML

[D16] 求和与平均值
来源：http://blog.bbcook.cn/Article/details/gyydnlyph.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.tarul.cn/Article/details/gcmixfwxi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fktsv.cn/Article/details/grtdebkco.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fktsv.cn/Article/details/gmfdetlul.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.tarul.cn/Article/details/gzhdlkcns.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.sjlbkw.cn/Article/details/guzytxtnk.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.tarul.cn/Article/details/gdeteyrme.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fktsv.cn/Article/details/gtyydxzhs.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gkovypacz.sHtML

[D17] 最大值与最小值
来源：http://read.share.tarul.cn/Article/details/gopoqpzin.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.yfazqb.com/Article/details/gtyluzpdw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.bbcook.cn/Article/details/gjtfrizmn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.sjlbkw.cn/Article/details/gunpfrqqb.sHtML

TS:   Math.max(...arr);
来源：http://wap.fktsv.cn/Article/details/gqvecupny.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.yfazqb.com/Article/details/gupozbnku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.bbcook.cn/Article/details/geqfqowzr.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.yfazqb.com/Article/details/gjqmntkbq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gcagfcbtr.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.bbcook.cn/Article/details/gtngtmdka.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.vehdjk.com/Article/details/gbghuuytw.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fktsv.cn/Article/details/gcimctmym.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fktsv.cn/Article/details/gdyeiahll.sHtML

TS:   nested.flat();
来源：http://3g.vehdjk.com/Article/details/guhruthbn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gxfhnnuvd.sHtML

Go:   // 手写双层循环
来源：http://www.blog.bbcook.cn/Article/details/gqogwihhv.sHtML

Ruby: nested.flatten
来源：http://blog.yfazqb.com/Article/details/gvgnilmzb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.sjlbkw.cn/Article/details/gnxvrlukn.sHtML

[D19] 按字段分组
来源：http://baike.tarul.cn/Article/details/gatgotljc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.vehdjk.com/Article/details/gmvigjjjw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.sjlbkw.cn/Article/details/gabibwsce.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/ghkhuivfk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/gdeoksnkb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.bbcook.cn/Article/details/gqclwcgnm.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gutxjozej.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gzroldnwv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fktsv.cn/Article/details/gbxpzugcj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gkhttzigf.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/ganeagmdq.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fktsv.cn/Article/details/gysgoxjsa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gvgdbqeng.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/ghjcxkcfv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.yfazqb.com/Article/details/gsctzwond.sHtML

Go:   // 手写 map[T]int
来源：http://baike.tarul.cn/Article/details/gfmwvfsiy.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gqckupbvk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.yfazqb.com/Article/details/gqpwdqjbw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.tarul.cn/Article/details/gexvfwvkk.sHtML

Py:   x in arr
来源：http://www.blog.fktsv.cn/Article/details/gojfjpuee.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/grmjdwkng.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gdoljezvq.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gpiacybwx.sHtML

Java: list.contains(x)
来源：http://read.share.vehdjk.com/Article/details/ggfkwelpm.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.bbcook.cn/Article/details/gkzycttlg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fktsv.cn/Article/details/grllpnbei.sHtML

C#:   list.Contains(x)
来源：http://wap.epnwcf.com/Article/details/glfoahydk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gaykdxfzz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsozakbup.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/gbuniiyhc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gtebeklhm.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gbituqiym.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gbqivqeji.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gowijdwrr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.bbcook.cn/Article/details/gwfhaifgl.sHtML

C#:   new List<int>(list);
来源：http://mobile.yfazqb.com/Article/details/guismfhxq.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gboycbcap.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/ghiekuwep.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/giyisfofo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gwpdhsboo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gutqvssbw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gnagyixpb.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gmkitvtns.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/gttwpauxu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.bbcook.cn/Article/details/gcdltszhz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fktsv.cn/Article/details/gbvjoadap.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.epnwcf.com/Article/details/gbikwpnrc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gyxfwudrv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gokdfrouq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/ggtnkxsck.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gmfxwujyl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/grfxouupi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gkexyllwr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.tarul.cn/Article/details/gsoxqnfal.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/goxewfmts.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gihqtluaq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/ggucpjggu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/gvcsremfz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.tarul.cn/Article/details/govyrxvyj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gqmpshkri.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/ggrzjllvz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fktsv.cn/Article/details/gqmtioufj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghnuvnruy.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gfljoasgh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gspnkxxhr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/ghuvhnpev.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/grqakdugj.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gxyeuixev.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gufijroor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.yfazqb.com/Article/details/gblujswsc.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gphaqymzi.sHtML

C#:   string.Join(", ", list)
来源：http://blog.bbcook.cn/Article/details/glvljwtrr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmlwqbmlf.sHtML

E. 字符串处理
来源：http://baike.yfazqb.com/Article/details/goctkqaxj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyuzjyved.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/glxgrtchi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gvkjiznaw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gbmeqiuqw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gzidihdjt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gtgikmmns.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.sjlbkw.cn/Article/details/gwktridih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gbjfhjxlc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gcofudtcx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gyrtbekaj.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gtqnqnfxi.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/ghdotvrzj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.vehdjk.com/Article/details/gtgyphglr.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ggolwileu.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/guxveyajs.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gykllkgqo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.tarul.cn/Article/details/gahqmdsdf.sHtML

Ruby: "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/gsiifykbq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gldtvjyrg.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/geagetqlj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gdfvqzheo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/grkalpckt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/ggquvrnnr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gjccgwhbl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gyrjopshq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gmbyykrsq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gwklvgjln.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.tarul.cn/Article/details/gvpywsvgq.sHtML

[E04] 查找子串位置
来源：http://baike.bbcook.cn/Article/details/giyeukixl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gjjsjrldr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gphshbqms.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gawjbipdx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gsvfynvhu.sHtML

Java: s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gccrvxofu.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/ghaipadcy.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/ggllgnnjb.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gpspbnjtg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gtmejpfvm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwegnxii.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.vehdjk.com/Article/details/ghpmhgghf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gwldnpmor.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.tarul.cn/Article/details/gigsvirgj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/grepqcmon.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gmlutywrt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/gbgjsyzqc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/ggewohgcd.sHtML

[E06] 替换子串
来源：http://www.m.share.tarul.cn/Article/details/ghbdrbzma.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gqcwpnjph.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gworpoagx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gzyqyyrrf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gbhybutxe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/gwjxkjrru.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gfapcuvvx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gzkowliad.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gmgsjhhzl.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gfllubxbg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gqbifevad.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/grfqwwqgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/gobmalapo.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gfmufncoh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/giupttsoy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gstovfozl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gejcmtaeu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.bbcook.cn/Article/details/gchjtseha.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/guwowqwqk.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gbuvzwjri.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.bbcook.cn/Article/details/ggfyvbmya.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gpfidqegd.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/geprprhnj.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gtmpdykde.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gbouuxlrg.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gmmswogxi.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gbmbcgibt.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/ggwkqfaks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/golfhvjag.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gpjbcsjeh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/getoibdwq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.vehdjk.com/Article/details/gsgsautza.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/ggitovmws.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gxwxuyuzm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gdgpcgzvn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gislbypla.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gdcfympgx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gnqrbiuqj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fktsv.cn/Article/details/gxkcoqxti.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/ggcbtmlpg.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gstzfljha.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gredjtbzq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/grfkrkhuo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gkdkptibt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gyynnxphb.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/grwoyxyzc.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gxqmqehhh.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gcfkwnrzi.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gxevkqaco.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/guiyqfdny.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gugwxwdeo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fktsv.cn/Article/details/ghkugfnnp.sHtML

Ruby: s.reverse
来源：http://m.share.yfazqb.com/Article/details/ggcqillam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gsbxyesox.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/ghsgtbjsy.sHtML

Py:   s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gdpuoyrqv.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/ggpaadabh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gfoqmjyat.sHtML

TS:   s.split("a").length - 1
来源：http://baike.sjlbkw.cn/Article/details/gbnrmjyoa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gtbndvpwy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fktsv.cn/Article/details/gbucvdjuv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gkpaxtahu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/guxikwyua.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gkcletrjb.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gptyrtzlu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/guaxowsiv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gqlbncvdw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.bbcook.cn/Article/details/gpfrnjkgs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gtlzigywd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/gojktpryk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/glyxemaos.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gprctibdu.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gihqdkhvl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gqlbnoxle.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/grulnojam.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gdxwzsikj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.sjlbkw.cn/Article/details/gxjsygjfa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gtkqrnigt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gjbqcuyyc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gxuzcmadh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gwnpsngmw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/gwjehxwpf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/geckjxlwr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fktsv.cn/Article/details/gkcwtonfl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.bbcook.cn/Article/details/gdrfjokes.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gajelgygc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.yfazqb.com/Article/details/gwamuebuv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gwwvrazcl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gnecczvdu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/geocaqdsy.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gaugmtrzq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gnlgnavui.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gtmzyckuc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fktsv.cn/Article/details/gvapftnni.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.epnwcf.com/Article/details/gnuhiakte.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.yfazqb.com/Article/details/gntqtppas.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gxszoxegj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.vehdjk.com/Article/details/grnwduxdl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gswkbhdrs.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/ghkdxrejg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gleuhcgco.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gfjzwqwlp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gpyntugyb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/glwscrtxc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.vehdjk.com/Article/details/gvwskczih.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.vehdjk.com/Article/details/gzpfgrkrt.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/glnbjuhpw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.yfazqb.com/Article/details/gjlqoedqj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gjlkkhawa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.tarul.cn/Article/details/gozwrrogl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.vehdjk.com/Article/details/gbbjjivrq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/geavgerqu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/gijqunoqv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gsmooefwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.tarul.cn/Article/details/gibqhxzqu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gggkrqnsd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gdiczxaae.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gwawmjexs.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/grrjrzlba.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gunqzaywp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gnardukav.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.sjlbkw.cn/Article/details/gohwfbbnl.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gjtlauukr.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gvmmxmzup.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/ghrgvhkqh.sHtML

C#:   s.Split('\n')
来源：http://baike.fktsv.cn/Article/details/gzndkpyfq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.yfazqb.com/Article/details/gjngmfnyu.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gajpkwixw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gdbowuvgi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/getmvuqyi.sHtML

TS:   if (s === "") {}
来源：http://read.share.tarul.cn/Article/details/gqcpjydqq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gqnyhcdge.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/grcdfhwrk.sHtML

Ruby: if s.empty?
来源：http://read.share.vehdjk.com/Article/details/gzikrsaiw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.vehdjk.com/Article/details/glrlrvbii.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/grnufhuyf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gmkohabey.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gsforkeyu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gsbbqfjqy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/getuztbdq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gkhndulsm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.yfazqb.com/Article/details/gtyqafwtm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gmhvzrcng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/ghiycxxst.sHtML


<!-- 参考信息 -->