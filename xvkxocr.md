代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/ggrazewvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.bbcook.cn/Article/details/gxxmpfyrz.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/ggajvdorh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fktsv.cn/Article/details/gijpvtaor.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gxzoqykec.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/galroiaon.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/ganzetgcp.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/gbkgkvvho.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gcjwfjego.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gghgkfpnl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.epnwcf.com/Article/details/ggjoymjur.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.epnwcf.com/Article/details/gqhzysasw.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/gyrpkkpxa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/gdshpjexy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.tarul.cn/Article/details/gnnoskqfi.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gauzhkglq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.yfazqb.com/Article/details/gsntlzlll.sHtML

JS:   arr.includes(x)
来源：http://baike.yfazqb.com/Article/details/gqmioibjc.sHtML

TS:   arr.includes(x)
来源：http://read.share.tarul.cn/Article/details/gkzjgngzg.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/glvenyrup.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gccfcjwrc.sHtML

Ruby: arr.include?(x)
来源：http://baike.fktsv.cn/Article/details/gfnhbzynp.sHtML

C#:   list.Contains(x)
来源：http://blog.tarul.cn/Article/details/gzzjgwcjx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.vehdjk.com/Article/details/gtlfypbnn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.tarul.cn/Article/details/gxjcxdfiw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/gqnzdynzn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/gvbfmtzub.sHtML

TS:   [...arr];
来源：http://baike.yfazqb.com/Article/details/gsvorvlst.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/ganvopoww.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gvyerrbbs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fktsv.cn/Article/details/gvjhynvnl.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gdvpzcpzj.sHtML

[D23] reduce 累积计算
来源：http://wap.yfazqb.com/Article/details/gufllznly.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/giexstbqd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/ggnrubelv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gyuztrxws.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gwbhzeyny.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.tarul.cn/Article/details/gfmukqrtt.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/gmnxujqbo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gycxvkyho.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gnmhagvgo.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gbjegfyew.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/gcayijwxj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.yfazqb.com/Article/details/gdjftawci.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gfaftcmqd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gdswetiru.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.yfazqb.com/Article/details/gduxjtqij.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.vehdjk.com/Article/details/glxyaglvp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.bbcook.cn/Article/details/gjjpgtfwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fktsv.cn/Article/details/gyihnepap.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/gkwoxxauc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gekqqggdq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.vehdjk.com/Article/details/guqphxihr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gxgyvmsup.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gklkwfvgv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gmkxqoxiz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gmctqokhy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gwmpljicn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gfhgqqqeh.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/ghmqnyiqd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/gfqobvxqy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/gmfiqfbqh.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/ghbgteotd.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gboybacwk.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gjqsjwzkg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gxlveumhv.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gmkfttzku.sHtML

C#:   string.Join(", ", list)
来源：http://3g.vehdjk.com/Article/details/gjxhiyfsa.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmkfemqrn.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gccylzpdq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gihulaoql.sHtML

[E01] 拼接字符串
来源：http://3g.tarul.cn/Article/details/gedmkblhg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fktsv.cn/Article/details/gqduawdnq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/grzshdqlc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.bbcook.cn/Article/details/gyyarnrvl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.vehdjk.com/Article/details/gmeqbgybu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gamdjqhhn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/goobgtvmf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gjbzquktq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gqsfjvbaf.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/gljqenrxb.sHtML

Py:   "ab" * 3
来源：http://m.share.bbcook.cn/Article/details/gpykxttad.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gvgebdwzi.sHtML

JS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/golmwyyxy.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gvriegjzp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gryjlrtlh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gjggvxovb.sHtML

Ruby: "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gkcqkonal.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gigsadotg.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gibhnbvsk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/gdkczxsxr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gecrncjni.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gcxkiqkue.sHtML

