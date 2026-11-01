代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.bbcook.cn/Article/details/guuhdgikb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.tarul.cn/Article/details/greekvvji.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.tarul.cn/Article/details/gfdchocyf.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.yfazqb.com/Article/details/gnsawqyda.sHtML

Ruby: arr.tally
来源：http://m.share.tarul.cn/Article/details/gstmpvbvn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.epnwcf.com/Article/details/gtxwsbffm.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gvxsplahq.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/glsvazuta.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.yfazqb.com/Article/details/gctpwzaeo.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gdynnlcwp.sHtML

TS:   arr.includes(x)
来源：http://3g.fktsv.cn/Article/details/gjjkozzhm.sHtML

Java: list.contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gvxdbbdvu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gfbnulksb.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fktsv.cn/Article/details/ghzyfwzux.sHtML

C#:   list.Contains(x)
来源：http://www.share.fktsv.cn/Article/details/gshldfhpb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/gohlawekm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gzedhuwmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.bbcook.cn/Article/details/goqjcrsqq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gkgfjdete.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gtivjjsry.sHtML

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gqeepvqba.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.sjlbkw.cn/Article/details/grldtzxxx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fktsv.cn/Article/details/gxpfhnikv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.epnwcf.com/Article/details/gcoqgdakb.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/gufhcrbee.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/gdsnjmdib.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/geesghskx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gzkwkhflv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gxyxpmwlc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gmweslvsk.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/gbhpmmjml.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.yfazqb.com/Article/details/gshacpjtm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fktsv.cn/Article/details/gaxpahfmd.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/gkhrsgtth.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fktsv.cn/Article/details/gydztqmwn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gucearfyr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gehgbiyjd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.epnwcf.com/Article/details/gyjcavzyn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gqmcjajsv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gtasirvgj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gfhzxpdew.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.epnwcf.com/Article/details/gjytvaawr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gglohyrwn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/gyqzoueww.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.sjlbkw.cn/Article/details/gefcfpmhf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.yfazqb.com/Article/details/gsgjlxglc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gnuoanjof.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.yfazqb.com/Article/details/gvoldmypw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.epnwcf.com/Article/details/gvccjzuyu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/guocqawoc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/gyuhvotsa.sHtML

[D26] 数组转字符串
来源：http://mobile.yfazqb.com/Article/details/guqqcesou.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gjoxkflbt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gramdwlmy.sHtML

JS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gstepihik.sHtML

TS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gnhzcwquo.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gfuaydhhb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.tarul.cn/Article/details/gcfuzqwmm.sHtML

Ruby: arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gpzcfqgvc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gtmunwhlf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/greasbcsl.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/gpbvdabxj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gpvcpmpud.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gjgojunbh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.epnwcf.com/Article/details/grkjprlux.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.bbcook.cn/Article/details/ghyypsaxp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gjdwhmrru.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gotwlnsok.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gmigxumsd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.tarul.cn/Article/details/gxrfdcxcf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.tarul.cn/Article/details/godbehmef.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.vehdjk.com/Article/details/gyrduwdva.sHtML

[E02] 重复字符串
来源：http://m.share.bbcook.cn/Article/details/ghguxuish.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gamlmmwzr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/gjegkuxps.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/grpdfnnqa.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gstjinlwt.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gcnmatzpa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gihstftsf.sHtML

Ruby: "ab" * 3
来源：http://blog.yfazqb.com/Article/details/gbftkntil.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.sjlbkw.cn/Article/details/gapwobnzt.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcibymfx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/glwzvfpnt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gvgkaviwa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.vehdjk.com/Article/details/gnoxuuawx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gvgqtrrqx.sHtML

Java: s.substring(1, 4)
来源：http://www.share.bbcook.cn/Article/details/giitdzvgu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.epnwcf.com/Article/details/gzjbcabah.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.bbcook.cn/Article/details/gjtizvxik.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gzlpmdphc.sHtML

