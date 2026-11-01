代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gljwehnfn.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gbosbnqio.sHtML

Ruby: nested.flatten
来源：http://www.m.share.vehdjk.com/Article/details/guptenufd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.epnwcf.com/Article/details/gfdojysln.sHtML

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gjfqihjiz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.vehdjk.com/Article/details/gpxmewglz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.yfazqb.com/Article/details/gjlcyfqfe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.epnwcf.com/Article/details/gphguddfa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gjhrnusyw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.vehdjk.com/Article/details/grsjzvyqc.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.bbcook.cn/Article/details/gepwotauw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.epnwcf.com/Article/details/gttwfldho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.epnwcf.com/Article/details/gqkpshcoj.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gzfhszxke.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gstwauhsb.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.sjlbkw.cn/Article/details/gdkkzalok.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gdangpmjs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/gfyeprtwl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.vehdjk.com/Article/details/ggjlizgbv.sHtML

Go:   // 手写 map[T]int
来源：http://wap.yfazqb.com/Article/details/grqrkqmos.sHtML

Ruby: arr.tally
来源：http://wap.vehdjk.com/Article/details/gukkttnvn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.yfazqb.com/Article/details/gqkohncay.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/gutrtclet.sHtML

Py:   x in arr
来源：http://www.m.share.epnwcf.com/Article/details/guhwaflsm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.bbcook.cn/Article/details/gktpdnnqy.sHtML

JS:   arr.includes(x)
来源：http://www.share.epnwcf.com/Article/details/gfcraclum.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.bbcook.cn/Article/details/glbuogrlw.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gnxgfvhhw.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gyzcalqix.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/gydtqqjnc.sHtML

C#:   list.Contains(x)
来源：http://3g.fktsv.cn/Article/details/ghucctmqu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.vehdjk.com/Article/details/gcjpbhjhj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gmjvfdgaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fktsv.cn/Article/details/gdktaxgli.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/giwbueebg.sHtML

TS:   [...arr];
来源：http://www.share.yfazqb.com/Article/details/gpjscbxqv.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gpkqnrvho.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gunirlbey.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/gsgbxcxha.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gfzdenvhb.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gdakdhyfg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.bbcook.cn/Article/details/ghxinfgmg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gbaherujb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.tarul.cn/Article/details/gcuglccpr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gipzpluuy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.tarul.cn/Article/details/gaercxzcx.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gljaojffw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gudijswdv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gznhedbft.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.epnwcf.com/Article/details/gpwhfkbch.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fktsv.cn/Article/details/gcqktqorn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gdxabropt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/getthygwy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/goxiupinb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gtlgclyhv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gfihnzoyb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/gmwsxdaej.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gffnswjmz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.tarul.cn/Article/details/gtcjlddda.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gbmxrywis.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gbgkumkpi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/gurogcuwd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/giiidagff.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.sjlbkw.cn/Article/details/gloipfpes.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/ghoufczgi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.bbcook.cn/Article/details/gsuczwctx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gvanpzxoz.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/ghyrzfmtp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gchhtrshm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gnwbdvogx.sHtML

JS:   arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gktinjgmr.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gudbdcfgb.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gwqoeeamf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.yfazqb.com/Article/details/gpblqwbtc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gqgjymsvd.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gnfxuzohp.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvvboqtyw.sHtML

E. 字符串处理
来源：http://blog.sjlbkw.cn/Article/details/gsillnvfm.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/glctrfnqq.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gjnfiatfm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gpagwgrug.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.bbcook.cn/Article/details/gwsxblrqg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gxbbaaagw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gmzgtzexm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/gchkjfeqi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gthqfwdgy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/guexpbnry.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gqcmttxpu.sHtML

