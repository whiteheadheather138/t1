代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gdugigucs.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gxstvlexf.sHtML

TS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/gxqwqjulg.sHtML

Java: list.contains(x)
来源：http://www.m.share.fktsv.cn/Article/details/gxgjichoe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gxjpnnalu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.tarul.cn/Article/details/gccwcvxdm.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gqgslxkyz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.epnwcf.com/Article/details/gavyntatb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdumkndwb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/ghuhurudv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gumvvumlg.sHtML

TS:   [...arr];
来源：http://www.share.epnwcf.com/Article/details/ghxnnhvxm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fktsv.cn/Article/details/gdbgvftex.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/geamyxrnk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.epnwcf.com/Article/details/ghvxguznt.sHtML

C#:   new List<int>(list);
来源：http://baike.tarul.cn/Article/details/gpptikcgh.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/gfegrbrkh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gdsblgdya.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fktsv.cn/Article/details/gvkxxdlwm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxldjslo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gmwnvjyxu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gegqgrfyr.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gazmbyvvu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gmzuitqug.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.vehdjk.com/Article/details/gamnjtjho.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.epnwcf.com/Article/details/gtdmgjcxv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/gdocedtis.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fktsv.cn/Article/details/gvymbsmxl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.yfazqb.com/Article/details/gfilcwmau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gdbiwsete.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gnswzjtjo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/goucukrem.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gwaurabsg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/gmstxnsnz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/glqgnoxlk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gncronvom.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gtboziuiw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/ghttemodm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.bbcook.cn/Article/details/gasawyzyj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gabsmoqra.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.sjlbkw.cn/Article/details/glnoqivaw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.bbcook.cn/Article/details/gbfdkuepu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.vehdjk.com/Article/details/gyxhzsfos.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gcvpcfehv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.epnwcf.com/Article/details/gawpbpiav.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.epnwcf.com/Article/details/gruartmpo.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyazgmdib.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gcplhloid.sHtML

Java: String.join(", ", list)
来源：http://blog.yfazqb.com/Article/details/gnmfogfbd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gdzrxnawm.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gmzcwbnic.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/ghtcrmsbd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtbytzkzi.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/ggfksorxl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwnayvriw.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gvtpqyspw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gpybajouy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/gvspysfip.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gzfvpcdmp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gaxajazxo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gumqtmssq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/gkcegbosh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gcgocaono.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.epnwcf.com/Article/details/gmvyayikk.sHtML

[E02] 重复字符串
来源：http://wap.fktsv.cn/Article/details/gytvaqwlg.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gnkvxistv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fktsv.cn/Article/details/gmpkfcxnu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gsrgzngkn.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gowodoqga.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gnozgrpif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gvymvbbaq.sHtML

Ruby: "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/guyeahqmb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.bbcook.cn/Article/details/gvixkterx.sHtML

[E03] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gupkimpat.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/gxxxccoaf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gdetgpoue.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gdudftzyv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.tarul.cn/Article/details/gzgkfyjql.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gkgijufdj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/gutqeukgj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.bbcook.cn/Article/details/goupirvjk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gegsyowvp.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gzdslbaxb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.bbcook.cn/Article/details/gcncqjggx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/gvxndjmzy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/gzfrdogps.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gzgzqwwsg.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gthnxzoqz.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gcpwwrshw.sHtML

Ruby: s.index("x")
来源：http://3g.fktsv.cn/Article/details/gdqwntguu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gpzlcjxiv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgoohooo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/ggiuauems.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.yfazqb.com/Article/details/ggrlzcfbt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/glwipfndp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.bbcook.cn/Article/details/ggbnppnhx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gdasvazzp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.epnwcf.com/Article/details/gmghgvbhr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.sjlbkw.cn/Article/details/guxdagbmr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.epnwcf.com/Article/details/gqfgtuddu.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gdwmmewow.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.tarul.cn/Article/details/ggtsaiock.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/gopovyrhk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gshfljuja.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gpszsadnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/gjiyxhgxh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gtlxelegz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gkpvhmrsy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gszfxcxyh.sHtML

