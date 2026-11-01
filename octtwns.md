代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.tarul.cn/Article/details/gkoxevyti.sHtML

Go:   // 手写双层循环
来源：http://www.share.yfazqb.com/Article/details/gazjivovx.sHtML

Ruby: nested.flatten
来源：http://mobile.vehdjk.com/Article/details/gfthitrdk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.vehdjk.com/Article/details/gtwtbxnde.sHtML

[D19] 按字段分组
来源：http://wap.sjlbkw.cn/Article/details/gizjcpgsa.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.vehdjk.com/Article/details/gpueihaxw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.vehdjk.com/Article/details/gwwpmjjwd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.sjlbkw.cn/Article/details/gsayyoqer.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gbbfcwaqq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.sjlbkw.cn/Article/details/gshimzzro.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.epnwcf.com/Article/details/gqndpcist.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fktsv.cn/Article/details/gicvjxhsa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.epnwcf.com/Article/details/gfuygwsqx.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gqibpgsul.sHtML

Py:   Counter(arr)
来源：http://read.share.bbcook.cn/Article/details/gvwxqqevy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gsotazfvr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gfdlqylpj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gnghnimzy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gezhgsxac.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.tarul.cn/Article/details/gulehvubk.sHtML

Ruby: arr.tally
来源：http://wap.sjlbkw.cn/Article/details/gapvybxia.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fktsv.cn/Article/details/gnexqwxfw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.yfazqb.com/Article/details/gxqkteteo.sHtML

Py:   x in arr
来源：http://m.share.vehdjk.com/Article/details/ggctqgenw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.vehdjk.com/Article/details/ggdfuudyt.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gzklcqxgt.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/gvactbzqu.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gmyljuutw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gkfkhyabd.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/gkkcspnfl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gybeunban.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/grerjhsup.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gczryezxg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/gxyfbamfv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gqctftsve.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gerttlmhn.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/grcufkexn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gsndqvjla.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/griqcnjyd.sHtML

C#:   new List<int>(list);
来源：http://blog.fktsv.cn/Article/details/gqrradfbc.sHtML

[D23] reduce 累积计算
来源：http://wap.bbcook.cn/Article/details/gajsevlhh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/gjowltjjy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gqtajanup.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/gbmyhvjbv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/grtdkanih.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gfxtsyllt.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gufihpylm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.yfazqb.com/Article/details/gjimmiwui.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/geqdccvrd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gzhocdcwt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gxovtcbpi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.tarul.cn/Article/details/gnoikitcb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gptubzwuc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gevylyewa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gyprxtppz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/ggsybocbc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gxpoedyee.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.bbcook.cn/Article/details/gyskrzgit.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gqdrsudpq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.tarul.cn/Article/details/gsjimwauy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gynuztuwq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gatjiznqo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fktsv.cn/Article/details/guvzumdwn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/grwyvzeod.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.tarul.cn/Article/details/gtehgrtxd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.yfazqb.com/Article/details/gqztojxge.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzihhbwqe.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/gbqyvxdmi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gnfechqqm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gmdkqtwto.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/ggtvisqnb.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gulsentii.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gvbcojqhe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gcjxfsort.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gvvfwatqk.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gyivpbwdi.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gnibgvfgh.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/glibubzbf.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnuvwwrdd.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gvdbhjkds.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/ggxpsosij.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gufexrofb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/ggdwktdvm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gqmjfejip.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gonfuvmyh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.tarul.cn/Article/details/gaobpxmzu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/glwapxnge.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/grbeizsor.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gvkkaxcxt.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/ghnvgesxs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.yfazqb.com/Article/details/gbkkmeylk.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gjmzavrls.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gbflltqdz.sHtML

Java: "ab".repeat(3)
来源：http://baike.yfazqb.com/Article/details/gzdskuera.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.sjlbkw.cn/Article/details/gdvwyhuqc.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/gtfcdcztu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gimjzuote.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gbbgetldj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/gdcqwrtmn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gnkbdkrtg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gmmtzabxm.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gshvovnyv.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/gzccedmwt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.yfazqb.com/Article/details/gsteogwhm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.epnwcf.com/Article/details/gcuwizsof.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gctoqigzi.sHtML

[E04] 查找子串位置
来源：http://www.m.share.tarul.cn/Article/details/gnpiwhzxk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/gurlesepl.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gjibjfcth.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gvemodllc.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gpjrtmewa.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gnysixwxf.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gdcznxnya.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gzlnxyvqb.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.tarul.cn/Article/details/gkpoceoqn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.epnwcf.com/Article/details/gkqywcetr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/gvxapdrox.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fktsv.cn/Article/details/gpkijcrpw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/ghhzuukxq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.tarul.cn/Article/details/gzrxrreyd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gxpqghbxu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxjarter.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gxosygcuo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gxlkshbmz.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/gayvsndrs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/goytsmjgc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gvcugucox.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gygnuznpz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gvxjbqfin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gdngbaint.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gazjhbypl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gaabtkrga.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/goikfbuyp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.epnwcf.com/Article/details/gzjdoxhub.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/grxstulbt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gsgmxjhao.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/grnntxzii.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/gcqukffyw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gwacybxar.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gkqxravcx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.yfazqb.com/Article/details/gmchkpgfi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gernujnvo.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fktsv.cn/Article/details/gpcmfettd.sHtML

Py:   ",".join(items)
来源：http://3g.epnwcf.com/Article/details/gyxftqfho.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gupekvhaq.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gzosretqf.sHtML

