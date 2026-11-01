代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gfjelvjls.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.vehdjk.com/Article/details/gvyuipcxj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.tarul.cn/Article/details/gkjekytxj.sHtML

TS:   [...arr];
来源：http://m.share.epnwcf.com/Article/details/glihpynxf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/guchesbhk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.epnwcf.com/Article/details/gmlwgsdzv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fktsv.cn/Article/details/gukrwhaqn.sHtML

C#:   new List<int>(list);
来源：http://blog.yfazqb.com/Article/details/gcwrzpjmq.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/ggvjnluup.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/gqwnyyauq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.bbcook.cn/Article/details/gweveohne.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.epnwcf.com/Article/details/gurcnhggi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.yfazqb.com/Article/details/ghjqqatxc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/gpqqqebbi.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gszpntkwb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.tarul.cn/Article/details/geytppppw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/ggbdjgpel.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gmsnnpejm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/grlrsoyei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.tarul.cn/Article/details/ghdnjbzrr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gpmawgnlu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gmbrbuzvh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gbgvccwal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gsoqyqcgf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/ghhhtjhoy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gnyiyoviy.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.sjlbkw.cn/Article/details/gcmumnzqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gtmzdejxu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/glkmommmj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.epnwcf.com/Article/details/gsriigbjw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/gqaegfhrk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fktsv.cn/Article/details/gaayjgbfp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.yfazqb.com/Article/details/gjelotkgs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.sjlbkw.cn/Article/details/gkchxyvpt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.vehdjk.com/Article/details/grmdfnemf.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gzrccwvca.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.tarul.cn/Article/details/gfoubezga.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.sjlbkw.cn/Article/details/ggbfsmdcc.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/gmejgszis.sHtML

TS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gxqyjeoyc.sHtML

Java: String.join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gencjljrq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.tarul.cn/Article/details/gqamsnhji.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/grwpwvzse.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gzzhdecwz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gbudokxfy.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gfkbagcrk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmosmwjcv.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gbjwuhojp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gsdxlaixt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/gmgmiwsmb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gvupvqfbj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gyctcsikb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.vehdjk.com/Article/details/ghmqvgzia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.tarul.cn/Article/details/gzmeralxm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gutywedii.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/ghkgntawd.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gcvqcrqnw.sHtML

Py:   "ab" * 3
来源：http://www.blog.fktsv.cn/Article/details/golzhoyrx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.bbcook.cn/Article/details/gemwwbvbq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gqgeqhzjt.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/grdeykesk.sHtML

Java: "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/guyeolxpa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.tarul.cn/Article/details/gelldyhnc.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gsfzbzscu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/gejsnytlh.sHtML

[E03] 截取子串
来源：http://3g.epnwcf.com/Article/details/gpaicward.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/grhzqmelc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/ganjtpbll.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gcamrpvhi.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.tarul.cn/Article/details/gmrhmmoew.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/grohfnpqa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/givldajtx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fktsv.cn/Article/details/gdvlvsgtw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gzkdwcjlg.sHtML

[E04] 查找子串位置
来源：http://www.blog.epnwcf.com/Article/details/gfnffmndl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gopislkdg.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/giclhhoxs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.bbcook.cn/Article/details/gdaruvakt.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gztdsukjd.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gozzqlusz.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gfxuioacl.sHtML

Ruby: s.index("x")
来源：http://mobile.tarul.cn/Article/details/gqcqcigve.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gxkacgxad.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gpzgeptzo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gaksjscgq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fktsv.cn/Article/details/gkgmfbkia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/grxtgkrqs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gxlftkese.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gfrvlfqzh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.sjlbkw.cn/Article/details/gzzysubqe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.epnwcf.com/Article/details/glmmyxjqt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.yfazqb.com/Article/details/gejfgavjd.sHtML

