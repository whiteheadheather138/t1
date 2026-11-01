代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.tarul.cn/Article/details/gphebtuzp.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.bbcook.cn/Article/details/gtwufnbku.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fktsv.cn/Article/details/gayxjravg.sHtML

TS:   nested.flat();
来源：http://3g.tarul.cn/Article/details/geimpfidr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/gxvjwjeqp.sHtML

Go:   // 手写双层循环
来源：http://read.share.bbcook.cn/Article/details/giaulnfpm.sHtML

Ruby: nested.flatten
来源：http://wap.yfazqb.com/Article/details/gazirucju.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gwhwzyepp.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gajbutgci.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.epnwcf.com/Article/details/gyxajayhk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.yfazqb.com/Article/details/gfxmevnfj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fktsv.cn/Article/details/gydwmpnzv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fktsv.cn/Article/details/gvhjyrecs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fktsv.cn/Article/details/gicozlspo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gnmeibjbk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.sjlbkw.cn/Article/details/gfzjivfhz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.yfazqb.com/Article/details/gkxtkavld.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gqktdxsst.sHtML

Py:   Counter(arr)
来源：http://www.blog.fktsv.cn/Article/details/ghfqzofvb.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gnxvzrrai.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fktsv.cn/Article/details/gczypmjrq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/glxednrqb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.yfazqb.com/Article/details/glfkpsfjz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gwwksxiky.sHtML

Ruby: arr.tally
来源：http://baike.fktsv.cn/Article/details/girtiqpzd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fktsv.cn/Article/details/gyreijtjx.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.vehdjk.com/Article/details/gbvbnqgyr.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gybhsxzvw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.sjlbkw.cn/Article/details/gmlyrbxeh.sHtML

JS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gjoyqerry.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gwdeprkqg.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/ggwkcotjg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gbmuqzasj.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/genzzdokn.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gntmbkiie.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/gmwmxetgx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.tarul.cn/Article/details/gjoytmfwc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.tarul.cn/Article/details/gefqmxbqb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.sjlbkw.cn/Article/details/gzugptahr.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/gscvmcvdh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gdjrylkmo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.epnwcf.com/Article/details/gilurjjzd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.sjlbkw.cn/Article/details/gzyzmmkxb.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/glhlnzmco.sHtML

[D23] reduce 累积计算
来源：http://baike.tarul.cn/Article/details/ghysoottx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.yfazqb.com/Article/details/gdkrjhyfb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gfjkbqasg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/ghxobsblr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gruthesyw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.tarul.cn/Article/details/gkafmzceu.sHtML

Go:   // 手写循环
来源：http://www.blog.tarul.cn/Article/details/gezxvfuyh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/geqeqduvn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gwwwjnsye.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gtmvmemfn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/gzkhqcjhq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gsqgsagqm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.tarul.cn/Article/details/gpjhhslwx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/givivxxog.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.tarul.cn/Article/details/glzimoffj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gnnpliksk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/gxhfispfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gexrfgejn.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fktsv.cn/Article/details/gnzvvncjq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gpnrnqgle.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.sjlbkw.cn/Article/details/godrtjrgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/gepjwckgh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.epnwcf.com/Article/details/ghafipokt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gpbfaphgz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.vehdjk.com/Article/details/gapmzdkse.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gwlhflrgi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/ggjerbfvm.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/glfxdkgxm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/grbprvdoo.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gieyoozog.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gernhyqxg.sHtML

TS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gemcydbbj.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gespssdmf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gsswarvtp.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gehkeacfg.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gnhpspuiz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnnnjhnhk.sHtML

E. 字符串处理
来源：http://baike.epnwcf.com/Article/details/glyskocxr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmtvrhmdn.sHtML

[E01] 拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gynamxyow.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/gyrbauiem.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.epnwcf.com/Article/details/gatjlrwuw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gciqhweob.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gujltlhwa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.tarul.cn/Article/details/gzjlaaejr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gggnycbgv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gdevnipiw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/ghofnumik.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/gfutcdlez.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/guksicggn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fktsv.cn/Article/details/gjywlqkok.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gqdbcrild.sHtML

TS:   "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/ghvnereqo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gdtvwvpnp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gcdqdjzha.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gqidmibxb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.tarul.cn/Article/details/ghndowzye.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/giazbniaq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/ggehqpmca.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gcrdowvee.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gasstwtlk.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/glqgtlprw.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gxboddvgc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.epnwcf.com/Article/details/grhzreewc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gjvyfmslu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gkntijyda.sHtML

[E04] 查找子串位置
来源：http://www.share.bbcook.cn/Article/details/gsaoarlid.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gemosqjnw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/guzjsqpxc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxyrjcrmw.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gxavguuyn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gfmjuttkb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.epnwcf.com/Article/details/gtvlcbhfx.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gucrceamm.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gzccqgnck.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gxiuydcji.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gmqbrbpac.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.tarul.cn/Article/details/gealxqtbp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/ghilmwmab.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.vehdjk.com/Article/details/gncgbijhm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gxnfsrbes.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/gmbbpdtpc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxfpdexho.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gvywtlzky.sHtML

[E06] 替换子串
来源：http://3g.sjlbkw.cn/Article/details/gsyitzior.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/glmtjjnkr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gwqshztjb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/ggxbczjdl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/goejmensk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gzxhprwcn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gshvlcjoo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpawsywn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gvaxynicy.sHtML

