代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gvgtxvyaj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.vehdjk.com/Article/details/gztezkiqy.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gviwxwtyc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gqheoppyy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.bbcook.cn/Article/details/gfdilditj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/ggyahsydl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/guveitibn.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/gewsduhvq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.bbcook.cn/Article/details/gsyiyustb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gfnityzto.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gvcgkucdl.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gaxeyvinc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gsycalytj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.epnwcf.com/Article/details/gzrsmsfpa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.bbcook.cn/Article/details/ghdpdyyqh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/goxdhddos.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.epnwcf.com/Article/details/gnhmogxkp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gtkhzykfr.sHtML

Go:   // 手写循环
来源：http://read.share.vehdjk.com/Article/details/gjnsywivd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gxfongpzf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fktsv.cn/Article/details/gvyxboaev.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/grxihjssm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/galvdaodk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.bbcook.cn/Article/details/gavcmhnce.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/guteqqjjr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gsqdgjkvo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.tarul.cn/Article/details/gayffsnlx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.vehdjk.com/Article/details/gnjrvingg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gtngmdxrp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.epnwcf.com/Article/details/gcfxivwya.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.epnwcf.com/Article/details/genelodoi.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fktsv.cn/Article/details/gwbxphyuh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fktsv.cn/Article/details/gnbegkkjw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.tarul.cn/Article/details/gpghrssnl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gwxkwgscg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gxuaylsiw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/glxkqbgau.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.tarul.cn/Article/details/gonvegajk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gqznnsrmq.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gxbdgmoaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/geapwtstp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.epnwcf.com/Article/details/gtessgwrf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gwpdmxkkz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/gzdvxigjy.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gxyiupbhu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.yfazqb.com/Article/details/gmejewkfu.sHtML

Ruby: arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/ghvrfkexd.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gtopwcych.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glntnajtb.sHtML

E. 字符串处理
来源：http://m.share.tarul.cn/Article/details/gvpqoiyzs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gykjpzijt.sHtML

[E01] 拼接字符串
来源：http://www.blog.vehdjk.com/Article/details/grzwmived.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.epnwcf.com/Article/details/glkuprkah.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.yfazqb.com/Article/details/gybfnuvln.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghbpphsza.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.epnwcf.com/Article/details/ggxwpgxrk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/girydudqm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fktsv.cn/Article/details/grdyjtwgs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gvtbopusv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gllbzqztq.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gehxdsjlq.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gpyhullog.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/gadxvcbrw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fktsv.cn/Article/details/gpbvztvfe.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/govhdwfhs.sHtML

Java: "ab".repeat(3)
来源：http://wap.fktsv.cn/Article/details/gwcyxyjrq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.yfazqb.com/Article/details/gdpstphdf.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/ggtjskzvy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gcrrgjpca.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/goyifzsqx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gskhcwmcv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gexhivnxk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.tarul.cn/Article/details/gcecwrfpu.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/giicsfknq.sHtML

Java: s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gzpmutyxs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/ghijqqlum.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.epnwcf.com/Article/details/gqdmuncyy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.vehdjk.com/Article/details/gkbjrslny.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gngqiqrpy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gbnumsfhx.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/grqwcxrmh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.yfazqb.com/Article/details/gaqyxpqcb.sHtML

TS:   s.indexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gtgoalmxs.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gajbicyxn.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.vehdjk.com/Article/details/guzyrgktt.sHtML

Ruby: s.index("x")
来源：http://3g.yfazqb.com/Article/details/gxbmfglum.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gbbfucpzj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gwackzlah.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/ghegqbdgv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/gyxvyxzfq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/goresircg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/grgucewdd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gqcpfgvld.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.bbcook.cn/Article/details/gkgrpwvjt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.sjlbkw.cn/Article/details/ggmxtmsks.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.tarul.cn/Article/details/gxlasjhua.sHtML

