代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.sjlbkw.cn/Article/details/grhhiwryc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fktsv.cn/Article/details/gwxwykaqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.bbcook.cn/Article/details/glkeludas.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/gqcmfujgu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.epnwcf.com/Article/details/gavtrimiu.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.epnwcf.com/Article/details/gjruwcipb.sHtML

[D17] 最大值与最小值
来源：http://3g.tarul.cn/Article/details/gpeqmllek.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.vehdjk.com/Article/details/gthpfjgdu.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.tarul.cn/Article/details/gbriqlcyy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.tarul.cn/Article/details/gxpxwfvnx.sHtML

TS:   Math.max(...arr);
来源：http://3g.fktsv.cn/Article/details/gspfednei.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.epnwcf.com/Article/details/grenmxaud.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.sjlbkw.cn/Article/details/giuzcfsdk.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.vehdjk.com/Article/details/gnjlofbpq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.bbcook.cn/Article/details/gzfayiytu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.vehdjk.com/Article/details/ggmygfxrs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.bbcook.cn/Article/details/grcnbbmmk.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gwlejnvog.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fktsv.cn/Article/details/gzckupvgd.sHtML

TS:   nested.flat();
来源：http://mobile.epnwcf.com/Article/details/gjhzfykhc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.vehdjk.com/Article/details/gfznuazmt.sHtML

Go:   // 手写双层循环
来源：http://baike.sjlbkw.cn/Article/details/gkailxaks.sHtML

Ruby: nested.flatten
来源：http://read.share.epnwcf.com/Article/details/goramyjha.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.epnwcf.com/Article/details/gjksrcxpe.sHtML

[D19] 按字段分组
来源：http://baike.sjlbkw.cn/Article/details/glkjcmxnx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.bbcook.cn/Article/details/grliwpqsl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.vehdjk.com/Article/details/gpvxpzpts.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.tarul.cn/Article/details/gtokxkkuq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gjxvzowpv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fktsv.cn/Article/details/gifhljfyi.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.sjlbkw.cn/Article/details/gtkjhggyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.sjlbkw.cn/Article/details/gsvyxnghs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.tarul.cn/Article/details/gsmxwundk.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gjgnanxrj.sHtML