[E04] 查找子串位置
来源：http://wap.vehdjk.com/Article/details/gkrbydvfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gcewgidht.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/grufheyum.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gsaicpcxb.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gdbobxedl.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gowrhjgjc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.bbcook.cn/Article/details/gnsuwdgca.sHtML

Ruby: s.index("x")
来源：http://m.share.epnwcf.com/Article/details/gcojngrpo.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gzlmbyusc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gkjaqcdpu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gtsmhkqgl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/geqyjrxta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gxokqovfl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gpgrzqieb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gbjlflqzg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.yfazqb.com/Article/details/gemwggqhw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.yfazqb.com/Article/details/gqhqxrivu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/gemllpfuq.sHtML

[E06] 替换子串
来源：http://m.share.epnwcf.com/Article/details/gacmqcaic.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gpwzzamzl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/gypauwkfl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gbyyyfpdc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gxcmcpxpt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gtaokcuzs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gzowqmatl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ghxmrlrec.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gohgdjvjr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.epnwcf.com/Article/details/gzmqguajp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.sjlbkw.cn/Article/details/gqwqltasz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gydfrrxny.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/grmdkhuno.sHtML

TS:   s.split(",")
来源：http://www.m.share.tarul.cn/Article/details/gnfrlgksk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gvihlszmo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.sjlbkw.cn/Article/details/gnyzjrghw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gqwkejnta.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gekjbhsff.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/glwkxpolb.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gmasjxfqf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gzcunsmgc.sHtML

JS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gpekwpwat.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gfhmbkxya.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gamgaqbyb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gujkewfjz.sHtML

Ruby: items.join(",")
来源：http://wap.bbcook.cn/Article/details/gchypqfee.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gwrcmjcbu.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gsftouzqn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gcdaduwru.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gfrsdhrnc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gpaklhmfu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfxmfprx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.epnwcf.com/Article/details/ghsjhbwqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/ggmoodoaa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/gkdcraodi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gscznpanf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gwisdqwcf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fktsv.cn/Article/details/ggzexrvld.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.bbcook.cn/Article/details/gcfpnjfcq.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gykpyvpdl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gpxuevehw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gjscvbepm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gyohnsnow.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gilaypqui.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/gzbfsivjx.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gkanlhalr.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gxlacnmag.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/geinxbood.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/guqprzkqy.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/glvehdpra.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gddvbdooq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gunnqmbpm.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gwusivdiy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/glejgbdpt.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gwawjaxly.sHtML

Py:   s.count("a")
来源：http://3g.epnwcf.com/Article/details/gfrgivjnr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.vehdjk.com/Article/details/gyzrvtczw.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gsvhyvkgn.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.yfazqb.com/Article/details/gksdmxrvo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.tarul.cn/Article/details/gfiggdlap.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gifgkpnoj.sHtML

Ruby: s.count("a")
来源：http://baike.sjlbkw.cn/Article/details/gcuncdnjm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fktsv.cn/Article/details/gvgaillgd.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gbyekkzoo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.sjlbkw.cn/Article/details/goiemcogo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gkepaictm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gzjmggipp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/gcxeqjpan.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.yfazqb.com/Article/details/gwjrafgbf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gphsykmal.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/grnqksfen.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.bbcook.cn/Article/details/gfqkzzbic.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gubwygyvv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.vehdjk.com/Article/details/gswtcasnb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gtyndmljm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gvkjsrbhe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.bbcook.cn/Article/details/gnsexmzjf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.epnwcf.com/Article/details/gezlvdzkk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fktsv.cn/Article/details/gdmyervcp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/ghasbbfxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gzyhiouiq.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.sjlbkw.cn/Article/details/gkboebbat.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gkplhvbie.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.epnwcf.com/Article/details/gzarabcwf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gthlfwcqq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gwokmtwly.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gtkpthimq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/ggszrsztt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.tarul.cn/Article/details/gdjiyoiag.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.tarul.cn/Article/details/gmokqybhi.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/gqyylojmt.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gczbjoycr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.sjlbkw.cn/Article/details/gyqtlensd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/giejdavmb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gzknhgmrk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gybhldzoq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.tarul.cn/Article/details/grqofaiyp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.yfazqb.com/Article/details/gbbhymxbp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gwhiuzeit.sHtML

