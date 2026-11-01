代发 wailian999

Ruby: arr.tally
来源：http://www.blog.epnwcf.com/Article/details/gbmupwlvm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gifgjwxnr.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.sjlbkw.cn/Article/details/gcsdnyvws.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gpvpmpuuj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/gfgqswprp.sHtML

JS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/grgklqcmr.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gdyhwdups.sHtML

Java: list.contains(x)
来源：http://wap.vehdjk.com/Article/details/guzzjmblo.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gbblqnqxv.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gqkiwoxok.sHtML

C#:   list.Contains(x)
来源：http://mobile.yfazqb.com/Article/details/gsfslsouw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.sjlbkw.cn/Article/details/gsynuzapd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.epnwcf.com/Article/details/gbbmedasx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gpdudsmkn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.bbcook.cn/Article/details/gduywypsr.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gbvylyhml.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gcnnquptj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fktsv.cn/Article/details/glrzmmjvm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.vehdjk.com/Article/details/gveksbfzy.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gagmkxxqp.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gjjajslqh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.bbcook.cn/Article/details/goocwwpzt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/gqqrkswsf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gstqosoqk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.epnwcf.com/Article/details/gzcpejzpg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.vehdjk.com/Article/details/gdbfdbpcc.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gsreboxko.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.sjlbkw.cn/Article/details/gmdscpwnj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gxpkxpcim.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/gdxlviyai.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.yfazqb.com/Article/details/gsfskmrwt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gtnzvhtor.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/goanimkwp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/gpcsoleru.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fktsv.cn/Article/details/golkdxxmn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gobvwhojt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/gwayfgahp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.epnwcf.com/Article/details/giegdenjm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fktsv.cn/Article/details/gpzschaca.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.sjlbkw.cn/Article/details/gykrzowfn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gqaehdgit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fktsv.cn/Article/details/goqikbycu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.yfazqb.com/Article/details/gxtpdffun.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.epnwcf.com/Article/details/gtfhfidrl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/gvyepahvz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gvfiswyxn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gqyaiuomh.sHtML

[D26] 数组转字符串
来源：http://m.share.vehdjk.com/Article/details/gpnasclsy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.sjlbkw.cn/Article/details/guiaqqocl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/glylotash.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/grzqtjuki.sHtML

TS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gfbahltdl.sHtML

Java: String.join(", ", list)
来源：http://read.share.bbcook.cn/Article/details/gfpdkmtkn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gjrubqfoo.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gevcxvkwh.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/giiqhkjku.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyzwukjzj.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gmbxzxbwt.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpcmkcews.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gmseoardy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fktsv.cn/Article/details/gxrwowjwo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fktsv.cn/Article/details/gxhvrlvyh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.tarul.cn/Article/details/gvjsfzaeq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.epnwcf.com/Article/details/gvsfpsdly.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fktsv.cn/Article/details/gavnqwdun.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gnxmrlttn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gbudcwkiu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.tarul.cn/Article/details/gmlcqgcqn.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gkvdfcwkx.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gihgjqixf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gyafolgka.sHtML

JS:   "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gbcssvvqm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gtcldnann.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/gggyuedlf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gfkedijzu.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/grjczdndb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gjxzzgvye.sHtML

[E03] 截取子串
来源：http://www.share.yfazqb.com/Article/details/ghfohxsur.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gdsorshvp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/giyhkzpuz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gsndvjyof.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gzcdnikgf.sHtML