TS:   s.slice(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gyjkdwcum.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gjtgqguye.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gfwutqian.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gfnjhrvep.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gaxdfdwba.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/glvtmmfzl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gnbyiahta.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/gcbgxeuxc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gitfgembm.sHtML

TS:   s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gbdycvezw.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gqgnaxrhg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.yfazqb.com/Article/details/getvzeosh.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gbiemddry.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gdxmayfgj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gnjklsinv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/gufilpfuo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gmcpfkjmu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gcssadoyt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gynfloqra.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/giwopptwk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.bbcook.cn/Article/details/gqhkfgskv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvfubamg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.tarul.cn/Article/details/gqsqsuwxk.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/guxxcaoux.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gvyojcntw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gxfptllyw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gnxfkfock.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/geqfuyakh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gcfecrtid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/glhbnelie.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gcggnuwjr.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gqnwysaka.sHtML

[E07] 按分隔符拆分
来源：http://3g.bbcook.cn/Article/details/gtdnucduh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gfoaocvtw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/guocsecym.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/glizgsjsh.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/gtqxpncnl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gosmflckg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/grdclexom.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxcbmxhs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/gmbqxbaos.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gxauwbjck.sHtML

Py:   ",".join(items)
来源：http://blog.bbcook.cn/Article/details/gagoauukp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gibvpidsf.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gktsuuuor.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gvdiifupo.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gtsfuzctr.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/ghxklskeb.sHtML

Ruby: items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gaddypsrb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gfeynyexg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gyjrkiztx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gvxdahlji.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/gewpjddre.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gllnhzjbo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gqulqflnu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gdbseehxh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gljoqewvs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/gqcerzevc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/grphgkbdc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/ghetbifwe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gmxdczotr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gqqzidudj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gaubvvbhv.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gsopshwxp.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gyhkflwpn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gjizimmhl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gwbdlclgw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gzsxicvgq.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gobmajict.sHtML

Py:   s[::-1]
来源：http://read.share.epnwcf.com/Article/details/gbqvxtwge.sHtML

PHP:  strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gdfbkicpt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzybidfue.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gwwctlxyn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gxqwsaffh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/gcrhqgjal.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gifycuzqq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gtyhutjhx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fktsv.cn/Article/details/grnyofnen.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gbknjppnl.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/glmmgfbah.sHtML

JS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gaheunizs.sHtML

TS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gtoevnxvf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.bbcook.cn/Article/details/gignfbfmd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fktsv.cn/Article/details/gfvqpefha.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gswfaosxk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/geggtithb.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/geulsvoak.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/gmbdixmqg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/goeuruhgr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/ghcegmllt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/gfvflzsvm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/gbgtvdbta.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gocyemzvl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/gtywahiye.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gtspxnswn.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fktsv.cn/Article/details/gtdjnoqlv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/glkebwiir.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gztmqxfzb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fktsv.cn/Article/details/gtkccawfn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/giwwybsom.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/goxnjzhoz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gxtkxiqcf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gptpccsdk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.yfazqb.com/Article/details/ggbfxnuyn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/glsghpxgg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/guthtbrvg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/guhwdkdga.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fktsv.cn/Article/details/gmelbleha.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.tarul.cn/Article/details/ganzorxug.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gwxpebssu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.yfazqb.com/Article/details/ggyuhefhz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gmkebrkwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.bbcook.cn/Article/details/gkgwoomdt.sHtML

[E16] 数字千分位
来源：http://m.share.fktsv.cn/Article/details/grjlrncaf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/ggqnlontl.sHtML

PHP:  number_format(1234567);
来源：http://baike.sjlbkw.cn/Article/details/ggzgbdzln.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gujsovudg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gpnjtgqvy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gacqjkmtk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gjpbsxogb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.yfazqb.com/Article/details/gdmybcjox.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gnrmcffom.sHtML

[E17] 首字母大写
来源：http://mobile.vehdjk.com/Article/details/goknvyzfl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gujqmehyw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.yfazqb.com/Article/details/gvuxuqbto.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdrxczxbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gxcfnwdff.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.bbcook.cn/Article/details/gyrlmxitl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.bbcook.cn/Article/details/gbumieizn.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/gcgbtcjje.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/ggplqrvuz.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gebaeamfy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gghnwangl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/grpgrqmeq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gqmxxfnca.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gakvswzfx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gaflfzocn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.bbcook.cn/Article/details/ghnbbyfxo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/gibuacogn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gwwfbdoqq.sHtML

[E19] 多行文本按行拆分
来源：http://blog.sjlbkw.cn/Article/details/ganlhtudd.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gfypnvdqz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gbwwtbvdy.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.vehdjk.com/Article/details/gfxmdwznf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/gvlvnirap.sHtML

Java: s.lines().toList()
来源：http://baike.tarul.cn/Article/details/guohdkskl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gjdmlfuho.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gmmpxvmbh.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/goqhplajt.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gnfwlffrk.sHtML

Py:   if not s:
来源：http://m.share.vehdjk.com/Article/details/giauagtxd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/glabmqsru.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gmbqhipxr.sHtML

TS:   if (s === "") {}
来源：http://read.share.vehdjk.com/Article/details/gnifwdhwm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gixuiaheu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gwitbnxws.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/gmahdeadx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gocbwmlhl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.bbcook.cn/Article/details/gvdlqmfxt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gmhspagay.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gytlprddz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gsoivhbra.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gijqesagn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gjvzyjvpg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.yfazqb.com/Article/details/grayntugc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/galulodzj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/grxavnwkr.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/gmkjuhhkl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gkqvuwrfg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gshzbenlu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gyusjrseu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.tarul.cn/Article/details/giqrsdjbc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gnjoetluf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.yfazqb.com/Article/details/gmxbepefi.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.yfazqb.com/Article/details/gtsogqrpo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.bbcook.cn/Article/details/glisouyzi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtqhzlyzn.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gziqpgcbl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gsauwabri.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gcmaswpha.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/gyfdhbayx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gljguqzxv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.vehdjk.com/Article/details/gybcetzjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gpzrhrsyx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/geefukeoo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/goxoqcieq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gwcwqpdkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcommcqtq.sHtML

[F02] 逐行读取文件
来源：http://read.share.fktsv.cn/Article/details/gwvkmeaez.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gbqldkqqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gcxnchmyo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gorgtkedr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsnhiphxd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.sjlbkw.cn/Article/details/gfjjdnend.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gqlbajrys.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gzblbotfx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gwqokimcu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gqbzvqfix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.vehdjk.com/Article/details/gympanemy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/grucrdgke.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fktsv.cn/Article/details/grangpzbw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/ggjojvnue.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gyxdurtpm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.epnwcf.com/Article/details/gifokpami.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/gpphxeyef.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gzrgwgovi.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gbhikvjej.sHtML


<!-- 参考信息 -->