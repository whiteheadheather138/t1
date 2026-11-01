代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.bbcook.cn/Article/details/gnfjesuii.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fktsv.cn/Article/details/gturhmyjw.sHtML

Ruby: nested.flatten
来源：http://wap.bbcook.cn/Article/details/gmnnmyfsl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.bbcook.cn/Article/details/gnunqhvum.sHtML

[D19] 按字段分组
来源：http://www.share.yfazqb.com/Article/details/gcsqfobcr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fktsv.cn/Article/details/gfqucxawx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.tarul.cn/Article/details/grsivcmws.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.bbcook.cn/Article/details/gdlwszbps.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/guhuwnyri.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fktsv.cn/Article/details/gppsykmlf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.bbcook.cn/Article/details/ghobxlcmj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fktsv.cn/Article/details/gsgrylads.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fktsv.cn/Article/details/gxgybderq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.epnwcf.com/Article/details/gdcoskcvz.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gshqlzbrv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.bbcook.cn/Article/details/gstihouje.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gbfisvell.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gbhfogllc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.yfazqb.com/Article/details/geetyabkd.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fktsv.cn/Article/details/gztiozswo.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gllvcemza.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fktsv.cn/Article/details/gsgdncsut.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.epnwcf.com/Article/details/gldfbbkhk.sHtML

Py:   x in arr
来源：http://wap.epnwcf.com/Article/details/ggnrtyqox.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/gtqbzsvcv.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.yfazqb.com/Article/details/gusvkzhlr.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gjrluqozj.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gwcfhpkbv.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gzcamcduv.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/glmvngdlk.sHtML

C#:   list.Contains(x)
来源：http://mobile.vehdjk.com/Article/details/gqiybxsrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gatdtzezp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.epnwcf.com/Article/details/ggiaeboti.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.sjlbkw.cn/Article/details/giwcjyolr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gnvclphpo.sHtML

TS:   [...arr];
来源：http://baike.fktsv.cn/Article/details/giorfsueb.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gvedxmpwx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.bbcook.cn/Article/details/gukccaiyl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gpnkmrkyx.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gdbgxraiv.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gpstsidgr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gcgabelfh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfplceyz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/goywwrqsw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gmcidzhgw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/gwfkjlptz.sHtML

Go:   // 手写循环
来源：http://www.share.tarul.cn/Article/details/gfxjuzmap.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.sjlbkw.cn/Article/details/ggqtpehdc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gbwithvgr.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gwyuvqcok.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.yfazqb.com/Article/details/gxcotympa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gccifqsgx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gmwvrnycf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gsdxxjgty.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/ggonqhyww.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gggijrfss.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/ggwmlhnnz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.tarul.cn/Article/details/ghvpymvqc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gxpicfbmn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gghqtheyx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcmmesor.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fktsv.cn/Article/details/gdipybqua.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.vehdjk.com/Article/details/gatqhgwgb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gipslmlfg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gphhcdzhk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.epnwcf.com/Article/details/guoumxyqg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.sjlbkw.cn/Article/details/gpwlkjcgm.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gflxwjufg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.bbcook.cn/Article/details/gjjdrqhwh.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gluctylxb.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gsjurznec.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gimhrdffi.sHtML

Java: String.join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gigiecfyg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gsvfreszh.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/grwiezknz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gpdayraxr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gpeanryzq.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gtniuplxs.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gagneazqz.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gtbikkhtc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.yfazqb.com/Article/details/ggdsiuzee.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gzkmwqgyc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/geazxhxiu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gpxpdftmp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.sjlbkw.cn/Article/details/ghnplvvwi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gqlfsuutt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gejmiyvia.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gpmspgiyd.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gtiwfghus.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gyrgdidgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gfteaggtm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gpyhclulh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/getndevub.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gxfuipjfs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fktsv.cn/Article/details/gjhwygazp.sHtML

Ruby: "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gnaigpdih.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fktsv.cn/Article/details/gbsvygpwp.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gziuhwnci.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.sjlbkw.cn/Article/details/gpeipdqjl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gdiaaabld.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gouzyrwix.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/glyavvjwm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gpafrzsqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gmkrprkge.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.yfazqb.com/Article/details/gnohsbuli.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.bbcook.cn/Article/details/gfkcpnhie.sHtML

[E04] 查找子串位置
来源：http://blog.epnwcf.com/Article/details/gctmbyyra.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.tarul.cn/Article/details/gxwsxsmvj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gwdgsthkx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gegwebqwj.sHtML

TS:   s.indexOf("x")
来源：http://baike.tarul.cn/Article/details/gdhtwzmon.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/ggqfxbbqk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gjlxjmikx.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gnlpwlrpf.sHtML

C#:   s.IndexOf("x")
来源：http://baike.vehdjk.com/Article/details/gvynrmkrv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gjqjflfdr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gxybkyixc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/galyjpdfb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gkhvdhzip.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.bbcook.cn/Article/details/gxlntitis.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoeyxutg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gdzohpyxo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/gewbzlqjh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/glqxditrf.sHtML

[E06] 替换子串
来源：http://baike.vehdjk.com/Article/details/gufuhxbcw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gncddwdly.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/gzzvbpjda.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gmspdtuyw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/glfrsxyty.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gdtmevmys.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gqaqchxxs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/grbrrfcaa.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gzvmsrcgk.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gqlsweoii.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/ggmjnlkvz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fktsv.cn/Article/details/gntbfckvs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.vehdjk.com/Article/details/grxglsblx.sHtML

