代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.epnwcf.com/Article/details/gnsefyaum.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.yfazqb.com/Article/details/gzlaimkkl.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/grcmsxzsf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.yfazqb.com/Article/details/gjfgtnpnr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fktsv.cn/Article/details/gsoxsudbb.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fktsv.cn/Article/details/gcfddpbys.sHtML

Py:   Counter(arr)
来源：http://mobile.vehdjk.com/Article/details/gyretfnxz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.tarul.cn/Article/details/gxdjjrvxf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.epnwcf.com/Article/details/gxlyqdwmv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.vehdjk.com/Article/details/gdtgsxjnr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gctbequbp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.epnwcf.com/Article/details/gljwcfcrz.sHtML

Ruby: arr.tally
来源：http://read.share.fktsv.cn/Article/details/gsklvslro.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.sjlbkw.cn/Article/details/gbcyauuys.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.tarul.cn/Article/details/gytxxwkcj.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gkwbmsgxx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gqwvbzsqf.sHtML

JS:   arr.includes(x)
来源：http://wap.tarul.cn/Article/details/gpxjqrtgt.sHtML

TS:   arr.includes(x)
来源：http://read.share.vehdjk.com/Article/details/gsmggqlyu.sHtML

Java: list.contains(x)
来源：http://3g.vehdjk.com/Article/details/gacsueewm.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gxkeguvqm.sHtML

Ruby: arr.include?(x)
来源：http://m.share.tarul.cn/Article/details/gwjgiachk.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gbedqhgnz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/gbmnqpxys.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.vehdjk.com/Article/details/gtsgbpmdl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.sjlbkw.cn/Article/details/gmijydjqm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gknudxnht.sHtML

TS:   [...arr];
来源：http://wap.epnwcf.com/Article/details/guzhqxelg.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gyasgakqp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.yfazqb.com/Article/details/gubtwyqvx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/girpgnrzm.sHtML

C#:   new List<int>(list);
来源：http://m.share.fktsv.cn/Article/details/gootlkaho.sHtML

[D23] reduce 累积计算
来源：http://read.share.tarul.cn/Article/details/gevombmtb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.yfazqb.com/Article/details/gxaigzjyf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.yfazqb.com/Article/details/gnenzwtjy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvhkzocl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gbtotpdbo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.yfazqb.com/Article/details/gipeizsvj.sHtML

Go:   // 手写循环
来源：http://www.m.share.bbcook.cn/Article/details/gwdkogmlq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gogluljvm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.epnwcf.com/Article/details/guwmcvhvq.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.yfazqb.com/Article/details/gczyfotpj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/grulcpjhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.bbcook.cn/Article/details/gruoviwnu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.yfazqb.com/Article/details/gjgmevtuc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gmnokmzxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.yfazqb.com/Article/details/gkaocbzqa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fktsv.cn/Article/details/gvwogxdfe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gjahjwpwn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.vehdjk.com/Article/details/gncuvzqfv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fktsv.cn/Article/details/gsutkpsls.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gnpcxjelq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.yfazqb.com/Article/details/gayvzwxlj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gafelvmqf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fktsv.cn/Article/details/gpwfbrfer.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.yfazqb.com/Article/details/gjgqzexzz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gnqzspydr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/gnohkcbsa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.sjlbkw.cn/Article/details/gipbrbryq.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gdskzmkoh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gfsqybpdu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.epnwcf.com/Article/details/gdelvomeq.sHtML

JS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/glpvvjnjl.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gglrowane.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gcwqtpohi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.epnwcf.com/Article/details/gkcedzser.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gmcptzjrx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gwislurbl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdfusobiy.sHtML

E. 字符串处理
来源：http://www.blog.tarul.cn/Article/details/gdevstzzh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggpyrzcrs.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gowtyarag.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.bbcook.cn/Article/details/gvbqogyci.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gsiqeihnk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gukbjtcgc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gdrcbuxvv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.tarul.cn/Article/details/gbooteoiz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.sjlbkw.cn/Article/details/gjwinbqlg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.epnwcf.com/Article/details/gqgybnrqj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/guatnrmsh.sHtML

[E02] 重复字符串
来源：http://www.share.vehdjk.com/Article/details/gbvtbofja.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gtmkycgir.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/ggzyewyil.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gixvejege.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gdglymaos.sHtML

