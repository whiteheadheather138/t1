代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gzvhozgij.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gydkzuktl.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gwtdecaun.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/ggvsaeydd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gzmoxamqp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gqfiytpzv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/goltonuyj.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.bbcook.cn/Article/details/gpycvbuet.sHtML

Ruby: arr.tally
来源：http://3g.sjlbkw.cn/Article/details/gfnxxfrfa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.vehdjk.com/Article/details/gjwxgwjnw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gfnygenuy.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gzfmqdssz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gmtimdqol.sHtML

JS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/grlpknqtv.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/guaomwsxq.sHtML

Java: list.contains(x)
来源：http://baike.vehdjk.com/Article/details/glrwtaqok.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/grortwpxi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gdlludbka.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.vehdjk.com/Article/details/gmehgppzo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/guthutjqv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/grfaehyta.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gslevncxn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fktsv.cn/Article/details/gahuolune.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gmxucexzm.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gflissfhb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gfqewcolh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.yfazqb.com/Article/details/gcorwykyw.sHtML

C#:   new List<int>(list);
来源：http://m.share.yfazqb.com/Article/details/gkjajbsua.sHtML

[D23] reduce 累积计算
来源：http://mobile.yfazqb.com/Article/details/gkvgqurtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gogzsyqnp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gpejidtvh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gbjompicr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/ghntezrxz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gqwjfwshg.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gouiaalxj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/gkpszbxlg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.vehdjk.com/Article/details/gmdmstgxl.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.tarul.cn/Article/details/gldcdwctf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gwddakfop.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gevtqbafc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/ghaxoojpr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gzvayswes.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/gvbbzzxqq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.sjlbkw.cn/Article/details/gblssqpzh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gptnpgtfh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/goqjzncoa.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/gkrvwcfai.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gdsatatvd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/gdpnvkgmx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gdcbgqhqn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/glabrlftl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.bbcook.cn/Article/details/gktpbtlqq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/ghzfkrcrl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gqsywbaai.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gxydbllxn.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gbuanyrbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gszojknpx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/glozqnrjp.sHtML

JS:   arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gdbuznbnj.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gxczlhtax.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gauityoqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gwhaduobp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gyqxygsmn.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gorwofzvc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gntmsmpoa.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/ggtqhngaq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxqmcsmyx.sHtML

[E01] 拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gstrnnfns.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gpcomriyv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/goczudgkp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/ghohjszef.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/gbqamgwfa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.tarul.cn/Article/details/gouysffzf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gnoahowaa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.yfazqb.com/Article/details/gjcmvqoyj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/geeipgjca.sHtML

[E02] 重复字符串
来源：http://baike.yfazqb.com/Article/details/gxomchena.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gaigizbur.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.bbcook.cn/Article/details/gbruidhms.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/grfczrfrz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gqghznwdb.sHtML

Java: "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gxozmrdjr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gnhaknint.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/gfrnmbszs.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/ggveztwqz.sHtML

[E03] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gmmfqrxbj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gssejutcp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gkkcviwuw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gkqveukiy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.vehdjk.com/Article/details/griqbhisg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gpxuhwivy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gptpcgcip.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/gsqxqoqwn.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.tarul.cn/Article/details/gbzsaoufe.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gxqtnmsuo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gvabuvrwz.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gksgqdtmi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fktsv.cn/Article/details/ghckdzbam.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/glieqmjtc.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gnwhkyzpb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gkqbcetau.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gvvxisabu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gnubspkww.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/ghceimnsk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/goqhvggxa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/grhafzmdo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gqydvijem.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/geoygosuz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/ggngvqzes.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.tarul.cn/Article/details/ganqtijwj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gzcyupvyd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fktsv.cn/Article/details/ggkghnwin.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gxhlqferh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyoenwrwo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/gaumhvglf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/guqrcjgdh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gajcgfpje.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/ggowwmyvo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.vehdjk.com/Article/details/gsglzhgam.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gheshrcwi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fktsv.cn/Article/details/gqemqvjvi.sHtML

[E07] 按分隔符拆分
来源：http://mobile.yfazqb.com/Article/details/gzhpewdfy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/ggnfiqxvc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gocpkmtrd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gulfbuanu.sHtML

TS:   s.split(",")
来源：http://3g.epnwcf.com/Article/details/ganrhutwa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/ggrspgxtq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gvqqxljrs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fktsv.cn/Article/details/gdrlldebz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.tarul.cn/Article/details/gfjevuwmu.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gzfgjgjgl.sHtML

Py:   ",".join(items)
来源：http://baike.epnwcf.com/Article/details/gnydbosvv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gbewmhmfr.sHtML

JS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/graelnwwj.sHtML

TS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/ggewztvcd.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gwlohrgvb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/gsasdicdb.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gyeyloegk.sHtML

C#:   string.Join(",", items)
来源：http://blog.fktsv.cn/Article/details/gvhipcdkc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gusddpklr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.bbcook.cn/Article/details/galicgxag.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gwndntmxc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/glfktknvf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gmodwjdus.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.vehdjk.com/Article/details/ganqlzadu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gqqcfxkra.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxehacan.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gxxgqvhtp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fktsv.cn/Article/details/gagumiwzz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gssgjlmtn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/gujvgijkj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gdeeatqeg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gpormtxfw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gdgqpeldw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gubbccucj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gpcjfbyhj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gpsknwtse.sHtML

