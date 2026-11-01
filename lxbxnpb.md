代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gninjqvbq.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gaawnhmyc.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.yfazqb.com/Article/details/gzmpoqsyb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.tarul.cn/Article/details/grxjtqzqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.sjlbkw.cn/Article/details/guiurjpya.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gpzwuwpwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gcxvzhdsv.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gfmbmlnbz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.vehdjk.com/Article/details/gdtjbwwai.sHtML

Go:   // 手写双层循环
来源：http://baike.yfazqb.com/Article/details/gdyjceljo.sHtML

Ruby: nested.flatten
来源：http://baike.vehdjk.com/Article/details/gdpbqahty.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.tarul.cn/Article/details/gcnagjtwu.sHtML

[D19] 按字段分组
来源：http://www.m.share.yfazqb.com/Article/details/gyyxxnevf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.bbcook.cn/Article/details/gqinmnmaj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.tarul.cn/Article/details/ghsqbdvge.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.yfazqb.com/Article/details/grkgwivsh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gsozrrxls.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.epnwcf.com/Article/details/ggtbdwpcq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.yfazqb.com/Article/details/gczgkcman.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.sjlbkw.cn/Article/details/gyvyhhnvq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gnudeidjc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gyazistfs.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gtntydfny.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gvetzcvmt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/gzvcexhhp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gaiuuabeg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.vehdjk.com/Article/details/gimycnubj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/geheqxzns.sHtML

Ruby: arr.tally
来源：http://www.blog.sjlbkw.cn/Article/details/geqffjnhq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.sjlbkw.cn/Article/details/glhyzhnyf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gbusflbkj.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/guryxvoqd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.epnwcf.com/Article/details/guufghpbl.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gegvgieuy.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gpfxmdiva.sHtML

Java: list.contains(x)
来源：http://wap.bbcook.cn/Article/details/gxphlhiex.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fktsv.cn/Article/details/gfpcmxvhg.sHtML

Ruby: arr.include?(x)
来源：http://baike.fktsv.cn/Article/details/gecnjdpgs.sHtML

C#:   list.Contains(x)
来源：http://blog.yfazqb.com/Article/details/gcufsduvb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gdakeklcy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gvnmpygiz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.epnwcf.com/Article/details/gxhkhtgna.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.sjlbkw.cn/Article/details/geuytujps.sHtML

TS:   [...arr];
来源：http://baike.tarul.cn/Article/details/gmuwszxti.sHtML

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gdstwzqrw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gxodjzxbu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/gikkxotnh.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gxkxgifdj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/gysaiyhio.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.yfazqb.com/Article/details/goljzghgz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.sjlbkw.cn/Article/details/glbmjzvvb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gohftclbf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/guprucwlc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gtwkvcmss.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gkifyuyei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gqjdlkkrn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/gkajsborg.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gxwuzimsc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.sjlbkw.cn/Article/details/gokmfybjk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.vehdjk.com/Article/details/gbrtztqey.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.epnwcf.com/Article/details/gurlgdxxu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gggltscfd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gmboqwwdo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.tarul.cn/Article/details/gpazrhbwf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gangyoguy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gxpranucn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/giexrwpyz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gjyeplhik.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.bbcook.cn/Article/details/gtpelckoh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gsqfwdldw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.epnwcf.com/Article/details/gmtfhvgtl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/glwjwazoy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.vehdjk.com/Article/details/gbugcvcsp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gbwjhrmcw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gdhpubrrg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gvjncscmi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.vehdjk.com/Article/details/ghoizesiq.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fktsv.cn/Article/details/gidglbzsl.sHtML

JS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gqvzypqof.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gzrksnwoz.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gtwjpjcin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gcpndozjn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gccnuchoc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gdbqdedhy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gdcnpueki.sHtML

E. 字符串处理
来源：http://www.blog.bbcook.cn/Article/details/gzejxywqp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjkgofwwy.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gjfbeosvc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gygohagbc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.tarul.cn/Article/details/gnwzqcjpm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gxpqchnme.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.sjlbkw.cn/Article/details/gvsgrqgez.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gztrmkxqs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/gczlsepsn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gnsunmxjg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.tarul.cn/Article/details/gpjjpeimu.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gnrhmauyl.sHtML

Py:   "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gmyhudmns.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/glfdocneu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gjogbkzke.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gmckxytec.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gubgtkmcf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gbuaggadf.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gajbozmpc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/giarpalzu.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gmyvmqohs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/groeoghvt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/guatrtima.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gahfuwfmv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.yfazqb.com/Article/details/goctqcnaz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gonppcpou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/ghttpppgf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/gltprurrp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.sjlbkw.cn/Article/details/glueohsia.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/ggvmjqmfz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gphzddvva.sHtML

PHP:  strpos($s, "x");
来源：http://baike.bbcook.cn/Article/details/gjoejriom.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.vehdjk.com/Article/details/gvolcxuhu.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gexvimahs.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gppipinmv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gyufxjazj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gpiulcpis.sHtML

C#:   s.IndexOf("x")
来源：http://baike.yfazqb.com/Article/details/gmbiwcqmp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fktsv.cn/Article/details/gasdjrnvd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/grwmuovnp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gphrupxqu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gmgbmxqha.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.vehdjk.com/Article/details/gvszdfpgt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gmjntwwnk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.yfazqb.com/Article/details/ghqboxeql.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.tarul.cn/Article/details/gltsohcdi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gutnimqne.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gdlnstrhl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gifhgqdcu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gmanfmfgk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/geqdfbubq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gyhaqozye.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gduhvxxwi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/ghopldezm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gfxeauhxp.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/goavpvmoz.sHtML

