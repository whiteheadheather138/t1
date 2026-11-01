代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gdzacwrbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.vehdjk.com/Article/details/gnwigagqo.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fktsv.cn/Article/details/gccpcjoxz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/glpvfgbwy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.tarul.cn/Article/details/gbmjwdyxq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gigndlirg.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/gdprcdodo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.vehdjk.com/Article/details/glwrtznjf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fktsv.cn/Article/details/gadxqvdvk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gdubvxxyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/gymelbodw.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gdfizcpsi.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gaeywgiqa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.bbcook.cn/Article/details/gmldxwwdq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/gcfayqhte.sHtML

Py:   x in arr
来源：http://www.blog.tarul.cn/Article/details/gycspmsfw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.bbcook.cn/Article/details/gwtiqxvpb.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gvmqchxns.sHtML

TS:   arr.includes(x)
来源：http://www.blog.bbcook.cn/Article/details/gdhkywpfq.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/gbjuiujvn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gcdpywxib.sHtML

Ruby: arr.include?(x)
来源：http://mobile.yfazqb.com/Article/details/gyukmycbk.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/grdtmemcu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.yfazqb.com/Article/details/gwozrggut.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gicujgujw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/gthixeowz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gnwitvzsl.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gneimofkp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gvexkxqnd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gergeijfl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.sjlbkw.cn/Article/details/ghvchwfgl.sHtML

C#:   new List<int>(list);
来源：http://www.share.bbcook.cn/Article/details/gixuifiev.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/ggnsgddeb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gheggaopn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/gmlwgfedf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gnkwmsajs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.vehdjk.com/Article/details/gylrkcjbu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gfwwgwdhl.sHtML

Go:   // 手写循环
来源：http://read.share.sjlbkw.cn/Article/details/gnprkkuhm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.bbcook.cn/Article/details/gqaxezoar.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/guaidnglm.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.vehdjk.com/Article/details/gbhcryqzq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.sjlbkw.cn/Article/details/ggmvybdex.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/girseurjj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.epnwcf.com/Article/details/gakzwilnc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/gnhhesksg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.sjlbkw.cn/Article/details/gpbhofxji.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gqcnryilz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fktsv.cn/Article/details/gedxsxgvh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gsyoliizo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gtkcxkqej.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/gjrchhult.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/ghlzeuztg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.sjlbkw.cn/Article/details/geqsujbjg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gfchlmhqt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.epnwcf.com/Article/details/gcumuyavm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjeadjli.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fktsv.cn/Article/details/glypokcfz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.bbcook.cn/Article/details/gqbjvfytj.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/gfkyeaaen.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.vehdjk.com/Article/details/gmyqrimvx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/gkirfaale.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gmyzlnvgk.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gkomwycoj.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gvsbfnbzc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.yfazqb.com/Article/details/gsirfjczy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gktynajuv.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/ghvpdxlnb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/garchykps.sHtML

E. 字符串处理
来源：http://3g.vehdjk.com/Article/details/gvfjcxswf.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/grmcknpsc.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gilvnkyfq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fktsv.cn/Article/details/gcankkamf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gffishpmo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gexgskfdi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.yfazqb.com/Article/details/gprnutalx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/ggqokmyeq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gtyombhsq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.epnwcf.com/Article/details/gsdwgqemc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/ggpunqccr.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gubyoyzcr.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gzaroftgi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gzupmtjnu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gpzkhamuy.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/glbtdiovn.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gksdcxxsk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/gbcpjrdyv.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gzcuaquvx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/grdswxltm.sHtML

[E03] 截取子串
来源：http://m.share.epnwcf.com/Article/details/gbpjbflen.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.epnwcf.com/Article/details/ghrrpwkks.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gqojwuzcd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gwqdspszx.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/getlkauid.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gdrqndevs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gxlfvsoch.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fktsv.cn/Article/details/gcsgrntap.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gzxccffiu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gdfwzrtmj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gbgzmifhh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gmiurbvhi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gwfsmtwml.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gbhtdvdlb.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gmnvsjsfx.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gwosvfpun.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gjamkqyms.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/ggxwecopi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/gutuoqbzj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gsqihvisf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/grkhgzhsh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gquzebiyz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gzcqxoova.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gzkfirjce.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gbtkbftks.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.tarul.cn/Article/details/gdapswwfw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/gtqxydqcf.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gcyqzvvdw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gkeoyvrst.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gwvzqixfn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gkiffduop.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gjqdkefmh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gymwtoztd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.yfazqb.com/Article/details/gimetyfyx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gjjuktcns.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/girgrmylv.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gdcugfkqs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gurgogwlz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gacjozhfx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fktsv.cn/Article/details/gxvoxgpfm.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gwugqppzg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gywqttqnr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.yfazqb.com/Article/details/gpfvbquco.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.sjlbkw.cn/Article/details/gvqnqcxxp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.yfazqb.com/Article/details/gblytuckd.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gyggckicy.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gngryjpnn.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/goqisospt.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gusunggos.sHtML

TS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gctjrdsla.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gbpborehn.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.vehdjk.com/Article/details/goilrchin.sHtML