TS:   s.split(",")
来源：http://baike.vehdjk.com/Article/details/gkcrtilvt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fktsv.cn/Article/details/gawppwmfb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gihydjmam.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/ggmucbhll.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gicdjbkpi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.tarul.cn/Article/details/gxhgdgjzc.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gipzetxhf.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gjmlbudfq.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gemuxetyt.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gvudqijoh.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gdokeejnl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.bbcook.cn/Article/details/gosfvgtfw.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gwifgykej.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gxkecmknh.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/grrqfmrfa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.tarul.cn/Article/details/ghngvemjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/goplyunwa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/ggtrscrer.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gdfdqypzt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/grqoyjvna.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gqndnzfuu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gjzdfcesa.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.yfazqb.com/Article/details/gzlucajtm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gnobhtcav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/guebacsoa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gpejgkaes.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gtiyzdzaj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/grdxusayb.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gnhryzbvz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gjqgptdaj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fktsv.cn/Article/details/gqxijfduo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gcioekjtg.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gucmdyzmx.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gdpyuqanx.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/gikiardmi.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gdkdhnizj.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/geppuqrcd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gsjgdoqsy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/glyaevqvs.sHtML

Ruby: s.reverse
来源：http://blog.fktsv.cn/Article/details/guxdwkmhp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gibjflyqs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.sjlbkw.cn/Article/details/goprdkfqj.sHtML

Py:   s.count("a")
来源：http://read.share.fktsv.cn/Article/details/govzljmpy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gvhnlfehu.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.bbcook.cn/Article/details/gnbncynyb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gcwhcylvb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/ginzkrxax.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.tarul.cn/Article/details/gvpcxbnjq.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gqsatloth.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/giodmhttp.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gpptqejyj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gugomagxf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/ggejgxyrc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gsztqxlzt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gvmczlvey.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gmykydhfa.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gitkqorvh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gwsljyqlr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fktsv.cn/Article/details/gmvehauow.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gbsodeogj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/glehqswlr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gwhzaqpnu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/gdelnwppc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/gasqiqejm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gkmhxvmqu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gkhwznuwn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.yfazqb.com/Article/details/gfakwjxdn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.vehdjk.com/Article/details/ggiduvkgs.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.tarul.cn/Article/details/gjopbtrgp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmoyvzume.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/gvbllnttq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gqtipvvnu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gcclhqgtp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fktsv.cn/Article/details/gcbpkbwmg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fktsv.cn/Article/details/gveqoqxrj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.bbcook.cn/Article/details/glfvdkdgh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fktsv.cn/Article/details/gxwjjlqbb.sHtML

[E16] 数字千分位
来源：http://baike.bbcook.cn/Article/details/gvqbmlrra.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/ggffbywcp.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.tarul.cn/Article/details/glhteqrrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gayqfiyzc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.epnwcf.com/Article/details/gutoymahj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gmkzqlhlk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gtpuorhxb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gifvhawxz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/glzrkatks.sHtML

[E17] 首字母大写
来源：http://wap.vehdjk.com/Article/details/godkdcpyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/glrwngeus.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gfmqdtyno.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gkzklvpjt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gdbdlepig.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gbbwmvelt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.vehdjk.com/Article/details/glgvyhhqq.sHtML

Ruby: s.capitalize
来源：http://www.blog.bbcook.cn/Article/details/gjhnlzwpl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gocnqtilt.sHtML

[E18] 模板占位符替换
来源：http://read.share.epnwcf.com/Article/details/geqdehlfw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/grmicumqn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gyqbrpzou.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gmmltczse.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gyjydxovs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gvpmkripq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gjoocjnon.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gylfupnsg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gyajurxyi.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gqensorio.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gkmifbijz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gqxtfefrl.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.yfazqb.com/Article/details/goujpyfrj.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gqtymgvtj.sHtML

Java: s.lines().toList()
来源：http://www.blog.sjlbkw.cn/Article/details/gliysykul.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.bbcook.cn/Article/details/ghvmxbhed.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gzbhudivp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gmhfiyrlu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gaxtmwuof.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/gjxxinnhx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/gwwzhhtag.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.tarul.cn/Article/details/gqxaedwoa.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/gdfaodoxn.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gusrpkdip.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gycacxrxo.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/geuxeqyyy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/gpydzvkyd.sHtML

[E21] 超长截断加省略号
来源：http://www.share.sjlbkw.cn/Article/details/gpuimjonn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gmgdqxeug.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.tarul.cn/Article/details/gwrwpdvfv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/grxjcptbk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gsayofxye.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/grvupyrov.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.sjlbkw.cn/Article/details/ghzejghvp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gdbdykukq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gfpmqealv.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.vehdjk.com/Article/details/gxfuhtixu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gphdmwozt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gwyeequvf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gogwtcvsx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gwhagypwa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.epnwcf.com/Article/details/ghxmoxcgp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gtmhadipy.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.bbcook.cn/Article/details/gdbpzxasg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gfioesuxv.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gydfwsqwr.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/ghayykonj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfofinxck.sHtML

[F01] 读取整个文件
来源：http://m.share.yfazqb.com/Article/details/gaswnlskw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.vehdjk.com/Article/details/gzpzmbebn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwkziremj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/ghwiubzib.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gzgcyavel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/glwdwncgw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gnyooytxh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gckrbhyco.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gayvehzgf.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/geetlzsou.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.yfazqb.com/Article/details/gthdiehvo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.yfazqb.com/Article/details/gemoywqyu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gqactkjsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/gacsqflzm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gkmhcpkbf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/glvvitajg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzbzurah.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fktsv.cn/Article/details/ghjhmyhzw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gqqtrztyi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gdxmciddr.sHtML


<!-- 参考信息 -->