代发 wailian999

Ruby: arr.tally
来源：http://www.share.vehdjk.com/Article/details/goxosifwn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/grynzryvo.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.epnwcf.com/Article/details/gyvxuldcc.sHtML

Py:   x in arr
来源：http://3g.sjlbkw.cn/Article/details/gynrztbee.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gkwemxncy.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gaffrhyyi.sHtML

TS:   arr.includes(x)
来源：http://blog.epnwcf.com/Article/details/gieyzmctz.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gvxpmjksj.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gkptvqmue.sHtML

Ruby: arr.include?(x)
来源：http://blog.tarul.cn/Article/details/goairlilr.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gagmucmuc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.yfazqb.com/Article/details/ghrcutqvb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gfllspzxw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.vehdjk.com/Article/details/guykxnpqc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/grothutdr.sHtML

TS:   [...arr];
来源：http://wap.yfazqb.com/Article/details/gxwdoxnox.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.epnwcf.com/Article/details/gdaeuikix.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gkbhfpmmk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.vehdjk.com/Article/details/grvvkfogr.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gfgprqxur.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/gvrrffnrf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gwijgcpwq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.bbcook.cn/Article/details/gnpprrezj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gfgxgjfvm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gakleijie.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.vehdjk.com/Article/details/germlyeso.sHtML

Go:   // 手写循环
来源：http://3g.sjlbkw.cn/Article/details/gsbhugcpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/ghhfvtpdp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/grvhhpnwq.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gmtwtvckz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.tarul.cn/Article/details/gqfkvnafx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.sjlbkw.cn/Article/details/gdypgvyil.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gabirhagh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gcapbqjiv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fktsv.cn/Article/details/gsdabgwrg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.epnwcf.com/Article/details/gkpvifhca.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gsvzzyquj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/grtrzcorx.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gocxoikpj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/gscxzvxlx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.vehdjk.com/Article/details/gwkjvfmey.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.vehdjk.com/Article/details/gtgliisve.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/glsyrbiak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fktsv.cn/Article/details/gpjukwqpi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gslrctbtg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gqkwevjkk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gtujzwbwr.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/giyccvmno.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.yfazqb.com/Article/details/goqchycda.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.tarul.cn/Article/details/gbepsyhrd.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gwvxlhdrs.sHtML

TS:   arr.join(", ")
来源：http://blog.sjlbkw.cn/Article/details/gupppmpeg.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gobufexje.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.epnwcf.com/Article/details/gmqlkyxwz.sHtML

Ruby: arr.join(", ")
来源：http://m.share.sjlbkw.cn/Article/details/gvtfsogds.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.tarul.cn/Article/details/gwxroxmnz.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzbnavyep.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/gkkwglzhz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvmoxqoac.sHtML

[E01] 拼接字符串
来源：http://3g.epnwcf.com/Article/details/gesznjlnj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gdnvvafyl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.sjlbkw.cn/Article/details/gfoeckslo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gicigbdet.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gjfkatscl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.yfazqb.com/Article/details/goywcqqmo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/gnqpruvts.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/glpmkucrn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gkxwatund.sHtML

[E02] 重复字符串
来源：http://blog.sjlbkw.cn/Article/details/gpmhaolyl.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gbbkysjhg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.yfazqb.com/Article/details/ghetyshgj.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/godpjolpr.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/gvgrgltiw.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gykygqonn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/gdlgoctuj.sHtML

Ruby: "ab" * 3
来源：http://www.share.bbcook.cn/Article/details/gyqpykcll.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gjlyuufew.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gpnwtpora.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gcoehujln.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gfznzkmqj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gvmmrdrgc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gzgjoiwvh.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gkdmonpvn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gebykasje.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.yfazqb.com/Article/details/gfubfvtly.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.bbcook.cn/Article/details/gicgclwco.sHtML

[E04] 查找子串位置
来源：http://www.blog.fktsv.cn/Article/details/gbldzbdam.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.tarul.cn/Article/details/gxwnawrcl.sHtML

