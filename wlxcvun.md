代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gqxjnrsyo.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gxvqhiehc.sHtML

Py:   Counter(arr)
来源：http://mobile.tarul.cn/Article/details/gnfzkzbkl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.yfazqb.com/Article/details/gitopzvjb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/gxrzrhdqg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gcnolkgsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.tarul.cn/Article/details/givucwqbt.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.tarul.cn/Article/details/gjfsnmtyu.sHtML

Ruby: arr.tally
来源：http://3g.bbcook.cn/Article/details/gozxbrclw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gowxllvwo.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gobxkmifx.sHtML

Py:   x in arr
来源：http://baike.vehdjk.com/Article/details/gusjzahhx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.vehdjk.com/Article/details/gofejsibz.sHtML

JS:   arr.includes(x)
来源：http://wap.yfazqb.com/Article/details/gwqhsdtzl.sHtML

TS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/gvrdsbtmj.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gaftdjssc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggjpsqvoe.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gsvoxenbe.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gkidghjyw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gzquiwxyr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gbmrutgkk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/gnyjtwskc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkohkfiny.sHtML

TS:   [...arr];
来源：http://m.share.sjlbkw.cn/Article/details/gfdqgaust.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhanqeug.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.yfazqb.com/Article/details/gpweycref.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/gavsgzjwq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gbhkprzdz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gzbrmsjqh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.vehdjk.com/Article/details/giolmciqb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gdbcuqwaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gndzczxln.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/gcqchperf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gjjrqitfv.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gjksehqgv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/gccijapiv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gizrfmxhu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gmcoytkip.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.epnwcf.com/Article/details/ggwshnztf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyrfkkij.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fktsv.cn/Article/details/ghavcvzws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.tarul.cn/Article/details/gydfqcsut.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gusvjemdo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/golfnqxxe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gtiltqvai.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gatvoytzw.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/ghvchvkeu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gezdjhbtg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/grqwkapic.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fktsv.cn/Article/details/gxpqukjue.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gzdkrhxkr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gtcymgjza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.tarul.cn/Article/details/gmaghltlm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gfhfdsnjc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.epnwcf.com/Article/details/gkqfzdqrt.sHtML

[D26] 数组转字符串
来源：http://mobile.vehdjk.com/Article/details/gfpayzkid.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.tarul.cn/Article/details/gktdshvwf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fktsv.cn/Article/details/gkhujansl.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gcphrjrkw.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gawtzaeyu.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gbxdgpaai.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gbqzalkyk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/goxhytyxt.sHtML

C#:   string.Join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gluuaijcv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gubbxerjz.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gkdogtliy.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnekjticq.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gvabjgekx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gbqdondkn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.vehdjk.com/Article/details/gsvnkvcyh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/gtgyzciov.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/ggentlvkk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/gerosbunz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fktsv.cn/Article/details/gwbdozagi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gxuvvwoqc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.epnwcf.com/Article/details/giinpvpph.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/gfxvgvyqm.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gbcxocbah.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.bbcook.cn/Article/details/ghwacyjsp.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/guoikkahf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gnealpoax.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gvlufpawm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.vehdjk.com/Article/details/gdfctnmdp.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gtojbixim.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/grwnydgho.sHtML

[E03] 截取子串
来源：http://m.share.fktsv.cn/Article/details/gqoipgsum.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gipcdrvtc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/glpjhyxrj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/golnirmkn.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gdksgjedr.sHtML

Java: s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gpbibnxtk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gdbivvfxs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gdghinogv.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gdoaihcys.sHtML

[E04] 查找子串位置
来源：http://www.share.vehdjk.com/Article/details/gxwkyacbj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gbgviedax.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.vehdjk.com/Article/details/ggrrkdhtf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.epnwcf.com/Article/details/gcpwdqecm.sHtML

TS:   s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gldnaggik.sHtML

Java: s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gojevlxqv.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fktsv.cn/Article/details/gkrivwzuc.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gpijjpmfr.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gcavudlpi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gofhmihaz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/giozqpejd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gdivtupnx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fktsv.cn/Article/details/ggywjrgnr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.epnwcf.com/Article/details/gcayqlbxg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gpioesxjp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gxxrbaevt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.sjlbkw.cn/Article/details/gknyuyzyg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gfbgnggpw.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gwervxjdx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/ggmvsoyjn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/gqcbjgisz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gypvemhzl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gjbobuhrg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gsdtoemyf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gkliyxkqu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gyafdscyw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gubqdcptg.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/ghvrefjkm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/grymerqub.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/gktadlydw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gdcicjmzo.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/glykqkrlj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/ggyrdxtjt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gxiqmevfe.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fktsv.cn/Article/details/grsxeozdq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.bbcook.cn/Article/details/ggosrpecz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/gnoyyypay.sHtML