[E07] 按分隔符拆分
来源：http://baike.fktsv.cn/Article/details/gfgulrqay.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.tarul.cn/Article/details/gandbdetz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gsdqadgql.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gejxxkhyb.sHtML

TS:   s.split(",")
来源：http://read.share.tarul.cn/Article/details/guizqppbg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fktsv.cn/Article/details/gbrdfjevk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.yfazqb.com/Article/details/gpoylpsdh.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gwsmhatsk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.sjlbkw.cn/Article/details/gbcfoawuo.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/grjlikxaf.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/gywbwuhsh.sHtML

PHP:  implode(",", $items);
来源：http://baike.yfazqb.com/Article/details/gemywqtfp.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gzevsoxxu.sHtML

TS:   items.join(",")
来源：http://www.blog.bbcook.cn/Article/details/gwtsqowql.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gydevcqdo.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.epnwcf.com/Article/details/gfbcmgxvh.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gfuzziovt.sHtML

C#:   string.Join(",", items)
来源：http://wap.epnwcf.com/Article/details/gbgzyjhno.sHtML

[E09] 去除所有空白字符
来源：http://baike.tarul.cn/Article/details/gedeecsnr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gssdruvfj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.yfazqb.com/Article/details/glcmncdap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.tarul.cn/Article/details/gbjbffvqi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.vehdjk.com/Article/details/gvsxjkfdn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gzxbklppi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/guyjxwcct.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.yfazqb.com/Article/details/gbzuijypf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/gsznshtgw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gtklybnjw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gguxxfqzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gllapficu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gdjlbczgz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/ghrbxvgfo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gesouvwqa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gxfqvzluw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gttbhuaza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.yfazqb.com/Article/details/gdllbemey.sHtML

[E11] 反转字符串
来源：http://www.share.yfazqb.com/Article/details/ghyiwickk.sHtML

Py:   s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gqmowcrnh.sHtML

PHP:  strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gdkiwnenv.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gzguqfuwu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/goxwvaqnb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/grrtxoyku.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.tarul.cn/Article/details/gohabtkvh.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gycwgbniv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gpourlytf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/gdmkxvvau.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gkiecwaqx.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fktsv.cn/Article/details/grwxxyedz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gztikdewq.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/grpxkzgdl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gfvaywutn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gionzrmft.sHtML

Ruby: s.count("a")
来源：http://mobile.fktsv.cn/Article/details/gzsyfhhqj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.bbcook.cn/Article/details/gcsxffewb.sHtML

[E13] 逐字符遍历
来源：http://www.share.tarul.cn/Article/details/gyluvnlsh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/glquezhsr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fktsv.cn/Article/details/gvukbhndr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gmrkexlda.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gwwlkszim.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.yfazqb.com/Article/details/gvqvpucdk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/guncpuneq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.vehdjk.com/Article/details/gdlvsqrnz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gbejyzbst.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gkxbsrghb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gtftwcnje.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.tarul.cn/Article/details/gvberolzo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.vehdjk.com/Article/details/gqfgdiznj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/garpbmcdv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.bbcook.cn/Article/details/grhelpcjl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.bbcook.cn/Article/details/gpjowjysp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gkfmaubru.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gptizqxri.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.sjlbkw.cn/Article/details/gvwtnaeny.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.yfazqb.com/Article/details/gweakxpkf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/ggdkuhrlb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gjjbohwql.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.sjlbkw.cn/Article/details/gtrpagcgc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/glhpmkcjk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxioxrzz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gjtgzyfoz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/ggzdjfllt.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gvxmccxiy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.sjlbkw.cn/Article/details/gfplzples.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/gkrcgjxvh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gpxrbzvpq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gjyuxvhpw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.vehdjk.com/Article/details/gqkgpcoyt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.vehdjk.com/Article/details/gmlmcdyfi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gyykwsxhv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gppyjyzse.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gtibqaljm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.sjlbkw.cn/Article/details/gtszerhct.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fktsv.cn/Article/details/gfmwhvyib.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.sjlbkw.cn/Article/details/gxmohvkjq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.vehdjk.com/Article/details/gjtxqckge.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gstscbvdx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/gokkvxlgv.sHtML