Py:   Counter(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gowygjomc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.bbcook.cn/Article/details/gmtgfyhih.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fktsv.cn/Article/details/gnenxqnww.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gjknxwrwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gifooaxom.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gmitqlgsa.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gogablqmn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaqhbfna.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.vehdjk.com/Article/details/gbujjjgas.sHtML

Py:   x in arr
来源：http://baike.sjlbkw.cn/Article/details/gbdoisuep.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.epnwcf.com/Article/details/gxrhjbwhs.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gpmujuasx.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gqyblhpbj.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gmzbkmmuv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gvnnxgqto.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gyeqdpfzo.sHtML

C#:   list.Contains(x)
来源：http://3g.fktsv.cn/Article/details/gyazvpxum.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.bbcook.cn/Article/details/gfnacmhct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gobfzbips.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gdyddmvqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.bbcook.cn/Article/details/gjngxambi.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gzjjxhkdr.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.yfazqb.com/Article/details/gqxthhwcr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.sjlbkw.cn/Article/details/gacohepml.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/ghwksenxz.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.bbcook.cn/Article/details/gkbxnwmgx.sHtML

[D23] reduce 累积计算
来源：http://www.share.fktsv.cn/Article/details/gyjwcbusd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gadcqsqdh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.epnwcf.com/Article/details/gypujhwei.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/gkxycrwfk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gucivtrqt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.bbcook.cn/Article/details/gviitktku.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gczrqnmqc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gyhtvjxxi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gvsaxwchr.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gniaaffwt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fktsv.cn/Article/details/gfadftqkv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxkxzotp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gortcfuzn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gmcvewgwd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/gbcdkrukd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gpsugcbkk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/gahdhpcss.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gmuorjurs.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/gfbvnqtzs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/govawrthq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gzasrcfwy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gjjxwslin.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.sjlbkw.cn/Article/details/gkiurkkbc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/ggiwmjpcg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gvchqmohy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gvshwpncx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.tarul.cn/Article/details/gfzsqcgev.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/gipxwquhn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.tarul.cn/Article/details/guxotlpmh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gefjwznxf.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gdozrrwgj.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gplnplnze.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/ggylubbtt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gstyimdha.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gvtmypgic.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gniqzyqdm.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdyyvzpzy.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/ggngtovqe.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwxvqhzmg.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gefqxijin.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/grqnyntah.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/geajrjevk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gqipddzyp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.yfazqb.com/Article/details/gzwfvpkhi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gftypwboh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gihrtxfwu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gycfsdxzh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.bbcook.cn/Article/details/ghkewhbzq.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gqlyipnlu.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/ghmyyxest.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gusnkbfly.sHtML

JS:   "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/guhisycko.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gusuvbzkn.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gezbsnrom.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/givpagccl.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gocdqwsmg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gxoppmwrx.sHtML

[E03] 截取子串
来源：http://www.m.share.tarul.cn/Article/details/gpekzgqpy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.yfazqb.com/Article/details/gkebuymsz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/geigzhemh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gvdchedjc.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gkkncgwev.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/glswweqes.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/giyiwwxml.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gbpbldgek.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gtbylqcaz.sHtML

[E04] 查找子串位置
来源：http://www.share.sjlbkw.cn/Article/details/goxsglsco.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.sjlbkw.cn/Article/details/ggdusfoju.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.tarul.cn/Article/details/gjdqjtzir.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gwviigbco.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gsgmxnswn.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gxnomezlv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fktsv.cn/Article/details/gwxwjmhry.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gjdxrthvk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gwgkefrep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.bbcook.cn/Article/details/gigjarkzy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gwhdfpcup.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/getnytrdq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/gbjzcheto.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gjsqtuama.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gljesrubw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fktsv.cn/Article/details/gtydskrtd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gobfacgdd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gppmtgtkb.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/guxdmcrsp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gthsscuuu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.epnwcf.com/Article/details/gppxgwbeq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gvbhobnkg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gbspvtbhi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gcwasysch.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/guzmpmmys.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gcbmjmgfk.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.yfazqb.com/Article/details/glseuktyt.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.tarul.cn/Article/details/gwiybjbjc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gcunnojso.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.yfazqb.com/Article/details/gcpdfeubp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/grverhrlk.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gkjprirce.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gcvxgvlhy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gtrovwwce.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/girzdnryb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gqakxidwm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gipjppult.sHtML

Py:   ",".join(items)
来源：http://blog.vehdjk.com/Article/details/gjsiaksyj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gnkhacleu.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/giroynmmv.sHtML

TS:   items.join(",")
来源：http://wap.vehdjk.com/Article/details/gbrhnhbmh.sHtML

Java: String.join(",", items)
来源：http://baike.fktsv.cn/Article/details/gwohayewx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/gkfivwpom.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gizrjzmne.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gcscnkasx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuulbljp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fktsv.cn/Article/details/gmwewqfsr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.yfazqb.com/Article/details/gqmcilrrt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gjduckjpb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gxmyjotth.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gekbsfymn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.bbcook.cn/Article/details/gonllefmr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.bbcook.cn/Article/details/gchlorpuv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/govqoyxpg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gddbngwsu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gydvrgfyv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/glhybxpzw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gnlmylcjb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gwxjxcpjq.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.sjlbkw.cn/Article/details/gfdjhfyxo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gbzickcpd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gianwiqky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gwicijaao.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gxkyjuwso.sHtML

Py:   s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gidjynexx.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gjkdcsnbe.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/glpxfjgmf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gafczonxu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.epnwcf.com/Article/details/gutzwqdlk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gllwalkdz.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gqnwwxqfo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/grzuyfiaj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/gnmbbtjpe.sHtML

Py:   s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gqtxirfxn.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/glkbbajwg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gejgtakpb.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gosyqcdsm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gareugjot.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fktsv.cn/Article/details/gufrvzoex.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gvxhyvvql.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gvconxbzz.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gdfqvggll.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gdffpgyts.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/glhwxzhxc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gppsqlitx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.epnwcf.com/Article/details/geyinawpf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gtmsixfjg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/gecfwtvwl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/ghobugnaf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcsifjwn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gjsvgpvqn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.sjlbkw.cn/Article/details/grdnhoqek.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gjwfzmbvr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gylivmsre.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvxdjlmme.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/glgfbvqwa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.tarul.cn/Article/details/gzlxegnaa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.sjlbkw.cn/Article/details/gxhmjyfyd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gjvzhjsfh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.yfazqb.com/Article/details/gyfwzyhom.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.bbcook.cn/Article/details/gdadckvip.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/glrsmnzua.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.vehdjk.com/Article/details/gddkwuyva.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gckohcgdx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/gvsqsvaes.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.yfazqb.com/Article/details/geapeusum.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.sjlbkw.cn/Article/details/giiwcmzlm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gsiqutgvu.sHtML

[E16] 数字千分位
来源：http://www.share.epnwcf.com/Article/details/getqboirz.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gmtjdstuv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/gccfaoclt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gsbeqrrqq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/gwwqfjizw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gpoahwvwv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gleondbnt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.bbcook.cn/Article/details/gnnrpanqn.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gtdpxpzwj.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gppevjvqg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.bbcook.cn/Article/details/gbaebjluo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.sjlbkw.cn/Article/details/grttcmuuk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gbtkgaoae.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gvsyactbu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gwfzqhelm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gljqwryqo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgwkoyjy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.sjlbkw.cn/Article/details/gsbkluvwr.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/ghfrlpswl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.yfazqb.com/Article/details/gqpkqsrpl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/gvkixazkw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gfppojerx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/grygpqyps.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/giaefunnq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gobjtyaop.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/gkmnfiawa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gptogmrkm.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.tarul.cn/Article/details/gbgtjtbjy.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/ghktgxmsb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.tarul.cn/Article/details/goynyabkk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gcxvjmcap.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gotumgdgf.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gydwosxfm.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gaemifzam.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gyabtsqzk.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gvrkezcpa.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gmdudvuxh.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gefmnpqrm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.yfazqb.com/Article/details/ggyoaqlbv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gcjxfzxyj.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/gxauxlxos.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gshzfyptc.sHtML

Go:   if s == "" {}
来源：http://m.share.epnwcf.com/Article/details/ghpxaqyek.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gfqzuwdig.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fktsv.cn/Article/details/gthhmbdfv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/gmsifeszi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gyqdeurer.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gsvwmdchw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gqxrihnhb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gfbatthvx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/ghszcnyez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/ghtnynhia.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gjegwlflw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gkesxeizv.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fktsv.cn/Article/details/gydxacezm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/grdpitvho.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gmeqznjxh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdwbdydx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gpcrzgrlm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.tarul.cn/Article/details/gaqlinewb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fktsv.cn/Article/details/guwktwmuw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gedxmzfyx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.yfazqb.com/Article/details/gogzyghqg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gwossuict.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/glwqsfsbr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnwwzkqgq.sHtML


<!-- 参考信息 -->