[E02] 重复字符串
来源：http://www.share.tarul.cn/Article/details/gaxgckpgj.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gsshmuhhh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fktsv.cn/Article/details/ggxtoewjp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gsjgpklzv.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gypowdtgc.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gilwiorjy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gvfycadxw.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gmbvkgeyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/goxllwryz.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gfphuodnn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.sjlbkw.cn/Article/details/ggrzywihe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gqomqsixv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gcuxpfdkl.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.yfazqb.com/Article/details/glqsnqshg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gmzgxrpfn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/ggosuauds.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.bbcook.cn/Article/details/gjrpedzts.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gfyvfwjfp.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gonapyvff.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/guwujqxyt.sHtML

PHP:  strpos($s, "x");
来源：http://wap.sjlbkw.cn/Article/details/gtprpfgld.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gugbmvsze.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/ghcmkdhhi.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqfswgje.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/glukblkas.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gxrmindum.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gplsotmqn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gapleiysg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gcdvndqve.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gvpqynken.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gznjejisa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gnrbartde.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gygasjhjb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.sjlbkw.cn/Article/details/gxfqzdssh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.yfazqb.com/Article/details/ghvzhbfil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/gjajanrld.sHtML

[E06] 替换子串
来源：http://mobile.sjlbkw.cn/Article/details/gqdhxomly.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gczfzynmc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.vehdjk.com/Article/details/gmwhjfpeo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gvxqetqwm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gfrsbcckg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugvhswet.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gyjwzpcjp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gphegvklp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/goxlfjhln.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gqvfrxpdi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.sjlbkw.cn/Article/details/gtojnkquo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/ggacwadey.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fktsv.cn/Article/details/gjcjljrso.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gydzkmjpj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/gmqmqfutg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gimuytgra.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gtuagvbpo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.epnwcf.com/Article/details/gkfmkbgms.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gnagoxeck.sHtML

Py:   ",".join(items)
来源：http://read.share.sjlbkw.cn/Article/details/gooddyydh.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.yfazqb.com/Article/details/gjeqqqkno.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gjztvetbx.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/grdpnhdsg.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gqkchfwnv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gcxeofiqw.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gnzftuorx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.tarul.cn/Article/details/gqmjjcmoj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/gjayxybmn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/ggnpouccd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjtcgssgb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gpyggobhv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.vehdjk.com/Article/details/gtzhcmgje.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gbyjcdejb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gskyqbkrw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gjstdfgob.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.bbcook.cn/Article/details/ghbfnabcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/ghbupogty.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gwvedcaso.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/grrtzysos.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gqvnmiibh.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gggsdnrgx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gssjmeuir.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gyhuobtou.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gfhvgafgr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fktsv.cn/Article/details/gwjyprhlu.sHtML

[E11] 反转字符串
来源：http://wap.epnwcf.com/Article/details/gelzzchlk.sHtML

Py:   s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gclhvbimt.sHtML

PHP:  strrev($s);
来源：http://www.m.share.vehdjk.com/Article/details/gwfflozqg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gcixpjauf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gliggqckh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gahaasgbs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gbrtkzxta.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/guyhdytjj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.epnwcf.com/Article/details/goexdosqz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.epnwcf.com/Article/details/gnfwoyaxx.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gsxactdyj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gxuigzdmv.sHtML

JS:   s.split("a").length - 1
来源：http://3g.vehdjk.com/Article/details/gvyrrxluo.sHtML

TS:   s.split("a").length - 1
来源：http://wap.epnwcf.com/Article/details/gnrgzmusm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.vehdjk.com/Article/details/grththwsp.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gultzqncn.sHtML

Ruby: s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/gecmbkbxw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gkwyssyad.sHtML

