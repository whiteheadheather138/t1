代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.sjlbkw.cn/Article/details/glslifmgz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gpdcmkncn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.bbcook.cn/Article/details/gqbuchlli.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/gmiwvswxd.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gpgfbdeye.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.tarul.cn/Article/details/ggcnseajy.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.sjlbkw.cn/Article/details/gddeemxpc.sHtML

Py:   x in arr
来源：http://m.share.epnwcf.com/Article/details/gfgrdnmok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gwsskdgsd.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/gwyqliniw.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/gaojttkqg.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gzrtngtbt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gkdtoasft.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gdhagahpo.sHtML

C#:   list.Contains(x)
来源：http://wap.fktsv.cn/Article/details/geaharvtk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.yfazqb.com/Article/details/gvtfxfbqo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/graabzcaq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.tarul.cn/Article/details/gelganbme.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/gsczwdnej.sHtML

TS:   [...arr];
来源：http://blog.fktsv.cn/Article/details/gkeybmnzf.sHtML

Java: new ArrayList<>(list);
来源：http://blog.tarul.cn/Article/details/gotsdhcvw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gwwkojlbb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.yfazqb.com/Article/details/geluryeul.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gaecacvsi.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/gbvbeclee.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gbvwxexaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gnhanszsd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gzkmbsmyj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/guurjkmhx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.sjlbkw.cn/Article/details/gdavgcvyw.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gjkboqsfu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gxqzitvez.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtbakjby.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gtqrlgvhn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.bbcook.cn/Article/details/gceufstun.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gnnmwkgod.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gqcdaxzwk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gdqrkaoen.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gthvsnbfx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gfwfulwbg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gsxpgcrbd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.sjlbkw.cn/Article/details/gwuydndoe.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.epnwcf.com/Article/details/gsmaqebkk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/ghtghbira.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gfydmwbgo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.sjlbkw.cn/Article/details/gsqhmfjpb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.vehdjk.com/Article/details/gozgwnowi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gqqfbhlqc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.sjlbkw.cn/Article/details/ghvyeorve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gutqwbkgd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.bbcook.cn/Article/details/gqcigblrp.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gmzdobsgm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fktsv.cn/Article/details/gvcrityuy.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.sjlbkw.cn/Article/details/gckoruhkq.sHtML

JS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gtyvkaxou.sHtML

TS:   arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gamhszycz.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gbnydqnks.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gkbvppdmh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gixhihrds.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gicumvhaq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grtvdlivg.sHtML

E. 字符串处理
来源：http://read.share.vehdjk.com/Article/details/gciertfpm.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/geghhmuhd.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gtupkdnpr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.tarul.cn/Article/details/geuxfhvhp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.yfazqb.com/Article/details/gzuufedlt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gsivnnfyc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/greojllnt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gavqdlfcd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gmjahruzs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gkzynnqeh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.epnwcf.com/Article/details/gxemznbpx.sHtML

[E02] 重复字符串
来源：http://baike.epnwcf.com/Article/details/gcmogspnp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gnznkczti.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gpnwigcao.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gyvhkifrl.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/ghpckkiwh.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.vehdjk.com/Article/details/ghysfytkl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/gkiubaeoj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gergifoug.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.yfazqb.com/Article/details/gdmvknkqk.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gweurejvj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/gddkslaky.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/goprijcia.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/gvcjndmaf.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gaptpsuoj.sHtML

Java: s.substring(1, 4)
来源：http://read.share.yfazqb.com/Article/details/grxqptouw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/gizhguccr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gikmdpuog.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.vehdjk.com/Article/details/gqimykkzx.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gonlhdzfv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gvkvshihl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gospaucae.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gngzlwvdq.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gubaanokd.sHtML

Java: s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gkqhzuyqk.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.epnwcf.com/Article/details/geqiqbzhm.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gzhuzyhmr.sHtML

C#:   s.IndexOf("x")
来源：http://3g.epnwcf.com/Article/details/gyclkzcsd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.bbcook.cn/Article/details/gsncvxhap.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.yfazqb.com/Article/details/giuosqekz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.vehdjk.com/Article/details/gnfwfdibh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ghiunlckb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gftyfzspe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gyxtfmrra.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gqweatlra.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.yfazqb.com/Article/details/gptounqfo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/guadgroef.sHtML

[E06] 替换子串
来源：http://wap.vehdjk.com/Article/details/guukbdqty.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gdoyeyqmn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.tarul.cn/Article/details/gxqmpwaxz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gofutmgbh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gdlwwrbvg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gfwvfkbtu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.epnwcf.com/Article/details/gxtbfnhgi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.yfazqb.com/Article/details/gexkfqovi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/gmkwvbkfl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.epnwcf.com/Article/details/gilbfbvnn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gmqsuwudx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gygupvrmq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/ghjqxfsxp.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/gpbodnwyh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gcxbiuftf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gzzahqesr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/gxlytjiqy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.sjlbkw.cn/Article/details/gsjipnxbo.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.epnwcf.com/Article/details/grryyokqx.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/glwxiqomi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/ggprawjan.sHtML

JS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gkwhmqfpv.sHtML

TS:   items.join(",")
来源：http://blog.fktsv.cn/Article/details/gqsjmnafn.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gvpwuwvwv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gvirlouin.sHtML

Ruby: items.join(",")
来源：http://baike.bbcook.cn/Article/details/gdeasacmg.sHtML

