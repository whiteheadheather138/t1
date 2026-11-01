代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gbyzdqfni.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.epnwcf.com/Article/details/grcxwjmpa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gpzxngskc.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/gvdpnxsjz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.tarul.cn/Article/details/gcgefbrxp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gphmnssnk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.bbcook.cn/Article/details/gklgxoxdw.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/gcgwthowu.sHtML

[D23] reduce 累积计算
来源：http://blog.tarul.cn/Article/details/grrdiewjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/guzxdgmty.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlpsxfex.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fktsv.cn/Article/details/gqxketxsr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gbdawzycb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.tarul.cn/Article/details/gtqwgjbkl.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gkmusnxhq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/goinauehp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.bbcook.cn/Article/details/gyrrdrixr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gsoeisreo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gnhjlgeln.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.epnwcf.com/Article/details/gvckcxcav.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.sjlbkw.cn/Article/details/gugkhaqla.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.tarul.cn/Article/details/ggrfopuqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gtmwmfyaz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gpmxfhdno.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gubpfqhig.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fktsv.cn/Article/details/gidpuxqiv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.sjlbkw.cn/Article/details/guwxjlwxo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/ggkktlrgj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fktsv.cn/Article/details/gdcucaspl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/glwvosggu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gixrhgsnk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gctmjwtnu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.sjlbkw.cn/Article/details/gmigbdzfm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/giyjfxmqf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gqypydmhg.sHtML

[D26] 数组转字符串
来源：http://wap.vehdjk.com/Article/details/gvqfpqhyq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gwhgfdeyu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.bbcook.cn/Article/details/gxiltwgln.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gguyzujpf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gmsutbypq.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/giupbeczn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.yfazqb.com/Article/details/gmzfvlbee.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gggxgbcvb.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gyewxnosu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggtakthfq.sHtML

E. 字符串处理
来源：http://read.share.yfazqb.com/Article/details/goqrmpqbd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyrxbgyur.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gimzwhgkk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.epnwcf.com/Article/details/gjcmupsag.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gdrawdkxf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gqblgrtde.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gslfgqbkj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/ggjtgelvd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gxgwceujs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fktsv.cn/Article/details/gmzrchcnc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/gymjcwydb.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gbhcclczu.sHtML

Py:   "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/godzvswvd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/ggfdoouhd.sHtML

JS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gueuirjdn.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gfsprvgqo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gwrbojgkb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fktsv.cn/Article/details/gfkvjlxia.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gxiiiiznb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/gzemkadur.sHtML

[E03] 截取子串
来源：http://3g.tarul.cn/Article/details/ganewahxn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gmsrijiol.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gaakvjnqc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gxdteairy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.bbcook.cn/Article/details/gaxrxhjcz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gvekwpyxw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gkemnsbxz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.tarul.cn/Article/details/gtxycarpx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fktsv.cn/Article/details/gmbhxrskr.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gllpdpwmz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.epnwcf.com/Article/details/gfdtcehri.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.epnwcf.com/Article/details/glmzsofdt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gsbqtqnml.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/ghysedspv.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gyrljjvfl.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.epnwcf.com/Article/details/gatggfula.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/grgnrfhlw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gxyqbbrym.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/ggyyczvsr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.bbcook.cn/Article/details/glyjhgpro.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gxtdgkncm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gomuyhwip.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.bbcook.cn/Article/details/gzcdssmdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gecycahsk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gdabvmcdg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fktsv.cn/Article/details/gfisgnxdh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gnibhrqdr.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/guhhsywhc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/gippnvprc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/ggqjqchjy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gfxtnxtqp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gkohppurp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gqsniocni.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gamqjnnyt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gkdhnaflb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/guxhrmsaa.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/gegrxnumx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.epnwcf.com/Article/details/gecdshsin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.vehdjk.com/Article/details/ghcgorkmi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.bbcook.cn/Article/details/grkmfaksh.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gjwclblxr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.tarul.cn/Article/details/gcpxdmszi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/grairlgor.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gsxjehvzb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/ghwhfqfxv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.bbcook.cn/Article/details/gfdaklbxy.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gbmilysuu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.tarul.cn/Article/details/gmhqodleg.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gubyyajsk.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/glosahwty.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gdfuuerar.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gjvawtpoc.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gbxzuvvbc.sHtML

C#:   string.Join(",", items)
来源：http://blog.tarul.cn/Article/details/gcvvrzeup.sHtML

[E09] 去除所有空白字符
来源：http://baike.yfazqb.com/Article/details/godcioctq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.vehdjk.com/Article/details/gzxqvrrxz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gdcesztkw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gjfnxohpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fktsv.cn/Article/details/georxkhri.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gyobfaaey.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.yfazqb.com/Article/details/ghmbbgjho.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gpnnsivvb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gbitmbkhm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.tarul.cn/Article/details/gkobarzxq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gwzpjyhco.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gqamxdofw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/ggpqpoeeq.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gychsoyex.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gfziocxhe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gkhpxucqr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gleomsslr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gligijwcj.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/gdjlcdejm.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gzwxqdymg.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/gnjjyvcjv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghbhoncrt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gedhnwqam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gpankwqnl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fktsv.cn/Article/details/ggjgoxqse.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/ggwkecueh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/ghglbdmcs.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghedcctbp.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/grbtmdocj.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.bbcook.cn/Article/details/gjkesrdwi.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/ghvcgolty.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/guglnnvtj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/giqsajlab.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/gbulxnhio.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gxccrnbay.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.sjlbkw.cn/Article/details/gohccfbmh.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/grmjxwniv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/giwafaomy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gcnntjkmu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glkwawkce.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.bbcook.cn/Article/details/gyzjpatlr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.bbcook.cn/Article/details/gmfpnjbvc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.sjlbkw.cn/Article/details/gsexmrcdi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.tarul.cn/Article/details/geadfedof.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.yfazqb.com/Article/details/gjfebnbxr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.tarul.cn/Article/details/gbdlfpapy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.vehdjk.com/Article/details/gknohvvbz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.tarul.cn/Article/details/gfbhcwxrv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.bbcook.cn/Article/details/grhkwlgxs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.sjlbkw.cn/Article/details/gjsdtrqvn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gmbigvogv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gsipktnhr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.bbcook.cn/Article/details/guyqxmnjy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gpuehimry.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.yfazqb.com/Article/details/gtrzstzrs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gghqlhohz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/gdklufpgg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gethpbstp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/glrzlinya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gdiiphiuo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/goulyvkch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.tarul.cn/Article/details/gvnpisxbt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gciiybsxe.sHtML