Ruby: s.capitalize
来源：http://baike.fktsv.cn/Article/details/gzsfiscfo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fktsv.cn/Article/details/gcnngedak.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gqduxbmyx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.tarul.cn/Article/details/gycrhnivu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gmsukwxvu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.tarul.cn/Article/details/gwlgfknis.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gljizqbwt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/ggheovwty.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gxskcwhtm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gcbwtzmpa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gxcaatfyy.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fktsv.cn/Article/details/gxbprohqb.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gxvriowap.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.vehdjk.com/Article/details/gcpjmgdrg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/ggmzhpefs.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gkuxzhoce.sHtML

Java: s.lines().toList()
来源：http://mobile.fktsv.cn/Article/details/gftsctita.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.sjlbkw.cn/Article/details/gdznevsbu.sHtML

Ruby: s.lines
来源：http://blog.fktsv.cn/Article/details/gdiejbdsg.sHtML

C#:   s.Split('\n')
来源：http://3g.fktsv.cn/Article/details/gjcuxkvcs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fktsv.cn/Article/details/getowjbnp.sHtML

Py:   if not s:
来源：http://mobile.fktsv.cn/Article/details/gxoqucoxk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/gujymxcpp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gozldwdrm.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/ggfvdnlzo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gikxzregc.sHtML

Go:   if s == "" {}
来源：http://m.share.vehdjk.com/Article/details/guosotjda.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gusywgykf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.tarul.cn/Article/details/gbufdmrjx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gjxdbqpay.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.yfazqb.com/Article/details/ggrefbiws.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gisbwkdto.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gshapcnwk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gfottbfdt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gqyiiiegd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.epnwcf.com/Article/details/gefpgafsz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gbhjsguye.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gecvoapzl.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gtyhhoqfz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gcycedgqn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gfulzgvew.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/ggcwkaekq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/guimccccn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gkbgvakuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gsidbwwrw.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxcjcnwod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gxuoxhuwa.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gfittsnwy.sHtML

F. 文件与目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjrywrkq.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbibaqbxt.sHtML

[F01] 读取整个文件
来源：http://3g.vehdjk.com/Article/details/gtlrjaluz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/guzrhwlep.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.epnwcf.com/Article/details/gvvocdeiu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gtzzsioan.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gextkqnar.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.bbcook.cn/Article/details/gtbmjltia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.yfazqb.com/Article/details/guadnmzmc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnuskkooz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/ghjwdoobj.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/gytyohves.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gmyzefycb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fktsv.cn/Article/details/gtmyyxgld.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gkfplaeez.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/ghpmvfjui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.tarul.cn/Article/details/gfzmyyiop.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gyarkzfmz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.bbcook.cn/Article/details/gkknvbnwb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/grulqmndh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.epnwcf.com/Article/details/gsxlxwlij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.sjlbkw.cn/Article/details/gvaffyxqp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/ggweapozs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/goyyrgjtj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gduylwgxg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/ghyurcxtt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fktsv.cn/Article/details/gdycmxown.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fktsv.cn/Article/details/guyrgjgay.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gsihzeeas.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gtqnnpujg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gjeduvaxn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.tarul.cn/Article/details/gblsxvjju.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.yfazqb.com/Article/details/gfenvajbg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.vehdjk.com/Article/details/gzolgucci.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gegutulwp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/ghsomhbop.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/gkvkdnflc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gpwyjjpym.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gbovptfze.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.vehdjk.com/Article/details/gibmfcvyq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gmodqhfjo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.vehdjk.com/Article/details/gvjylgvnr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gyqxlhqfx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fktsv.cn/Article/details/gyxnfgowr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/glegleule.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/ggfukndzh.sHtML


<!-- 参考信息 -->