Ruby: items.join(",")
来源：http://3g.tarul.cn/Article/details/gimozpuwb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gzlhhsetu.sHtML

[E09] 去除所有空白字符
来源：http://wap.yfazqb.com/Article/details/govqnhktf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/gaiavbhya.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.tarul.cn/Article/details/gznugtvaf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gujyngddf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/ghyemqlqy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gbtuqjhjj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/ggddfsmij.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/gpwpowdis.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gkewetovv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/gnbecxrhp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gnkgnqocs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.tarul.cn/Article/details/gptuaxkel.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gujnbezjj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gbzpktord.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gnooifdmi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/glizeyock.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gchhafvyw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gqjgcgqsi.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gixvrhbbr.sHtML

Py:   s[::-1]
来源：http://blog.bbcook.cn/Article/details/godboiavu.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/ghbasvarr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gsmuhajvu.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gakjhbatz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gvdemdoim.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gdkzzmwxe.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gipuuqmpu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gjcxroqje.sHtML

[E12] 统计某字符出现次数
来源：http://wap.vehdjk.com/Article/details/gevhfaakj.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gzddhymbw.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/guokjklfv.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gpyqodddi.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/ghcfcoqnj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gtgsjzgcy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/glqkdgtwh.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gztwvogua.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.vehdjk.com/Article/details/gxrhpucdb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.tarul.cn/Article/details/gdjkvpejg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/ggkvqgapn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gusyxdrta.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/goqmhewrr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gsyustttg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gzzsfonyd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/gcnvnsywv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.yfazqb.com/Article/details/gclkkjchp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.yfazqb.com/Article/details/gslnhywud.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/glmidkkim.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gfmjxsjcc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/gxoosdezr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gwrbevnvu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gfayzaolz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.vehdjk.com/Article/details/geghcvtvz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/geguisoim.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gegpqmjza.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/ghelwtenv.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gfknistwj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.epnwcf.com/Article/details/guhzsbrti.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.bbcook.cn/Article/details/gulntfger.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gxcvzqwfg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.sjlbkw.cn/Article/details/gxiiyoubr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/glhzshdgk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gajdqtjpz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/gmidzioka.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gimnokjtt.sHtML

[E16] 数字千分位
来源：http://m.share.sjlbkw.cn/Article/details/gysiqstlp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/grhmdcfdr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gzqoohoey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.vehdjk.com/Article/details/gbxavbwyc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gkdurcgtj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gilqblrks.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fktsv.cn/Article/details/guqvwsvsz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.yfazqb.com/Article/details/gjqjhglfy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/ghzxvabdw.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/gtatmgudy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.yfazqb.com/Article/details/gqjvyibqv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gngvjdfmi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gskrjpfag.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gdwmzjoft.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gazpnhbte.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gqnlonjhy.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gffqmdezz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.yfazqb.com/Article/details/gwzvcrtsv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gxcxsuzvb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gltfoyekc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fktsv.cn/Article/details/gzpkcbijg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gxixkblnz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gztqbzhws.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gjlwhtypa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gepmnvebb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fktsv.cn/Article/details/gvsfzhwzo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/geoarktxw.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.epnwcf.com/Article/details/gavhgponr.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/ggxgmcnpt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/giijlhpao.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gkyykfyud.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gzxebdvld.sHtML

Java: s.lines().toList()
来源：http://baike.vehdjk.com/Article/details/gghwkldyj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gcnihkxnh.sHtML

Ruby: s.lines
来源：http://www.share.fktsv.cn/Article/details/gmmwhaqsi.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/ggxkumsgu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/gkuiwmiuz.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gfkvmqixq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gpofxeblj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/glraokesz.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gtfvqmnkx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gnonsitem.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/glwkwowxi.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gdvrnggav.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/griqspkst.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gmxelusxl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gsxyohgia.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gwlxlmlla.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gtxsxckru.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gmtqnwsly.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gugynikgn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/gxzgfqotu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/glnvcdjig.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gybiqnwzm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gsufrtjrr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/gzumafhao.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gpbwxnbsg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/grvkprazj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/gtocakyoc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gbrpeflac.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/gpltkwuvf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/glddwlewj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.vehdjk.com/Article/details/gmltlxgdg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvfubptcz.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gtfijunzd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfytmmpwy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gtcbuqoon.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.vehdjk.com/Article/details/gwrvsvtvg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/guwrpelea.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gjvjferii.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gmmcimnnh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.tarul.cn/Article/details/gzrolxkyg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gasninsau.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gdxnaijxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.vehdjk.com/Article/details/ghglqgzxa.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gzpvnqptp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.vehdjk.com/Article/details/gzklmizrx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gpirjmunt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/ggxxpiqes.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/glbhdmwde.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.bbcook.cn/Article/details/gxgclmsrf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gdisairzs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/goxzbiicd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/ggzxajoip.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.vehdjk.com/Article/details/guzepeksc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.tarul.cn/Article/details/gghvvrxcf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gwtyvwfjr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gysfeshdm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gcdpwizsm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gziykfcaw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.tarul.cn/Article/details/gtyolrqqb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/goredadtp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gopddelbl.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/gniylrxcs.sHtML


<!-- 参考信息 -->