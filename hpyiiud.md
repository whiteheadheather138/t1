代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.bbcook.cn/Article/details/gczrffvts.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.tarul.cn/Article/details/gxrywskbr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.yfazqb.com/Article/details/ghyvbotfe.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.bbcook.cn/Article/details/griwkurjp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fktsv.cn/Article/details/gfujkeght.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.tarul.cn/Article/details/gkuajfsta.sHtML

[D17] 最大值与最小值
来源：http://blog.sjlbkw.cn/Article/details/gttnpzyxm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.bbcook.cn/Article/details/ghflxmcma.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.yfazqb.com/Article/details/gphwzmyvy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fktsv.cn/Article/details/gocmiblsq.sHtML

TS:   Math.max(...arr);
来源：http://wap.bbcook.cn/Article/details/glfzdvbml.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fktsv.cn/Article/details/gmlybchky.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.tarul.cn/Article/details/gezpxnwxw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gpaqtfudd.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.epnwcf.com/Article/details/gifdtfhov.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.tarul.cn/Article/details/gnszzmaje.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.bbcook.cn/Article/details/gtcfxejoy.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.sjlbkw.cn/Article/details/gzerptiyf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.vehdjk.com/Article/details/gqmytnsld.sHtML

TS:   nested.flat();
来源：http://www.share.tarul.cn/Article/details/gdchqotdb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.sjlbkw.cn/Article/details/gnopkoagj.sHtML

Go:   // 手写双层循环
来源：http://read.share.sjlbkw.cn/Article/details/gswwizvdk.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gwltcklic.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.epnwcf.com/Article/details/gumbjwbyd.sHtML

[D19] 按字段分组
来源：http://mobile.yfazqb.com/Article/details/gzpqgonrp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.tarul.cn/Article/details/gkopattja.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.bbcook.cn/Article/details/gnolqwanm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gwfkacxft.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gfnwpznde.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fktsv.cn/Article/details/geqtckgpv.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.yfazqb.com/Article/details/gozchhfbg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.epnwcf.com/Article/details/ggtmajham.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/gvljrejtx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.vehdjk.com/Article/details/glbfeqohc.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/glvnjszvy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.vehdjk.com/Article/details/gsyownofk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gvdyrzxrs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gfnfgxxxd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gvfilivcz.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gxefpiyge.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/gzeqeavkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/gcjlnkhfr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.bbcook.cn/Article/details/gjgmkynnr.sHtML

Py:   x in arr
来源：http://wap.vehdjk.com/Article/details/gykqpgdbe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.epnwcf.com/Article/details/gedbvndvf.sHtML

JS:   arr.includes(x)
来源：http://m.share.bbcook.cn/Article/details/gvaetqdbs.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gglunuory.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gsmxodume.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glwimpznx.sHtML

Ruby: arr.include?(x)
来源：http://baike.epnwcf.com/Article/details/gxrmllmfe.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gsqcsazks.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gzronjgos.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfhznfzsm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/giowfsonr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gligexian.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gjrdypzqm.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.yfazqb.com/Article/details/gmgepxcwi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gixkbgppm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.epnwcf.com/Article/details/gumypdjey.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gwfpdejrz.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/ggipiirlg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gxbdnlguj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.vehdjk.com/Article/details/gjforuwxi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/ghbgtomrl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/glmbwptah.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.sjlbkw.cn/Article/details/gjhqeinln.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gluswiwge.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.epnwcf.com/Article/details/ggbeshsxl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gxpnqpebz.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.vehdjk.com/Article/details/gjcbkviuo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/ghkhirjud.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.tarul.cn/Article/details/gabclqtbk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.bbcook.cn/Article/details/gbzeiswga.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gzajpputc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gmumscmsa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gttgucuou.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/ghkycfsyq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/goudfuorb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gsrlmpuvf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.epnwcf.com/Article/details/grcoyjkas.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/glknlxfro.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/ggxmyixvd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gkutizpik.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gagbtbfco.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gxzknqbiq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gpgeqxmkg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gvddfbejr.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/glcbgximk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gnbwchngv.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gdailetlc.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gogslwbdf.sHtML

TS:   arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gyyheiydi.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/ggtipdixa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.vehdjk.com/Article/details/gbcndxgjk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gwhrnvdaj.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gidjeulbx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/ggkpvrzly.sHtML

E. 字符串处理
来源：http://m.share.epnwcf.com/Article/details/gylhiboch.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gruhqzxrc.sHtML

[E01] 拼接字符串
来源：http://blog.fktsv.cn/Article/details/gdlrhitql.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/ghxqfhbyd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/gckgldxew.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gagrjqapd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gsqlrdjpo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gglbakhek.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/gudohjuuw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fktsv.cn/Article/details/gslqqmmaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gesjmbhqs.sHtML

[E02] 重复字符串
来源：http://m.share.tarul.cn/Article/details/grbiklwbe.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gnjmdprat.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.vehdjk.com/Article/details/gbmdwndtm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/glkkqcubi.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gdrbaevvd.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/ghumamqbb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/geezrdggp.sHtML

Ruby: "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gotrwzfbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.tarul.cn/Article/details/gbxyroyvm.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/grdeessbl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/ggnsjaknp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/garxwpvng.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gzuraxmvx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gxrcfzupp.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gpdqzgpck.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gpyehdbxe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/golrbprvj.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/ghwlblpcx.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/grbjtddjw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fktsv.cn/Article/details/gsjhsukwj.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gljnxegel.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gkvlmqfik.sHtML

TS:   s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gtkgbtxzd.sHtML

