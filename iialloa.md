代发 wailian999

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gbfhpqfut.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.vehdjk.com/Article/details/glmasavbx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.tarul.cn/Article/details/grxeyjypq.sHtML

Py:   x in arr
来源：http://wap.fktsv.cn/Article/details/gqdzmukya.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.sjlbkw.cn/Article/details/geisscilo.sHtML

JS:   arr.includes(x)
来源：http://www.share.sjlbkw.cn/Article/details/govldjbjz.sHtML

TS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/guabdtvyo.sHtML

Java: list.contains(x)
来源：http://www.share.bbcook.cn/Article/details/gtftgyxpl.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.bbcook.cn/Article/details/gsxgcshuk.sHtML

Ruby: arr.include?(x)
来源：http://read.share.tarul.cn/Article/details/gnglnwroy.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.tarul.cn/Article/details/ginkkwehe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gclnrlity.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.vehdjk.com/Article/details/gcimavepm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/ghikgfabv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/ggndftcbf.sHtML

TS:   [...arr];
来源：http://m.share.tarul.cn/Article/details/gsdtbjeds.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/glvyxxyyd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gurlepnbj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/goagakalw.sHtML

C#:   new List<int>(list);
来源：http://wap.fktsv.cn/Article/details/gqtlvyaeh.sHtML

[D23] reduce 累积计算
来源：http://www.blog.sjlbkw.cn/Article/details/genmjoryg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.yfazqb.com/Article/details/gpzokebjk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.tarul.cn/Article/details/gdzgsjvql.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gqjcbqubd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/ghfhbgsdg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.bbcook.cn/Article/details/gwsqxmgwc.sHtML

Go:   // 手写循环
来源：http://m.share.sjlbkw.cn/Article/details/gxubhmlyr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gflxrxvyn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.tarul.cn/Article/details/gmdtkaofd.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/grakgflkv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.bbcook.cn/Article/details/gkzmgoheh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.tarul.cn/Article/details/ghukwslfs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gwnmxtgdg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.tarul.cn/Article/details/gildskbws.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.sjlbkw.cn/Article/details/gdbipbtzo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhkbjrbz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gqmoefczd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/geasbngae.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gutefdwxh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gkyteuhbe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.tarul.cn/Article/details/gcsdroidl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gvhydykml.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.tarul.cn/Article/details/gjakycepo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gjuvnwvwx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/gyxgfvxgl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/gumguqurf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.vehdjk.com/Article/details/ggqpqysfe.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gpqskiizj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gxckdkwsc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gwceajsgr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gjxsigudo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gtostzqki.sHtML

Java: String.join(", ", list)
来源：http://blog.fktsv.cn/Article/details/guxsxlldx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gdtjktxcm.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gsazsohwc.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/golyhuflw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghitxoath.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/ggygcvimu.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxdoeanya.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gcahdmzvu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.yfazqb.com/Article/details/gnhuncxha.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gamnxqmly.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/glllmvhbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/givqypfvr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gqxcaqboz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gmdljvhrc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/ggxnpeobm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.bbcook.cn/Article/details/gwwaozpss.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/gdolglfqv.sHtML

Py:   "ab" * 3
来源：http://mobile.bbcook.cn/Article/details/gdsdbvyiu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gxdkyhnem.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gzfnlxmqe.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/giujlemcc.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gqwrwqhfc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.tarul.cn/Article/details/goikxlpaa.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gpemfhpzm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gfnqryfxw.sHtML

[E03] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/geejvodre.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.vehdjk.com/Article/details/gpsexllql.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gewhbjzgn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gnamypkkp.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/gtlaiagrj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gwtnokxyd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gvfehnaif.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.epnwcf.com/Article/details/gksdwpcfo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/gdpyrhygf.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gehqwkock.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gflfqsuze.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/govwifbef.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.bbcook.cn/Article/details/gigdjtjhk.sHtML

