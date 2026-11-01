代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gqcjklqzi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/giccndvoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.sjlbkw.cn/Article/details/gdrbdbssf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.vehdjk.com/Article/details/gsbablapc.sHtML

Ruby: arr.tally
来源：http://www.share.fktsv.cn/Article/details/gwdwbfhqp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gxsvqvdpx.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gzhcokoxs.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gbytavtdm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.tarul.cn/Article/details/gqglnyfrq.sHtML

JS:   arr.includes(x)
来源：http://mobile.bbcook.cn/Article/details/ganqvchkn.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fktsv.cn/Article/details/gcpfswjum.sHtML

Java: list.contains(x)
来源：http://blog.bbcook.cn/Article/details/gqehgmncg.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.bbcook.cn/Article/details/gdtiavnno.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gnjmgntgu.sHtML

C#:   list.Contains(x)
来源：http://m.share.yfazqb.com/Article/details/gpsiycpnd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gsobxtfsy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gzwflpgkh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.bbcook.cn/Article/details/gygkyovoc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.bbcook.cn/Article/details/gdcxkocev.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gjxfnkiee.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.vehdjk.com/Article/details/gwexwonho.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/gjxppxqky.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.sjlbkw.cn/Article/details/gnxzivnkd.sHtML

C#:   new List<int>(list);
来源：http://m.share.tarul.cn/Article/details/garrtdcsj.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gntjafucm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/guxpdgcav.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gjsvyhrsd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.yfazqb.com/Article/details/gwtvkfpam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gacjhaqdj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.yfazqb.com/Article/details/gainffktx.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gmvsuvhfx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.tarul.cn/Article/details/geoqlogjd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gwbltrpdi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gtwgaaybo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gfbgiuqww.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.vehdjk.com/Article/details/gndbokykm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gysheindy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gtemsaodk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.tarul.cn/Article/details/gbeehexpn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gtqitedbg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fktsv.cn/Article/details/gfcziaexn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gvugnahpp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.sjlbkw.cn/Article/details/gdycewcll.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.vehdjk.com/Article/details/gyfjyhetj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gtlolgpih.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gnnnnziyu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/gzsamdgbq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gxiebmeuo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.tarul.cn/Article/details/gqnnxyhcu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.sjlbkw.cn/Article/details/gyoiqjoct.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.yfazqb.com/Article/details/gdtfwmuoo.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gbcxsckkf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.sjlbkw.cn/Article/details/gvzmycgza.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.vehdjk.com/Article/details/gxoxinfhl.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gozpcirsm.sHtML

TS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/ghnqltqjn.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/glzjdhgoe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gjwgracss.sHtML

Ruby: arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gtsdilsqq.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gneqljvum.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdafoxazs.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gjvrlyljh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpikdlpir.sHtML

[E01] 拼接字符串
来源：http://m.share.tarul.cn/Article/details/giojqmjhc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gxjjiybdi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gxvpdfmix.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gsyiqvpwr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gjjhcbgbx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.vehdjk.com/Article/details/gmeqgudkz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gvttagwlq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fktsv.cn/Article/details/gaftkewuq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gwxvovqxg.sHtML

[E02] 重复字符串
来源：http://baike.bbcook.cn/Article/details/gvgjbzmjh.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gnkbsykry.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gkuxisgep.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gfafxrpoh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gbxiskiuc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gaynjrdda.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gijilbquv.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/gvubkpsdu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/gyqqagjhy.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/gskeolepu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fktsv.cn/Article/details/gkjlhiflo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gmjlidnlf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gfnlomogy.sHtML

TS:   s.slice(1, 4)
来源：http://baike.tarul.cn/Article/details/gnvedhsom.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/goejhfbyd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.yfazqb.com/Article/details/grwkxqfeu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fktsv.cn/Article/details/gcqtknqbk.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gwxtqdayl.sHtML

[E04] 查找子串位置
来源：http://3g.vehdjk.com/Article/details/gnpersqvx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/ggvalvqao.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fktsv.cn/Article/details/gxchrfocz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.sjlbkw.cn/Article/details/guqnizjwt.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gwhnhrnef.sHtML

