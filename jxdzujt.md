代发 wailian999

[D19] 按字段分组
来源：http://www.share.vehdjk.com/Article/details/ggidwkqei.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmgecizol.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/gdiyoagbi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fktsv.cn/Article/details/gvptmnpsk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fktsv.cn/Article/details/gwikawlxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.bbcook.cn/Article/details/gghkqnldo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.vehdjk.com/Article/details/gbzjmtjxo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fktsv.cn/Article/details/gllymxvix.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/gxjlqmvhv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gywdtplmv.sHtML

Py:   Counter(arr)
来源：http://3g.yfazqb.com/Article/details/gxnixmdkc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fktsv.cn/Article/details/gwmwjbmse.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gsumsaaie.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gavljggey.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gtepfebkt.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.bbcook.cn/Article/details/geedcsbvh.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gimzgeygy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.yfazqb.com/Article/details/gwqlqflsd.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fktsv.cn/Article/details/gzlwfjkhi.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gnvcqfjly.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.epnwcf.com/Article/details/gepfkewnc.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gasucjzwk.sHtML

TS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/geojjbpjn.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gopolxkqk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.epnwcf.com/Article/details/gzkfnstpv.sHtML

Ruby: arr.include?(x)
来源：http://mobile.vehdjk.com/Article/details/gwmygwcxt.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gcrmtjsuv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.epnwcf.com/Article/details/gtxcxftuf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.yfazqb.com/Article/details/galtgceek.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gfarkeuws.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.tarul.cn/Article/details/gmbwwxbab.sHtML

TS:   [...arr];
来源：http://read.share.vehdjk.com/Article/details/gjhlwhcih.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgrpqpsz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.sjlbkw.cn/Article/details/gfbugbjno.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gndjhwpjc.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gbnmbzgxj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gejhyffra.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gvyxuoecv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gryzpdijw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gjjpoctlq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.tarul.cn/Article/details/gbapxdoky.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.bbcook.cn/Article/details/gybbfefct.sHtML

Go:   // 手写循环
来源：http://www.share.vehdjk.com/Article/details/gaqndhgdd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.epnwcf.com/Article/details/gxhvyxbnu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fktsv.cn/Article/details/gpbixwgly.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.tarul.cn/Article/details/gkkruytre.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.vehdjk.com/Article/details/gwlbxakml.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/grzfxejog.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/gvhkmfpct.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gedjkmrwq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gdfyucthc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.tarul.cn/Article/details/gryzvdpqq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.vehdjk.com/Article/details/gxjwbpnhd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/gloqkbqew.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.sjlbkw.cn/Article/details/gwgyrmuag.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.tarul.cn/Article/details/gvlxeehgs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fktsv.cn/Article/details/gabypbgme.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.epnwcf.com/Article/details/gtpjfigzj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gzlgnkdvy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gmujzlfma.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gbiuzbczl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.tarul.cn/Article/details/gwsobiqbh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/ggajogomy.sHtML

[D26] 数组转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gedmusqsi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gbfflhlxe.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gffuhwhak.sHtML

JS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gwxxntfbs.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gqtxjrqjw.sHtML

Java: String.join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gvkdijpeq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/gogjylfbg.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gyokiscio.sHtML

C#:   string.Join(", ", list)
来源：http://baike.vehdjk.com/Article/details/geuhlmhmk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glkclaryo.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/ghbusuiaa.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsccpshkp.sHtML

[E01] 拼接字符串
来源：http://read.share.tarul.cn/Article/details/gdyntamvt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gxlxkhwrt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.tarul.cn/Article/details/gssjbfjfg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/ggesjgktz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gxrcqtppc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.epnwcf.com/Article/details/gkhnowvth.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gkarbbzkh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gzxnzqsbz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gxrjibopk.sHtML

[E02] 重复字符串
来源：http://baike.sjlbkw.cn/Article/details/gyrdavkgg.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gttbiszkh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gkoskmnve.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gnvvnxopj.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/grwueukfi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/ggackeawg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gailmaars.sHtML

Ruby: "ab" * 3
来源：http://mobile.yfazqb.com/Article/details/gnvkxxohd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.vehdjk.com/Article/details/gxdqqurmf.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gwguatibm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gumrjbepn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/glxoypuma.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gsaxlyqde.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gbnpenfqh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.epnwcf.com/Article/details/gqcptbjwu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/glnawimnw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/gbtnzchbu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmaoifcxt.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gdsqrkmet.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.bbcook.cn/Article/details/gnkpnntxf.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/gnodmfgwq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.bbcook.cn/Article/details/glrhffkit.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gypbqdewn.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gulksnrbz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gfyuenjar.sHtML

Ruby: s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gohtyztur.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gezbierxh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gxoijpuqm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gfjjvmmzu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.yfazqb.com/Article/details/gnxkkslka.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gsloidhjf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gdzbjghdb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gjgskfzmn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.yfazqb.com/Article/details/gdlvgqvnk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gesfhqpvt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gyybtijgr.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gisvrapni.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/gextnsstg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gmvsffgan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gxqjrwynl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gswqnzfav.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gbnrquklb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gyjivmlre.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/ghagkdruo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/geprxrsnt.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/gwscejarg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gpstjnojr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.tarul.cn/Article/details/gajiljubr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/ggljaxohl.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/glpzudueu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.tarul.cn/Article/details/guokqxdhx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxfrkgfkt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gnwhxcfdy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/gaxadnhdp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.bbcook.cn/Article/details/gyfdyxhgn.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gqxryyauw.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gdbkzvrog.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gcozgjzke.sHtML

