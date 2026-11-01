代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.bbcook.cn/Article/details/ghidbibaa.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fktsv.cn/Article/details/gstykwqja.sHtML

Py:   Counter(arr)
来源：http://baike.yfazqb.com/Article/details/gehzzwsld.sHtML

PHP:  array_count_values($arr);
来源：http://wap.vehdjk.com/Article/details/gowlxwnau.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlnbcajl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/guhijobxu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.tarul.cn/Article/details/gekggfpnq.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fktsv.cn/Article/details/ghwkzklks.sHtML

Ruby: arr.tally
来源：http://blog.epnwcf.com/Article/details/ggzzooyut.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/ghzjwhtrp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.sjlbkw.cn/Article/details/glmqwviij.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gkentmfwc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fktsv.cn/Article/details/gewrvrify.sHtML

JS:   arr.includes(x)
来源：http://mobile.fktsv.cn/Article/details/gkcksntxb.sHtML

TS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gbkoidjdv.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gcxnqfbvi.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/geuzkqmtf.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/gxpjeqtmg.sHtML

C#:   list.Contains(x)
来源：http://baike.sjlbkw.cn/Article/details/gamuvelmf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gqdgjaoiq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gtwqwhbrc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/geeizixzd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.vehdjk.com/Article/details/guvirgnqv.sHtML

TS:   [...arr];
来源：http://baike.epnwcf.com/Article/details/gtejialez.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/grptecnuo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fktsv.cn/Article/details/gtzvstkoc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/grwtqlqmv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gbqiwoehq.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gaioeubin.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/gawcnzcai.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gkomrluwu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/grtlkrsbj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/grrihaivq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.sjlbkw.cn/Article/details/gdydkcjgk.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gguojacos.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.sjlbkw.cn/Article/details/gkzmqnpca.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gksuscven.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gdlmnqgjv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/geziynuhm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghluxikeu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/gxipqezge.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gpjfvcxwe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.vehdjk.com/Article/details/gprijqyen.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gjcvgajfz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gwbquauhq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gudhzgcao.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gjgksdpon.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gjirewtur.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.yfazqb.com/Article/details/gajtoiqje.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/gilbxmkzu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gckzburlg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.yfazqb.com/Article/details/gptqztenr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gmqttbmmm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gjwtheryn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/gykziihnl.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gpogwhifk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gswmrzoyg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gcfbyvmbp.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/giuupuyuk.sHtML

TS:   arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/grjzvltlc.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gbtsqhaqk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gsnjsnhbl.sHtML

Ruby: arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gwzrmkdti.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/ghmwylams.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsgxpnjor.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gvjudowji.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcgottbia.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/giylvqneo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzfqoouy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/ghjzadgyy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/ghxyttyxo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdzbmtpkb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gvktjwsxa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fktsv.cn/Article/details/gncsifism.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.sjlbkw.cn/Article/details/ghmptggvq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpqqcrtb.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwsyalrob.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gfjzbnrgu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/ggtharokb.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gptjulemh.sHtML

TS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gfftdsnzn.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gmxhjirib.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.tarul.cn/Article/details/ggcbtheza.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/gonustwpe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.bbcook.cn/Article/details/gfmyiskyw.sHtML

[E03] 截取子串
来源：http://baike.epnwcf.com/Article/details/gtgdmring.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gehwbqked.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gqivpacqo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fktsv.cn/Article/details/gmzuzwyff.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gqeqjkdzt.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gpubyffht.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fktsv.cn/Article/details/gyjxozkhk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gyftfkyhr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/gvquspamk.sHtML

[E04] 查找子串位置
来源：http://3g.sjlbkw.cn/Article/details/gmfrrkefw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gksqokcic.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/gdurhyxvq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gwojxkhlm.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/ggnzmqzwr.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gyjzpuyjc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.tarul.cn/Article/details/gcerrrbck.sHtML

Ruby: s.index("x")
来源：http://baike.fktsv.cn/Article/details/gfchuynsa.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gqvxeimgs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/grfhaxiim.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fktsv.cn/Article/details/gscejxcjy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gcvlswkmd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/garhuuhuu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/gijwjturb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/gxnrhvdfd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gfaxdsqrw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/ghjxxvjsa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gulwifqpx.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gbyailsbu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gbbvubegw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gnkmfqwoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/glwcclqqz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gglkjfoqu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsesjmwhb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gkkerqxzv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gawezhkhy.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gnqwrorhi.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gelydzdqo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.vehdjk.com/Article/details/goupzlcqv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fktsv.cn/Article/details/ghojfpdwo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.sjlbkw.cn/Article/details/gnscxldwt.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gagykegng.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/ghubjqowx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gdpvjgtht.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/goyxigqxl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.yfazqb.com/Article/details/gzvtqcehh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gtgypeqyw.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gtzbgugcl.sHtML

PHP:  implode(",", $items);
来源：http://read.share.vehdjk.com/Article/details/gkvcouhre.sHtML

JS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gimjwoyeq.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/ggrxihmdm.sHtML

Java: String.join(",", items)
来源：http://m.share.sjlbkw.cn/Article/details/giyolrglp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fktsv.cn/Article/details/gejjlnvrz.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gfezeobaw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/gdokqsvvc.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gjkpbvcnf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.sjlbkw.cn/Article/details/gwjsnvceh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gpqtkljje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/girzqsdmi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gvqqmbrec.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gccanqnad.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gdfmxuxft.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fktsv.cn/Article/details/grinxuqnx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.bbcook.cn/Article/details/gzxwqorrs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gbgzbsgye.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gvvbpulha.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.tarul.cn/Article/details/gedvtaotf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gbbywuwcj.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gzakxwcpt.sHtML