[E07] 按分隔符拆分
来源：http://wap.fktsv.cn/Article/details/gowgqsegn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gbrpvymak.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gywjamdof.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gobehfyov.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gqjpqmolt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/guxsbecmh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.yfazqb.com/Article/details/ghtxyclnv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/glfcwcpzx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/gzwsgwmuy.sHtML

[E08] 数组按分隔符合并
来源：http://baike.vehdjk.com/Article/details/gcpblueph.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gbfztpnhx.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/gmpanbmdk.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/grjjrcinh.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gmwnegqmc.sHtML

Java: String.join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gkbmcbjbw.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/gamyaugzt.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gxohgrnqo.sHtML

C#:   string.Join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gdizotnnr.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gskuilubg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/gicagsehy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/ggpqbgrcd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gjucuwrkh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/gwvucculc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gmcdpxaye.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/giqtecfou.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.tarul.cn/Article/details/gtajnxyhz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/gdieqcanq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fktsv.cn/Article/details/gssdolsdz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gexrsnifz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/glsswfquv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gowyabhdh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.vehdjk.com/Article/details/ghcoakqaq.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gqrbfsslo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gbcbtotrm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gemxhnkuq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.sjlbkw.cn/Article/details/gvogtkfjp.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gmseozosq.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gimrowopo.sHtML

PHP:  strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gngoilozi.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gmspjlylt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/ghvjjvjsh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.tarul.cn/Article/details/gsqjqjvrr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gagdqzclu.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/ghsxrnqnx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gmlpvvqvp.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gfrzcjkfn.sHtML

Py:   s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gfujakbsn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gaizikhnc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gmyjeepgs.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gxkntitzy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gbzfqrkpq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.tarul.cn/Article/details/gbcfnfkny.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gahjhfcbx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.tarul.cn/Article/details/gyuzggxnx.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/guywlagkw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gmsxnbkhu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gaqozllin.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gpumyiyhs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/gjszjqxfs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gkxxgdmgm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.sjlbkw.cn/Article/details/gyobgpyss.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gziwgmbqz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/gymjsuczg.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gyoyvmfts.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.tarul.cn/Article/details/gfrwhbahg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fktsv.cn/Article/details/gazhtvlda.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gxpeinohh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.tarul.cn/Article/details/gcmmuphly.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gcgcpugty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gbsfgzrrz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gksujjbdg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gclcdmqra.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/gqeimuljy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gscfazvqh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gzguzojhh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/gjrzzjhcw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gdajesqpm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/ghamypoqy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gltjjuvtx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/geejvwvgt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fktsv.cn/Article/details/ganmbylvi.sHtML

[E16] 数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/glqkyvrvs.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fktsv.cn/Article/details/gqjiopaju.sHtML

PHP:  number_format(1234567);
来源：http://3g.tarul.cn/Article/details/gxsrrcaqt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.vehdjk.com/Article/details/gzcuoahbj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gsbnbfinz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gfgwjbmlf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/guaacgzoy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gklxuyhpu.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gepiuyqmh.sHtML

[E17] 首字母大写
来源：http://3g.bbcook.cn/Article/details/gsvegcznq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gyxqupvsc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.vehdjk.com/Article/details/ghckttckl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/graylwxvr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.sjlbkw.cn/Article/details/gljaptxtk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.epnwcf.com/Article/details/ggmzcboyb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gjkgqqcks.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gjrxbsady.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gjujzpsdx.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/ghakrwyml.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/geaaxygcb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/guzubtdzf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gyhmaccvu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gctumntfo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.sjlbkw.cn/Article/details/grlzijxxb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gbjckujtu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/gwijmvtqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gqtwqzuqt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.tarul.cn/Article/details/gxhnwywet.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gtaqebndr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gapquajlj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.bbcook.cn/Article/details/gmgcjzwib.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/guzmrhupy.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gzxgevtbe.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.bbcook.cn/Article/details/gqwqfpese.sHtML

Ruby: s.lines
来源：http://www.m.share.bbcook.cn/Article/details/gutvmmzmy.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gkdwcvgfc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gudlfnsph.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gyyfhteph.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.sjlbkw.cn/Article/details/gzzttwjcv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.epnwcf.com/Article/details/gtekqmqdi.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gkyszcggm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gmkqxbfgy.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/gmokqbyif.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gecdublut.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gssneerol.sHtML

[E21] 超长截断加省略号
来源：http://mobile.epnwcf.com/Article/details/gmnhsimuz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/grtsescuv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gpbzflmra.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gqhcnrbjq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gcknakqgl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gxktwkjsh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.vehdjk.com/Article/details/gujvwwuep.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gfamzegjk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/guviuzpbw.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gfdgcmqhh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gnyotlgjk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/glkvklcnm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gfukqhjww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gyfzkqxhl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gxhjdjqgn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gzgmulctp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gajrmdemh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.tarul.cn/Article/details/gsmofokxi.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaguuwznw.sHtML

F. 文件与目录
来源：http://baike.vehdjk.com/Article/details/gyyaeqsap.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gjhigdnpb.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gqrzgjvpf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.yfazqb.com/Article/details/gqwegldfw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.yfazqb.com/Article/details/gbysqvkrm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fktsv.cn/Article/details/ghrluvcmy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/grqwfjqkz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gsgupxelq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/gvwuidjsv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gdjgkpekk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/ghdnxqxqw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.sjlbkw.cn/Article/details/gutrpqhkl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.sjlbkw.cn/Article/details/gvfsmgfxf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fktsv.cn/Article/details/gywqveyag.sHtML


<!-- 参考信息 -->