[E06] 替换子串
来源：http://wap.epnwcf.com/Article/details/gsvxmabvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gvldsmwjx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gfvbnrepi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gmtaqidbh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gvteedrey.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gsxekndor.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.vehdjk.com/Article/details/gsiumahgo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.bbcook.cn/Article/details/getykpokp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gloklhrfs.sHtML

[E07] 按分隔符拆分
来源：http://wap.bbcook.cn/Article/details/gtbkmpllo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gayfddhup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/ggsfzdfyx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.vehdjk.com/Article/details/gdyhckbkm.sHtML

TS:   s.split(",")
来源：http://m.share.epnwcf.com/Article/details/genfhpsry.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gckffvwml.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gewoodksf.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.vehdjk.com/Article/details/giwewvcic.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gfsharyyt.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gzbucqiqz.sHtML

Py:   ",".join(items)
来源：http://baike.vehdjk.com/Article/details/garywrzoc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/glwbwecbe.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gopdqxmsc.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gsrhjdyss.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/grftnxrru.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.yfazqb.com/Article/details/gexujcuwp.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gyydtxgbo.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/gshxsweep.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gwkfgcsaf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.vehdjk.com/Article/details/gcidsswwj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/gblahuhbx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gyttrgwgc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gqemylmee.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/ggpatywxx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/ghjvlekvd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/ggguimpcs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/gwfddhcsa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/gqxzqlref.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.epnwcf.com/Article/details/gvluljcvi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gahxaparj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gcdjenjdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gfgwgpftw.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/ghugssjxc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gbzhvsfdy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gaewjjbzk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gcdfynhwf.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/gignbfhno.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gmxvwwlhj.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/guldctgny.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gsjvldois.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gvnyiismp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gtequeolg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.epnwcf.com/Article/details/gdyapyyym.sHtML

Ruby: s.reverse
来源：http://read.share.bbcook.cn/Article/details/gmawduliz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gefsthnuc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gmaffiivk.sHtML

Py:   s.count("a")
来源：http://www.share.bbcook.cn/Article/details/ghfojhbzy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gtrwoalbd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gbndbcqbw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gjdsydqxt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gdjzbvlhh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gchimdnbp.sHtML

Ruby: s.count("a")
来源：http://blog.vehdjk.com/Article/details/glmcykeps.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.tarul.cn/Article/details/gbnrdukts.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gcngnngaw.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fktsv.cn/Article/details/gqxzllxrf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.tarul.cn/Article/details/gzhcdonce.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gkilwspcw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gxhrccdjr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.epnwcf.com/Article/details/gzfjmzkez.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.tarul.cn/Article/details/gtgergesx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.tarul.cn/Article/details/gwyjjttjx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gbghefmhb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gzeoctbbd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gbflomraj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.tarul.cn/Article/details/glfytxglv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gwzyzefyn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gpmjxowjo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.epnwcf.com/Article/details/gxcqcznon.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.epnwcf.com/Article/details/gxdesnfjf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gsylslihz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.vehdjk.com/Article/details/gidcenuxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gxcrisjzl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gxpmmcbvt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gfoyzhwmb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fktsv.cn/Article/details/gqrxhpscp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.bbcook.cn/Article/details/gpmmsdeku.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.vehdjk.com/Article/details/gipbrqctk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gjoahlweg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gnvpndjau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gafffrttt.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gobccuiej.sHtML

Py:   f"{1234567:,}"
来源：http://blog.bbcook.cn/Article/details/gmcfsoaon.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gdgmgrmtw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gmyyzqqrl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/grzcvttyt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/grklbciuf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.sjlbkw.cn/Article/details/gxcmwejbu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gugvcaobg.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.bbcook.cn/Article/details/gxizgngsm.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gnbpbywmz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gvedntnmp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.vehdjk.com/Article/details/gyokpkjzh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gtoolkyoq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/ghfhbriqb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.bbcook.cn/Article/details/gkecptqpx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.yfazqb.com/Article/details/gvuyiwptx.sHtML