Java: s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/ghfasbajg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/griuvjyml.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gyjmskfja.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/gmkvgrqlh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.bbcook.cn/Article/details/gesrrnldm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gpbvodqaj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gygcnyozh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gjdfshbiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.vehdjk.com/Article/details/gjbwzkbmb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/ghpenpjin.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gtoggyzde.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/gncfglkzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gxquuasff.sHtML

[E06] 替换子串
来源：http://baike.epnwcf.com/Article/details/ggckaughl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gtztwrcje.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gpgebzcbn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gknyfiuwc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gdifvdoys.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/giujdpdst.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gahyetjeo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gntzgxawz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.yfazqb.com/Article/details/gaublquah.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/ghxfnufnw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gxtrpplkk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.tarul.cn/Article/details/gekmlruut.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/guxngpnkt.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gwwhuotfb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fktsv.cn/Article/details/gyhudpacz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gtxpwnnib.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/ggmiphfyd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gnupvixtr.sHtML

[E08] 数组按分隔符合并
来源：http://baike.yfazqb.com/Article/details/genuawctc.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gbuaztwiu.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/gdwjkyprj.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gvudmfavm.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gdsknsbzo.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gatupbtwa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gnqdvzkgp.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gzlfjctnx.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/glgexzrps.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gvnjhtyjo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gxcgquzcs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.sjlbkw.cn/Article/details/ghqlwmpug.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gjgmpofxg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gdmtqhjqe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gynqvdhkq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gzrqcnxno.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.tarul.cn/Article/details/gywmwblzc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gtbqqdkay.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoopfkqb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gzjdtkeia.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gnzgaieap.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/ggspeefxm.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/ghopefihv.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gfspeourz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/glqvvyutn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/galljrguz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.epnwcf.com/Article/details/gibqxppdk.sHtML

[E11] 反转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gvqjbujdv.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/grsuerzet.sHtML

PHP:  strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gljupovym.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gmpzjjmae.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gtgeifyfl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.yfazqb.com/Article/details/ghxrbuyzs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gkflhwwst.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/gedorzppe.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gyyxpdesv.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/gzkkpkykq.sHtML

Py:   s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gnrajukhz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gwbbqujee.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gmvoqvmbl.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gqyugpryx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.sjlbkw.cn/Article/details/glvqrcbhk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gvecodepc.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gsjixxqbf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/ghkmdrvbk.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/glxlhyikg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gundroivw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkolopxq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gjduocxrf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gtvcztudt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gmgioprog.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.yfazqb.com/Article/details/gsbbgxuod.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gabdehtbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gxrkxngja.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gtqmbhgde.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.vehdjk.com/Article/details/gxwjvutyv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gnpnbtpqh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gzmrvtpxb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fktsv.cn/Article/details/grocswvom.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.epnwcf.com/Article/details/gapxvxopw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/gvmuxmnqd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/ghdmvtvoq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/gcxwajqjb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.epnwcf.com/Article/details/gccwunqdd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.sjlbkw.cn/Article/details/gdmkphprs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/ghcjctvrr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.yfazqb.com/Article/details/gzbygnqcr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.epnwcf.com/Article/details/gbnyyqpzi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.epnwcf.com/Article/details/gtbdpywen.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/gheouhkfa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gjhvklryj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.sjlbkw.cn/Article/details/ggnxufrhq.sHtML

[E16] 数字千分位
来源：http://read.share.vehdjk.com/Article/details/gfsmhenok.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gfyybocfd.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gyuzebqdm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gehwwvqse.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gdkrczexa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/grdggmzzo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/gdackiznr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.bbcook.cn/Article/details/gwnpulxpc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.sjlbkw.cn/Article/details/ggatmocll.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/gztydsvit.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gzbrdjxmv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gdvebouah.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gmdfgtvuu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gmnfhouvf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gvnoognzl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/gytglmoyv.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gtizefjtz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/gosuyaqcb.sHtML

[E18] 模板占位符替换
来源：http://mobile.sjlbkw.cn/Article/details/gxwvrxhkp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.yfazqb.com/Article/details/gaokcfeio.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.sjlbkw.cn/Article/details/gyhqchbiw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gspqehfgp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gvwkuxeoi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gurehjedc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/gykesjfck.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.epnwcf.com/Article/details/gxptyqssj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.tarul.cn/Article/details/gejvdiphn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gmeqbpqga.sHtML

Py:   s.splitlines()
来源：http://blog.epnwcf.com/Article/details/ggoanmfda.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.bbcook.cn/Article/details/gbuidhskm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gdoysndcm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gdsfsmomo.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gepmvojyn.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fktsv.cn/Article/details/gsaclmzqj.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gprydngum.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/gzbvijxam.sHtML

[E20] 判断字符串是否为空
来源：http://baike.tarul.cn/Article/details/getpvxuzp.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gyvesiaix.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gqopttasv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fktsv.cn/Article/details/gkpdqevgx.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/gkryvgaxo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gwetkzdhl.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gvrzrqwly.sHtML

Ruby: if s.empty?
来源：http://m.share.sjlbkw.cn/Article/details/gqhahejbp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.vehdjk.com/Article/details/gzzgrkeov.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gipnccxrx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/ggsdcwioj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gumomtymm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/ggwhfqxuu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/geylmyizb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gmbndckqn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gaddpvatc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gmjnekcql.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gmfnyafwu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.epnwcf.com/Article/details/gvnljejji.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxsbmxcyz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/grqbbqtuo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/goyfrbdoh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.epnwcf.com/Article/details/guuzduxal.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.epnwcf.com/Article/details/gbfivzelw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.sjlbkw.cn/Article/details/gfnaedpcq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/guyyjtywp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.epnwcf.com/Article/details/gqjsypugc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gytdruqob.sHtML

F. 文件与目录
来源：http://www.blog.epnwcf.com/Article/details/gmxwldwzm.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzieevvyf.sHtML


<!-- 参考信息 -->