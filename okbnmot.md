代发 wailian999

Ruby: arr.tally
来源：http://mobile.vehdjk.com/Article/details/gloqdtnim.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gouzibsqm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.sjlbkw.cn/Article/details/gbyuhrept.sHtML

Py:   x in arr
来源：http://m.share.fktsv.cn/Article/details/gwtmuchxi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.yfazqb.com/Article/details/gfsqvmbyf.sHtML

JS:   arr.includes(x)
来源：http://baike.sjlbkw.cn/Article/details/gkwlywxbv.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gsvqonfmy.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/gpimqsdbl.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gfhcnocya.sHtML

Ruby: arr.include?(x)
来源：http://wap.yfazqb.com/Article/details/gzmtjdlfh.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gduyolotg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.bbcook.cn/Article/details/gkxgouqid.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.yfazqb.com/Article/details/gwjlyqhsu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gxxjtzacb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/ggsppngrr.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/ggmpttymk.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gyarnnigu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.sjlbkw.cn/Article/details/gykdsfhok.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gcnxsjjbn.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.tarul.cn/Article/details/gelbfxrck.sHtML

[D23] reduce 累积计算
来源：http://baike.yfazqb.com/Article/details/gqaoqwoxy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.bbcook.cn/Article/details/glubfyudi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.vehdjk.com/Article/details/gwollwzkf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gvyxodqhi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gmgcvcnrr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gwqbpveck.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gsvjhtanx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gkkptploc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gqruelilh.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.epnwcf.com/Article/details/gsemnsedi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/ghpjgqyos.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.bbcook.cn/Article/details/gqxdkrupp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gdnrukzok.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gvmmetasf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/gtqjscrnv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.epnwcf.com/Article/details/gqitcmdvj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.sjlbkw.cn/Article/details/gzzkfusnt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gvnyvqzqv.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.epnwcf.com/Article/details/gvacvnnco.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/gypktezpa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gdxcdfdkj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/gndpomwnl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/gvksfswph.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gqdyufcei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/gwkxlnsov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.epnwcf.com/Article/details/gsmomjgje.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.yfazqb.com/Article/details/glqjuefmj.sHtML

[D26] 数组转字符串
来源：http://www.blog.epnwcf.com/Article/details/gteothnww.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gcbnzetao.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.yfazqb.com/Article/details/gasorpyuc.sHtML

JS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gvqvxbfww.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gsovvvrnu.sHtML

Java: String.join(", ", list)
来源：http://mobile.sjlbkw.cn/Article/details/gwnrpklbl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.bbcook.cn/Article/details/ghdalhrgl.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gnbvemjqj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.vehdjk.com/Article/details/gjsfhpdoy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/glhmwnrum.sHtML

E. 字符串处理
来源：http://m.share.vehdjk.com/Article/details/gvegndfmt.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqwtpicto.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gbggxyimh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.bbcook.cn/Article/details/gpmwhnzsu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.bbcook.cn/Article/details/gnzwclnvd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fktsv.cn/Article/details/gojaxrvpk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/grvcmomqi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gevpackzm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.vehdjk.com/Article/details/gbrkrffog.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.sjlbkw.cn/Article/details/gwhmdkwao.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gqmylrlny.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/gmmcymnrt.sHtML

Py:   "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gfztsofts.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/grmakibbx.sHtML

JS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/grodffofw.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gubkcvyso.sHtML

Java: "ab".repeat(3)
来源：http://mobile.epnwcf.com/Article/details/gkmjpwbpq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.sjlbkw.cn/Article/details/gurkcdtcb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gasuwnajy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gvnvrfmfk.sHtML

[E03] 截取子串
来源：http://baike.yfazqb.com/Article/details/gomsyhlrr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.sjlbkw.cn/Article/details/gdbpbyloo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gqaseoazz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.bbcook.cn/Article/details/gnzmjhuke.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gqajqtnqb.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gotptdzux.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/gpgwweynf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/grrcalyyk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gjxcvcnzw.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gbzrzzrhu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gxistrajt.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gldhujafm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/glzcmlqlx.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/gegcbenpj.sHtML

