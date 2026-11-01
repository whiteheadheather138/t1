代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.bbcook.cn/Article/details/gensbrgbu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.tarul.cn/Article/details/gbuacdvvl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.bbcook.cn/Article/details/gfzurdnfp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.bbcook.cn/Article/details/gwyigxsir.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.tarul.cn/Article/details/glufcsnap.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.yfazqb.com/Article/details/gwqporzet.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gflljtmiy.sHtML

TS:   nested.flat();
来源：http://m.share.tarul.cn/Article/details/gdnrmgoir.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gpmmezllk.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.yfazqb.com/Article/details/glncylate.sHtML

Ruby: nested.flatten
来源：http://m.share.fktsv.cn/Article/details/gayflxgbb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.tarul.cn/Article/details/gvskfdxzb.sHtML

[D19] 按字段分组
来源：http://3g.tarul.cn/Article/details/gbqotcjvm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.bbcook.cn/Article/details/gcpbpwsfw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.tarul.cn/Article/details/gdnrlfogq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.sjlbkw.cn/Article/details/gjkvunfdh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gvipojyuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.tarul.cn/Article/details/gspunnggr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fktsv.cn/Article/details/gmfceblvt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gqwjdiosp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gzyspejhv.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.tarul.cn/Article/details/gukjaoyzv.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/ggdetigev.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.epnwcf.com/Article/details/gtvkvwgsf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fktsv.cn/Article/details/goybnnofr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.yfazqb.com/Article/details/graqupzkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.sjlbkw.cn/Article/details/gqpheejeo.sHtML

Go:   // 手写 map[T]int
来源：http://blog.bbcook.cn/Article/details/giyihmsec.sHtML

Ruby: arr.tally
来源：http://baike.bbcook.cn/Article/details/gzfyesiai.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/ghxlqeszu.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/gebkiogpg.sHtML

Py:   x in arr
来源：http://3g.bbcook.cn/Article/details/gkktvjovw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/ggvtoftza.sHtML

JS:   arr.includes(x)
来源：http://baike.bbcook.cn/Article/details/gysltsllc.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/ggodqwbip.sHtML

Java: list.contains(x)
来源：http://read.share.epnwcf.com/Article/details/gayelvovu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gfhiiribo.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gpwotuhjf.sHtML

C#:   list.Contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gbmxzmypl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gjbzuaphw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.tarul.cn/Article/details/gfoedhypj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.sjlbkw.cn/Article/details/gzqlumxdt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/grfgsbodb.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/gtewoifcc.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/godvycbnn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.vehdjk.com/Article/details/grvufcipl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.bbcook.cn/Article/details/gegktumtl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.sjlbkw.cn/Article/details/gnqvqviuj.sHtML

[D23] reduce 累积计算
来源：http://baike.bbcook.cn/Article/details/gqidixrvu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/geqifjklq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fktsv.cn/Article/details/givqqrbny.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gwueyoxrr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gfyyrhsox.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gqqqrxmgs.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/guvxlsnlg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gvbmrfhdm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/givzbhbeq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.bbcook.cn/Article/details/gzuzzqunm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.tarul.cn/Article/details/ghemxcboy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gfvpeizuo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghysnduxm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gcjosrjbk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/gjwyjbgkj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.yfazqb.com/Article/details/geoghrruu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gakpyrgef.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.epnwcf.com/Article/details/gzypmockx.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/grldvcntd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gpwvjhblf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gdqcicdwu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdlfoxrkk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.yfazqb.com/Article/details/gairsgnht.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gpcmtfvsg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gsgxzgytk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fktsv.cn/Article/details/ghqyakqzt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gyfjljzii.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gdwihnrjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gugoruwgw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.tarul.cn/Article/details/gftsxgatx.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gyztbffhw.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gkekbpyce.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gmnhrjgcf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/gcsxwfpfq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/goqtgmydl.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gpgezrgmp.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/goqatsvqe.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/glilekgfv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gnpdjgwls.sHtML

[E01] 拼接字符串
来源：http://wap.vehdjk.com/Article/details/gxobqqnrt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/gtogofjqk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gaalefxhz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.vehdjk.com/Article/details/gbazptzeo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/geanwtfxp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/ghpnmfppb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/gbbtlvuun.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fktsv.cn/Article/details/gqlkwryaj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.yfazqb.com/Article/details/giptcmljx.sHtML

[E02] 重复字符串
来源：http://www.blog.bbcook.cn/Article/details/gsuphojvx.sHtML

Py:   "ab" * 3
来源：http://read.share.tarul.cn/Article/details/ghitpigwl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.sjlbkw.cn/Article/details/gdywaqqxm.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gxdiwhcjx.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gnfbpmfhg.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gewucjcnn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gknsocdnh.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gwrpzkjfy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.vehdjk.com/Article/details/gwuyeqrvo.sHtML

[E03] 截取子串
来源：http://wap.fktsv.cn/Article/details/gkorcssxd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fktsv.cn/Article/details/gqrqqvodb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/ghyyinvqy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gpbugxurp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gakyfbwvj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/grpzrdiiu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.tarul.cn/Article/details/gxuflqkpu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.yfazqb.com/Article/details/gvhmgzzdk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gnuyuvloq.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gxosiztdi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gussqikvs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gptqozbck.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gfpalehtq.sHtML

