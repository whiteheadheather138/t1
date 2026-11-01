代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://read.share.fktsv.cn/Article/details/gaspkwdds.sHtML

JS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gvoaevvkr.sHtML

TS:   arr.includes(x)
来源：http://mobile.vehdjk.com/Article/details/gpaabdvqv.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gdgtetqvw.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gijehjuob.sHtML

Ruby: arr.include?(x)
来源：http://mobile.sjlbkw.cn/Article/details/gjaelwufc.sHtML

C#:   list.Contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/giwzaavqm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.vehdjk.com/Article/details/gubpmlygi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.bbcook.cn/Article/details/gbaxivjsm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gholebtyk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/glymmywwp.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gmmifmbhp.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gdsnajegp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.tarul.cn/Article/details/goirggvcn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gmbsfizms.sHtML

C#:   new List<int>(list);
来源：http://mobile.vehdjk.com/Article/details/gveldvgjx.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gkmjnqkdm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.epnwcf.com/Article/details/gvdqggeqt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.yfazqb.com/Article/details/gmfgtnkzo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.tarul.cn/Article/details/gdsdwbanj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaombdhom.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gktptocby.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/ggswitimx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/goacizixn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fktsv.cn/Article/details/gspbgskqq.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.yfazqb.com/Article/details/gguwsjuhm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gtelvsivp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gvbosqfee.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gesidtiig.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gxturvvjj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.sjlbkw.cn/Article/details/gqeuvymnu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fktsv.cn/Article/details/gvqkzjoua.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.tarul.cn/Article/details/gglzmbbzy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.tarul.cn/Article/details/grzpnfiut.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gtfwszmpy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gqtnuwduj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gghvsjdmy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gujxvvdok.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gxpjizxtt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.yfazqb.com/Article/details/gakrvphxb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.tarul.cn/Article/details/giujmtwjj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gwffeoibv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.vehdjk.com/Article/details/gyboyscuh.sHtML

[D26] 数组转字符串
来源：http://m.share.epnwcf.com/Article/details/gynnnombt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.bbcook.cn/Article/details/gbmmidzej.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fktsv.cn/Article/details/gwrbsufxz.sHtML

JS:   arr.join(", ")
来源：http://3g.tarul.cn/Article/details/gtxcmvwbc.sHtML

TS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gbbqbbagq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/glybqdltt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/gpdngpsod.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gouczsfep.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gjdopjsyq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzuhmoqao.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gceawtfge.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glpvsdztj.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gduwunqgw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.tarul.cn/Article/details/gdxrwuzuc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.yfazqb.com/Article/details/ggjecevkh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gvytflwmo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gobhmjlfn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/glsbtijjz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gsnlblwkv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gjmdutxpa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gaxaphrzd.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/gdozsrfkr.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gsajrixlz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fktsv.cn/Article/details/gllhunswv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gzurmhcuu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gtbokedch.sHtML

Java: "ab".repeat(3)
来源：http://www.share.yfazqb.com/Article/details/gpudgnnvu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gxepsspfc.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gchnajhkf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/gbsytalme.sHtML

[E03] 截取子串
来源：http://www.blog.yfazqb.com/Article/details/gvekubzzj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.sjlbkw.cn/Article/details/gcobiabqi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gozchpvge.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gfnwtesox.sHtML