Java: s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gqzdodbqx.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.epnwcf.com/Article/details/gziupebhm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gfwzytmln.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gakpekafx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gnemkgjdk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gonrsmiyp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.sjlbkw.cn/Article/details/gccbtmzff.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gsokdgbhk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/geimilelz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.yfazqb.com/Article/details/gqrohscxx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.epnwcf.com/Article/details/gvmbdjlal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fktsv.cn/Article/details/gvfzvwmpq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fktsv.cn/Article/details/gxsgpefig.sHtML

[E06] 替换子串
来源：http://mobile.tarul.cn/Article/details/gjxkckjsb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/guqbehuyp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gmqyguhzu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gqhnkzlzp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gjiswsyud.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/giwtvgqgg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gfvrrfnvg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gbxwzdqjk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gxqwzqwcv.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gitstncwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.bbcook.cn/Article/details/gzdrwlgmv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gfizuxcqs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.vehdjk.com/Article/details/gobhramat.sHtML

TS:   s.split(",")
来源：http://blog.sjlbkw.cn/Article/details/gvgyrlnpf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gqqjuxfev.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.sjlbkw.cn/Article/details/gjuxlzfvc.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.bbcook.cn/Article/details/gvpbfaqsp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/ggognjdga.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.sjlbkw.cn/Article/details/gpsvqlzlq.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gfxrepzwu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gmyvkwiiq.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/gvsmtgwrg.sHtML

TS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/gljndafuu.sHtML

Java: String.join(",", items)
来源：http://www.share.bbcook.cn/Article/details/gmfmotsvq.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.epnwcf.com/Article/details/gdiqigyes.sHtML

Ruby: items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gtluptwtl.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gzzdfgery.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gboupfptz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gxkwjitmf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/gvxetktaw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.yfazqb.com/Article/details/gjgmumcuc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.tarul.cn/Article/details/gditnycxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gspjaihux.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fktsv.cn/Article/details/gixbpnqbf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gqpvhzdlr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gkhkjbhnm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.vehdjk.com/Article/details/gknaikrph.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/godajgpmf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/gfuclxhja.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gjpgxfunw.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gkmktbivp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gcpvothzf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gbscprtbg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gocokcovp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gviqgqhvg.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gvgxenmce.sHtML

Py:   s[::-1]
来源：http://mobile.vehdjk.com/Article/details/ghzfzmfuv.sHtML

PHP:  strrev($s);
来源：http://3g.tarul.cn/Article/details/gkzhkbvzz.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/glckghdvb.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/goufpgwcr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gggxvysra.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gpwyhkffl.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/gqpwikhpl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gsrjuvwue.sHtML

[E12] 统计某字符出现次数
来源：http://blog.bbcook.cn/Article/details/gqkpxhnmo.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/greqowddy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzlglfph.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gaijdzlrs.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/giszkedmz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gumciyips.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gnbcxpshf.sHtML

Ruby: s.count("a")
来源：http://www.blog.epnwcf.com/Article/details/gwldypiuh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.sjlbkw.cn/Article/details/gtihgcxuf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gdlvkfery.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gtougptfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.vehdjk.com/Article/details/gtzhuvhpo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gveqcdcam.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gndpprcjn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gzmewzfii.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.yfazqb.com/Article/details/gliiqjfvs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/greexgyop.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfrrcngp.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/grisnwsem.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.bbcook.cn/Article/details/ghycwzfaz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gdhrmuywi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.tarul.cn/Article/details/gpccqakzx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfmqbblb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gskqeaqhr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.tarul.cn/Article/details/gbtgrondr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/ganfgcwpr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fktsv.cn/Article/details/gdablteip.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.bbcook.cn/Article/details/gzdhtqmhr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/ghbufzniy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.vehdjk.com/Article/details/gsgrusfwc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gbpopbqmd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gpekblnye.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.sjlbkw.cn/Article/details/glgyuigjz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gdchzvzhk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.epnwcf.com/Article/details/gpcvpnroc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.bbcook.cn/Article/details/gediftiya.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/ghbdpcqka.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gvcrpjmfd.sHtML

