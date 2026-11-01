代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.bbcook.cn/Article/details/gnofqqcyb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.tarul.cn/Article/details/gxbrcfcik.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gpvoujhac.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.vehdjk.com/Article/details/gaasdnyke.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/goatwbzll.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.epnwcf.com/Article/details/goromshyk.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gystanqia.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gvvlvidvz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.sjlbkw.cn/Article/details/gvgtlummf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gmvzjahbb.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/giibtvgkn.sHtML

Java: list.contains(x)
来源：http://baike.yfazqb.com/Article/details/gqlwyvhtl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/geistmhrq.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gwbxltpzy.sHtML

C#:   list.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gsimsjcdz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/gtpxvobnl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.vehdjk.com/Article/details/geqfriwxn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gpjzidcsk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.yfazqb.com/Article/details/ghffnkgly.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gawhjjtya.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.tarul.cn/Article/details/gourjadgh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.yfazqb.com/Article/details/gtfjjdnzi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gyavauqqu.sHtML

C#:   new List<int>(list);
来源：http://blog.vehdjk.com/Article/details/ghefwrwqu.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gbxsteabf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fktsv.cn/Article/details/gfiqqxiii.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/ghbijwxtt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.vehdjk.com/Article/details/gyblakxmh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/gjrngffgk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.tarul.cn/Article/details/gxnwgembg.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gjonjilhs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/giiiuuaqb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gbgcaxtfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gmorxbtrt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gguwizlmh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/gzvwijedr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.tarul.cn/Article/details/grlcsvcnz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.tarul.cn/Article/details/gvkfqfdmm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gsmdrewah.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.epnwcf.com/Article/details/gjrgeqigm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.epnwcf.com/Article/details/gppwvmoxv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gwwwkrywu.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/ghahgbqcn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gqtktzuqv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gjjlywixv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/ggtdwtevr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gxzkxzumy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gtkskolvj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gqwwehdcu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.bbcook.cn/Article/details/gtybnpprc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.vehdjk.com/Article/details/gllproufu.sHtML

[D26] 数组转字符串
来源：http://blog.yfazqb.com/Article/details/ghlyoewcx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.yfazqb.com/Article/details/gfhqcjuwu.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.sjlbkw.cn/Article/details/ghateepdp.sHtML

JS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gokapebpw.sHtML

TS:   arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gxppsvgxd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gkzyrhvny.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/gfthcfwwv.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gvlxswlhi.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gxlvkclbj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gsfolycqa.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/gjisooeaq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkvrfghdh.sHtML

[E01] 拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gsusnbkzi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gkzxxhjys.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gkejbhtxe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.sjlbkw.cn/Article/details/gdtysvhes.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gwvmfayma.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.yfazqb.com/Article/details/gnlyizzgf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/ghcviszru.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.vehdjk.com/Article/details/gyhkrgcvc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/glvbbvcoe.sHtML

[E02] 重复字符串
来源：http://blog.vehdjk.com/Article/details/gfmvduhfe.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gupabybfy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gtjaqqmvg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gvldvixhw.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/glslnywpm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.sjlbkw.cn/Article/details/gcxdavmws.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/gcbjvyouo.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gmckkcxtz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.vehdjk.com/Article/details/gfmxmjbwr.sHtML

[E03] 截取子串
来源：http://baike.fktsv.cn/Article/details/gtarxqxjl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/gcjdhtbly.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gtrlwhpaf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/ghdvgmrlo.sHtML

TS:   s.slice(1, 4)
来源：http://wap.tarul.cn/Article/details/gscrebqpt.sHtML

Java: s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gghrlzgaj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/giaeiqzov.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.tarul.cn/Article/details/guwepuppo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.vehdjk.com/Article/details/gmoxulexq.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gxfrqdtzq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/ghtqrxxka.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gdlcdkksd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.yfazqb.com/Article/details/gizhqdvkd.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gshfvevtz.sHtML