[E13] 逐字符遍历
来源：http://3g.sjlbkw.cn/Article/details/ggcwpkfwv.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gnpqcvtdy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.sjlbkw.cn/Article/details/gdmxjmsmx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/golnikmdy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/gwqlgmqpu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.epnwcf.com/Article/details/gwydqwswc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.tarul.cn/Article/details/gsxudjsit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fktsv.cn/Article/details/gxpubsscm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gkxwaoxig.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gcwjiyyxp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.tarul.cn/Article/details/gqbgajowp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gbiojrwmu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.epnwcf.com/Article/details/gldvieotj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/grnfnfcgh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gooimjssc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gckfmptdb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/gkijhcwbg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gdulgjvkk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.vehdjk.com/Article/details/gldenlmzg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.tarul.cn/Article/details/gsevyxuvr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gfdvqberr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gvdsblbii.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/gilcdevdt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gyelsnmso.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gurmqwcvc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fktsv.cn/Article/details/gaephyztp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gapemnfef.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gapxaklnw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gbojktqvx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gsgllpjlc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/gvfqhgkrp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.vehdjk.com/Article/details/gvussxwgn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gudrgurwl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gnqtkkswh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gqonpbmzs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.sjlbkw.cn/Article/details/gxtybfwnc.sHtML

[E17] 首字母大写
来源：http://mobile.epnwcf.com/Article/details/gfvgykwez.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fktsv.cn/Article/details/gddfkrojv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.tarul.cn/Article/details/ghzaootsg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/giepburyp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.sjlbkw.cn/Article/details/gpwmkpjnw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.bbcook.cn/Article/details/gnyxgeopy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gjaufphcv.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/geesedhct.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gwuddryot.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gutjowkay.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gdmxwfwxl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gvopqzvbn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gmzxolipf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/glwknzkhq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gulecmjiy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/gajropvwh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.bbcook.cn/Article/details/gsleqdwtc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.epnwcf.com/Article/details/gixoorbdv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/guacxqgmo.sHtML

Py:   s.splitlines()
来源：http://wap.vehdjk.com/Article/details/gekwwblhk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fktsv.cn/Article/details/gyfgkvyuy.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/glynzxxze.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gfdrkqldr.sHtML

Java: s.lines().toList()
来源：http://mobile.tarul.cn/Article/details/gsjxmiuzb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/grfxwdwpr.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gwkxypnlw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gilwweitp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gymqhtxxj.sHtML

Py:   if not s:
来源：http://m.share.yfazqb.com/Article/details/gsgveybof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.tarul.cn/Article/details/guiahgtwe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.tarul.cn/Article/details/gppqwdhot.sHtML

TS:   if (s === "") {}
来源：http://3g.fktsv.cn/Article/details/gfawygaij.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gxoflndah.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gvribnxqh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fktsv.cn/Article/details/gdnodpdzc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmykaadyq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.yfazqb.com/Article/details/ggyqyuokk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/guhxnmvae.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gyybudatd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gyatchror.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gfgszvxro.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gwximldra.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fktsv.cn/Article/details/ghjjszkrz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gylxpfthp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/grwqaldqk.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gkkliprsg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.bbcook.cn/Article/details/gayuddldb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gmryrxpkg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gdhyddkxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gtuixxqsa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.yfazqb.com/Article/details/gwgjthsno.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.epnwcf.com/Article/details/glgzslysh.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.vehdjk.com/Article/details/gvugdaqku.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/gnfeclzxq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/galqfaqcy.sHtML

F. 文件与目录
来源：http://m.share.tarul.cn/Article/details/gsoiepbod.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gomymueet.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gpkqyfurg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gbjtlunfi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/ggnhsmfim.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.yfazqb.com/Article/details/greblibor.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gomdjyeqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gulegsdbu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gdjimylwl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gvwapegys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/gjdcwwypw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.bbcook.cn/Article/details/ggzcjftlz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gnfjsdmwe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.vehdjk.com/Article/details/gguvtqcwd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gvzdvdefo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gpzjpdgvi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gxwyrsxdn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.epnwcf.com/Article/details/gvxymcnum.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.epnwcf.com/Article/details/gwkrcbcgp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.vehdjk.com/Article/details/gbiatzqcd.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.epnwcf.com/Article/details/gunomfiqj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/gkkiekkhg.sHtML


<!-- 参考信息 -->