C#:   string.Join(",", items)
来源：http://m.share.tarul.cn/Article/details/gplrfzzna.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gxraoyasm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/gymzoageo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/gpnuojvtx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gakzisiac.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gmcjiphhf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gcwnxnfww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gdaoebdnn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gxzjygsqd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gbxikkeqp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/geusioclu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gnihknuhb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gvfdqxakh.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/giqcpzdpl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gkqvglhib.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gntrsnaqg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gadigbltk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gtgfnxjbi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/goemdbezo.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gmmplhqfs.sHtML

Py:   s[::-1]
来源：http://mobile.tarul.cn/Article/details/glgzdxkll.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gahngrclj.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gylmzcyyt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ghygntbmd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.tarul.cn/Article/details/gftbwtauh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gnkdjuilt.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gafsakwos.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gtsmfwcre.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gqsbfxqhi.sHtML

Py:   s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gcunthatw.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gupmrhhto.sHtML

JS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gdnxpbcwf.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/gvdsbtmau.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.bbcook.cn/Article/details/ggqvuzbuh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.sjlbkw.cn/Article/details/gnnosracd.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/guelvftqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gukmmtvim.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/goonhgosz.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.tarul.cn/Article/details/ghxodtcgm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gfxnsjnit.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/ghyhcisyw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.tarul.cn/Article/details/gncsrpyao.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gebtxpjnl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.vehdjk.com/Article/details/gwxuswwfx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.epnwcf.com/Article/details/guyhrcsqn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gyfbboxui.sHtML

[E14] URL 编码与 Base64
来源：http://baike.vehdjk.com/Article/details/gejkgdmko.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gxpfgdlcx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/ggowtekke.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gvjhebrbg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gbvyhtzeu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gfdojmauq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gncvygdsw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.epnwcf.com/Article/details/ghkmhewub.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.bbcook.cn/Article/details/gxjfxbtbi.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/giatwhkys.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gnhzyrdew.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.vehdjk.com/Article/details/gkgdlufbi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.tarul.cn/Article/details/gjptnajnp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gebbhuasd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.sjlbkw.cn/Article/details/ghjdfkiex.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.yfazqb.com/Article/details/gqudjnwvi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/guzsglujt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.epnwcf.com/Article/details/gbalsoytg.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/goyxngatc.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.epnwcf.com/Article/details/gqxicywvk.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.yfazqb.com/Article/details/grwgzqbzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gymnysvsl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gpusqhkfk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmafkczss.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.bbcook.cn/Article/details/gbhterfen.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/gmsyqrrgy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gspfophfx.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gvwgwszel.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gqoggkzlq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.bbcook.cn/Article/details/gacfzhkdl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gdtjwlhbi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/gqsxaomsb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gahbcvytj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gvtlyojxl.sHtML

Ruby: s.capitalize
来源：http://wap.tarul.cn/Article/details/gsfuuhsaz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gwunxhpbn.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gdkgxnrxi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.bbcook.cn/Article/details/gpzfduiwi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/gueqnkert.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gxmnbshgl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/garibghdz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gsfxdudrj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gdtwjsebb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gmpngmxyz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/glqymnveb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gacnjvldw.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/gezdthyzt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.tarul.cn/Article/details/gkedfmuey.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gxysmzaeu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gsvphcopf.sHtML

Java: s.lines().toList()
来源：http://3g.bbcook.cn/Article/details/ggrbtxfku.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gwdqbqbrk.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gtxykkdjj.sHtML

C#:   s.Split('\n')
来源：http://3g.epnwcf.com/Article/details/gvvrpcrft.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.vehdjk.com/Article/details/gjfwrxcxv.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gdoezvorp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gpolwfdnc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gabdkbmjf.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/grpwhpteu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gqrmbgmjr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gvdnfurwl.sHtML

Ruby: if s.empty?
来源：http://m.share.bbcook.cn/Article/details/ghutmbbrd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.tarul.cn/Article/details/ganqphcvi.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gjryijsnu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/gmjgpadrl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gabyzmlkq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gqbfjzhah.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gmguakwqq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gtrdmzkuy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gdizabmwd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fktsv.cn/Article/details/gyprihumo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gadaellos.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gmzlaoueh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/ghmziovsi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gdflvdgff.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gihhxcrov.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gjsaxavmr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.bbcook.cn/Article/details/gqlporcdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gqrdkhjzx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.vehdjk.com/Article/details/gylqfpwmz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.bbcook.cn/Article/details/gbribpixg.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxwciwjtc.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/gfcdtyyzc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gevniwrpk.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gdxpltlfm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gzziddxoh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/ggtlurlbp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.yfazqb.com/Article/details/gvnnaxpth.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/griihwidy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gjhisruxm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gvzvqjrmh.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gvextvyyy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/glefmpubk.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gvdtnzvyw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.yfazqb.com/Article/details/gyigapiyt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gjnejovcy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/glmlpqean.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.epnwcf.com/Article/details/gmudedkqk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.yfazqb.com/Article/details/gpmbzkhgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/gquqttjsc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gduvfdasp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.tarul.cn/Article/details/gluhxbsht.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/gqgqmedrz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/ggfdjuxsm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.vehdjk.com/Article/details/gwpinfmlw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gmnujtubs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.vehdjk.com/Article/details/gqgetfdxg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fktsv.cn/Article/details/gfmkqikbf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/gmdouyuyi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gqkhplzxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/gfvvtzanl.sHtML

[F04] 追加写入文件
来源：http://m.share.yfazqb.com/Article/details/gbzfetpjh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fktsv.cn/Article/details/gnxljmerj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/gvsombidz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gcsiyntjw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/gnosrneav.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gwdjhghmf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gbdhilkkj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/giwjxczbm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.bbcook.cn/Article/details/ggbibuwvl.sHtML


<!-- 参考信息 -->