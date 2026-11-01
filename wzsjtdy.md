代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://read.share.yfazqb.com/Article/details/gwmqencgd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gqepddqce.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.epnwcf.com/Article/details/gmjtgnfvf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fktsv.cn/Article/details/gwmfckioy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gmvrjrayf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.vehdjk.com/Article/details/gyksutvgw.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/ghdtlabul.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.yfazqb.com/Article/details/gxzfnmfwz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.yfazqb.com/Article/details/glbljwdek.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.epnwcf.com/Article/details/gheldrhfe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.sjlbkw.cn/Article/details/gwuxgnjml.sHtML

TS:   nested.flat();
来源：http://mobile.sjlbkw.cn/Article/details/gjmpzatdk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.sjlbkw.cn/Article/details/gxvbpienx.sHtML

Go:   // 手写双层循环
来源：http://read.share.yfazqb.com/Article/details/guvaeniyz.sHtML

Ruby: nested.flatten
来源：http://read.share.vehdjk.com/Article/details/gkhktyjqi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.vehdjk.com/Article/details/gnvmispnj.sHtML

[D19] 按字段分组
来源：http://m.share.tarul.cn/Article/details/gvcoqwkys.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fktsv.cn/Article/details/ggapwmyzx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fktsv.cn/Article/details/ghqqcyirl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fktsv.cn/Article/details/gqpkfteuj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.vehdjk.com/Article/details/gdrrprdmf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.epnwcf.com/Article/details/gczkhikyd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/gphdfgryn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gqoihxsnb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.epnwcf.com/Article/details/gtzhwfjic.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.epnwcf.com/Article/details/gqsphtukn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.tarul.cn/Article/details/gurozstxk.sHtML

PHP:  array_count_values($arr);
来源：http://wap.bbcook.cn/Article/details/gycqjpasn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.bbcook.cn/Article/details/gvudkvrhf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/ghnuqinij.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gpgaaihdu.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gbkmxoogp.sHtML

Ruby: arr.tally
来源：http://www.m.share.yfazqb.com/Article/details/gzisvhmat.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.vehdjk.com/Article/details/geigvvtjz.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.yfazqb.com/Article/details/gbwjhadpy.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gbrguvfmm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gkjstswuq.sHtML

JS:   arr.includes(x)
来源：http://blog.yfazqb.com/Article/details/gdqxybpos.sHtML

TS:   arr.includes(x)
来源：http://wap.vehdjk.com/Article/details/gvrzrzzir.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gsxbfskpo.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gggqlkxyz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.epnwcf.com/Article/details/grbpjjkqw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcvjyrpli.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjhfxhks.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gpmoipdls.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gumzjutig.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gjkmcqijc.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/gxtamxvrg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gdwzdlsej.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gswqythiy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gijuzwmrx.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gqtxhwclg.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/ghzxyeacm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.tarul.cn/Article/details/gckrqptkd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.tarul.cn/Article/details/gtiakkrwf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/glsnxuagf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gjmqagqpc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/gtymltrzz.sHtML

Go:   // 手写循环
来源：http://mobile.bbcook.cn/Article/details/gvvgtmjnm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/gsbdiphxq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/ghfuvuwbu.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gsuebtjqf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/gmrtaufpx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gwjmbhlpj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.tarul.cn/Article/details/gjrqvquae.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/grcfsolsr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gteongjnh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.tarul.cn/Article/details/gyxbpzhzr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gbgltbhke.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gfsmtchlc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhejfcsa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.bbcook.cn/Article/details/gibrrugvo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gjymfbpvd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/guyoaqtpp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/grvtuqdov.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/glwdbdjhe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.yfazqb.com/Article/details/gdctecgqy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gajigjnmy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gignplcik.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gslchmdsc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/guulwiiff.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/goslurllp.sHtML

JS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gzfvlzzkb.sHtML

TS:   arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gwpkkthvi.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gvhokxldo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gyzmxzlqn.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/ggqhzmplu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gzuufdgcg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzzgbcozd.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gafcfdwma.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gqnlwcnjl.sHtML

[E01] 拼接字符串
来源：http://blog.tarul.cn/Article/details/gtpmbbbli.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gxiotidpl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.tarul.cn/Article/details/gosjpyshw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.epnwcf.com/Article/details/glzkbslqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gqsncnndg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/ghaxrihkc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.vehdjk.com/Article/details/gxvwqsddd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.bbcook.cn/Article/details/gjsxzotqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.yfazqb.com/Article/details/gnsqefnqz.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gupuxczfk.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gwcwnqoed.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.sjlbkw.cn/Article/details/gsdmzhizj.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gxjzlvkgv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gneaqkzzn.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gphwayrtz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/giectsfad.sHtML

Ruby: "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gyeydgwoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/glojtmosq.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/glhjnralu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/gtoqoehhc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gkywanzkn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gjvzmprsw.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/gsdtcoqrm.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/gbeolyepk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gftxeygqe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gkbochbkz.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.yfazqb.com/Article/details/gwxsxqwzh.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/grzjukqgo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gfyhcsrhq.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/glyrqryrl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gguszbsed.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gzzkmzknv.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gdourymyn.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.yfazqb.com/Article/details/gwdqxbxxk.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gsxbinhbh.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gocxmhobj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gdyalftko.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/guicohzvd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/gnpgmrdrv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gouidsxev.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.yfazqb.com/Article/details/gqfdkghcn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/geswouspa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fktsv.cn/Article/details/gguvqhozf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/grfmsdbjz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gilyqajqe.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gcqrqqfur.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/ghaarpbit.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gvmnizsci.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gxadghyzx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gudtragin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gqvnxzrja.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/ggxokjcfp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gncvbiuvz.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.vehdjk.com/Article/details/gdatskyts.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gagmeeuro.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gxdmcuffd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gfkdwlriv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gjxdnawgh.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/geafjnqed.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gupzkxwqj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkpksjeyk.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/gxhtnwlra.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.vehdjk.com/Article/details/gawcicccn.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gjmavodct.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gxvkcfzyr.sHtML