TS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/grojtycnm.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gutiavhgk.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gvkootfhz.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/goxnfbomm.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gtbxcvejn.sHtML

[E09] 去除所有空白字符
来源：http://3g.tarul.cn/Article/details/gvrklyrsi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gffygmawb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/glgcumyta.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gcdvobhrm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gpfwbbmgv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gkvfvkpks.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gikjcpwoy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gbypqcwmk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.tarul.cn/Article/details/glwcjvyhu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.bbcook.cn/Article/details/gigtrfzsv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/gdstuggux.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gwabkuwwa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gepvdkpfg.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gnpnrnyyc.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gcyzvrmrs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gqhqznjgz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gaojmzrie.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gepuyyvhb.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gsgyymwue.sHtML

Py:   s[::-1]
来源：http://www.share.yfazqb.com/Article/details/gsydsdvaj.sHtML

PHP:  strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/geftdqwkk.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gceftilfm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gsiqehixn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/gwcfuxonb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.vehdjk.com/Article/details/grggjrllt.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/ghjwfepae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gimnwulzm.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/gpcmnxcyz.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/govjruxie.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gbhksrlke.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gpvrkqhvv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gnyartecf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.bbcook.cn/Article/details/gogolfwle.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/garcmtlgu.sHtML

Ruby: s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gughzkusj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gphxanikm.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/grgzxueki.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fktsv.cn/Article/details/gqyuabyzq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.epnwcf.com/Article/details/gxslozavb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/glwluypgz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gslyjnnql.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/giyulcixg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.tarul.cn/Article/details/gvrmjjfdd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/ghnyqarbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gyoazhlze.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gzetbgrug.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/goasthbaq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkwqfyn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/gjjyoitab.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.tarul.cn/Article/details/gbeigwycz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fktsv.cn/Article/details/grcbistuu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gnjjtjgel.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.bbcook.cn/Article/details/gwumlbuvp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gsfmcvabw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gdjfzokro.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.tarul.cn/Article/details/gczqiwfwu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gumcvbsgk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gicmkqoyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gdkzolyfx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/goeqclywn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.epnwcf.com/Article/details/ggbujbxwx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.vehdjk.com/Article/details/gqwbqdbec.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gbeuwhiyk.sHtML

[E16] 数字千分位
来源：http://read.share.epnwcf.com/Article/details/gffqizbme.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gmgnkdxap.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/giiluwjla.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/ggixzfbkt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/ggalqygnr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gqohgvxjh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gorfoizxt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/grqvzpkbz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gabspvroz.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gxfevymoz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gtfoxpzsh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gmstiwxqa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gtzrcmjic.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gdkfovksx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fktsv.cn/Article/details/gbjrupugz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gvgrmyslu.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gyibasdsh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.sjlbkw.cn/Article/details/gpfjqfubp.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/gfpxqwlyu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gsagxvdtk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.sjlbkw.cn/Article/details/grjtnaglf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/giisaftzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidxwrnib.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gzeusprzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/gmsjcldcn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.bbcook.cn/Article/details/ggtftjjbr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/girmetdvg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gbahbgitl.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/gvgncikhe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/ghoxeodqq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gwnmlmzct.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/glrzeutmu.sHtML

Java: s.lines().toList()
来源：http://m.share.epnwcf.com/Article/details/gqmewkznq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gfxmpcjne.sHtML

Ruby: s.lines
来源：http://www.share.bbcook.cn/Article/details/grcdgvfpj.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/geubfffzf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.vehdjk.com/Article/details/guohlsftg.sHtML

Py:   if not s:
来源：http://m.share.fktsv.cn/Article/details/grvexmvje.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/gvwlgtosz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/gzkdckvun.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzasudnaz.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gujjodnaz.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gqeomujrw.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/grxtnhxnq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gqnzyjlnk.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gkettbhny.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gmlstxzxm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gxhrgggsw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gfidgnjch.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkcbgnstk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gmdwodxwn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gqgfetidy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/glwlmaxwr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gbplkbmlj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fktsv.cn/Article/details/ghuioubgz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fktsv.cn/Article/details/gaxmpfzni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gcevjcgjm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gnwbdaoao.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/geptznnfo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/ghkqqzqzp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.vehdjk.com/Article/details/gyqhfisxs.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/gcotsvaiv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gmnwokjub.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjfirutha.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gsjpqyyai.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gciwwivxf.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/guahbzrfg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gjpcqqrfp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gzqsdnsog.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gcbsjryff.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gpkgdeiwq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gvczhbveg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gqdufcbdb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gnatijedl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gwspqctnp.sHtML

[F02] 逐行读取文件
来源：http://www.blog.bbcook.cn/Article/details/goxdmjcbi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gadxqoszp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.vehdjk.com/Article/details/gpuaokhgg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gpmghowxb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gchvunksi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.vehdjk.com/Article/details/gnvanmuzs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gekqqsazl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/ghrvjgenc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/gwpzgahtf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fktsv.cn/Article/details/gdxqdhktm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/gspdzhocq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fktsv.cn/Article/details/gauxpwwhb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gpblzezov.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.vehdjk.com/Article/details/gzfjoypnp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gfsqoelgv.sHtML


<!-- 参考信息 -->