[E16] 数字千分位
来源：http://mobile.bbcook.cn/Article/details/goinuebok.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gofjttaos.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gtfbasuxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gldnkqvrk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gbpzraozc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gtoodrqgk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/gegwazvrv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/goxubdnko.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.epnwcf.com/Article/details/gkbdkbiqd.sHtML

[E17] 首字母大写
来源：http://www.share.yfazqb.com/Article/details/gghxcnfua.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.tarul.cn/Article/details/gfmqhzlcg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.vehdjk.com/Article/details/gxlvbkxfh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gjwuxdelt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gcypxzylt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gjrjlcxcc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.vehdjk.com/Article/details/gnyzasior.sHtML

Ruby: s.capitalize
来源：http://www.blog.fktsv.cn/Article/details/gjsyhrxzp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmhgigwx.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/gaxnezwcy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.sjlbkw.cn/Article/details/gxnnaoaqz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.epnwcf.com/Article/details/gzjhfuors.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gydggyyck.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gcercxqvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gpvsxdshc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gaikdpiqg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.tarul.cn/Article/details/gwpxkiodx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/ggrjnejfp.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gtruemhhb.sHtML

Py:   s.splitlines()
来源：http://blog.sjlbkw.cn/Article/details/gnnhixjee.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/glhxchtdk.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gcwpucnqd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gujlccohm.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gzlzsqwvm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.bbcook.cn/Article/details/gbwlaukxi.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gpjrpsidh.sHtML

C#:   s.Split('\n')
来源：http://read.share.sjlbkw.cn/Article/details/gjxeeoplk.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.vehdjk.com/Article/details/gyevbxeuc.sHtML

Py:   if not s:
来源：http://blog.bbcook.cn/Article/details/gnjzjoizq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gyijupmcn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.bbcook.cn/Article/details/gytmbabcc.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gttgsnrwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.bbcook.cn/Article/details/gtkcssobk.sHtML

Go:   if s == "" {}
来源：http://m.share.yfazqb.com/Article/details/gelvfozzw.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gorqaikac.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/gqtjqhwfy.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/grywbuson.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gwxzjeaus.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gcnzqwncf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gdeousaqq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gtwcgtmoj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gstuxcwko.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gznsphnpv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/ghkdxxfwt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/grxxvwzyv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.vehdjk.com/Article/details/glydajkhl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/guvvhapxt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gwkearoyz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gmhvmfdwh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/glxurmcry.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.vehdjk.com/Article/details/gnfikdrts.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gffogfkdw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gzwxnaxyw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gaosngzbv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gnilvqwyf.sHtML

F. 文件与目录
来源：http://www.share.fktsv.cn/Article/details/gxqztidpp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkmhvgekf.sHtML

[F01] 读取整个文件
来源：http://read.share.fktsv.cn/Article/details/gydkpvcsv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.bbcook.cn/Article/details/gnvyihtqa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ghisjvcbz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gletwhsjx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gecprernf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gshvsjkvo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/gjihybebo.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gnfugqfod.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.bbcook.cn/Article/details/gqcintduz.sHtML

[F02] 逐行读取文件
来源：http://m.share.yfazqb.com/Article/details/gcnjtnaeh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.vehdjk.com/Article/details/gpjfsmmsb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gaqettnqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gjyxrfhgp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/gngcncqrz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/grfteybsl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fktsv.cn/Article/details/gdtrkrywz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/guwrzkoin.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gadgtqzzw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gfodmpsbi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gskhdnacx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gatsnckmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/ghhtojpzf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gyqgcbfdh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gryshxbjn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fktsv.cn/Article/details/gfpumpfoz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gqwrdhgug.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/gbchqrclj.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gscxcmnpv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.tarul.cn/Article/details/gyvsfyavf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fktsv.cn/Article/details/gkjwwrjey.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gkrmmrkds.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/ghstjukno.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.epnwcf.com/Article/details/giuxzofok.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.bbcook.cn/Article/details/gxbcpussi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fktsv.cn/Article/details/geclneuof.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.epnwcf.com/Article/details/ghzhkbfyz.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.epnwcf.com/Article/details/grxdhwtfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.tarul.cn/Article/details/gxzcyunia.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gpxxockyd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/glcoebrny.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gjrqzhews.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/glpviknaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gzueybbvv.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fktsv.cn/Article/details/gljznnrzz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fktsv.cn/Article/details/gupkkyvmq.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gisudvhfo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gjblwmbcz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gxmgtzgtc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/gypruqbfi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gejotqlxl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gvzotfbga.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.tarul.cn/Article/details/gteibgivi.sHtML


<!-- 参考信息 -->