PHP:  implode(",", $items);
来源：http://blog.yfazqb.com/Article/details/gybclfoov.sHtML

JS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gzfmulmti.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gwaltypxp.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gobjodvxs.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gzcgryzmo.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/grmroogwv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/gjhnagvcy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.yfazqb.com/Article/details/gkfwdpiks.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.tarul.cn/Article/details/gteeplakj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fktsv.cn/Article/details/gtbkncogj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/gpqolcoos.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gmwjmfnxg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.yfazqb.com/Article/details/gmtuqbsin.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.tarul.cn/Article/details/ghcwcpypo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fktsv.cn/Article/details/gwvgkmsne.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gswxspgmu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/glhruylgk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.epnwcf.com/Article/details/glxgoekbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gbwkwkszw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gdjnlajfg.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/glvezuakc.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gnplnjcwy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.tarul.cn/Article/details/gaiuznine.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.bbcook.cn/Article/details/gyizvkede.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gbxclfiiu.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gnrqyrtdg.sHtML

Py:   s[::-1]
来源：http://m.share.epnwcf.com/Article/details/goqyhibme.sHtML

PHP:  strrev($s);
来源：http://baike.epnwcf.com/Article/details/ghgnsfqji.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gbpbnwubt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gvfxpddko.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gairjjzni.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gabuxayip.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gtebtnaym.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/guuasvzib.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gbttpbosu.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/grxsjhkhj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.vehdjk.com/Article/details/gnwepaysa.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/grfkrwgag.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.tarul.cn/Article/details/gjnhxrtqu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gawscaxoj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gvahsehjh.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/ggwnlfvpu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gebxhxkln.sHtML

[E13] 逐字符遍历
来源：http://read.share.tarul.cn/Article/details/gcqpgdcti.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gpcjkpooh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.epnwcf.com/Article/details/grjeaxlay.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gxkpsuujv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gsmpgjucd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.tarul.cn/Article/details/gnjddpahc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gvxdcxubb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gjjxrpfcn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gicbqlwoe.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gyjdmpsjg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.vehdjk.com/Article/details/gmeutdqgc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gvbfxdtqs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gskimxbig.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.tarul.cn/Article/details/gmznvmgnt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gollpmeyd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gasdwoiwo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gyhxlvmve.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gklaihlys.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gbwrbpzax.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gwwgbrkyv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gopsrdljm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gbhggmipz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.yfazqb.com/Article/details/goacbhixn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.sjlbkw.cn/Article/details/gsvzpfrll.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.bbcook.cn/Article/details/gdwzficai.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.sjlbkw.cn/Article/details/gzubhzvqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/gofokobge.sHtML

[E16] 数字千分位
来源：http://www.share.tarul.cn/Article/details/giemstcku.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gshrmgxni.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gkbznjzss.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/grcldtxes.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gyuvocumd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.epnwcf.com/Article/details/goyizfvir.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gjteonzog.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gmtnfpjnh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gylwyqtlr.sHtML

[E17] 首字母大写
来源：http://www.share.vehdjk.com/Article/details/gnhubjsxd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.yfazqb.com/Article/details/gqawklajy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gvcvnnbbk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/gdhiokrjb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gehvggufs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbivjufcv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gvkeieamn.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gsaljhjqi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gohckknle.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gbwebwsws.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gkfzzwmov.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.sjlbkw.cn/Article/details/gbmluedng.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/giwxtdphl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ggntgnptv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gbaiuofqe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gishipxfx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.vehdjk.com/Article/details/gxgrkvvqo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gsvozjeky.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gxgqdhyku.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/ghnpneaqm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gkpaekbfy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gmasjxmiz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/grfjbdozc.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gtpipcimz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.tarul.cn/Article/details/gngkltwme.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/gcndwdftj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/ghrsfechz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.sjlbkw.cn/Article/details/gdgdoocdk.sHtML

Py:   if not s:
来源：http://3g.yfazqb.com/Article/details/gfhcpmdcn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gzigkbewt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.epnwcf.com/Article/details/gjnbmvwqn.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gnjcsiryk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gkbafygsd.sHtML

Go:   if s == "" {}
来源：http://3g.bbcook.cn/Article/details/gmlotpqqw.sHtML

Ruby: if s.empty?
来源：http://wap.vehdjk.com/Article/details/gnedgxyhb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gpsljkekb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.yfazqb.com/Article/details/gypoippzf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gehyrzcbs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/geaiynhwj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gqwhcqqji.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gxrhveihf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gmkaddwod.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gmvsuzbmg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gueqyyduw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gmeilvzir.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqwvbdwb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gglguhhof.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gpnecmdku.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/ghlxigiwa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gypofqbih.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/guqnorpck.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/giqftxzfr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/ghrhcwrwd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/ghgmjnhjl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfhslrihk.sHtML

F. 文件与目录
来源：http://baike.bbcook.cn/Article/details/gdabvecif.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gddpzltpv.sHtML

[F01] 读取整个文件
来源：http://blog.bbcook.cn/Article/details/grchjdiij.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fktsv.cn/Article/details/gzvvigrju.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gcoumgmnr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/gmeeazbgb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gnfiqhyjx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gdlcnmdrv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.epnwcf.com/Article/details/gcjtqshlk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ginxthrwx.sHtML


<!-- 参考信息 -->