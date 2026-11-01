代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.share.tarul.cn/Article/details/gllvlwmwj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.yfazqb.com/Article/details/grlobiwxm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.epnwcf.com/Article/details/guhuvgjek.sHtML

Ruby: arr.uniq
来源：http://m.share.tarul.cn/Article/details/gyqrrhblk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.yfazqb.com/Article/details/gvzljwjmk.sHtML

[D16] 求和与平均值
来源：http://3g.fktsv.cn/Article/details/glrugtusa.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gczdgyqxr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.bbcook.cn/Article/details/gsopqgrne.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.bbcook.cn/Article/details/gkccvzqaz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.bbcook.cn/Article/details/gdretiirf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.sjlbkw.cn/Article/details/giyloefwg.sHtML

Go:   // 手写循环累加
来源：http://baike.yfazqb.com/Article/details/glumkxslr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.bbcook.cn/Article/details/gruysaznu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.sjlbkw.cn/Article/details/gycpsdkjj.sHtML

[D17] 最大值与最小值
来源：http://mobile.yfazqb.com/Article/details/gbrkxncxl.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.yfazqb.com/Article/details/gonrhnavr.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.vehdjk.com/Article/details/gyayecwcm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.yfazqb.com/Article/details/gordxyinf.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.vehdjk.com/Article/details/gzsdyuuyo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.sjlbkw.cn/Article/details/gjgqbychj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.yfazqb.com/Article/details/gffkabhnv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.tarul.cn/Article/details/gehmsipnm.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.epnwcf.com/Article/details/gppssujwe.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gqazeuefl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gfxwmuklo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gnwdqrioi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.vehdjk.com/Article/details/gybyskyoy.sHtML

TS:   nested.flat();
来源：http://www.m.share.epnwcf.com/Article/details/gqchjvmyl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.vehdjk.com/Article/details/gpoehwetn.sHtML

Go:   // 手写双层循环
来源：http://baike.bbcook.cn/Article/details/grggtxlel.sHtML

Ruby: nested.flatten
来源：http://baike.yfazqb.com/Article/details/ggllbcgnw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fktsv.cn/Article/details/gzfujhnfl.sHtML

[D19] 按字段分组
来源：http://wap.yfazqb.com/Article/details/gwzfypket.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fktsv.cn/Article/details/gvjbrcqah.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.yfazqb.com/Article/details/glfkcvtsx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gnxxqtfxr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gkdefrywm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.vehdjk.com/Article/details/gquvnuvlz.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.tarul.cn/Article/details/gubfzpafi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.tarul.cn/Article/details/guobxngpw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fktsv.cn/Article/details/gavulrvgp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.epnwcf.com/Article/details/gsgmldxtp.sHtML

Py:   Counter(arr)
来源：http://3g.tarul.cn/Article/details/gcuwcxjfz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/gdqqytcej.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gomjybhfu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gguwnzwyf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.vehdjk.com/Article/details/gvzqmblsr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.epnwcf.com/Article/details/gtksmgtwx.sHtML

Ruby: arr.tally
来源：http://blog.fktsv.cn/Article/details/gibwlqbky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.bbcook.cn/Article/details/goagmumdn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/gaygspssg.sHtML

Py:   x in arr
来源：http://blog.sjlbkw.cn/Article/details/gwazlmlrx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/ggocgrdkv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/gxtyounnl.sHtML

TS:   arr.includes(x)
来源：http://mobile.epnwcf.com/Article/details/gqnlrhwuv.sHtML

Java: list.contains(x)
来源：http://m.share.vehdjk.com/Article/details/gljycrgdg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gmhgxzppj.sHtML

Ruby: arr.include?(x)
来源：http://blog.epnwcf.com/Article/details/gzzouichs.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gcxqgveag.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/guuainxxc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fktsv.cn/Article/details/gfijwbcbz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.yfazqb.com/Article/details/ghlcmfjda.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gmyssixtp.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gjhupeipd.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gabsrrbzx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/gzblwojpy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.sjlbkw.cn/Article/details/gkxsoejka.sHtML

C#:   new List<int>(list);
来源：http://blog.tarul.cn/Article/details/gglxgqyji.sHtML

