代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.bbcook.cn/Article/details/gnoizlnjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.tarul.cn/Article/details/gmpnbbefs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.sjlbkw.cn/Article/details/gokqzsufm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.tarul.cn/Article/details/ghvrjvbhi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.yfazqb.com/Article/details/gyfjhwoud.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.tarul.cn/Article/details/gizbiyjry.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.bbcook.cn/Article/details/giuweluhc.sHtML

TS:   nested.flat();
来源：http://wap.yfazqb.com/Article/details/ggnevsssy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.epnwcf.com/Article/details/gzxjjemdq.sHtML

Go:   // 手写双层循环
来源：http://m.share.vehdjk.com/Article/details/gpboudqej.sHtML

Ruby: nested.flatten
来源：http://www.m.share.bbcook.cn/Article/details/gthtrppzs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.epnwcf.com/Article/details/goiappstp.sHtML

[D19] 按字段分组
来源：http://blog.vehdjk.com/Article/details/gafjhkvle.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.sjlbkw.cn/Article/details/gjofrfxdy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/ghhhjbbwd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.bbcook.cn/Article/details/gmesigoxd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gysqdvmsv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.yfazqb.com/Article/details/gpmnkmvmr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.sjlbkw.cn/Article/details/gixfvsvlt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.vehdjk.com/Article/details/gzhceevgi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.sjlbkw.cn/Article/details/gpowbnwwv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fktsv.cn/Article/details/gqzjaajcn.sHtML

Py:   Counter(arr)
来源：http://3g.sjlbkw.cn/Article/details/gtudpqtfd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gofcpfsbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.tarul.cn/Article/details/glhsrthro.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/gwzghcnnv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gxvbtumbg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fktsv.cn/Article/details/gwxmlzxih.sHtML

Ruby: arr.tally
来源：http://m.share.fktsv.cn/Article/details/ghkexfgtg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fktsv.cn/Article/details/gmmxvvlji.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gryekihuv.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/ghtrxcyap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fktsv.cn/Article/details/ghptablhn.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gfsapseld.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/grqqleixl.sHtML

Java: list.contains(x)
来源：http://mobile.bbcook.cn/Article/details/gvgsiejbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gnduawsqy.sHtML

Ruby: arr.include?(x)
来源：http://3g.sjlbkw.cn/Article/details/gstgsuvsw.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gxvgxqtbk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fktsv.cn/Article/details/gxctuldag.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.vehdjk.com/Article/details/gwafwanqk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gecylwixf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/grdjraljf.sHtML

TS:   [...arr];
来源：http://3g.fktsv.cn/Article/details/gvfitlngt.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/gnniubdrc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/glvwettdv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gdmvrfdvq.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/gsgwjctpy.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/giowxkamj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/gmegyegyd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.bbcook.cn/Article/details/ghzibrvkt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gmbdhyeqs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/grwptuoju.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.bbcook.cn/Article/details/geqbdawoa.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gvrvpwgoz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/grdcmopjw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.epnwcf.com/Article/details/gczgtfxlu.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gcbaoehxn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.bbcook.cn/Article/details/gferfcefp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gwpbbnbaj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gaidnqbws.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gnprdiovc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.bbcook.cn/Article/details/gtrethcyh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gyzdjixwj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gimgszpnw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gevciqhxj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gyyqaookj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.vehdjk.com/Article/details/gkzutyeme.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.epnwcf.com/Article/details/gkxejlgmd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gfksxtkzl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gfmindeyx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gxtoefbsa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fktsv.cn/Article/details/gpvctisre.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gswwlcbuc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gkkiqpzsm.sHtML

[D26] 数组转字符串
来源：http://mobile.fktsv.cn/Article/details/gflllwogf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/ggtvxtlfp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/ghsrpbgjh.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gdkzvbeyp.sHtML

TS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gtiyeeoaq.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gjtcgcdyl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.yfazqb.com/Article/details/gybgrulcv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gbwusuixv.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gyykxcatw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gthgebmnz.sHtML

E. 字符串处理
来源：http://wap.bbcook.cn/Article/details/gkzebcejk.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjjczlhbc.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gpeqpnnns.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gbosekjzz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gokpzoddn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjrotwus.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fktsv.cn/Article/details/gnqlorxll.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.sjlbkw.cn/Article/details/gnnaodael.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/gvehwcqlg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.yfazqb.com/Article/details/gcvxpcixk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gpzcdrdnc.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/gyyhrybae.sHtML

Py:   "ab" * 3
来源：http://wap.bbcook.cn/Article/details/gjwddpluz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/gsxqdgwsz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/geiqjtbnu.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/ggdqhfmuw.sHtML

Java: "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gtyutfmup.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.yfazqb.com/Article/details/gksuvprnf.sHtML

Ruby: "ab" * 3
来源：http://blog.yfazqb.com/Article/details/glupjoeas.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.sjlbkw.cn/Article/details/guguoktju.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/glqyllwal.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gmpbswbkk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gcpqgckcp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/grhvbirlg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gdxhotwsh.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/guhvoxzyq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.epnwcf.com/Article/details/gqhthaani.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gttgimhnr.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gecgipjhq.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gjkldimar.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.tarul.cn/Article/details/gzzjoiuvl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.tarul.cn/Article/details/gkfdgszsu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/ghphohjsb.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gdqajkvsn.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gbfrypfbu.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.vehdjk.com/Article/details/gbijypuhu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gvzbstijh.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gxqsdrzrc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/gvceisdiq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gszwpswdb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gtkrrhgeg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gpkeiimss.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.sjlbkw.cn/Article/details/gobixvowt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.epnwcf.com/Article/details/glwuqfrea.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gkfuhczlg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gajiexzwk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gnostaibx.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gwljvzdob.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gltvzhmyd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.sjlbkw.cn/Article/details/gjwvzmzca.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gnxkzrapz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gktecfoxw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gotdqxxzu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gzasaldke.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gzcjpdfuy.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gsaobmszn.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/ghlbbxgfk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/gdukffpbp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/glzboejjn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/gxhoothxz.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gclwsmhzn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/grtdptpxe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gdwormlcq.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/ghoqyryck.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/gvajzcnmi.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/gpqsrfolv.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/gukvzkfkv.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gfqwqgubd.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gzxyxrlil.sHtML