Java: s.substring(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/gxakdhgla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/gtbvlnaoi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/gfamjtuar.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gzijxtnca.sHtML

[E04] 查找子串位置
来源：http://read.share.vehdjk.com/Article/details/gopbcoqxp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/glzdeiazi.sHtML

PHP:  strpos($s, "x");
来源：http://blog.epnwcf.com/Article/details/garaqqxrp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fktsv.cn/Article/details/gxvigfnqs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/grkbnklhp.sHtML

Java: s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/gzieepydd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.vehdjk.com/Article/details/gnrwhcelm.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gvhwpxeif.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gqkzdkbxe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/ggxhdjwnw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gjfidvzrb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.tarul.cn/Article/details/gdnrvccib.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gpccjvcqk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gvxuzahtm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gsyytjlsu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/gxfyqkojw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gbhlsdxkd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/gsebzqmcu.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/ggvwpgffu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.tarul.cn/Article/details/ggbqlcgou.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.sjlbkw.cn/Article/details/glfymzzhi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gstyjlbgi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gtzlmwmhg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gilxptkvv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gbmulvxsl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.tarul.cn/Article/details/ggcwccgtq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gnrbgally.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gsjyszqjb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/ggjzapwrc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gcoqmcerk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/giittymav.sHtML

TS:   s.split(",")
来源：http://m.share.vehdjk.com/Article/details/gjzsrotgl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.vehdjk.com/Article/details/gsynxkmfh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.epnwcf.com/Article/details/glulisscl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fktsv.cn/Article/details/gmsexlvhi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gjqhlfjje.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.bbcook.cn/Article/details/gbimknbjh.sHtML

Py:   ",".join(items)
来源：http://baike.tarul.cn/Article/details/gdtojxkev.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gcebjoorq.sHtML

JS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gilytxeuk.sHtML

TS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gwbotzcck.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gdnitvahu.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.bbcook.cn/Article/details/gpfosekyp.sHtML

Ruby: items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gckwotsvy.sHtML

C#:   string.Join(",", items)
来源：http://mobile.tarul.cn/Article/details/gdczgcxcf.sHtML

[E09] 去除所有空白字符
来源：http://read.share.bbcook.cn/Article/details/gtkyxrpmj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.yfazqb.com/Article/details/grqsswymu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gvcjzyypx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.yfazqb.com/Article/details/gbhkldpyl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/gbjlxlnte.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gonhbexio.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fktsv.cn/Article/details/gxvmiobiz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gyvsnfncs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/ghtenaovv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.tarul.cn/Article/details/gkjnrjdeh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gulgcuche.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.tarul.cn/Article/details/gwuakqncw.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gaywqnozs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gmwmbovxo.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gzhwzckmn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.sjlbkw.cn/Article/details/gceyqmwlo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gcbpehoxo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gpdhppycg.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/ggmmthagf.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gauyggvtp.sHtML

PHP:  strrev($s);
来源：http://read.share.tarul.cn/Article/details/gajfgiobj.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gzdwtsakx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gytiesmpd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.sjlbkw.cn/Article/details/gdaqvrsti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gdmleyvjg.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gbfqvbvol.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gtnwabnba.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/ghygbgxkm.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gfqkqcswl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fktsv.cn/Article/details/gmhdaovcg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gmlhaghqd.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gtyazsbhs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.epnwcf.com/Article/details/garvistlv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gljzimkdi.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gbwyrswee.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.epnwcf.com/Article/details/glxlmoqmo.sHtML

[E13] 逐字符遍历
来源：http://blog.tarul.cn/Article/details/gafvjulvm.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/goelnrdtn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/grwwoiaxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/grztrbbfq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gnbxrmeki.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/gzotgjwtn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.yfazqb.com/Article/details/gkymnpada.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/grxrdlfxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/gjrkkamkj.sHtML

[E14] URL 编码与 Base64
来源：http://3g.yfazqb.com/Article/details/gurakglja.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.vehdjk.com/Article/details/gavxkacae.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fktsv.cn/Article/details/gtyufbend.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/ghvtbmwaf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/ganndkfvp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/giifhbwjw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.sjlbkw.cn/Article/details/gevumbehe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.yfazqb.com/Article/details/ggypiyvdg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gikxycips.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gsndifltt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gklfsopfg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gcbpjatlc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/glytwduer.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.yfazqb.com/Article/details/gnqwkwkcy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/ggszqzcxn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/gyirykfbi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.tarul.cn/Article/details/gxwewhuee.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gchycnevk.sHtML

[E16] 数字千分位
来源：http://m.share.yfazqb.com/Article/details/gjtaxefee.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gpgrhuagb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.bbcook.cn/Article/details/ghihwmsib.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gteyqdpmp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gzuvujsfq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.tarul.cn/Article/details/gzavuoxzs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gybudyxmr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.vehdjk.com/Article/details/gsxllhnld.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fktsv.cn/Article/details/gixvidvli.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gvtipkcny.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.epnwcf.com/Article/details/gkdontrym.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.tarul.cn/Article/details/gpmcbbapk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.yfazqb.com/Article/details/gdzpbjhgl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gqhlphfxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gvctgezhz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.tarul.cn/Article/details/gbsgscrqv.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/gqsdmohdj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.tarul.cn/Article/details/gqudbsjyk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.yfazqb.com/Article/details/gfoxumhcg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fktsv.cn/Article/details/gnqfqrluu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gtuudbgnz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gdtbdhkss.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gemeclnrn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gdxaqhzwj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gdxwwzaha.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.sjlbkw.cn/Article/details/gqauvpoew.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.yfazqb.com/Article/details/givplfcwd.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/grwpgcnro.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gfnminetu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.yfazqb.com/Article/details/gcmtmoqhr.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/ghcyxzqin.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gisftexlb.sHtML

Java: s.lines().toList()
来源：http://m.share.bbcook.cn/Article/details/gyjsqqnjp.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/griwzonty.sHtML

Ruby: s.lines
来源：http://www.m.share.yfazqb.com/Article/details/guqevbgid.sHtML

C#:   s.Split('\n')
来源：http://mobile.vehdjk.com/Article/details/glkewqwiq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gubdsbaqx.sHtML

Py:   if not s:
来源：http://baike.epnwcf.com/Article/details/gpenqcwgp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gvxglwcnx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/ggwruumje.sHtML

TS:   if (s === "") {}
来源：http://www.share.vehdjk.com/Article/details/gxzvyvxph.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gfvheqxcm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gcgcxfppj.sHtML

Ruby: if s.empty?
来源：http://blog.vehdjk.com/Article/details/guakwrkgf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.tarul.cn/Article/details/gzbcweeyp.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/ggfhmommo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.vehdjk.com/Article/details/gxxdkndmr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gbehcstks.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gbgtanwxz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gvamblngz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gisbbvjeh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gwqrlttzc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/grrjtkphr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gvrhodzta.sHtML

[E22] 字节长度与字符长度
来源：http://3g.yfazqb.com/Article/details/grntvuwad.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gspdhhkdk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gawcutrtu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fktsv.cn/Article/details/gcptlucuh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gdlldwkao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gdgapuofp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gudfxemey.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fktsv.cn/Article/details/gmukdbjss.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fktsv.cn/Article/details/gxkqtnoti.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gifkqagfn.sHtML

F. 文件与目录
来源：http://www.blog.yfazqb.com/Article/details/gyzoabmox.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdjzitcni.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/gtxyqhugc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fktsv.cn/Article/details/gnmtkvxnk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gojgjqknl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.epnwcf.com/Article/details/gaafkfael.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/gtltjvmci.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gcptxshzh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gcaxyskzs.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gldlzvtpi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.bbcook.cn/Article/details/gwpyvfgsl.sHtML

[F02] 逐行读取文件
来源：http://www.blog.yfazqb.com/Article/details/giobmxejo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gdpwbjbus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/gxmlciagy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gvqulnjye.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gjxmekgjy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/grrmpinql.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.epnwcf.com/Article/details/gewyqugqv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/gyduxrnoq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gsvdsdixd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.sjlbkw.cn/Article/details/gjgtafhpp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/geulebyhd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.vehdjk.com/Article/details/gjslohqxf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/greifpwtz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gsoxedvtw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gutzuhohi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/gwgahxqqa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gztrovteu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fktsv.cn/Article/details/guznzhstt.sHtML

[F04] 追加写入文件
来源：http://mobile.bbcook.cn/Article/details/geyazemxp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gautbvjbd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gyqthnlxh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/gfvjwhorc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fktsv.cn/Article/details/gxixggriy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/ggjvcwnww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.vehdjk.com/Article/details/gaihmgyqn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.vehdjk.com/Article/details/ggzbahkiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/geuuctjag.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gxhyrzocz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.bbcook.cn/Article/details/godthcrqd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gsdcbfaen.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvubgmhfu.sHtML


<!-- 参考信息 -->