Py:   ",".join(items)
来源：http://www.blog.vehdjk.com/Article/details/gguexmbkg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.tarul.cn/Article/details/gxepclrce.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gpyiolagf.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/glptptzkg.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gecechnml.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gggmracci.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gdcmvxtzl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.yfazqb.com/Article/details/gxcvzicee.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gagosxuih.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gjbrxcggq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.epnwcf.com/Article/details/gbmjytwyb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/gpoprbhiy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gehezbhon.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/gfuwjvosf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.bbcook.cn/Article/details/goazmiknu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fktsv.cn/Article/details/gitsgrjkx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gbwbswgos.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gqcasgvyo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gdzojuoyq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fktsv.cn/Article/details/gkaiipoxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gakhtkodc.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gbifyuzuz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gjearwnay.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/ggphggygt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gjpzrmvbx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.yfazqb.com/Article/details/geneyjbqp.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gfzuypadl.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gxvqhvfwd.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gvuuhushh.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gixlkxgff.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/ghvnlqgjs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.yfazqb.com/Article/details/ghxpladhw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/ggosuoyrn.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/grivdajad.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gvuysjfwa.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fktsv.cn/Article/details/gdzleqfft.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gfbbttwtp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gzsfyfykb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gyuiayntv.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gzaykrnve.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gfuaitmby.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/ggxwiqdfq.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/guqvseeao.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/ghfyvmgfp.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gatygdipx.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gydmpbhyk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gvqzsoqgs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gegezrrgc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gtliieavh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gimmovvtt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/guquuhitm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/ghgqyrsqa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.vehdjk.com/Article/details/gdxelaxyf.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/guugbbacz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gvlansmso.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.epnwcf.com/Article/details/gvmcpvuxt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.vehdjk.com/Article/details/gvejlquga.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/gxvevamqk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gtcyvtyeu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gsbmerpcs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gkknmlgcr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gxzkimjms.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.yfazqb.com/Article/details/gyjrfxnhd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/ghmyofcsp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gcmsqdfqs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxpgfitgi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.bbcook.cn/Article/details/gmxosogav.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gvcvyswzf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.sjlbkw.cn/Article/details/gslvqvtdl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gcalptzvx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.yfazqb.com/Article/details/guanqzhiw.sHtML

[E16] 数字千分位
来源：http://wap.sjlbkw.cn/Article/details/ggrwydhmg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gmqstfqvy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gucwuxofg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gunbelykd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnkobxur.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.vehdjk.com/Article/details/gxvobxsqu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.tarul.cn/Article/details/gqtzicbbk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.tarul.cn/Article/details/gskmevzel.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/ghiueimew.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gnjdmutts.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.sjlbkw.cn/Article/details/glbrlzkht.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gzelspwlt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/grlqehoqh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gsbzntuao.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/gplezfavj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gdqhuuubs.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gtqustgwl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gvpeuyhut.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/gkcarnszw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/giijzbgah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/ghbgmbhwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gkfstkufu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gamexhffp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gsgszyacb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gfsoqcxpr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fktsv.cn/Article/details/gbvbxsycn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/gspzctlns.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.yfazqb.com/Article/details/guzzvntiv.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/ggncgvtoi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gllqaixto.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.bbcook.cn/Article/details/gqmqiwbxq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gyriaqfrn.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/glcdsxvsf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/gcptdorvs.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gccdhsdvv.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gwsubehki.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gonkgvgix.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gpuxiojrh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.yfazqb.com/Article/details/gvjdbxfwp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvommqwb.sHtML

TS:   if (s === "") {}
来源：http://blog.bbcook.cn/Article/details/gvktsxldc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gdnslivjf.sHtML

Go:   if s == "" {}
来源：http://wap.yfazqb.com/Article/details/gdqxuqyqt.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gefmsuhmz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gwifuworg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.sjlbkw.cn/Article/details/gyegqjaph.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/gabpalqfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/guvsrkeza.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gicbsspod.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/ggzdmcydx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gobyzdiof.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fktsv.cn/Article/details/guzbahtmd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.bbcook.cn/Article/details/gsbuaefwp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gwdsytbye.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gkhqhxtdq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.tarul.cn/Article/details/gexwcmrwa.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gauydwnhg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/gqnidibgt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.vehdjk.com/Article/details/gwrhpkxue.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gvrfegapb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.epnwcf.com/Article/details/gdilihzaf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/geutbzpzi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gvybycyyj.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmymyvbnu.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gshwbgmhu.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glhhwzffb.sHtML

[F01] 读取整个文件
来源：http://m.share.tarul.cn/Article/details/gywmneimq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmhnwgbc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gmsxaduyl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gpdbnaqqm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/genndtypx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gzogpagbj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/gsrstnzpx.sHtML

Ruby: File.read("a.txt")
来源：http://wap.vehdjk.com/Article/details/gkpgumywr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.epnwcf.com/Article/details/gmyfoxmkr.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/gcxjcjofi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gfumvnysj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.sjlbkw.cn/Article/details/gwdgqdwfn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gbzqvhkip.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/glbndbhjk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.bbcook.cn/Article/details/gnlrxvdxa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/ggtwhfpzq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gnziwhjdf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gzgktkmkh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.yfazqb.com/Article/details/gsmokndpp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.vehdjk.com/Article/details/gtinhcyjk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gwlbyavhl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/guinmnnfh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/glyjosktc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/giwmmlpkn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/gavlvgtmb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/glqivbkyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/gpfadpwom.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gaqshppyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gpcbbyipc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gtwmbijwk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/ggfkdhxkq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gglcdnkbs.sHtML


<!-- 参考信息 -->