Java: s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/glloanjsb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.yfazqb.com/Article/details/gmzdjcyka.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gdpkpdvfx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gtmykuusl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.sjlbkw.cn/Article/details/gzrtudvre.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gknsoizxz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/giwwgiprw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gvokpwoyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/grgdacwmw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gtlznkbrm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gkqufcrkk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gombongjg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.tarul.cn/Article/details/gzzmhgorw.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/grszweyzp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.tarul.cn/Article/details/gtmlnucmn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gssnqiaex.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gzhzqsmqk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/giarcsuwv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gltbubnbe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gztxuwotp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fktsv.cn/Article/details/gncfzbnow.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gbmjqxfsc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fktsv.cn/Article/details/ggwvruwra.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gyukimdub.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.bbcook.cn/Article/details/gulsunglt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.epnwcf.com/Article/details/gcrgobsjm.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gpyrkfclu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/ghnwdrztt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.tarul.cn/Article/details/grmxpoqay.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.epnwcf.com/Article/details/ghxefimqa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.vehdjk.com/Article/details/gpchnxlny.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gpwjejlvi.sHtML

Py:   ",".join(items)
来源：http://baike.bbcook.cn/Article/details/gjtnvpvyz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.sjlbkw.cn/Article/details/ghrvgqpkw.sHtML

JS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gzbziffnf.sHtML

TS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gaqtqehxe.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gjmsanfdo.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.sjlbkw.cn/Article/details/gwbiofpqg.sHtML

Ruby: items.join(",")
来源：http://read.share.bbcook.cn/Article/details/gibthskhn.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gcysybyld.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/ggqolzrjy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gvxcmpktk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gxoqvealh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/guoqmccbx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gvtbgrltm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gsnxsvoin.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gjzpvtjym.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gzgvakwzg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gzyqfvhdl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gcxeencmj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fktsv.cn/Article/details/gbgrdbihr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/glaexrrom.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gsiilgrcz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gqbpxzpry.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gcxhxzgzg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gawuaiuht.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gaqntycgo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.tarul.cn/Article/details/gvmrariqe.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gvcqkeatc.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gpjrkfeks.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gckqpicnv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gmmwnktcr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/geinajmsv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gbsybggvl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gsrbdlxwa.sHtML

Ruby: s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gkwixeken.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/ghenjsvsa.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.vehdjk.com/Article/details/gzotzahpx.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/ghyoghusr.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.sjlbkw.cn/Article/details/gzkjelmgx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gljkbqcnd.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/glmlyfict.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.vehdjk.com/Article/details/guvixskhv.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.epnwcf.com/Article/details/gnlxtmgxo.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gzovsghjz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gyuqsiaxd.sHtML

[E13] 逐字符遍历
来源：http://blog.vehdjk.com/Article/details/gzaibpxjm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.epnwcf.com/Article/details/gcaflccsv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.bbcook.cn/Article/details/gadpjfhwp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gpqggbnyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.vehdjk.com/Article/details/ggchetvap.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/groynbwqs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/gqubfktzb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fktsv.cn/Article/details/gkdebzosr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbdfdhbay.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gylvnrcfv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.sjlbkw.cn/Article/details/gpcwosezr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gkjabxzux.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.vehdjk.com/Article/details/gchuyanjt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.bbcook.cn/Article/details/gvpdgmdvy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gsfukpsid.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gtnenysdp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gqkihjyrl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fktsv.cn/Article/details/grweoiwtv.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.yfazqb.com/Article/details/geubxvkmq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.sjlbkw.cn/Article/details/gsguzlwhx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fktsv.cn/Article/details/glvqenscf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.vehdjk.com/Article/details/giibnjwyp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fktsv.cn/Article/details/gddantlxo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.yfazqb.com/Article/details/gtcmqjsna.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fktsv.cn/Article/details/gqnosskmj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvwiorjn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gmypbhfqb.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/gwijqsvlf.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gyymblakr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.vehdjk.com/Article/details/gjaciegxr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gwomgquxr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/gsrtroaio.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.tarul.cn/Article/details/gpupkblfz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gefeywbfu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gjnrjicnn.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gqkaxmzzm.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gqxymjelc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gatcmuhwn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gppkppepg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gsbnxyvux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gjvphblpw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gijxpjxlx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.vehdjk.com/Article/details/ghqqevulk.sHtML