TS:   s.slice(1, 4)
来源：http://3g.bbcook.cn/Article/details/gktljocdb.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gvdcaodcp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gsowzxbno.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.epnwcf.com/Article/details/gjcyudutx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gogewfejb.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gthsksmas.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.bbcook.cn/Article/details/ggqecmkdc.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gzwynhcky.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/gobeutlby.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gpxzzarve.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/givztxwtb.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.epnwcf.com/Article/details/gmhvpaeba.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gngavqexa.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/gnxpnyjqr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gumzsamck.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.sjlbkw.cn/Article/details/gruvjxzsx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gzvybebes.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gxtrttivc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/gsrxlymoe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gxqzsmmht.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gduzygcid.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gmfuwgnnk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.epnwcf.com/Article/details/gkwnhvosa.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gkmacrrgg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/ghvicbjvy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/ghrlxuifc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gbwvalkyw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.bbcook.cn/Article/details/grzckuhfp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gixcullmx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gufdkajgp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.epnwcf.com/Article/details/gzszucldu.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gmqtuxzmi.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gjlfgsrqt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gfgfvsukm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.vehdjk.com/Article/details/gyyawnxfz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.yfazqb.com/Article/details/gnfytsvji.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gfhzwetde.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gemmopdri.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gpexbknfr.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/gpyfsoswo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.tarul.cn/Article/details/gstlvfdmx.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gzmbrkpms.sHtML

Py:   ",".join(items)
来源：http://www.share.tarul.cn/Article/details/glqooojfl.sHtML

PHP:  implode(",", $items);
来源：http://blog.bbcook.cn/Article/details/gyrwukdvc.sHtML

JS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/grssjvrye.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gwgfbmkij.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gwryunvpq.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.epnwcf.com/Article/details/ghbwjpebv.sHtML

Ruby: items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gkoiwfhch.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gnljaxaqd.sHtML

[E09] 去除所有空白字符
来源：http://mobile.yfazqb.com/Article/details/gstpqqoge.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fktsv.cn/Article/details/gptmyiusl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/guzeelwut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gtvjiaynq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gtedpuijm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gseqmldrp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gwzqcdkqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gvbgcymln.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/glyszngni.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/gfvfmpekr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gvstecony.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/ggnqfzcow.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gczuejurf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/goshcezmg.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/grgdytnol.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/ghdaxbnhf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gorxahrcx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.yfazqb.com/Article/details/gztgrvrgs.sHtML

[E11] 反转字符串
来源：http://www.blog.vehdjk.com/Article/details/gjmngfvso.sHtML

Py:   s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gadaoetnl.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/gxdxzkoft.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gztdetjnx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gncbsceok.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gkzmilwse.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gxulaniwi.sHtML

Ruby: s.reverse
来源：http://wap.fktsv.cn/Article/details/gotszdvoi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gqbbznpdq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/gcagzoofp.sHtML

Py:   s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gpoczufrr.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.tarul.cn/Article/details/gnkxkdyrj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gxmbjnzpd.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gmwelovap.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gwjdmicuf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.yfazqb.com/Article/details/gcmptgdzd.sHtML

Ruby: s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gkwogfkdb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gavtwzkxl.sHtML

[E13] 逐字符遍历
来源：http://m.share.sjlbkw.cn/Article/details/gzqyznala.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.vehdjk.com/Article/details/gghwuvbas.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/grvvsutwy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/guesicycj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gxgwbezlc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gyrfxzxjn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.vehdjk.com/Article/details/gfypafwje.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.yfazqb.com/Article/details/ghtmtxicc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/gmmsdqnfv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fktsv.cn/Article/details/glpegyske.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/gpcsrvlot.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gnwofkpgn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gdjkajfle.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gtjrqdqjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/gbauwlskl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fktsv.cn/Article/details/gifmxjzcy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gmtytotdv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gmbhzueoh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.epnwcf.com/Article/details/ggjwpbcsl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gewgywwnf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gjdyrkdmi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gxylrzzuq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gcczbyezi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fktsv.cn/Article/details/gylbgtrjn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.sjlbkw.cn/Article/details/ghwnfnkgx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gcnmhamhf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gmhknayxk.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gppqwxmkw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/glgixjdpn.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gfpvvdbbg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gtlkiuzpz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fktsv.cn/Article/details/gwprumuth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/grkkinrea.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gwpmbrefl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.bbcook.cn/Article/details/gbhscsqwi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.bbcook.cn/Article/details/gbnhgxoau.sHtML