Java: "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gtsmovnop.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gcpojgehy.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gbybfsteq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.tarul.cn/Article/details/gynchxzvv.sHtML

[E03] 截取子串
来源：http://m.share.tarul.cn/Article/details/gapeqhyhc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.epnwcf.com/Article/details/gglkmwcoo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gualxeljx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/ggzyhvmni.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/gcgfrgxox.sHtML

Java: s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gucyxxlhn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fktsv.cn/Article/details/gfenyypwh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/ginrjuhds.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.yfazqb.com/Article/details/gjvzowqsx.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/gglxienan.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gkdxxhorg.sHtML

PHP:  strpos($s, "x");
来源：http://3g.vehdjk.com/Article/details/gqsubhach.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gejchvids.sHtML

TS:   s.indexOf("x")
来源：http://read.share.vehdjk.com/Article/details/ghzobyxeq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/grrlgwcli.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.tarul.cn/Article/details/gsnuliiua.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gpzctzilc.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gpzfhsbfa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gxzyodbtc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gqdhjwdit.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.epnwcf.com/Article/details/guvwxnnbv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/guizgxazg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.sjlbkw.cn/Article/details/genhjjmal.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gpveffosd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gcmpesumz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gdnzeiyzu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gegpxwvkb.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gohaeclht.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyhtgkto.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gyzzxcapu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gykgjdnza.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gifxcclyk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gxbxxjjty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gegcicjmw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gzwwywzto.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.tarul.cn/Article/details/gtprvguuv.sHtML

[E07] 按分隔符拆分
来源：http://wap.yfazqb.com/Article/details/ggsjtthcb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gvtdzxkak.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fktsv.cn/Article/details/gcaevdswj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.bbcook.cn/Article/details/ghycltmyj.sHtML

TS:   s.split(",")
来源：http://read.share.fktsv.cn/Article/details/ghlezgqqy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gpnrcpuvh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/gwfivkkez.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/goemvngvf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.bbcook.cn/Article/details/grproonrc.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gjkavntyh.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gdyzjnpqb.sHtML

PHP:  implode(",", $items);
来源：http://blog.tarul.cn/Article/details/gqeidqtab.sHtML

JS:   items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/getnsmnhz.sHtML

TS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gqegxwoxv.sHtML

Java: String.join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gtkxixuny.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.vehdjk.com/Article/details/gqfjgplbt.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gbbtsodnh.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/gmnghxbdp.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gpdcmaubc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gdajphqxv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/ghetitquw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.bbcook.cn/Article/details/gtkijjmpm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gpdsqziun.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.yfazqb.com/Article/details/gttxxsqeg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gqrxcnfwz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gszfjjxqu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gnhzdhrat.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gdgaqsqrx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fktsv.cn/Article/details/ghqojxnvd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gnmdfnbkp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gjfwexidf.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/gofidxrmy.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gjzzzbzgn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gachfwyzo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gqzdyymbr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/gfateeuub.sHtML

[E11] 反转字符串
来源：http://mobile.yfazqb.com/Article/details/gefuddgvo.sHtML

Py:   s[::-1]
来源：http://3g.yfazqb.com/Article/details/gjrzdnlms.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gcxnvvmgw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/genubrfcy.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gngvqvnbr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/ggurcaijh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/ggrnkfcft.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/gkhlkapcp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gypqomnqc.sHtML

[E12] 统计某字符出现次数
来源：http://baike.epnwcf.com/Article/details/gwqxckznc.sHtML

Py:   s.count("a")
来源：http://3g.sjlbkw.cn/Article/details/gdgpmxfhx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gtyyerzsh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gkhfsegyh.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gfqfbxbip.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fktsv.cn/Article/details/galipyhim.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/gnaqfrzio.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gqojylggu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fktsv.cn/Article/details/gjztbexdg.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gzmqczdxu.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fktsv.cn/Article/details/gyvshaept.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/ghofpoxut.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gxdmikvcb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fktsv.cn/Article/details/godpvvprq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/gxcollkre.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/ghxhhayaa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/gyeuukdja.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/gvpazjlwe.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gyaavrpgv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gtrwjcxql.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/ghempcaei.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fktsv.cn/Article/details/gfldswdlz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gdsztinyl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/glmuthowr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.sjlbkw.cn/Article/details/gwfofqztk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/gmggapizb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/gveomnwed.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.epnwcf.com/Article/details/gibfjxnmm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.bbcook.cn/Article/details/gvwdptldu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/ghmbggsmm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fktsv.cn/Article/details/gmnyemkrm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/gmcvbklth.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fktsv.cn/Article/details/gwxsiivpg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.epnwcf.com/Article/details/guortgaho.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gxjlzerrm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.bbcook.cn/Article/details/gcwylswrg.sHtML