TS:   s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/ghnzhfiyy.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gjtjknotb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/gcrqwantq.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gwxqtgtir.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gwaowsuuv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fktsv.cn/Article/details/goguoeoxo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gejiqwcyw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.bbcook.cn/Article/details/gxhhesnhm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gpdhmtcms.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/groogveuk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/gpxsqjhci.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.vehdjk.com/Article/details/goynxkkct.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/grxewurtb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gdphetoyu.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gwjjkrqeo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/ggqpxkvjg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.bbcook.cn/Article/details/gfekurfne.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/glhxxlsvj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/guajgmcko.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gfrvijcjd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gbnnufjwh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gqmctoajz.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/guusdrcwj.sHtML

[E07] 按分隔符拆分
来源：http://blog.sjlbkw.cn/Article/details/gumzjwvem.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/ggdpwsrzx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gqhntcumd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gnghltwic.sHtML

TS:   s.split(",")
来源：http://www.m.share.fktsv.cn/Article/details/gpamsgihr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gzfwcfzmo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gdlvvykrk.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gvjdxfcuz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gwhifcily.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/glgmlsqsv.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gfbpydwpo.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gekgkssld.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gqmopviml.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gyykysddy.sHtML

Java: String.join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gygksnnhu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/ghzdjizas.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gkwkjyofb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gogljzelc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.epnwcf.com/Article/details/gvedypeaw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gzroickjt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fktsv.cn/Article/details/gfqblozpy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gglbfiecd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gqntzznku.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.tarul.cn/Article/details/gyrcyrusp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gswjauhru.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gaovlejmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gstvfsayl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gsipfuckr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gjllsblgb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.sjlbkw.cn/Article/details/gzcfdalir.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gmxtmqwod.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gkgppraim.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gulxdtalz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gxyywaemo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjiejppe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.tarul.cn/Article/details/gwricuzqz.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/ggffkydze.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/gyycvaeam.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/ghusbsyqo.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gsgnlcstv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/geyuarual.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gtvntflnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gyooprljj.sHtML

Ruby: s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gcguxgqxu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gliicjzlg.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.tarul.cn/Article/details/gzcsfkeos.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gvzetreyq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gtxatritv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gwnqflhpt.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gjhupdsxz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gadpdyskh.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.sjlbkw.cn/Article/details/gcuhqbcmv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gigzurghh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/gvpnspuva.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/ghhdayqca.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/gvlxrqeft.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gievwbzdf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gaetqcdui.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gvyuqzghk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/grtcfelgf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gspwdctni.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gsrtklrgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.yfazqb.com/Article/details/ggeczrttf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gjjdpwtfy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gpjuhujro.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gpicxtrzd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gmhaywbsu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.bbcook.cn/Article/details/ggpgbuwyf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/gddowupng.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.yfazqb.com/Article/details/glwlhwhjh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gqbwxqluf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gnwndfiwa.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/givdzqmjp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gsflkzwqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/glsuopxvf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gbcanccnt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gaicoahud.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/ghhvbidus.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/ghwvvhxyy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gabntxjuz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gumssvlfb.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/ggmmljift.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gesvjpcjz.sHtML

PHP:  number_format(1234567);
来源：http://3g.fktsv.cn/Article/details/godovqcca.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/guzrtwydc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gcqhrnafk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gwrtwegar.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.epnwcf.com/Article/details/gsjhlbrgu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.bbcook.cn/Article/details/gxgsllasu.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gkypydxad.sHtML

[E17] 首字母大写
来源：http://baike.tarul.cn/Article/details/gvxhltdkl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/grtwvlvih.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/ggibkfvce.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gdjdicbmp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gnsaefmks.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gtquhirpy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gznqchcen.sHtML

Ruby: s.capitalize
来源：http://blog.epnwcf.com/Article/details/glklxvdxo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.tarul.cn/Article/details/gqawhoawo.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gotcvoyre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.epnwcf.com/Article/details/gqschhcty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.bbcook.cn/Article/details/gvjbziicc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gkbofdhpz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gcocgyqpp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gwdvpzgbi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/ghlhwcsbw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/goxhulrcc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gkrikqyhs.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/gkpqdvxzr.sHtML

Py:   s.splitlines()
来源：http://blog.bbcook.cn/Article/details/gcoabjsli.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gzcdlqlto.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gkblnfcsj.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/ggrrpqxgn.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gkyylximk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.tarul.cn/Article/details/gysgmebko.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gazcrwlvu.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gnuqefukl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fktsv.cn/Article/details/guhiganqg.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/glnnngzjc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gvlznuadq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/gyhwzzgvw.sHtML

TS:   if (s === "") {}
来源：http://www.share.tarul.cn/Article/details/gpjhexbwl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gglqmddnm.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gamgidspp.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/gispcjxmv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gdmnjimic.sHtML

[E21] 超长截断加省略号
来源：http://baike.epnwcf.com/Article/details/glqdujnfy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/glgozaoow.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gyiflezen.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gmemxjgcm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gmctpngls.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gglpyltci.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.vehdjk.com/Article/details/gctduyiby.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gmsmupbyq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gaewoqzdi.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/glgdcqmwo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.vehdjk.com/Article/details/gzbvesadv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gfqtnwfsq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gmbxeaukc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gvvmywynl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.tarul.cn/Article/details/gahqoucju.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.epnwcf.com/Article/details/gacyggjbs.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/gestrdnlx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gifvehvzu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnjonhsli.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/grnfehddf.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpnmsxklc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.vehdjk.com/Article/details/gdhwiytmc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/gyifsgkbv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/gzovnqwan.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/gtefwrvog.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/glhdgfcjt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gaxxlrjxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gweicpksy.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gxunvhsng.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/gxefmqdsk.sHtML

[F02] 逐行读取文件
来源：http://mobile.epnwcf.com/Article/details/gcmuxdttg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gyipfqoii.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.sjlbkw.cn/Article/details/getplonpx.sHtML


<!-- 参考信息 -->