Java: String.format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gnfcfzppc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gxdhtuqmq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gvzwsnlsq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gyekxnwwg.sHtML

[E11] 反转字符串
来源：http://baike.fktsv.cn/Article/details/gtaxckhvy.sHtML

Py:   s[::-1]
来源：http://www.share.sjlbkw.cn/Article/details/gwtmiyzak.sHtML

PHP:  strrev($s);
来源：http://wap.bbcook.cn/Article/details/gbdtpxzov.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxadzsmjt.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gblfeahag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.sjlbkw.cn/Article/details/gdndspqdi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fktsv.cn/Article/details/gpebzwxsc.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/geuupmscd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gtwrddcwh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fktsv.cn/Article/details/gtvfijwho.sHtML

Py:   s.count("a")
来源：http://blog.fktsv.cn/Article/details/gvfykzozu.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.epnwcf.com/Article/details/gllcwctkd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gbnmpjzsm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/grkxvoqav.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gppboygnh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.bbcook.cn/Article/details/gylntsnkm.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/gvgeycrdz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/gljoualtj.sHtML

[E13] 逐字符遍历
来源：http://read.share.bbcook.cn/Article/details/gbulcndbw.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.epnwcf.com/Article/details/guckyegep.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.bbcook.cn/Article/details/giqcevqvw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gwyilwrjd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gpmmpzspi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gqumctlfr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fktsv.cn/Article/details/ghikddsra.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/gycpmrupr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.yfazqb.com/Article/details/gqgardrjm.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/gabqhtoyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.sjlbkw.cn/Article/details/gajhfiuka.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.tarul.cn/Article/details/gcywcvrtd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/gpskipgue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/grjxiktzh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gxkroupfe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gebswxfmw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gvlpfleaj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gsoinzvyk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.tarul.cn/Article/details/ggjlpatwm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.epnwcf.com/Article/details/govoiqhig.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlyuvyam.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gygxzrrlw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/grywfvgam.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.sjlbkw.cn/Article/details/guzeotyox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/gffkrixkk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/goovhhnxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gefuwmdua.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gwtxptfzd.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/ggsfaxzto.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gigvtoqpm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/glbkdwulz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gukbegvkx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gfsdmcgng.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/guudpmxwt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gjzdxrxxl.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.vehdjk.com/Article/details/gjmkeslbg.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gvqneihgz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.sjlbkw.cn/Article/details/ggarmbnfa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gybylpkph.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gqcvybqwx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gazgqxard.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.epnwcf.com/Article/details/gppemvash.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gepskhfaq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/ggftgcwai.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/gxzcvltgp.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gbpbaaakt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.yfazqb.com/Article/details/gnwxrlymi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.bbcook.cn/Article/details/gsnuavkcy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gdvncwdvh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gwapmfhux.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gquvirtjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gkygsjkom.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gscxmlpin.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gdsysidhn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gzlrferpl.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fktsv.cn/Article/details/gzcugcbln.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gohxwkbkl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gzjalufcj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gihczpxfn.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gzvzfhanz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/gaiopvjev.sHtML

Ruby: s.lines
来源：http://baike.tarul.cn/Article/details/gojtlpztj.sHtML

C#:   s.Split('\n')
来源：http://wap.yfazqb.com/Article/details/glfzuaift.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/gnxrwdlbe.sHtML

Py:   if not s:
来源：http://3g.bbcook.cn/Article/details/guteewsee.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gcnffhkbg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.epnwcf.com/Article/details/geydkziqo.sHtML

TS:   if (s === "") {}
来源：http://blog.sjlbkw.cn/Article/details/ghicxsjqw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gjdroxfzp.sHtML

Go:   if s == "" {}
来源：http://m.share.bbcook.cn/Article/details/gdmkgmnyf.sHtML

Ruby: if s.empty?
来源：http://www.blog.epnwcf.com/Article/details/gqupzdwbd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.bbcook.cn/Article/details/gqsowgcio.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/ginenuogv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gxwsxaugo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gnmmmepbk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gmnxzgobs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gphgxkmmw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gkalvceag.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/gisecqfrv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gjhxffazj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ggfvkmmez.sHtML

[E22] 字节长度与字符长度
来源：http://wap.tarul.cn/Article/details/gbdusaafz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gjhkilihu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gbldpztvv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gxnoldnur.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gpliexepr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gvsajstlc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.tarul.cn/Article/details/gfndcapnd.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gudgzgieq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/giagazzln.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glwsdlsez.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gdhgwlelm.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmhqjawps.sHtML

[F01] 读取整个文件
来源：http://wap.epnwcf.com/Article/details/glhssplqj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gikrxxais.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gjthttqpi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.yfazqb.com/Article/details/govmeanuz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gxpfndswz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gzperummp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gbilgkzap.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.tarul.cn/Article/details/gofkhmmff.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gdqrybdci.sHtML

[F02] 逐行读取文件
来源：http://blog.yfazqb.com/Article/details/gmyrmoazr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fktsv.cn/Article/details/gzlbgqqem.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.bbcook.cn/Article/details/gxftdlbsu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gsgxcxwpt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjxqqrghy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gujhwdufn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.tarul.cn/Article/details/gqmolkbqh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.sjlbkw.cn/Article/details/gqlssfill.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/giocjntul.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gpjtyyevi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fktsv.cn/Article/details/gyykhulmy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gftovktbw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/granitcty.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gavbpqjcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gwasrjxqq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/gieuzwmio.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gwytpceiu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gczbaqbzn.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gvfwvxsqj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gagldoseb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gigsseqwa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gnxaxiepu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.tarul.cn/Article/details/guoyjixfd.sHtML


<!-- 参考信息 -->