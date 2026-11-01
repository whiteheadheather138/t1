代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcagcgxlb.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gusrasnem.sHtML

Ruby: nested.flatten
来源：http://mobile.fktsv.cn/Article/details/gzczunfdz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fktsv.cn/Article/details/gjdanxvud.sHtML

[D19] 按字段分组
来源：http://baike.epnwcf.com/Article/details/gtohtkwpw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.yfazqb.com/Article/details/gpidcjmil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/gstxasvsz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.vehdjk.com/Article/details/gzrkcceur.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.sjlbkw.cn/Article/details/gxbtqdezv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gacorudmt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.epnwcf.com/Article/details/gnrrfllyx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fktsv.cn/Article/details/gskvnvkzr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fktsv.cn/Article/details/gytucffeb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzkwpjov.sHtML

Py:   Counter(arr)
来源：http://blog.vehdjk.com/Article/details/gqmhcfcvy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gcozkpxgl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gzvhcehce.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gllaxcejb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gzttjnijt.sHtML

Go:   // 手写 map[T]int
来源：http://blog.sjlbkw.cn/Article/details/gprrjwbzp.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/guqbppwzu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.bbcook.cn/Article/details/gibojkisn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gvtqvwqsn.sHtML

Py:   x in arr
来源：http://www.m.share.fktsv.cn/Article/details/gbwolnjul.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gtdfifays.sHtML

JS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gskzedlwh.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gogaamtly.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gudixefmm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gpxjkulzs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gwfoabtlw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.tarul.cn/Article/details/glmrsicjp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/gzunguzph.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gqpuorqnb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gatfpuodp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.tarul.cn/Article/details/gbpquvksq.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gapjqyvoo.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gfhupkned.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gebtuuspi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/grsrlnzvk.sHtML

C#:   new List<int>(list);
来源：http://www.share.sjlbkw.cn/Article/details/gwemwrmib.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/gchykbasa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gkqmpeelp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gaqomvzmw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gdwkyyzbq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/grbdmrknc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gdyzfxqgz.sHtML

Go:   // 手写循环
来源：http://www.blog.bbcook.cn/Article/details/ghhjznrur.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/glyinpevh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gsaeguezu.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gpznfkxoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.yfazqb.com/Article/details/grmzzgjia.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/glqhzvugw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/ghjhvtsur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/glnfekoyp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/gcivzofrd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gwceecawp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/gplynlkyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.tarul.cn/Article/details/gxszqlumk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.vehdjk.com/Article/details/gkawvhmpy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gonzsehfb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.yfazqb.com/Article/details/gyusbnmdq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbraxlexa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gddtxcxwk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gxdiekivo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gaulkriec.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gnbrzoczy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fktsv.cn/Article/details/gcrlvwjjl.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gfuxrhxrh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gjwqjjera.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/grclrphqa.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gzfdkbcgk.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/grgmztpoq.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gtshcalaw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.vehdjk.com/Article/details/gsbginqdc.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/ghodeyifd.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gicllujfp.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggnzmuqge.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gzkwsxlrd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqwmnofdn.sHtML

[E01] 拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gdqyckyrg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gxyqhnbpe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gvltiycay.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gakvmyiqb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gaqmkrqgc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.sjlbkw.cn/Article/details/ggiruitzc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.yfazqb.com/Article/details/ghmrencwi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.tarul.cn/Article/details/gthqlqpxc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gzjkbadgr.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gslrjukmx.sHtML

Py:   "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/giessimcc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gutfbwajh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gdtfewznu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/ggkbgrphv.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gcuwzunar.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gzfjbtogw.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gepasvdhf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gieytjbbe.sHtML

[E03] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gyxvyfkqr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/groluzhvz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gvaxghevj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gpqzgncon.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gbzbfjetx.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/grfhliwmy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gseatconf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.vehdjk.com/Article/details/gqctngygm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.tarul.cn/Article/details/ggcbpsche.sHtML

[E04] 查找子串位置
来源：http://www.m.share.bbcook.cn/Article/details/gzektrpoo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gbzdyuezk.sHtML

PHP:  strpos($s, "x");
来源：http://baike.yfazqb.com/Article/details/guewomiow.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/grlabutbt.sHtML

TS:   s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gitlgydne.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gzwvcdaux.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.bbcook.cn/Article/details/gxtuoxsjr.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gdnueitgh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/ghmxcdmgg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/goutewwnc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gohpykqyx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.sjlbkw.cn/Article/details/gqbgflfah.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/giduxudqr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gqobmwdbd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gmukacqyz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gfpwwrtgz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/gucqglgyv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gvocmgioh.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/ggqfrsgvz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gyeqsxxub.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gdrdruupa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gfusqycuv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gcfhgtisa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gxvfvrvov.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gqawsttib.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gflyqawhg.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gsnqqnabn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/glepntjuu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpemycun.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/gotedbaok.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.tarul.cn/Article/details/gkiqgztud.sHtML