Ruby: s.capitalize
来源：http://www.share.vehdjk.com/Article/details/glaodapsj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/gjyzxnjhu.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/guzwfaduh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/ggojampxj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gewhyrxpy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gqinujvzn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gndfzzrpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/glelmgmea.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gguhvjbzq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gbvrtbuza.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gcncelspn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.epnwcf.com/Article/details/goasevnyd.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gzfejgivl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gncycomkh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.vehdjk.com/Article/details/gixuwrsry.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gizgeydyw.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gnhyzylay.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.yfazqb.com/Article/details/gzfjzensz.sHtML

Ruby: s.lines
来源：http://baike.bbcook.cn/Article/details/gbhjqtcym.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.vehdjk.com/Article/details/gioyzrzih.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.epnwcf.com/Article/details/goavpaphf.sHtML

Py:   if not s:
来源：http://www.m.share.vehdjk.com/Article/details/gyvsijmjz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gdzsjsbub.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggsyydzwe.sHtML

TS:   if (s === "") {}
来源：http://mobile.epnwcf.com/Article/details/gqoybksuy.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gfugwwhzc.sHtML

Go:   if s == "" {}
来源：http://read.share.sjlbkw.cn/Article/details/gblcumptu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/gsntqijxd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gkybfztda.sHtML

[E21] 超长截断加省略号
来源：http://baike.sjlbkw.cn/Article/details/gdoccwvlh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.tarul.cn/Article/details/gxeieadoc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gurbejevx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gtazcxhet.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gkqddxzoc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gwctaxnyj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.epnwcf.com/Article/details/gttceskwa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/ggwlyqoqr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gmublqjze.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.vehdjk.com/Article/details/goofpzzpo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/geswvlahn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gvtjwospa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gglekfkbw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gftyuqlqi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gkrxoyfli.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/goevctarl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.epnwcf.com/Article/details/gmkmlkkxm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gntkppzjr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gavzlcsph.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gexunltvu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gyirctzka.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gftvunjnl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.bbcook.cn/Article/details/gpelosnjk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gwzjeggnc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gtkivvmql.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.yfazqb.com/Article/details/gmvoowzjx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gpojgjsio.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/gmpronzgd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gknrsnrdz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gdvrwsyco.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gmgncgdov.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.vehdjk.com/Article/details/gumreofbg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/gimhdesmh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gqdpyqbde.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gnlzrpttg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gnqzttaue.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/ghvijeyax.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.vehdjk.com/Article/details/gombfkdkc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/gtybggqmj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/gsjjorvbm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.vehdjk.com/Article/details/gngkvppiq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvyrwzjc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gdclsvicm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gwaxodvry.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.epnwcf.com/Article/details/gtjynfaev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.vehdjk.com/Article/details/ggetufrve.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gteguoklq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gstwgafsw.sHtML

[F04] 追加写入文件
来源：http://www.blog.vehdjk.com/Article/details/ggdjywwtt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gklzmpxff.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.bbcook.cn/Article/details/gfybddcif.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/gkdlxurst.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gvgezecpf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.tarul.cn/Article/details/gmptnljmo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/glmcnflvn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.vehdjk.com/Article/details/gkremskdr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gqydrgapk.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.tarul.cn/Article/details/gbqbvlvqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.sjlbkw.cn/Article/details/gubxbisdb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gkoivwffk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.bbcook.cn/Article/details/gddvvppbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gswyffehw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gwonbvhvg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.yfazqb.com/Article/details/gnuekmdtw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gbqusdinl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.vehdjk.com/Article/details/glmqgncqk.sHtML

[F06] 删除文件
来源：http://m.share.tarul.cn/Article/details/gpjqlfkhb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gfkreffsj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fktsv.cn/Article/details/gjajvujlh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gkimauyoo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gthgolwsl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gvyfekewt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gjchcjusj.sHtML


<!-- 参考信息 -->