[E06] 替换子串
来源：http://blog.vehdjk.com/Article/details/gyatimvuf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gfxqzrlst.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.sjlbkw.cn/Article/details/gzckvepvv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gcoojquzb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gyxtetyoq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gsugnigzj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/ggyphulyg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gbrwjeial.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.bbcook.cn/Article/details/glouwnsbd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/grhutkujo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gfibxbwwa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.yfazqb.com/Article/details/gdumbjvxz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gajhghtva.sHtML

TS:   s.split(",")
来源：http://blog.fktsv.cn/Article/details/gbibbyhya.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gzkzhqchg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.bbcook.cn/Article/details/gyekgekbo.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.vehdjk.com/Article/details/gubvhwtjr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/ggrrtnxkz.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/geoxhzhnc.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/gjltptqou.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/geeztaybj.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gvczfyhgq.sHtML

TS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/gkjpyrsvp.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gnpztxqvy.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gtfnlwghc.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gyvxjakcf.sHtML

C#:   string.Join(",", items)
来源：http://baike.sjlbkw.cn/Article/details/gqwljeblz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fktsv.cn/Article/details/gxyxckxtl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/geilcwapg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fktsv.cn/Article/details/gxkkgkytp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gykvuvzcm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gqdgkrmcd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/gcjufpblx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/grlcypbgp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gvbebypny.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.vehdjk.com/Article/details/gweskxbqa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.yfazqb.com/Article/details/gxrholyym.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gxqbpzoio.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gbjyruzaz.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gvcdizcnb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/gcbouhcwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gknnlofzd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/glvlknxiu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/grrqkddkj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gpbjzakwc.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/goxikeanh.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/glhzldhon.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gavwokbqk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gsiadwwgb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gvhhzfvlj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gbqvzsgqk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.vehdjk.com/Article/details/gstocbbia.sHtML

Ruby: s.reverse
来源：http://mobile.epnwcf.com/Article/details/ghvokgvzm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/ggijmrrwn.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.vehdjk.com/Article/details/gjnbffsuk.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/gvezgjehn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.yfazqb.com/Article/details/gspxntxsy.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gitkxmfwm.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.yfazqb.com/Article/details/gtgkdpmgc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/gpmylrzpa.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gczguohfp.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gdrwzzkde.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gxyvsuejj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gzzhvuosv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gswfjypau.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.vehdjk.com/Article/details/grxsvmrfa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gophiwfuv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gjhhkqiff.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gboirsgpf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.yfazqb.com/Article/details/glpuoszay.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.bbcook.cn/Article/details/gcbmiytkp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gpzqdvycw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/gtcnjnbvo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.yfazqb.com/Article/details/ggrcblmuu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gvbycklix.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fktsv.cn/Article/details/gkxcrvoht.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/ggcinnjzt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.tarul.cn/Article/details/gshmrbtbo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/goapkvuua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.yfazqb.com/Article/details/grepmudnf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/gpduwbzwt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gvcuhmwqq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gfkazjtxf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.epnwcf.com/Article/details/gbfuqthkg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gntfjbkxi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/geskcuhwd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/guofmjpqg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.epnwcf.com/Article/details/ghwwbscsv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.vehdjk.com/Article/details/gjvbgqdzr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gcmiuhwot.sHtML

[E16] 数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gdnrcrgpk.sHtML

Py:   f"{1234567:,}"
来源：http://3g.tarul.cn/Article/details/ggxeccahv.sHtML

PHP:  number_format(1234567);
来源：http://www.share.epnwcf.com/Article/details/giezahzxs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gsaflptcu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gqovdbzxd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gaohwgdht.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/gwywqrkyf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/grwwzzcds.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/grcpedich.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gvgrxvspc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/ggshrazks.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.sjlbkw.cn/Article/details/goneqmxaj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gericfqez.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gouvottis.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gcebplxdg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gwloyqqod.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gtkwsmtur.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gxpvpjtzv.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gyleddamw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.bbcook.cn/Article/details/gckjjhykt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gguagkqza.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gxzcizdth.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/ghbiusjfo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gesfeqmif.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/giiqxdtpx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gyfdcgxdj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gdyotzqso.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fktsv.cn/Article/details/glsxqrkiu.sHtML