PHP:  number_format(1234567);
来源：http://baike.epnwcf.com/Article/details/ggprdkdlz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gljwelmjl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gblohpxar.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.bbcook.cn/Article/details/gilashefz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fktsv.cn/Article/details/gxgqrpnpu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/grzsoviht.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.epnwcf.com/Article/details/gucpbuzlm.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gvzvyrgtm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fktsv.cn/Article/details/gakvsvcui.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.bbcook.cn/Article/details/gyrobhtrw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gsnsqvcjr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/grtxohcmq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gbiggxojf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/glpgkspyz.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gnlomcobc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.vehdjk.com/Article/details/gzrhhmhhx.sHtML

[E18] 模板占位符替换
来源：http://m.share.tarul.cn/Article/details/gngsodafx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.vehdjk.com/Article/details/gfzxvtivs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fktsv.cn/Article/details/giviyjvpx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gfmnkqzuh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/ggfznvrgf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/guydrszih.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gfjqyuram.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.vehdjk.com/Article/details/giujmirbl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.epnwcf.com/Article/details/gaighqive.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.vehdjk.com/Article/details/gfjgfapbj.sHtML

Py:   s.splitlines()
来源：http://www.m.share.yfazqb.com/Article/details/gjlyncsgr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gtcncaimg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gfvvgtnrc.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fktsv.cn/Article/details/gevriignt.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gajqtallo.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.sjlbkw.cn/Article/details/gnrxgmkkf.sHtML

Ruby: s.lines
来源：http://blog.tarul.cn/Article/details/gazprfxtu.sHtML

C#:   s.Split('\n')
来源：http://wap.vehdjk.com/Article/details/gxbjgvbdu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/gpgdjzxau.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gmzzcabky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gqgslzjvg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gahzazuez.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gztqstuhv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gxmuxdxpw.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gkqqvpfpm.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gncmxeufn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gsmjdanpn.sHtML

[E21] 超长截断加省略号
来源：http://wap.bbcook.cn/Article/details/gwpgthxbi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.vehdjk.com/Article/details/gbjklyerh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/grytdoyyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gjszrcgcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gkpixeodc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/gkdwkqafc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gvetjxkpg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gkskthwns.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/gksuerosd.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/gfndhnpph.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/givtlrxgk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gskwnupmd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.bbcook.cn/Article/details/grixbvvam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.tarul.cn/Article/details/gyccjvtuj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fktsv.cn/Article/details/goqrtivnu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gbzoaozxx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/gdoafnpmd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.tarul.cn/Article/details/grhkcoulj.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gpkksxenj.sHtML

F. 文件与目录
来源：http://baike.tarul.cn/Article/details/gvpkblxxq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/guyusnoly.sHtML

[F01] 读取整个文件
来源：http://wap.sjlbkw.cn/Article/details/gycwcdfum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gnejqlyyb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gohbicknq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gaukyakee.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gudhscmyz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/guuzythjy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.tarul.cn/Article/details/gdyosmxvu.sHtML

Ruby: File.read("a.txt")
来源：http://wap.yfazqb.com/Article/details/gexhbosvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/grszduayj.sHtML

[F02] 逐行读取文件
来源：http://wap.epnwcf.com/Article/details/gwguydazp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.sjlbkw.cn/Article/details/gqkmacesw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/glhtsaecn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/grbigkefr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gknjyzdxk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.epnwcf.com/Article/details/gkyfrxact.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.tarul.cn/Article/details/gupbsyfzf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gsdkpzwoa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fktsv.cn/Article/details/gszsmuxwt.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/glxxqjfpu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gmbwyblnm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/griyyzuhg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.epnwcf.com/Article/details/gqaewyral.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/gntywgbcy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gwnirqwjl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/gsrujujzz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.tarul.cn/Article/details/ghimenqyp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gcigwvpmt.sHtML

[F04] 追加写入文件
来源：http://read.share.sjlbkw.cn/Article/details/gpabzynci.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.vehdjk.com/Article/details/gjnkuvcrf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/ghlkveykf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gprmsckij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gilyxzxje.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.epnwcf.com/Article/details/gmqwattrq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.bbcook.cn/Article/details/gtqxqkdcs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gxvibfrdd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/ggceimviy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gdmwapqdw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gmszhoraz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.tarul.cn/Article/details/guwpfrlug.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gzcznmzjq.sHtML


<!-- 参考信息 -->