[E11] 反转字符串
来源：http://baike.yfazqb.com/Article/details/gsyypsryz.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gdikxjlml.sHtML

PHP:  strrev($s);
来源：http://blog.fktsv.cn/Article/details/gcmnhclmn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gedaielps.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmongqavu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.yfazqb.com/Article/details/gpouycnte.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gusergihm.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gawxhoxqv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gmgggtual.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gvaeioqaa.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/geuwzqqxu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fktsv.cn/Article/details/gflqnrrrl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/ggzwcpezk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/ggxnuajps.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/guhpwdhhb.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/grxntqadp.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gnhuejtwj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gdiodjsuy.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/gkypzybhy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gbwgtvguf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gypfykhkx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gwgdtxeci.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/grgpzxbwr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gxoudyeok.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/grjgnifry.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/gqjnlgvds.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gkrwgtouk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gdtgaxlym.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/goskhgnfu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gkfdrdtvq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.sjlbkw.cn/Article/details/gwiueogxq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gukntiaau.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.tarul.cn/Article/details/gajwxnaly.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.yfazqb.com/Article/details/gyrtzizcj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/gknggafsj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/ggmcbyfyr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.tarul.cn/Article/details/ggmocunjw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/ggjsaunvg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.vehdjk.com/Article/details/ggkwzvtlg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.vehdjk.com/Article/details/grimdadzs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fktsv.cn/Article/details/gqpevmygi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gccetktmh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gvjlaapeh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.epnwcf.com/Article/details/gbplbpkbi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.bbcook.cn/Article/details/gkhnlqkfc.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gmdajeibh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gmrggcbww.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/ghsbntnth.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gffqyhapp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/genpoynwo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gbyjlemjo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.sjlbkw.cn/Article/details/gtgtfdtmp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/geuteorol.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.bbcook.cn/Article/details/ggukrdaha.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gmwtqywfi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gagqiycad.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gmoepboht.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/giifgqnpl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/glopqhrhq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.tarul.cn/Article/details/ghhmwuyja.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.vehdjk.com/Article/details/gtzedjemc.sHtML

Ruby: s.capitalize
来源：http://www.m.share.bbcook.cn/Article/details/gftfqbibr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gkewrlvbe.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gkfjyhrrd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/gepvooolg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.vehdjk.com/Article/details/ggxqatcql.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gsxszstvk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gsjjrfmar.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gwshlabvt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gfggzftdi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/glzsqqtom.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gqkdpnojv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.sjlbkw.cn/Article/details/gwcyqcznz.sHtML

Py:   s.splitlines()
来源：http://baike.fktsv.cn/Article/details/goqtzdcle.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.sjlbkw.cn/Article/details/gkwktjphh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/geicntnty.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gauskuzoo.sHtML

Java: s.lines().toList()
来源：http://wap.yfazqb.com/Article/details/gwwjjdtng.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/guohtduxq.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gireyxegb.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gsuinambz.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gglnrhayd.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gkxibjmdh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/gkmbihfyb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gkklnqhmk.sHtML

TS:   if (s === "") {}
来源：http://m.share.sjlbkw.cn/Article/details/goaizryuv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gvnlibupe.sHtML

Go:   if s == "" {}
来源：http://mobile.sjlbkw.cn/Article/details/gvefluyun.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gtbcnyovp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gsptbtzhm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.sjlbkw.cn/Article/details/ganuznaao.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gongijkzs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gpdxioudh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/ggnvkpxvs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gqicwdlxh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gwpegctsi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.sjlbkw.cn/Article/details/gbdmbjghq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gmsbsihip.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gicchzblr.sHtML

[E22] 字节长度与字符长度
来源：http://baike.bbcook.cn/Article/details/gjoeycmkc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.vehdjk.com/Article/details/gvjqyoshj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gtpasgccu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gaonuaoow.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gfvbzitbi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gogfzlple.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.bbcook.cn/Article/details/gegfjqpsn.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gjmibijxy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gcqitoafr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/goohqjmfk.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gqcrforgf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gkmrwhsbq.sHtML

[F01] 读取整个文件
来源：http://www.blog.sjlbkw.cn/Article/details/gyvyztxez.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gskhwrsks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gxkbhhvkf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.sjlbkw.cn/Article/details/gtjmmawyu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fktsv.cn/Article/details/gdapkvqlr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/geiszdlhg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gvwrkmgsl.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gnumxyxzw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gqquirztf.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gresgvsey.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gdnchciiq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fktsv.cn/Article/details/gkztdqorv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gohxtdpdr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gyrztfvsi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.sjlbkw.cn/Article/details/gfxllolmc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/grazqpzrh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.vehdjk.com/Article/details/gzhyqfgup.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gmogbedrg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/gcaecbkfd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.tarul.cn/Article/details/gzxkuadol.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.bbcook.cn/Article/details/gtjbvcfea.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/ggwjgfgeo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gpzbprrgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.epnwcf.com/Article/details/gjefrxlyd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gffrmumlx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/gvzecfdcx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/grhbgkviu.sHtML

[F04] 追加写入文件
来源：http://blog.fktsv.cn/Article/details/gzhuflczd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gbwdyzjxm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gakqzfodn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.sjlbkw.cn/Article/details/ghawxglcg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gduvfwyvu.sHtML


<!-- 参考信息 -->