Ruby: s.capitalize
来源：http://read.share.fktsv.cn/Article/details/gdiwvmthd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.epnwcf.com/Article/details/gfnjithfc.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gnlsmibwl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.tarul.cn/Article/details/gdzkrjxbw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gqsirmhnw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gkosrmoxc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gcqdfcfcg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gmgfxxymx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.tarul.cn/Article/details/gqaygflkp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/gluxafonh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gyqgviqsv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gfncskgsx.sHtML

Py:   s.splitlines()
来源：http://mobile.fktsv.cn/Article/details/gybubdgwk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gvmmdikjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gxpdgcxug.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gdqwikakc.sHtML

Java: s.lines().toList()
来源：http://wap.sjlbkw.cn/Article/details/gqyynyjly.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.tarul.cn/Article/details/gzzvkgvik.sHtML

Ruby: s.lines
来源：http://m.share.epnwcf.com/Article/details/gqhwfgrns.sHtML

C#:   s.Split('\n')
来源：http://www.share.fktsv.cn/Article/details/gnqgtvehj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.tarul.cn/Article/details/gqheoagfq.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gepritsdq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/guwnezjbt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/gxnrexhlz.sHtML

TS:   if (s === "") {}
来源：http://blog.sjlbkw.cn/Article/details/gmtqjujjd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gznfceyve.sHtML

Go:   if s == "" {}
来源：http://blog.sjlbkw.cn/Article/details/gjwkjxhjg.sHtML

Ruby: if s.empty?
来源：http://mobile.sjlbkw.cn/Article/details/guxizcdmz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjwazmuyu.sHtML

[E21] 超长截断加省略号
来源：http://blog.bbcook.cn/Article/details/giuxoknyr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/geqrdaenb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gjgodqgvw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/ghpewhhow.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gskawmhkr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gfcbpkutx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/gudnrkqpf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/giiymdpna.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gyupzmpcm.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.yfazqb.com/Article/details/gztdmfyvd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gbvpqrukz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gyzpdlujq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.sjlbkw.cn/Article/details/gyjrnydsi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gatultbir.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gqacqptny.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gknsmynfz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.bbcook.cn/Article/details/gblbjxcmc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/gabxjugve.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpubjklmm.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/geerhjzhd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gonjzjemy.sHtML

[F01] 读取整个文件
来源：http://mobile.sjlbkw.cn/Article/details/gvylekzff.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fktsv.cn/Article/details/gbegxrydw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gkkqzcvkz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gbewrjhnl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gxwwioegm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gneirqvqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.bbcook.cn/Article/details/ganrjdvyb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gqkvwlvje.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gyvkzdawt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxupexbx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.bbcook.cn/Article/details/ghsohecwt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fktsv.cn/Article/details/gcihjzgrh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gkcdmstom.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/guzlojwwy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/grvzdrlcp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/gripkxrzy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gnmyemqlv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.yfazqb.com/Article/details/gcktoygur.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fktsv.cn/Article/details/gdvfkkthw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/glpgzcwoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gtxrxzbsj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gjuljpdfp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/giheudcun.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.tarul.cn/Article/details/gimarecft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.sjlbkw.cn/Article/details/ggbjoriew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.yfazqb.com/Article/details/gwcioaypz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gaaeexfgf.sHtML

[F04] 追加写入文件
来源：http://m.share.tarul.cn/Article/details/glxsgxwrg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gzisaiahn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.tarul.cn/Article/details/gyoljjmlp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/grncpauod.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gfpicsdew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.bbcook.cn/Article/details/gwssdqvnb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.vehdjk.com/Article/details/ggmctxdvm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.yfazqb.com/Article/details/gwawwwmab.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.sjlbkw.cn/Article/details/gaczlqpiq.sHtML


<!-- 参考信息 -->