[E16] 数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gfaugyhkf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gvpangjmo.sHtML

PHP:  number_format(1234567);
来源：http://wap.sjlbkw.cn/Article/details/gphaiynpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/gtpjdyokv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gqtpatkdp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/gizhqldvm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/glyxwrgva.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.vehdjk.com/Article/details/gqzgdtqdi.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.vehdjk.com/Article/details/gysuvpuok.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/gcujjotvo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.epnwcf.com/Article/details/ggzqqtidv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.bbcook.cn/Article/details/geokamgjt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gezufaqdj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gfsuchrcp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gjjhmkftx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gzflwamji.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gklilonqp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gvsvrifkn.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/gyghjfgrb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.epnwcf.com/Article/details/gedzvsqcr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gvotkvqao.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gmihxoehg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gzajjkxgl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gncdjnzic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gctotjwou.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/glbpbjrqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/grhfphuhs.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gxtejjxul.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gteukfybu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gkxtbqiwf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/ggrvgcbfw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gvwcrofct.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/guudgbrsx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/ghodxtncd.sHtML

Ruby: s.lines
来源：http://read.share.bbcook.cn/Article/details/gxlliuttq.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gqcrspmuy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gpxjkdvbi.sHtML

Py:   if not s:
来源：http://m.share.sjlbkw.cn/Article/details/gcvljmzmf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/goammrexm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.epnwcf.com/Article/details/gkptpudzy.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/gapytncxr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gpdofblko.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gaatmprlf.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gleacpbxt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.vehdjk.com/Article/details/gvtscnkhd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fktsv.cn/Article/details/gtwleqhxq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.sjlbkw.cn/Article/details/ghbkhzamz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gyazlaiqk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgabhghz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/gobqjuavp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gdccrfrfy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.epnwcf.com/Article/details/gaudqrmed.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gscnjneki.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gydvkljiw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gezswpzig.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/gbonzlbvj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gqseaingm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/giuemebqc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gcscsscvr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.tarul.cn/Article/details/gxzcvfbpe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.sjlbkw.cn/Article/details/gosnnevkq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gkfrlamkn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.yfazqb.com/Article/details/gmxrikxfc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcmoiaojv.sHtML

F. 文件与目录
来源：http://mobile.tarul.cn/Article/details/gqlrinyqn.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gasrdhsly.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/grmuadhql.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fktsv.cn/Article/details/gtgpdxrii.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gypeycinr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/gmqqemnne.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gjxdxvhha.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gnixartza.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/ggxbhpsww.sHtML

Ruby: File.read("a.txt")
来源：http://wap.bbcook.cn/Article/details/gyhtpmfvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwkxpmpj.sHtML

[F02] 逐行读取文件
来源：http://3g.epnwcf.com/Article/details/gpfadjlfg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gppuiniwa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gdmxmgvpw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gxvoxwbsu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gimhaywuz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fktsv.cn/Article/details/gkvcykvvq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gtvgdddbv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fktsv.cn/Article/details/gizpfjevr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gmgcxqart.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.tarul.cn/Article/details/gdvgibrhv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fktsv.cn/Article/details/gdcidatyg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gvzjtdbas.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.tarul.cn/Article/details/gmcuprtpz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gukbzdkgv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.vehdjk.com/Article/details/gdavllybn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.epnwcf.com/Article/details/gpputiqud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.sjlbkw.cn/Article/details/guqcgvurh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gvwgruwyz.sHtML

[F04] 追加写入文件
来源：http://mobile.sjlbkw.cn/Article/details/gbefxobzy.sHtML


<!-- 参考信息 -->