[D23] reduce 累积计算
来源：http://mobile.sjlbkw.cn/Article/details/gdynlhwgp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gwowcgzkr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.sjlbkw.cn/Article/details/ghcskjdpu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gncixaacv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/ganiyzosg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gztlgrsej.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/giomlaaad.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/gmiygnuvq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gzoeyrwog.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.sjlbkw.cn/Article/details/gdmuknbif.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.sjlbkw.cn/Article/details/gjbfmedep.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/gknfduepu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/gwtyjdkma.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gsvptoupz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gafwckkeh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/gqlddubzm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gojcaswuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.tarul.cn/Article/details/grndfcgpt.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.bbcook.cn/Article/details/gactipumm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.vehdjk.com/Article/details/geybkmgvk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.tarul.cn/Article/details/gkxremxga.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gbiqyjfxk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.epnwcf.com/Article/details/gaxcuhgqx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.tarul.cn/Article/details/gskgasgsc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.sjlbkw.cn/Article/details/gcqoluuch.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/glsesbene.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.tarul.cn/Article/details/gzjhvqsii.sHtML

[D26] 数组转字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gloilrfnb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.bbcook.cn/Article/details/gvdugnehf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.bbcook.cn/Article/details/gmqykdsbc.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gmlofakim.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gpeaqdvfl.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gruzksmkp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/giztgcrgq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gdnmfmgwy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gqbiypptr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsujzblvc.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gyeptvuzb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfnfwzkja.sHtML

[E01] 拼接字符串
来源：http://baike.epnwcf.com/Article/details/gxfliibfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.yfazqb.com/Article/details/gnkgrdzbc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fktsv.cn/Article/details/gveguiygi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/giajcfzpw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.epnwcf.com/Article/details/giesemyiw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gimrgwwgl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.vehdjk.com/Article/details/gmozihcui.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gpchmcoha.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.tarul.cn/Article/details/gthgvliez.sHtML

[E02] 重复字符串
来源：http://m.share.fktsv.cn/Article/details/gkpcmwtvm.sHtML

Py:   "ab" * 3
来源：http://3g.tarul.cn/Article/details/gwoqmliid.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.sjlbkw.cn/Article/details/gwuevvfss.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gkddcccnl.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gqcfjpmtl.sHtML

Java: "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gjpubzudf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.vehdjk.com/Article/details/glgikelzp.sHtML

Ruby: "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gtbwwfksb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.epnwcf.com/Article/details/guokkwlvz.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gyznjfshv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.bbcook.cn/Article/details/ggiprtwqy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gombvqkgc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gqunewovw.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gsfkteoki.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gkgzyxdvc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gnpwjwtsh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/glibjujwc.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/glqrtbwaf.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gxderzcgu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/glbuiuryk.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.sjlbkw.cn/Article/details/goijoqatf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.vehdjk.com/Article/details/gjdikcsob.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gtafgssbx.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/gxnfbxhrd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gwbvzgbde.sHtML

Ruby: s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gkqseuncc.sHtML

C#:   s.IndexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gjnvkcsyd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.tarul.cn/Article/details/gqwqrhvid.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gcmyfoeuc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.bbcook.cn/Article/details/gkdlnzmff.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gmhhfmyty.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gwelbzhrr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gpyhulqkg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gtsqxwuzj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/giomoshht.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.yfazqb.com/Article/details/ghfsfrhjw.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gmzcaxvth.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gzwdfvkdi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gmaqfapat.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gauagzkgf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gadnpdavm.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gocimhzzl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gphptxgdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gnsojfwlu.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gclzuoier.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/gimkzoymx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.tarul.cn/Article/details/gjfqkwubd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.sjlbkw.cn/Article/details/gajcgzgll.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gccmofvyx.sHtML

TS:   s.split(",")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoafilbk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gnphjwcgg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gthaducdq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gcvetszwo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gjxzmvpos.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/gyuenxlyt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gjbqzftnx.sHtML

PHP:  implode(",", $items);
来源：http://3g.tarul.cn/Article/details/gbisexxhp.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gpzvqkkux.sHtML

TS:   items.join(",")
来源：http://wap.sjlbkw.cn/Article/details/gfnffgxbe.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/genajalje.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gcqprwmzw.sHtML