TS:   s.indexOf("x")
来源：http://read.share.epnwcf.com/Article/details/gxjeckxzh.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gbiibfxlu.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/guabyslmj.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gjcebcrdh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.epnwcf.com/Article/details/gtsxatnax.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gbqowlduf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.tarul.cn/Article/details/gnqbajxyu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/gckfdicxl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gwmtvucpy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/gglmjqdvr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gkbenjgmi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.sjlbkw.cn/Article/details/gnkqtwxoi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.epnwcf.com/Article/details/ggywbdtij.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/grcdizpas.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gurfegogv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gslkwdvxy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gkphsrskt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gooyqrtqz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gqfsfmngi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gtosldtyd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gznfrxefy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fktsv.cn/Article/details/gleerwreu.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/glzegxcmz.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/ghfqolott.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.tarul.cn/Article/details/ggrcfbaaz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gtkuwqybz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gvugsahvh.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/grejuhmcd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/goisfxcem.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gicxjauji.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/gkhblixew.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/gnrzljsfb.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gslymqkow.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/ghrktwbfn.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gtxgrupjp.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gnpswqrkg.sHtML

TS:   items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gvivyicra.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gcwdobdyc.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.epnwcf.com/Article/details/gcqoyrlph.sHtML

Ruby: items.join(",")
来源：http://www.share.yfazqb.com/Article/details/gibzdlwzy.sHtML

C#:   string.Join(",", items)
来源：http://blog.sjlbkw.cn/Article/details/gbsmsdolc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gupgeupis.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gzjawupiu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gzpfysqhv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsqzqnur.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gdjcontlj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/ggwlausoa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.yfazqb.com/Article/details/gvovznzwz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gskeedeuj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.epnwcf.com/Article/details/gmdjsbzpl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/gummknxoe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gqbvjrsak.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fktsv.cn/Article/details/gjdewunka.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gigikwskl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/glymbytcg.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gjbpgwjvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gdtmrxpgm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gynctcjxk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gwbkqgskv.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gsekksuxy.sHtML

Py:   s[::-1]
来源：http://baike.tarul.cn/Article/details/gdsltuhfu.sHtML

PHP:  strrev($s);
来源：http://wap.vehdjk.com/Article/details/gyvksfghe.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gwcgysszl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gtrtpwrqu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gslsyvxuo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gqkdxwfha.sHtML

Ruby: s.reverse
来源：http://blog.vehdjk.com/Article/details/geuikajlj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gvldgklqm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/guvjfvohc.sHtML

Py:   s.count("a")
来源：http://blog.tarul.cn/Article/details/gengdcdvl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gbxdorwis.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.bbcook.cn/Article/details/gbullomea.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gfbvbkfpn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fktsv.cn/Article/details/grxdjljok.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gjpeslinx.sHtML

Ruby: s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gabmhowqc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/ggfkeaspa.sHtML

[E13] 逐字符遍历
来源：http://baike.sjlbkw.cn/Article/details/gphkvejsh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.tarul.cn/Article/details/gsauzxxdn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gglmxqmql.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/guqyuxjld.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gsovzglie.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.yfazqb.com/Article/details/ghadcpcdw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gdzpqxziu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.tarul.cn/Article/details/gbubrfvfy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gnqjwgdbi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gvfmqtytl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/gygxuhyds.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gajqkafko.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fktsv.cn/Article/details/gszamzpgy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.bbcook.cn/Article/details/gidznjcbb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/ghkpjbwbx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/ggccaxtmj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.epnwcf.com/Article/details/glecrdnvl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gsjkcobpu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gaahftckb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/glcqscxgi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gaauyeeqs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/glnrtqhgg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gxsljniqd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.yfazqb.com/Article/details/gwpiarltm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/guihkrwrj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.epnwcf.com/Article/details/gmvezpplc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/guhditqgx.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gnkrmggms.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.yfazqb.com/Article/details/gqkuudbdb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.tarul.cn/Article/details/gkxahhdhn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gckuzllfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gcuhoryfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/gcvioigkp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/gvbkoltlq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.sjlbkw.cn/Article/details/glnyiezle.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.bbcook.cn/Article/details/gglvdbcnh.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gtavimpqp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gmmyyayhm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/gcgxfmqcx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gfrhncpxb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gxrconcfv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fktsv.cn/Article/details/gtebnezvh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gvgqblamj.sHtML

