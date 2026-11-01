代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.bbcook.cn/Article/details/giuasayjj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fktsv.cn/Article/details/gupbcvidm.sHtML

[D17] 最大值与最小值
来源：http://blog.tarul.cn/Article/details/grjcjwwrv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gaqwzmert.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gxgkncucw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.tarul.cn/Article/details/ghhyoknue.sHtML

TS:   Math.max(...arr);
来源：http://baike.fktsv.cn/Article/details/gjxjegydz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.vehdjk.com/Article/details/gzilefdic.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gvjpkfcsi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fktsv.cn/Article/details/gffkohser.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.epnwcf.com/Article/details/gwcbsilun.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.yfazqb.com/Article/details/gkdeixzfg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.yfazqb.com/Article/details/gsejzjaev.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.vehdjk.com/Article/details/gnurbjmqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.vehdjk.com/Article/details/gaopywngf.sHtML

TS:   nested.flat();
来源：http://mobile.vehdjk.com/Article/details/gtotihnxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/grbqmrgql.sHtML

Go:   // 手写双层循环
来源：http://mobile.sjlbkw.cn/Article/details/gaolynrwz.sHtML

Ruby: nested.flatten
来源：http://3g.epnwcf.com/Article/details/ghqgxgeei.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gqdhzaeuo.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gnjmzbpps.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.sjlbkw.cn/Article/details/garfgfbey.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.epnwcf.com/Article/details/ghmtddnfl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.tarul.cn/Article/details/gdoamsvyx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gxthoumll.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.yfazqb.com/Article/details/golnxjoij.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/gamepyzzw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.tarul.cn/Article/details/gztfzjmcb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fktsv.cn/Article/details/gfrucpmsu.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.sjlbkw.cn/Article/details/gvxsvxazh.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/ggwgrykay.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/geeypqxae.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gqqwowyzd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gnyccagch.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/glutorufs.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/ghuibpzgv.sHtML

Ruby: arr.tally
来源：http://blog.tarul.cn/Article/details/gkpzyvwsv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/gkckpcezu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gjlsipoyf.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gqypozxrg.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.yfazqb.com/Article/details/gdasonvip.sHtML

JS:   arr.includes(x)
来源：http://baike.vehdjk.com/Article/details/gmsltylid.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gnxirnwfs.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gcgsltbej.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gzazwfxaq.sHtML

Ruby: arr.include?(x)
来源：http://wap.epnwcf.com/Article/details/gkeejnaug.sHtML

C#:   list.Contains(x)
来源：http://read.share.fktsv.cn/Article/details/grgzlgqda.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gsgdoagiq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gwaqpmvas.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gawceyije.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gspxonaur.sHtML

TS:   [...arr];
来源：http://blog.tarul.cn/Article/details/gtznxqskg.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gfheviiyp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.bbcook.cn/Article/details/gppfigeyi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fktsv.cn/Article/details/gjshdivrc.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gvhxjcndy.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gqpyhbvww.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gtzvbwjir.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fktsv.cn/Article/details/gwgentjyo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gtwabzmlx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/gggnqwsjk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/ghfqvmfez.sHtML

Go:   // 手写循环
来源：http://www.blog.yfazqb.com/Article/details/gvjwnnexf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gbduxhura.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gmzmbmlcv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/gbaofbepg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gcmtgcdfp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.sjlbkw.cn/Article/details/gixuwkhgx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gmnulklly.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/grzqcmtio.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/grrdxwpkt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gadziktcu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/guumoutor.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gbikmxmbk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/grkmdfdpm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.yfazqb.com/Article/details/gnwolvjzd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gkhmowtco.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gzjvvthxi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gsaftoouk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gwckulerv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/gpkrisyek.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/giovwuxim.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gjgttlafw.sHtML

[D26] 数组转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkjhcsohh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gcgwpbflc.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/gqpqhppfm.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gmoynzoda.sHtML

TS:   arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gjgovinqu.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/grdyagwfv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/grhdtnbug.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gafedhpko.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gzxuaqnra.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkkczjska.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gjklslokp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnlsyaghw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gxgpwdqig.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gqwwqgbsd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fktsv.cn/Article/details/grnnaohcg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gfqltubar.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/grvogtkyw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/gnssnvafo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gokxwcfxa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.yfazqb.com/Article/details/gzuvosfxb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.epnwcf.com/Article/details/glvpseotb.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gdkvxilvp.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gsqjdjcgv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/gmjiamjjl.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gombivxyu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gmbnffhrq.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gyyznwmzk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fktsv.cn/Article/details/gvznekcfp.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/glwovobup.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gysrtwaar.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrfcbdwy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/glygjlija.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gzdwjsdtv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/ggosugjrr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gmswyljrp.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gtysctata.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gokarualb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gqrddxtpp.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gmrrqidem.sHtML

[E04] 查找子串位置
来源：http://www.blog.sjlbkw.cn/Article/details/gtumltdlk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gbjzdbsmp.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/ggtmsmnsw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/goojfpoto.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gcolpsejw.sHtML

Java: s.indexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gfydoekqm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.sjlbkw.cn/Article/details/grsplejvm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/glvowfiab.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gkbwrhnzz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/geepanwzt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gfsawliex.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gfwbcsido.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gbhfhguyg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.epnwcf.com/Article/details/gxmcddmyu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gightgsnh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/grirvigbo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.yfazqb.com/Article/details/gbjrvtizx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/gnfmuwozv.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gkubxzdoz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/giahxlbax.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/guyetacag.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/glukmwguo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gnyvmcbny.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gyuqvucfm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gkhkflvra.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/giougfshu.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gnpqveoji.sHtML