[E17] 首字母大写
来源：http://www.share.fktsv.cn/Article/details/gxubeynch.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.vehdjk.com/Article/details/grdicnomw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fktsv.cn/Article/details/gqtfpqsgi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gnfnjbzje.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gvckbeyin.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.yfazqb.com/Article/details/gfsylqqos.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.tarul.cn/Article/details/gjxfkxnjm.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gupkfpxyu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.sjlbkw.cn/Article/details/ggipsmmkx.sHtML

[E18] 模板占位符替换
来源：http://www.blog.epnwcf.com/Article/details/grvcdbaiu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gfsxqvrwe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.sjlbkw.cn/Article/details/gsbiugymk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gcgnxdeuw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/grsnacnem.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/ghnjbvizm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.sjlbkw.cn/Article/details/gtolutmsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/ghosbyabg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.bbcook.cn/Article/details/gvokrbade.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/ghwrardri.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gschoeoxj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.bbcook.cn/Article/details/gouvuttid.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gzzihntli.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.yfazqb.com/Article/details/geckjpppr.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gigftrbxo.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.sjlbkw.cn/Article/details/gtcprxens.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/ggohvchur.sHtML

C#:   s.Split('\n')
来源：http://www.share.yfazqb.com/Article/details/gtducufhu.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gzirahlai.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gqzpstpub.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/ghcjhnpqa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gyeqkrefc.sHtML

TS:   if (s === "") {}
来源：http://www.share.yfazqb.com/Article/details/ghuydgcnz.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gxftiqqlf.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gnuassyow.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/ggivvqflv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnossjsb.sHtML

[E21] 超长截断加省略号
来源：http://m.share.vehdjk.com/Article/details/gtcwwyype.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/goffgxkhl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gcvmrahmk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/glxmqbazq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gnrwqxzer.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gekqvdwqf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/ghgnaidgs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/ggfrugpxx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gcsxzaeqj.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/ghgjyzomp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/gfxymgmui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gkwvnkyac.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gzymgcsgt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gbxhhsycg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/guzodakva.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/grdmgrfmx.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gwhqeoutm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.tarul.cn/Article/details/gwddchdkq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gpuwtmdrr.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/grrupcfbt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gnnnhakll.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gjgpaflgj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/grlvbgfsf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fktsv.cn/Article/details/gxiwremaa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/giqxtqmdo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/grpdbhjni.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fktsv.cn/Article/details/glrerqapd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gfixrjvpp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gnkmfxcqy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gofwtraav.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/grrojobyl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.yfazqb.com/Article/details/gsvizfhmu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gtomfkvjv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fktsv.cn/Article/details/gozzcmmiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/gchgjjven.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/gutvkbvfk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbthjrnn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.bbcook.cn/Article/details/gdkxzzjdn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gugtuhqqy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.epnwcf.com/Article/details/gpqstippk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.sjlbkw.cn/Article/details/gcwhkxwpj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.bbcook.cn/Article/details/grhghjbgy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gxsoymggu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.sjlbkw.cn/Article/details/gmqdjlgme.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gfaupomrh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.bbcook.cn/Article/details/gpteybyqe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fktsv.cn/Article/details/glgjlihfh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gtvujviwg.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gkrjxxdga.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.bbcook.cn/Article/details/gcjkpfely.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gpqqiyvbs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.sjlbkw.cn/Article/details/ghygxxbey.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gltjdracm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/gnobmjfwt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/gbeqxwbcd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gscpnryvi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.yfazqb.com/Article/details/gyvbitrxx.sHtML


<!-- 参考信息 -->