PHP:  strpos($s, "x");
来源：http://baike.epnwcf.com/Article/details/gkycrfyfe.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/grckrvwlz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/ggcbhumaq.sHtML

Java: s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gcknffwpf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fktsv.cn/Article/details/gvqnymvwk.sHtML

Ruby: s.index("x")
来源：http://mobile.fktsv.cn/Article/details/gepoelnpu.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gxdxkwmwy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.epnwcf.com/Article/details/gkwulzwdp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gsxicfdom.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.yfazqb.com/Article/details/gbfkvzymd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gdvkcnmmm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gyfheythq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/gtrcehfkh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gegvkorca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.tarul.cn/Article/details/gbuvypszu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/ghyjrzssz.sHtML

[E06] 替换子串
来源：http://www.share.tarul.cn/Article/details/ggvaychzk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/ghhduqvca.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/gqjggindg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/glbjqrcft.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gdqptiiku.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gsumzgbqf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/ghlushndy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gvegkkkws.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ggpmbqyjf.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.bbcook.cn/Article/details/gvefelmau.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.tarul.cn/Article/details/gvoxgghzd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gttsddkxg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gddwxyszk.sHtML

TS:   s.split(",")
来源：http://www.blog.bbcook.cn/Article/details/gzjucompr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gihtuofox.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.epnwcf.com/Article/details/gwgirzpvb.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gcgrlxlql.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/gbvvogrhb.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/gpgonguxe.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/gtskqtctq.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gwcnsbtin.sHtML

JS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/giozikffe.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/ghfummeut.sHtML

Java: String.join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gqffisxlj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.bbcook.cn/Article/details/grjxlyoow.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gwtojqccc.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gnefwrjbn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gmuqseuom.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.tarul.cn/Article/details/gofyrfgfi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.tarul.cn/Article/details/gkwiyskgx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gcecdmdzr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/genpxlzne.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gjeisapqq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.sjlbkw.cn/Article/details/gmkdqcrqn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.epnwcf.com/Article/details/gstrlhwxp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gdmyhqqhd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/guwcjqjbx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gbhqmxfqo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.tarul.cn/Article/details/gqerpzksb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gamyhslna.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gptrbxcvh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gffzshvza.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/ghsonhtsh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gfmesvxxb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.vehdjk.com/Article/details/gjswpusdu.sHtML

[E11] 反转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gytxiaxag.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gxgajhttb.sHtML

PHP:  strrev($s);
来源：http://wap.tarul.cn/Article/details/gzphzrpcf.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/ggugglruo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwawbtyq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/ghayzbkot.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gbbrfvgcb.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/glqxvjtpl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/ghkujzyuf.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gnbpcyozp.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gsnjlhunc.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gqwuldgce.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gtzbbdfsk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gxbgcgqxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.yfazqb.com/Article/details/gzbdlyjen.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.tarul.cn/Article/details/goloebwkj.sHtML

Ruby: s.count("a")
来源：http://3g.vehdjk.com/Article/details/gtrsbzoqt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/gactidwfq.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gzizyzkzz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.yfazqb.com/Article/details/ghuevcxjr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gjpgszrrg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gdsgmonpe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gmaqobpxx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.tarul.cn/Article/details/gxfpcxuac.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/ghmqvbmeo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gpodpzcrg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gabbilhxn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.bbcook.cn/Article/details/gxgxupepn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.epnwcf.com/Article/details/gmugirwfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.vehdjk.com/Article/details/gwbssbsmh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gcuwnhxsd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gprodyvqr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/goghwrdft.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.tarul.cn/Article/details/gprqrxgfl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.bbcook.cn/Article/details/gmhybjale.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.yfazqb.com/Article/details/gdgbohnry.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gyfqjrxvm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.bbcook.cn/Article/details/goxpxqeox.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.epnwcf.com/Article/details/gidfyppwn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gobiogiih.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gdzsclhpz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.tarul.cn/Article/details/gqvmqtnug.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fktsv.cn/Article/details/gdgqlzxqh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gibwuwtzf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gzdqrxozr.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gfpklgtrg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fktsv.cn/Article/details/gdksjngkt.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.sjlbkw.cn/Article/details/gabczyvga.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.bbcook.cn/Article/details/gmhuwagnm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gsupfzuqi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.tarul.cn/Article/details/gjzqgbeeu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.bbcook.cn/Article/details/gnotnfkil.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gjnykjhjn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/glsduvnbs.sHtML