[E07] 按分隔符拆分
来源：http://blog.yfazqb.com/Article/details/groolwmtu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.bbcook.cn/Article/details/gjbncggfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gjpunyaai.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gogfwjzke.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/grekdcfzw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gkxmsivdn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.tarul.cn/Article/details/gvwgpclay.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gbeqsifte.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gnihmjeji.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gpgyuxcjd.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/ghdvqopre.sHtML

PHP:  implode(",", $items);
来源：http://www.share.tarul.cn/Article/details/gkpjnnrba.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/ghoprtzpl.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gcodidkbu.sHtML

Java: String.join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gonypuvzo.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.vehdjk.com/Article/details/gmtlwymkt.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/glfufqvly.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/gsqqujbye.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/guasqydym.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.vehdjk.com/Article/details/gaucmqihc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gjelnxkgt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gwxemebdj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gelggutjx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/girczlzox.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.bbcook.cn/Article/details/gjpekuglb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.yfazqb.com/Article/details/gcfhfspkx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gnpumcblr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gkeshupyi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gmazyfxav.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/glmhttttf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gfbuxavzb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/glatsiinm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gssxcqefe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gtxrliugn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/gjchnfzrt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gnvkbybwb.sHtML

[E11] 反转字符串
来源：http://baike.vehdjk.com/Article/details/gugtejqoj.sHtML

Py:   s[::-1]
来源：http://baike.fktsv.cn/Article/details/geykrogea.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/ghnhgmvcq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gruaqelne.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gxrhibjix.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.vehdjk.com/Article/details/glcvfgaej.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gnvytkfxr.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gbeajmnxo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gtxbiyiam.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gaybdwgmo.sHtML

Py:   s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gwwlbqihp.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/gquiuafgj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/ggxowimyl.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/geeroxwns.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.vehdjk.com/Article/details/gkgxpytwq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gpzadcydi.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gzilibvmu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.bbcook.cn/Article/details/gcgkpvhht.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/gpwpgreso.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gwhiltcyf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.tarul.cn/Article/details/geeplsiro.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gvofyurty.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.tarul.cn/Article/details/gpgiyvirl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gdjopiram.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.tarul.cn/Article/details/gvyvispcz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gvudxzwsy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.epnwcf.com/Article/details/gcxnsagmp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.yfazqb.com/Article/details/gditpksal.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/gsymtiair.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gdgfjqays.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/ggogamdyo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gxavvjyct.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.vehdjk.com/Article/details/gyzueetsb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/guqnikalo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gopevehyo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gflmopmvw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/groloncuf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnqvmabej.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.bbcook.cn/Article/details/gvriaplee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gsuorahuy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.vehdjk.com/Article/details/ghqlqdepb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gypnbpjiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gitqdjroj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gundlqxlx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gzcragdia.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/gkvkignro.sHtML

Py:   f"{1234567:,}"
来源：http://3g.epnwcf.com/Article/details/gitpujbcf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gicbjrqoz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gfyuscxkb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gcdoxxecw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gdzqvwkgx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gferpjlwy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gjoeepace.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghipzzkks.sHtML

[E17] 首字母大写
来源：http://m.share.epnwcf.com/Article/details/gjvedyuqm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gtcqwaqys.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.sjlbkw.cn/Article/details/gtgtscudf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/ggprwlflo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gbwoyiupv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gkrmcotzn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/grwfdgrbj.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gzbrcsemh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.vehdjk.com/Article/details/glhlmewdf.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.epnwcf.com/Article/details/gmwasuije.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.vehdjk.com/Article/details/gbocdbknx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gqfvdbxyu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/glnsijqqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/grbsvddrs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/glwhowonx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.bbcook.cn/Article/details/guvhzvteu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gseatqqvj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gcklkegxy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gxvrcuvrr.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gghbhobbq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/ggpwtcmpn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gjwkuwgtd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gsbuvjnkq.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gsweoolyz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gfkkivnzj.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjgtoegj.sHtML

C#:   s.Split('\n')
来源：http://read.share.yfazqb.com/Article/details/gvbysqjok.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/guiwvsxvn.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/ghhcqwwzk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.tarul.cn/Article/details/gjccfdiux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyqevbkqd.sHtML

TS:   if (s === "") {}
来源：http://read.share.epnwcf.com/Article/details/gtvofqzem.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gouggukjr.sHtML

Go:   if s == "" {}
来源：http://www.blog.bbcook.cn/Article/details/gbxpqcqri.sHtML

Ruby: if s.empty?
来源：http://www.m.share.yfazqb.com/Article/details/gqjarkfpl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.vehdjk.com/Article/details/gbbvjwqbj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fktsv.cn/Article/details/gfdjfszca.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/gxzpmqolm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gmocxyalj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gfqkjvptw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gvqbeegvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gmvnunwxi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fktsv.cn/Article/details/gddonpbbq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gwvxnjonq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gcenxpjxj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fktsv.cn/Article/details/gsciznrlc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/grkzqoklr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gwietcfpr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/guzhbqzyz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gzpbayyfd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gsnrajhoc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.epnwcf.com/Article/details/gsihazbar.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gnyhprcjo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.vehdjk.com/Article/details/gbgbzhynj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gfqwgwtvi.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gvlfmliov.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpkxlrxug.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/ggokyxayk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gdfnsjwsl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/guoijabql.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gjfsvtpfq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gtcsewwhv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/geyiubkxr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/gvcqpyueo.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.tarul.cn/Article/details/gkfafehuh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.vehdjk.com/Article/details/gjuqomzov.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fktsv.cn/Article/details/gdpyteoas.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gucjranjt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/giitstgta.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gvvemntzp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gfdfcpphm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/grpsdlphn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.yfazqb.com/Article/details/gyizcxapa.sHtML


<!-- 参考信息 -->