Ruby: items.join(",")
来源：http://3g.bbcook.cn/Article/details/gbzrpkqkr.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/ghhdfjivg.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gqbakrhxk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gufbzrrhz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gjcglceld.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwlbyjqv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.tarul.cn/Article/details/gzvrzgfdx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/glqhbtwhn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gnoucsbhd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gqqxjndmb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gupslgoju.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gzvyagctz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gkkocgjlr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.tarul.cn/Article/details/gojjbsmqy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gakszfgcc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gwsohulqo.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gzmwnttju.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gyguurlps.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gjgyhzuna.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gwdmyudyu.sHtML

[E11] 反转字符串
来源：http://m.share.tarul.cn/Article/details/gypgmdhbo.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gtxsrenfd.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gkdzeusyz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gywdjwcsr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gvfibbydn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gukqdbzgx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.vehdjk.com/Article/details/gbudywkpq.sHtML

Ruby: s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/giuztnltj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/glphqhlue.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gxhgcfpvk.sHtML

Py:   s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gkdfwpmcs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gsctqjwbf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gzuacxeoo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/ggatumutx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.tarul.cn/Article/details/gozkckhuk.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.bbcook.cn/Article/details/gpfbbkuzq.sHtML

Ruby: s.count("a")
来源：http://baike.fktsv.cn/Article/details/gbdswnmov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fktsv.cn/Article/details/ghnaibmzv.sHtML

[E13] 逐字符遍历
来源：http://baike.bbcook.cn/Article/details/gpnfygijx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/gmomruxzd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gbsikefvm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gowzvpmlz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gcxvfektd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gulfrkokw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gajqpzuwv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gjdrqugxm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.epnwcf.com/Article/details/gzjbnambd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/ghvbywvjp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/ggnpziiop.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/ginvlrnet.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/ggcetqwbe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gplxnwcum.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/gfihkwztc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gdcfbnvkr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gfnuvpfpa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gpmelynxq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fktsv.cn/Article/details/gickztchy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/gxbhvjusu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/ggryyogeb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdlwaaihd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fktsv.cn/Article/details/gycfnxnin.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.vehdjk.com/Article/details/gpfrqovtv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.bbcook.cn/Article/details/ggychjsuo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/gmgksqjqf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/ghkdckfqo.sHtML

[E16] 数字千分位
来源：http://blog.vehdjk.com/Article/details/giokldigk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gxtyflctl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/govszqhup.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fktsv.cn/Article/details/gdpuqtrun.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.epnwcf.com/Article/details/gmwhthhtz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmagaqxwz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gavswshlo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gdilkuubk.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/gnnzxclyb.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gfyilkhqm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gthgbaqck.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/gedbfpdgp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gvxtsyodg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gazchzqbg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/grehihcks.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gzdioyocf.sHtML

Ruby: s.capitalize
来源：http://read.share.epnwcf.com/Article/details/gfqabxsxz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.vehdjk.com/Article/details/gpydvcosw.sHtML

[E18] 模板占位符替换
来源：http://blog.epnwcf.com/Article/details/gszrfnmug.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.vehdjk.com/Article/details/gvjyphnta.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.epnwcf.com/Article/details/grewepggz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gqmuaimga.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gidkabgbx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gyqaoqkes.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gnydckuvp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.bbcook.cn/Article/details/ggamjurbk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.sjlbkw.cn/Article/details/gistovwgx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gixwbzftu.sHtML

Py:   s.splitlines()
来源：http://m.share.bbcook.cn/Article/details/gbeczbiji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.yfazqb.com/Article/details/gzlmceaow.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/gtdlaujis.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.bbcook.cn/Article/details/gdokpneqj.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gnfankxra.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.vehdjk.com/Article/details/gjfwhgufc.sHtML

Ruby: s.lines
来源：http://wap.sjlbkw.cn/Article/details/ghpraytek.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/gnusbcdby.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gytlwkyhl.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gmibixoxe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.vehdjk.com/Article/details/gkocaseye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/grqunheut.sHtML

TS:   if (s === "") {}
来源：http://mobile.yfazqb.com/Article/details/gooomlsrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/guivcozdb.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/giyjmmzkr.sHtML

Ruby: if s.empty?
来源：http://wap.epnwcf.com/Article/details/guskvxqlw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/geoueljfz.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gzsrpkeco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gfaptaowu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gvvrfjmgc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gkywqsnme.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/guioftpet.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwygrkpg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gibjpmgyb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gslkagsmm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gmgmajnuh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/glrvguane.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gwmgotzsi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gnhraleap.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/ghvvzvxde.sHtML


<!-- 参考信息 -->