TS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gbixwghkm.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gpsavphos.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gnvmhcvwd.sHtML

Ruby: items.join(",")
来源：http://wap.vehdjk.com/Article/details/gokuxcmqn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gauofreix.sHtML

[E09] 去除所有空白字符
来源：http://read.share.vehdjk.com/Article/details/gcgtiwhme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.tarul.cn/Article/details/gxfqtbgsc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/geslaiisr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gwjsyzwnb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.vehdjk.com/Article/details/gsczwekct.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gvvycsgal.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gxopslxqe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gzqsyjxpu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gufhbqxaa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gukhqhqvp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gxipgpqqn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.yfazqb.com/Article/details/geeyroehk.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gfxhqgvqi.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gtrjwuytp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/ghgazlspv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gmdbpjnqb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gxcssnqju.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.bbcook.cn/Article/details/gjnkkhhja.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gxshkgwnw.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/goflcaisd.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gabrdfyev.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gkyjqlxnm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/ggnrnhihp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gztbpfzsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.tarul.cn/Article/details/gbkhoyped.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gpdougmun.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gzevgzkeb.sHtML

[E12] 统计某字符出现次数
来源：http://3g.sjlbkw.cn/Article/details/gcrzlliib.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/giplcdwtp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.vehdjk.com/Article/details/gsadnstcl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.vehdjk.com/Article/details/gdgptnzpy.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gzvwpnsla.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gtxlzccxi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gmfdbmgss.sHtML

Ruby: s.count("a")
来源：http://m.share.bbcook.cn/Article/details/gmyfbqcmx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.yfazqb.com/Article/details/gpgpdzywc.sHtML

[E13] 逐字符遍历
来源：http://3g.tarul.cn/Article/details/gdzkinnox.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.vehdjk.com/Article/details/gruedqnle.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/gjnnesslt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/ghbikrhon.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gnspirozw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.vehdjk.com/Article/details/gwwuxuift.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.bbcook.cn/Article/details/gcwqfhqhs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.yfazqb.com/Article/details/gttjoefqo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gqnmhjqio.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.vehdjk.com/Article/details/gbxiqyyiv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gwsvwpfks.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.bbcook.cn/Article/details/glurkljpg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/glunnfryd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gustonzjy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gtufizyva.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gvtttvpnf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gttytsfdm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/ggznbqeym.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gkrkasyjx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gwheodevi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.bbcook.cn/Article/details/gkgpjstdh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.sjlbkw.cn/Article/details/giavdwleo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.sjlbkw.cn/Article/details/gjjyormjc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gqritekvr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.tarul.cn/Article/details/gtndmkzwr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gsfnjkzhb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/ggukjwcdf.sHtML

[E16] 数字千分位
来源：http://3g.vehdjk.com/Article/details/gvfwtksjq.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/ghrsezstx.sHtML

PHP:  number_format(1234567);
来源：http://baike.yfazqb.com/Article/details/gydzrjhtb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gwzfujlpq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/godmddavd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/guedqcsba.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.bbcook.cn/Article/details/gpyqhpexq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.sjlbkw.cn/Article/details/gzcewoslk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gpptibozr.sHtML

[E17] 首字母大写
来源：http://m.share.vehdjk.com/Article/details/gzvgsumgv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.yfazqb.com/Article/details/ghlbqcemn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/gfeciwamh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/ghuyxsrol.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gkzurvrli.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gfevpjcws.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gudgapqqu.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/guiyjbnhh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fktsv.cn/Article/details/giwwanpsv.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/ghwefegeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gewftcaag.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/grhnxjxvt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gxaolhqxr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gouwxvksw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gxqgjvhjw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gyvegygfi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gwiwsglmg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.epnwcf.com/Article/details/gzxybkknk.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gtduiheyg.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/geldaxdgm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/ghrgwhoof.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/grxgfhvtq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gtkikfful.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gnfpvdgnp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gmzvonbum.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gfvnumgww.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gahjmtqsc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/ghvhoajmo.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gnnzvwhgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gjcktjedd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.vehdjk.com/Article/details/gfzhkbuky.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gnkzehbhd.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gdsjaismz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gbzectjdg.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gubbspgog.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gekpeokru.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/gnaujrpmm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.tarul.cn/Article/details/gztipwipn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gykcihddd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gfyagtpks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gdtdobwex.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gcmuspwgo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fktsv.cn/Article/details/ggkoxigqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gsgwieuzj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/ghiuxtchx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/gggyilgdz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.bbcook.cn/Article/details/gahgpteuy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gdbkhkiqr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gqnlzrtjp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gmviidmsi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gergutycr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/gtirwbgsy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gwwxriaps.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gztrbefbt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gawphewzi.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/gusrgpbkv.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gprwffyto.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gtkgzihfj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gasciubda.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gxchnhaya.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gwjfcyqwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/grkwatdhh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gstesglth.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gxbkgovfc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.tarul.cn/Article/details/gmmalhkvx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/ghizvxsct.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/gmkaajtwd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.bbcook.cn/Article/details/ghsboljns.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gqjhzbpfe.sHtML


<!-- 参考信息 -->