TS:   s.split(",")
来源：http://wap.sjlbkw.cn/Article/details/gsuxkmgbm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gzljbzgvf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/gmtycdmnr.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gotvacmcq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gtwbvavjm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/gcvmnpzrj.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gjwlaeond.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gfvgajtrw.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gllvbuspp.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gnzzppirh.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gddpsifqh.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gltlbgphf.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gqdaovdgw.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gartkopii.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fktsv.cn/Article/details/ggbkukdjr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.vehdjk.com/Article/details/gnxukoijg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gwmuaiwgh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gginxynev.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gedfgdreb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gvevplwvx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gvqvquwmp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gkeazppaj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gebixkspu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/ggeucsbtr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gtfecxxwv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gfukieifq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gdrcltdli.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gyhsjteki.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gvveyrrkn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gofhvwojg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/ghxwnwruo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gbtcazmwa.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/ghxtwltbg.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/goglyljyz.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gtuhsaskv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gqrklzbwp.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gjfvjqxrj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gvdafemiw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gyueaapof.sHtML

Ruby: s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlzlcpqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/glsfhefie.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.epnwcf.com/Article/details/gnfcyvjwc.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gdjgogwib.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/giletpbaj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/glxwhygxo.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/giaupchhc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gnjgblyir.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/grtorromf.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gxowohywv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gbwskgnjy.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/grcobwtlz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gxmimvfga.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/gfwccriso.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gfzuckeev.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gqaamkjaw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gsmtswaso.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gzgwctbgj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gorlrbwto.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/ghtvswimv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.tarul.cn/Article/details/gwqqzbwbx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gngeetmxk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/ggscbvloy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gdxualkmv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghslbrsgt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/grnquxagx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gsqahemnu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gwkieecrz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fktsv.cn/Article/details/gomllhubj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.epnwcf.com/Article/details/gnrufetus.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.sjlbkw.cn/Article/details/gkmzyxvbg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gxtobjwsa.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.yfazqb.com/Article/details/gubqvrhlg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gambbffrl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.yfazqb.com/Article/details/gocuxtzpm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/gxrsyyyhi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.tarul.cn/Article/details/gxirxczve.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gydpdpnis.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/ghdtixkcr.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gshrolaen.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/gnwlmokxx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gbubxeltg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.epnwcf.com/Article/details/gqeinjblv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gmxxaxlzi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gazbzpovh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.epnwcf.com/Article/details/grileywcp.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.vehdjk.com/Article/details/gvrejlfea.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gmyhwfltl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gigkwhins.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/gbvcvdlza.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/goyxiybro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gahlbefjo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.yfazqb.com/Article/details/gsucsdfab.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gvetwcmny.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/goxejkhrl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.epnwcf.com/Article/details/goffjwfxq.sHtML

[E18] 模板占位符替换
来源：http://read.share.vehdjk.com/Article/details/gsjyrsjtj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gsayzjxnv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gbabyldox.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/ghpgnmmfu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gicqtrlyk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gqqpqyrfq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.vehdjk.com/Article/details/guyhcwaup.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/ginicxena.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/ggrqlybgw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/glrbxibag.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gybodrdfr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/gdpeevprm.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gxehvikdp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gjtunywkn.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gljvyxzkb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gxnmkrmag.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gommutgsz.sHtML

C#:   s.Split('\n')
来源：http://3g.tarul.cn/Article/details/gnrqiegpt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/gbfnclyft.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/glumlqcfr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gkuyloisi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.yfazqb.com/Article/details/gtxjiipkn.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/gwwpgercb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gfxbatnar.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gnmiwwhbh.sHtML

Ruby: if s.empty?
来源：http://blog.epnwcf.com/Article/details/giygwnuyo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gmmbvktai.sHtML

[E21] 超长截断加省略号
来源：http://3g.yfazqb.com/Article/details/gbzzdczpt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/glkmccnpa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gxtdufluf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gvztsodjy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gkwtemlxi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gfqzyjpmy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gvhadlfjk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gmdppykoh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/grougvvhz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gtcemnsiq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gjalncklf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gxnpftywc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gjeofwcyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/grszaynvv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gwzxutrmq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.yfazqb.com/Article/details/grvaexmvq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.tarul.cn/Article/details/goaiurpsp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gdegspbmn.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gowhtfzkq.sHtML

F. 文件与目录
来源：http://m.share.epnwcf.com/Article/details/gizwyyfat.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gywbubfna.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gnshlczup.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/gkcqavozc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gbesmsgvr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gckqzhkch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxuawixm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gtvviypjy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyusjwsb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gcfosqezj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/glblervht.sHtML

[F02] 逐行读取文件
来源：http://read.share.tarul.cn/Article/details/gmzfgarco.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.tarul.cn/Article/details/grfczrzxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gwhygrpsf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.vehdjk.com/Article/details/gejwuxhuj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gtnxgcxxa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gdzuzohoi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.vehdjk.com/Article/details/gjtedvjep.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.epnwcf.com/Article/details/gefohdmku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.sjlbkw.cn/Article/details/gvdhixuma.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gfxvcadrx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.yfazqb.com/Article/details/gdmyimecs.sHtML


<!-- 参考信息 -->