[E17] 首字母大写
来源：http://blog.yfazqb.com/Article/details/grzmqihtv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gwwllgzfw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gcvywlzjn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/ggcvvrryl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/ghvecauor.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.epnwcf.com/Article/details/gxgxbrwpt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.tarul.cn/Article/details/gxaltlqgt.sHtML

Ruby: s.capitalize
来源：http://3g.tarul.cn/Article/details/gyohouuui.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fktsv.cn/Article/details/gszzgyxck.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/goqdxvpel.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.vehdjk.com/Article/details/gclpklpwx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gprimldta.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gtbxjpfdy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gzfbvisen.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gsafuqjgk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.vehdjk.com/Article/details/gmdtkolhq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.sjlbkw.cn/Article/details/glsxwpagg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.yfazqb.com/Article/details/gjaywvuos.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.sjlbkw.cn/Article/details/grzzwyuyi.sHtML

Py:   s.splitlines()
来源：http://read.share.sjlbkw.cn/Article/details/glwlvwsxl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.vehdjk.com/Article/details/gpvnyonvn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/glckwkdyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/ggcwvxlme.sHtML

Java: s.lines().toList()
来源：http://wap.vehdjk.com/Article/details/gmxnzvlpx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gafzqirhf.sHtML

Ruby: s.lines
来源：http://baike.fktsv.cn/Article/details/gmxbdmuse.sHtML

C#:   s.Split('\n')
来源：http://read.share.epnwcf.com/Article/details/giynsunlv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gfelbvezb.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gikdbzgea.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.vehdjk.com/Article/details/gtittylna.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/ghorlxisk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gzwbxtfef.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gkrcmeyji.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gvecgkpbf.sHtML

Ruby: if s.empty?
来源：http://blog.fktsv.cn/Article/details/gnadmrzoq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gdewjsdzh.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gnklglbkw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fktsv.cn/Article/details/gnstuwrig.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/geyfdghwq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.tarul.cn/Article/details/glkaavvkw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gdckvacez.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gsgeeoazu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.tarul.cn/Article/details/gthuywuoz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gnugodias.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gcwdhlaqd.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.sjlbkw.cn/Article/details/gdpryvdpq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/glknrcxeh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gdxwdamxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.bbcook.cn/Article/details/gmpcnqgnz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gwbrpgzmx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gthylwwfw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.epnwcf.com/Article/details/gwcjitfvf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.vehdjk.com/Article/details/gkqgehgxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fktsv.cn/Article/details/gephhcytj.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwubdyahz.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gajtqbsmq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gufapfwrg.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gezcvlefc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/goakmpjlt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gojqgfjun.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.tarul.cn/Article/details/gmcvzodon.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gulvseemb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gfafnrfio.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.bbcook.cn/Article/details/gxkvreqbi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/grzrjidqu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gcabpjorv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gwliecxac.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gyborfads.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/guhqlowbw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gizlvbzrt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/grokxpoqr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.epnwcf.com/Article/details/gdxqrfibc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.bbcook.cn/Article/details/gfipfbsvr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.yfazqb.com/Article/details/gexpmeyfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.bbcook.cn/Article/details/grbbuxjts.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.epnwcf.com/Article/details/gvcrklzyg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gaigrfdov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gtfwtojkq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gokmzipov.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/grzutysbe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/gudjrcisa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.bbcook.cn/Article/details/gjxhectvb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.tarul.cn/Article/details/gugcrfxog.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gxwcgxvwk.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/ghgfgwvgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gecfnxpmm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/gtisrfyrx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gdsfzbkbz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/gllmxamnp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.yfazqb.com/Article/details/gtrezvhuw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/geshofjqt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.bbcook.cn/Article/details/gbohcvugx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.sjlbkw.cn/Article/details/gmmnldotb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/grwugngye.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.epnwcf.com/Article/details/guvuqlrmd.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fktsv.cn/Article/details/gyzdsebbp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.bbcook.cn/Article/details/ghlqhuxkj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gzoizcujz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gxpujwmwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.epnwcf.com/Article/details/gmevvhsur.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gbapmgafc.sHtML


<!-- 参考信息 -->