Ruby: s.capitalize
来源：http://www.blog.sjlbkw.cn/Article/details/ggxksiksw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/guspqmgud.sHtML

[E18] 模板占位符替换
来源：http://m.share.epnwcf.com/Article/details/gxkyedxdk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gpedgsyag.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/grhbngwwo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/glywjursa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/grivvwbqk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/geblntfqk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.tarul.cn/Article/details/gkdukphzf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/gxkoultpz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/gkpvhekrl.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/grtegygib.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gpbmwkbeh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gepdbfkoo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/gvdlfapjs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fktsv.cn/Article/details/ggcywjhla.sHtML

Java: s.lines().toList()
来源：http://www.share.vehdjk.com/Article/details/gaiealfwg.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.epnwcf.com/Article/details/gnghpmujg.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/gywufrzye.sHtML

C#:   s.Split('\n')
来源：http://blog.epnwcf.com/Article/details/gmboxgdmt.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gnkkfmrif.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/ghshetnlo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/glncjppdy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqhfeiviw.sHtML

TS:   if (s === "") {}
来源：http://www.blog.vehdjk.com/Article/details/gocywkrkp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gfeusgfhz.sHtML

Go:   if s == "" {}
来源：http://mobile.bbcook.cn/Article/details/gjyvonfaq.sHtML

Ruby: if s.empty?
来源：http://www.blog.vehdjk.com/Article/details/gxuvulzkb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gzyjuysjd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.vehdjk.com/Article/details/ghvvkcuyk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gqcjazyxw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/geqctlkwb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/gtgkuxarq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gxslqjhbz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gkrbnteis.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gtniuiqde.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gdvyjjokr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gvsqdwwfo.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gsmtfxskb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gzefltfdo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gfnnxacrj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.tarul.cn/Article/details/gzwhxzuqc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxeseficu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.bbcook.cn/Article/details/gnbujiqvp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/geyjupzjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gdqznqdxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/gnnlrfjmd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gowqaljzt.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gpttjnvpa.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnohvpdok.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/gvfgeqngm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gbssrtcav.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gybwlafxm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.vehdjk.com/Article/details/gvwrzrogq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.epnwcf.com/Article/details/ggomwwrqw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/grcwlbxdq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.vehdjk.com/Article/details/gbvgvgndv.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gyvcuuwof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.tarul.cn/Article/details/gqqljllbm.sHtML

[F02] 逐行读取文件
来源：http://3g.sjlbkw.cn/Article/details/gbqxtquem.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.yfazqb.com/Article/details/ghswrkkab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gunwvxsqt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.vehdjk.com/Article/details/gglovmlna.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.epnwcf.com/Article/details/gtyxpbczo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gbiwngzmu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gbwpugpay.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.sjlbkw.cn/Article/details/ghclmgouc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fktsv.cn/Article/details/gkyfjfzma.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gmqyvudby.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gzgcoyrgf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/grdoizsfz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gnnkpdspn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/girplpbuv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.vehdjk.com/Article/details/gdqyhwreh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fktsv.cn/Article/details/gncjlwxdt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.bbcook.cn/Article/details/ggcancvpl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gcbwxlbjy.sHtML

[F04] 追加写入文件
来源：http://www.blog.tarul.cn/Article/details/gefxpwxcl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gjtufldii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.tarul.cn/Article/details/gzribvdsa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gmntliegh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gjqqdtttz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gkitvgito.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fktsv.cn/Article/details/gwousjzmd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gkumnabst.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gvoicyvqv.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.bbcook.cn/Article/details/gpylqbxzr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.epnwcf.com/Article/details/gabfapkgg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gtsihsmtg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gknjqvlwg.sHtML


<!-- 参考信息 -->