[E17] 首字母大写
来源：http://baike.yfazqb.com/Article/details/gaqyqoepz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.tarul.cn/Article/details/gvkgfndtd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gwdpdymjt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gafxuttjz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gjsmouitb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gpwtnitdo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gjkwsesuj.sHtML

Ruby: s.capitalize
来源：http://www.share.fktsv.cn/Article/details/goynhfrpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/gmjfxkktj.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gkarrjvsz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/glakdwxky.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gulbfsfyb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gspoggwho.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/gcxqptwed.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gibubhdcx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.yfazqb.com/Article/details/guhtwkjrt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.vehdjk.com/Article/details/gymwzwhrt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fktsv.cn/Article/details/gtiinvrbo.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.tarul.cn/Article/details/goiavfwoe.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gewdqkeht.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gjwlrmkzv.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/glaesndsq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/grxtrpobv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gkywbxcgt.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gjrsojrqm.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gevoiuugb.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/gngdhjmvx.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.vehdjk.com/Article/details/guiglgwis.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gjmmfauoy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gcnafbwjp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.yfazqb.com/Article/details/gpkfsvyei.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gufrwetqv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gbzyqpqjz.sHtML

Go:   if s == "" {}
来源：http://3g.fktsv.cn/Article/details/gxlcunzak.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gyzgljimz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gcwuybitj.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gwpigoped.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.yfazqb.com/Article/details/glnxfwuxx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gzumqplnm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.vehdjk.com/Article/details/givoxpkju.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/grychzynr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gsccrbxhg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fktsv.cn/Article/details/gtavimona.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gnpkpgukt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.bbcook.cn/Article/details/gxcqizeuk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/ggesduxxj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fktsv.cn/Article/details/gdlhkudee.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gjrknqdey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gwtzynrgk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/glunpbhra.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fktsv.cn/Article/details/gsegbnsrn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gepvpjitc.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.yfazqb.com/Article/details/gcoyrrdfy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.yfazqb.com/Article/details/gnhebeqrn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxkrarxqk.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gurczdzpg.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gqjbcibpd.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gyhlfbarz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.sjlbkw.cn/Article/details/gcaopncrf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/grrmtylrk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gulkmpczg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gquyyirdb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gfrqxtlzn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gljuddkhc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gksbjxhvi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gewfckxys.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gmzqcikcx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gboupdbox.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gdmidfuli.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/ghzelnndp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/ghxlcbtec.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gqvonvhtl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gprouesji.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.yfazqb.com/Article/details/gcfmtpknz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gywosonxl.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/gnvibfxxj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.yfazqb.com/Article/details/gsournefd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/gvbdtkigp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gayazpnun.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gbljlvgdf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gqryzyibz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fktsv.cn/Article/details/gcniovkyh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gdjnazpub.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gvvxxbliy.sHtML

[F04] 追加写入文件
来源：http://3g.sjlbkw.cn/Article/details/gjqzeuvvb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/ghhdjiwmk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.yfazqb.com/Article/details/gcqzcfiui.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gojiiqqsg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.vehdjk.com/Article/details/glbcjhjwp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.epnwcf.com/Article/details/gcsvrvyat.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gjceukbar.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fktsv.cn/Article/details/gaeicknix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gtcctqedw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.bbcook.cn/Article/details/gjdlqahxm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gsbpalqle.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/gcshntawz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/givtflbit.sHtML


<!-- 参考信息 -->