TS:   items.join(",")
来源：http://baike.bbcook.cn/Article/details/gutdvyfmi.sHtML

Java: String.join(",", items)
来源：http://blog.yfazqb.com/Article/details/gzsdcwdrz.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gckfwedax.sHtML

Ruby: items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/grabzjeyb.sHtML

C#:   string.Join(",", items)
来源：http://read.share.vehdjk.com/Article/details/gwegqwqfo.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/gkgsmigjr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/gssiukdmh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.yfazqb.com/Article/details/gxtbzkesk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gaagpeoeg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gjfuedave.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.yfazqb.com/Article/details/gqdyckvwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fktsv.cn/Article/details/gnvksoniv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gdppxhcpk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gljxvopin.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gjfepnecz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gdphgryja.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/gnfxkpghb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gfqdekxtl.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gujzarqgb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gfzsrsinb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/glgodkatu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/ggsibcsma.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.bbcook.cn/Article/details/goddrziku.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/grydmosml.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gwzjjwksb.sHtML

PHP:  strrev($s);
来源：http://wap.yfazqb.com/Article/details/gglwhtoky.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/glpvnphrs.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gtgyskuop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.tarul.cn/Article/details/gxuxzxquz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gezfjdtbg.sHtML

Ruby: s.reverse
来源：http://mobile.fktsv.cn/Article/details/ganeykrws.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gnceypart.sHtML

[E12] 统计某字符出现次数
来源：http://baike.vehdjk.com/Article/details/grgldjzak.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/grqpkdzkq.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.sjlbkw.cn/Article/details/gjxsegpcr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gjsbkyzui.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/giqddzidt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/gfsrhwtpo.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gjixqtssr.sHtML

Ruby: s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/glbbufqpe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfjjppvi.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gdtrcfcfn.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.tarul.cn/Article/details/gpjvtvewz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gaeccvego.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gqipomncy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.vehdjk.com/Article/details/gdqmwnooi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gbdcrwgmv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gkjdvcoty.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.epnwcf.com/Article/details/gzqijcjas.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gpjgbvzzw.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gxcgyebxw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gvsncnshl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gaybdyayk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gunhccsay.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjyueqgan.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.vehdjk.com/Article/details/gixwnnsmk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gootxdmvo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.epnwcf.com/Article/details/gnzyfxwok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/gxybuyypg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gggjtsxmw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gslslqcab.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.tarul.cn/Article/details/gfviwpnfw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.epnwcf.com/Article/details/giqjdfzwj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/gejfwqtdb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gdsokggpw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gishurwwd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gqrojbfoc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gknijoazr.sHtML

[E16] 数字千分位
来源：http://3g.tarul.cn/Article/details/gsxeqdhgv.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gsffgisqt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gslhfjbrp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gwxxnpboa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gggintnrm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gdlooylvy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.bbcook.cn/Article/details/gycxkvrwv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gqjujgnsk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gurntfjmh.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gfzvbtawr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fktsv.cn/Article/details/gxpputmho.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gvuszdvgo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/goufwfnqq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gmbulianm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gsmmhbcbo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gpxegnnvr.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/grhasqrey.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/glfljswfs.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gcysurmna.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/gupeyqqzr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gplbfwumt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/goqztynkq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gyrihewnm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/ggzpqxmwy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fktsv.cn/Article/details/gibldjwqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/gknjljzzu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/glenlxwse.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.bbcook.cn/Article/details/gyowdmbqf.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/gwjjlondc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.yfazqb.com/Article/details/gthttkfbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gklsegujm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gcyhdndkn.sHtML

Java: s.lines().toList()
来源：http://mobile.yfazqb.com/Article/details/gwczkqemx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.epnwcf.com/Article/details/gzruoxmcr.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gfgbrabsf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gcnzgesox.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gsxpbteno.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gucpmbtbj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fktsv.cn/Article/details/gnkoswwys.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.yfazqb.com/Article/details/gsncjjzjn.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gvfpqasta.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/glyvspwcl.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/gdlzqkwgl.sHtML

Ruby: if s.empty?
来源：http://read.share.yfazqb.com/Article/details/ggciskihe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.sjlbkw.cn/Article/details/gaqfazaho.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fktsv.cn/Article/details/gyoucuevy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gkbrqkzes.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gcntehcln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gkpmlfcdy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gaxqxcpun.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gfmxygpel.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.tarul.cn/Article/details/glxrvikjc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gfslbxebh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gmdmoqphu.sHtML

[E22] 字节长度与字符长度
来源：http://3g.vehdjk.com/Article/details/gkahzywoj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjjyjozxi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gjmjmxmaq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gstfoxqzm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gnyeppnec.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gvlvjcwci.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.epnwcf.com/Article/details/gekqbdzqg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gmwqdefjm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gzgpzxahu.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnaqylhqi.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gtymgjtga.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giitpwfsi.sHtML

[F01] 读取整个文件
来源：http://baike.fktsv.cn/Article/details/gccndofta.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.epnwcf.com/Article/details/gimupsdze.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzjxslext.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/ggsaqejil.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gkwvmgwfk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.tarul.cn/Article/details/gogmfplhy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gvktnbtdj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gogywvcjs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gryobxcjr.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gdxwyhkaz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/glntmhfoo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gaderoozu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gsyclmktp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gzbbycemt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkisfavz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/glfujmjpn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gddrsotgs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gwihohixe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/guaavazcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/giyzozvga.sHtML


<!-- 参考信息 -->