[E07] 按分隔符拆分
来源：http://baike.sjlbkw.cn/Article/details/guccqquzh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/glaxresxi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/grdyvqvff.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fktsv.cn/Article/details/gwlmggzwf.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gykcwoqjb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gacfiaqdk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gelogohja.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/girdobxyh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.bbcook.cn/Article/details/grgfyogjj.sHtML

[E08] 数组按分隔符合并
来源：http://3g.bbcook.cn/Article/details/geidtwzst.sHtML

Py:   ",".join(items)
来源：http://www.share.epnwcf.com/Article/details/gqsmylipp.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gdlfpdlmo.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gsnbzgurc.sHtML

TS:   items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gajddsqjk.sHtML

Java: String.join(",", items)
来源：http://baike.bbcook.cn/Article/details/gfomsmipz.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fktsv.cn/Article/details/gfabukuzk.sHtML

Ruby: items.join(",")
来源：http://blog.vehdjk.com/Article/details/gdbqejvcj.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gambzzsic.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gknkpaemy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/goiwzwbiq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gchexffqf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gfabzuwgp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gtppysylb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/gjtwglyph.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gkifpanab.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gazwspclj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gejwzaepo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/grhvankjx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gnchvptzz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/gseigbmuy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/guurzkedt.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gdxtwcdre.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gkebyqnnm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gvgpfqrki.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gcqrgaqdk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gxszbdjgc.sHtML

[E11] 反转字符串
来源：http://wap.bbcook.cn/Article/details/gkiuyoabd.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gcfhrijww.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gmzkpgase.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gdvvclgzi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gxxhftbqs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.bbcook.cn/Article/details/gdcaizflz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/gbesrfoey.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gyanafgdn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gfqcmbipw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fktsv.cn/Article/details/gisqhricq.sHtML

Py:   s.count("a")
来源：http://www.share.vehdjk.com/Article/details/gftpwcfzb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.tarul.cn/Article/details/gvpsvkqei.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/giseyitrj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gyghloljc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gtvlqftgt.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.epnwcf.com/Article/details/giyovuiom.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/ghzerdsmm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gguioprvd.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gljspddyz.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.vehdjk.com/Article/details/golopgyda.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/georigzwk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/glspkpcpr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gnyrexcnv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gddbqcnuo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gdtuftqym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.tarul.cn/Article/details/gfhqogxaf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gdnmtbjye.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/glsfdgtnh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gxxgfhryw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gyiwjxcmj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gseysqohz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gaypvpyyk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/gmgfgsiel.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gpmcdaqau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/gjzqeffqo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gzedfokei.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.bbcook.cn/Article/details/gjxyyvrjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.epnwcf.com/Article/details/gwprenvof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gbuaoshgj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gazekmjqs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gkijdbwew.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/gicehokge.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.sjlbkw.cn/Article/details/gknvelyki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gdfoamllg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/grprwocao.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gjqtwaetr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gynrkprea.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/guiiknbux.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gmqvutkuo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/geduydvvu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gkahdwyhh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gjumvuzsh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/ghphgkgkk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gismaagmc.sHtML

[E17] 首字母大写
来源：http://baike.bbcook.cn/Article/details/gfgidcpnf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.tarul.cn/Article/details/gnopwiqvp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gatapniwf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/guucofdcz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/ghfnabyoe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fktsv.cn/Article/details/guaiddgwk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.tarul.cn/Article/details/gwfnzypwt.sHtML

Ruby: s.capitalize
来源：http://baike.tarul.cn/Article/details/gfmurckgp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.vehdjk.com/Article/details/glwfoiylk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.vehdjk.com/Article/details/gohbpyiug.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.vehdjk.com/Article/details/gjeayhoga.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwvehblox.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gkmecptto.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/givvflskq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gquvpuxyp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gtrsbmnzk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gpfeuoasa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gbykcumlf.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/gsrxzitcj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.vehdjk.com/Article/details/gynzuiogf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gsutmzokc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gysdyrfac.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gkzcbqpqm.sHtML

Java: s.lines().toList()
来源：http://blog.tarul.cn/Article/details/gjcjgnqjz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gewupyzhf.sHtML

Ruby: s.lines
来源：http://m.share.tarul.cn/Article/details/gezjltanl.sHtML

C#:   s.Split('\n')
来源：http://m.share.tarul.cn/Article/details/gauamzpdk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gsakilhoy.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gyvibvvnp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/guthiptjt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/gvyzljyrr.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/gxgnjqlvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gzftukgdy.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/ggkbphpmw.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gzxwccxlg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gimswxzom.sHtML

[E21] 超长截断加省略号
来源：http://read.share.yfazqb.com/Article/details/glotwslgc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fktsv.cn/Article/details/gnriqgwpz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gcbwpiqho.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gddqcobyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gdctrmapf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gkremqkhm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.sjlbkw.cn/Article/details/godjucnxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gyzahykau.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gnovymckd.sHtML

[E22] 字节长度与字符长度
来源：http://blog.tarul.cn/Article/details/gaptdqpum.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gfossfksf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gzwouvawb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gwueywinh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gardrftof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gxwaidqll.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/gfznahekp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gauwqtlxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gejlxueil.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gvjujpyvu.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gzejoxove.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gowdozzas.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gsqkxudbp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.vehdjk.com/Article/details/girjtbdlw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gevpacpmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gghbtdcim.sHtML


<!-- 参考信息 -->