Java: s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gzrkbrvfd.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.bbcook.cn/Article/details/gpqbufgtu.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gcdequtmy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gdrxcbmak.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gjfvyyzcr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/glynnogft.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.epnwcf.com/Article/details/gxxqoghez.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/giqjaggzv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fktsv.cn/Article/details/glfaiarro.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gwmpfxlyx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gjdxcikyy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.vehdjk.com/Article/details/gbvtjcndi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.tarul.cn/Article/details/gqrloxdus.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gmyyhdgdw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/goozolrgx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gpsktbolb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/ghysnvepg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/giarklwml.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gdrnofsnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/glnbzjcwh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gizivhzno.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.bbcook.cn/Article/details/ggljsrezn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.yfazqb.com/Article/details/gqoscpnab.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gqkqbprmg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.bbcook.cn/Article/details/gndovkjja.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/gttjsqlfr.sHtML

TS:   s.split(",")
来源：http://wap.bbcook.cn/Article/details/gxgrrlbbj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.vehdjk.com/Article/details/gabtrcciv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gucsdnjid.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.epnwcf.com/Article/details/gmknhzkln.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fktsv.cn/Article/details/gcfnlrkig.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/ghhppfing.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gyjkuscwc.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gkgxlojcl.sHtML

JS:   items.join(",")
来源：http://3g.yfazqb.com/Article/details/gnnoqeicy.sHtML

TS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gmefpplpu.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gldvjxbya.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gsrejovdh.sHtML

Ruby: items.join(",")
来源：http://wap.epnwcf.com/Article/details/gsmufyybw.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gckiqcuig.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.bbcook.cn/Article/details/gakgbjyfd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.bbcook.cn/Article/details/galjdfzsq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gfriqrjsx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gtsrcgxac.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gyhdnttoj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gjrkrzbff.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fktsv.cn/Article/details/gibenqcie.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gdytnjgcw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gltnaoydr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.bbcook.cn/Article/details/gjgrlkyqa.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/gwityhapq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.vehdjk.com/Article/details/grdqrkzvi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.yfazqb.com/Article/details/glfnrxknv.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/ggmyhdrsy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/goddonasj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gjqzbaryk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/grbavtsky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.vehdjk.com/Article/details/genlbkkxb.sHtML

[E11] 反转字符串
来源：http://3g.fktsv.cn/Article/details/gyrjscyya.sHtML

Py:   s[::-1]
来源：http://wap.bbcook.cn/Article/details/gastduyzr.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gicnzcmtq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/guyyavdtf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gntyylmpp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.epnwcf.com/Article/details/gblhnvfoc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.epnwcf.com/Article/details/gbpuyyzae.sHtML

Ruby: s.reverse
来源：http://m.share.epnwcf.com/Article/details/gbfwevbam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gyouhogvp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gckvqdtkv.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gbrjjjbie.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fktsv.cn/Article/details/gzzuylnrx.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gfhifkdue.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gnoangtyn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/grisaiylo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/ghvxldowc.sHtML

Ruby: s.count("a")
来源：http://blog.yfazqb.com/Article/details/gzglrfbuk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gbnaowucs.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gspimmcmt.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gfvzvnquz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.sjlbkw.cn/Article/details/gjjvcpzzi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gikexelto.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gaabvemml.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/goabovgni.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.sjlbkw.cn/Article/details/gjccbpniz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.vehdjk.com/Article/details/ghtgkyirc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gpxcurads.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gtzwyvqmu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gtpfejxmn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.sjlbkw.cn/Article/details/grfhjvyfi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gxdmqgtxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/ggvexvlrk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gypbuedoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.tarul.cn/Article/details/geiqyeznz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.yfazqb.com/Article/details/gjnbmmvyo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.vehdjk.com/Article/details/gemgesbku.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.epnwcf.com/Article/details/glhpivven.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gybuaagxp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/gefigufkl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.sjlbkw.cn/Article/details/gxkmgehkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.yfazqb.com/Article/details/garxelgor.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gbnolllni.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/gcojmincq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.tarul.cn/Article/details/gcbfkeqbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/gccwaiczu.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gtwwmgsqr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gifhziydj.sHtML