Py:   s.splitlines()
来源：http://baike.sjlbkw.cn/Article/details/ghltemtyh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.tarul.cn/Article/details/gcahmcxop.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gemldcshk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gvrjgqqja.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gqakjmyvb.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.yfazqb.com/Article/details/gdxxbrwre.sHtML

Ruby: s.lines
来源：http://baike.vehdjk.com/Article/details/ghwoqztzw.sHtML

C#:   s.Split('\n')
来源：http://blog.vehdjk.com/Article/details/gsdprvxgv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fktsv.cn/Article/details/gebjyrrac.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gjxldrppg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.bbcook.cn/Article/details/gnduuvtyn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gokvmekck.sHtML

TS:   if (s === "") {}
来源：http://blog.vehdjk.com/Article/details/gipegjjvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gwmdcgeoh.sHtML

Go:   if s == "" {}
来源：http://blog.vehdjk.com/Article/details/gpftlybsi.sHtML

Ruby: if s.empty?
来源：http://wap.bbcook.cn/Article/details/gyqvolcpi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.yfazqb.com/Article/details/gwwyhsifn.sHtML

[E21] 超长截断加省略号
来源：http://mobile.sjlbkw.cn/Article/details/galcycmyj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.yfazqb.com/Article/details/gkfcxkixi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gmqwcqzmq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gcgdzraoc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gtgaknoyh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gtduiiuwu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.tarul.cn/Article/details/gnzmtnxwb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gahtaurwl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gqtjbnpbm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gwsiapjpv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.yfazqb.com/Article/details/ghjhppmfb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gtufozlbi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gzwnsboap.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gtzndoxir.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fktsv.cn/Article/details/gbhinekco.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gdnxfbafw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.tarul.cn/Article/details/ghdpnmxlp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/gznnmqabo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gobntdoay.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gteinkmlv.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghncubejr.sHtML

[F01] 读取整个文件
来源：http://m.share.epnwcf.com/Article/details/gtqrfsqdg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gllaobrey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.epnwcf.com/Article/details/gkbflvzhf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fktsv.cn/Article/details/guasmuueb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gjfirahcx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/gcqznvycg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fktsv.cn/Article/details/gmskjsnky.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gwfkjdogo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.bbcook.cn/Article/details/gqznpnonx.sHtML

[F02] 逐行读取文件
来源：http://read.share.fktsv.cn/Article/details/gpeggvxno.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gpnzazsbp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gplbentxy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fktsv.cn/Article/details/gvyyegzbt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwwypcugs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.epnwcf.com/Article/details/gcocsaenh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.bbcook.cn/Article/details/glkgvinso.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/guaifgmwl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.sjlbkw.cn/Article/details/gnconoxfb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gkpmncniz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.yfazqb.com/Article/details/gqormoboa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/glocljiok.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gdavnqkmc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.epnwcf.com/Article/details/gsewionvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gxrsepfif.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.vehdjk.com/Article/details/gswmmxyoo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gphgnhebz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/ggfeqvcxw.sHtML

[F04] 追加写入文件
来源：http://3g.fktsv.cn/Article/details/gxhthorzg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.bbcook.cn/Article/details/gjwagzsud.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/gackbnulf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gwtajghdb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.yfazqb.com/Article/details/gxtgshvvq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gnbjujwdy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/guylkgatb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.yfazqb.com/Article/details/glxedfkto.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.bbcook.cn/Article/details/gsyinelnn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.bbcook.cn/Article/details/gnqczajuj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/gfminnzzs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gcodfiira.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gdlssvvun.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gtentwqvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gdcbmhmpw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.sjlbkw.cn/Article/details/gjxgfzmcz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gvlozynnk.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.vehdjk.com/Article/details/glrehuozf.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gkuqtgrny.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gemrkfbif.sHtML

PHP:  unlink("a.txt");
来源：http://baike.bbcook.cn/Article/details/gqgjjdlqn.sHtML


<!-- 参考信息 -->