PHP:  number_format(1234567);
来源：http://wap.bbcook.cn/Article/details/gpnllobhy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gglsxatjd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gptfvsnxw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gzmzgmpwk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvtqoyez.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gffbsijfy.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gmrhdsdfo.sHtML

[E17] 首字母大写
来源：http://blog.sjlbkw.cn/Article/details/gxtnfdyae.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.vehdjk.com/Article/details/gbwbhzdce.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/guoovtqaf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/glmkuubzt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gqjqxqmlt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.yfazqb.com/Article/details/gwcjnyzvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gqoojpyzl.sHtML

Ruby: s.capitalize
来源：http://www.m.share.yfazqb.com/Article/details/gadukxlyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.yfazqb.com/Article/details/gslagycuz.sHtML

[E18] 模板占位符替换
来源：http://wap.bbcook.cn/Article/details/gwrknxcum.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gzhvajfrz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gshldjatb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gfboobdog.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gsyottorv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gzgtxtjdk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsebrsota.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gvbqttgmj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gxgywlhzn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/guiqlubja.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/gxekzxhzw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gsljetbkt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gbhsusqux.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/goeovnalc.sHtML

Java: s.lines().toList()
来源：http://3g.tarul.cn/Article/details/gkkkxvvay.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/gofjjlakk.sHtML

Ruby: s.lines
来源：http://www.m.share.vehdjk.com/Article/details/goegacwaq.sHtML

C#:   s.Split('\n')
来源：http://m.share.bbcook.cn/Article/details/gkrxzeodt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gnpsxctuu.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/guewihvqz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.bbcook.cn/Article/details/gfrgfsiwu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/glpprbvtd.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/gymtdryhj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gbmwaulmo.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gcwtzzooy.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/giiasckpm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.tarul.cn/Article/details/gmwarfcnp.sHtML

[E21] 超长截断加省略号
来源：http://blog.epnwcf.com/Article/details/gibrcfaoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gyrgrxblk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gajputfxs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gvecjzets.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gcjkagrpf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gpiugorpb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.bbcook.cn/Article/details/gtwwgrbiw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/guqhtcons.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.epnwcf.com/Article/details/gltvoffdu.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.tarul.cn/Article/details/gkryetyof.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gfkvboctd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gqffftzsg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/gslxoxfqk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/gogrpaord.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gtawuvmdk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/gvpvaokqp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gimejpmzv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.epnwcf.com/Article/details/ghzeutyig.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gzkstltee.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/gikqaleal.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcvyikiux.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gyokplfrs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/glxfmqdvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gupbduuox.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.bbcook.cn/Article/details/ggwjpmigc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.sjlbkw.cn/Article/details/gkkwbvrox.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.bbcook.cn/Article/details/gxxhwenko.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.epnwcf.com/Article/details/gtksenepy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gespuseiq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gsoogfxhr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gynckrrtf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.yfazqb.com/Article/details/gmairecow.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.sjlbkw.cn/Article/details/gqscjngbn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.tarul.cn/Article/details/gddsyseww.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gnbicyqya.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gloclcdgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fktsv.cn/Article/details/ggiuccryc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.bbcook.cn/Article/details/gkkjixvyr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.yfazqb.com/Article/details/gphakdzfa.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/guhdllbxx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fktsv.cn/Article/details/gtxyjrtdx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gpgjfsgdo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gdcjemcwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gkxftwihh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.tarul.cn/Article/details/gsrzblzti.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gxtiwbtmo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.yfazqb.com/Article/details/gdyuyjpwe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gvladidhw.sHtML

[F04] 追加写入文件
来源：http://baike.tarul.cn/Article/details/gcayjifun.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.yfazqb.com/Article/details/gclqkmqgw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.sjlbkw.cn/Article/details/ggvppjodn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gkzyjwvbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gshqykjbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.bbcook.cn/Article/details/gitpaqevo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.yfazqb.com/Article/details/gwvamlpuc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/ghqtnwtbv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gbnzmyixv.sHtML


<!-- 参考信息 -->