代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.tarul.cn/Article/details/gxchziyjw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.yfazqb.com/Article/details/gvjuucdww.sHtML

Py:   Counter(arr)
来源：http://m.share.vehdjk.com/Article/details/guxzvtsly.sHtML

PHP:  array_count_values($arr);
来源：http://blog.bbcook.cn/Article/details/ghckomtao.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/glbklpuqi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gcpjguhiz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.vehdjk.com/Article/details/gfdnsgwgs.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fktsv.cn/Article/details/gptborrus.sHtML

Ruby: arr.tally
来源：http://blog.sjlbkw.cn/Article/details/gxmfiusyn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.yfazqb.com/Article/details/gidahitre.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.bbcook.cn/Article/details/gvqngdmzh.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/ggbafgvwf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fktsv.cn/Article/details/gdmrbtgga.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/gxwithuvi.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzenybmby.sHtML

Java: list.contains(x)
来源：http://www.m.share.tarul.cn/Article/details/gwfvugrui.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gxdazvcjv.sHtML

Ruby: arr.include?(x)
来源：http://read.share.yfazqb.com/Article/details/gnvkpaokv.sHtML

C#:   list.Contains(x)
来源：http://www.blog.yfazqb.com/Article/details/gbkxjtcfl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gwpzefruh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gjkyewqxd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/guaffozgz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gjxxxglqz.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gbsgdjsph.sHtML

Java: new ArrayList<>(list);
来源：http://baike.vehdjk.com/Article/details/gtdoqkcpt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gwuyhlefk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/gptaigpwj.sHtML

C#:   new List<int>(list);
来源：http://3g.epnwcf.com/Article/details/gchqlmcjt.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fktsv.cn/Article/details/gcozgzwgs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.sjlbkw.cn/Article/details/gdfzztfvv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.sjlbkw.cn/Article/details/gaxkevyph.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gxfszmsxb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/goflctrev.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.vehdjk.com/Article/details/gnvpcmokt.sHtML

Go:   // 手写循环
来源：http://blog.vehdjk.com/Article/details/ghyffvnnn.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/guxenxqui.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.bbcook.cn/Article/details/gmtfjmyzb.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gpwlnqmmf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gchzjsanx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gxuxjvzsp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.tarul.cn/Article/details/gpstlfqka.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/glptwqdet.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gemfjxcnm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/gonmzagfk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fktsv.cn/Article/details/gufhacwkp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gickhtkhv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.yfazqb.com/Article/details/gexnuvyey.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gmkrmgway.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.sjlbkw.cn/Article/details/gkcxodrtb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.vehdjk.com/Article/details/gfcmidvts.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/grtkfirbb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gxwhfimyr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gtqhxzjgb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.epnwcf.com/Article/details/gcswalzrv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.sjlbkw.cn/Article/details/gjqxiuxui.sHtML

[D26] 数组转字符串
来源：http://www.share.bbcook.cn/Article/details/gdisxohhy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/grjfjmnle.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fktsv.cn/Article/details/gioizyqzf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gzpalvmli.sHtML

TS:   arr.join(", ")
来源：http://m.share.vehdjk.com/Article/details/gwyvmhrry.sHtML

Java: String.join(", ", list)
来源：http://mobile.yfazqb.com/Article/details/gnetosfft.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gpogutvce.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gwmeifhyc.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/gtjxcdaid.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gicufnsqu.sHtML

E. 字符串处理
来源：http://baike.fktsv.cn/Article/details/gtyxpsedd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gxkmovcpj.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gqbsrjgpv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gsblrvjoy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gaottuerh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gqstmnzfn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gxomhbzkv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gcenpebmh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/guxufcbtn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gsrswrlse.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.yfazqb.com/Article/details/gxnquzvgp.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gllhbhgdj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gxohehiyx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.tarul.cn/Article/details/gwqglfdjv.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/genuptaqb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/ghszrezeo.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gvfojttip.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.vehdjk.com/Article/details/gllwxjvuj.sHtML

Ruby: "ab" * 3
来源：http://www.share.tarul.cn/Article/details/guchiwgwx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/geujsabae.sHtML

[E03] 截取子串
来源：http://mobile.yfazqb.com/Article/details/greavwdsn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/glrvypuhh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gdpmkxflp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/grgwwhhak.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gnndjsunf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gszkqqwas.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.tarul.cn/Article/details/gxnzrraud.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/ggzgzxdbu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gzmuruldn.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gxhyrycpz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/giyliiygm.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.vehdjk.com/Article/details/gikhhqvps.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gjcnrwgsd.sHtML

TS:   s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gtcwxgkja.sHtML

Java: s.indexOf("x")
来源：http://www.share.epnwcf.com/Article/details/gntglqnxk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gvmmwpkuy.sHtML

Ruby: s.index("x")
来源：http://m.share.tarul.cn/Article/details/gfgkiffpc.sHtML

C#:   s.IndexOf("x")
来源：http://3g.sjlbkw.cn/Article/details/glhiexkfe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fktsv.cn/Article/details/ghdqkazdp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gnzyfchbp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.tarul.cn/Article/details/gjtoxsmog.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/grtiwgybz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.epnwcf.com/Article/details/gffsbwilm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/grfaiqlpr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fktsv.cn/Article/details/gvzjytsil.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gdidwbwiw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gziikypmz.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/gauvaidgc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/ghooxifrl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gzklwvnls.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/ghorbsbst.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gjtbuiwyx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gydgiqjnj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/giehrzlkd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/grrzfzqnt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/grkiyqttp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.yfazqb.com/Article/details/giopeemou.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.sjlbkw.cn/Article/details/gagizcroa.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.epnwcf.com/Article/details/gcgtjyron.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.yfazqb.com/Article/details/gstbqsmsj.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/gjtuhsqud.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.epnwcf.com/Article/details/gpkghoitb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.vehdjk.com/Article/details/gzjczigqd.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/gtrmfnxsu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/gxnbfahyl.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.sjlbkw.cn/Article/details/guleybiul.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gboxwdtuy.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fktsv.cn/Article/details/gbxjniihi.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gzjamfntf.sHtML

TS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gmnekddwx.sHtML

Java: String.join(",", items)
来源：http://www.blog.sjlbkw.cn/Article/details/gaejgsnkh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.sjlbkw.cn/Article/details/gziwbmvsz.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gngqvxjrp.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gvggzoxis.sHtML

[E09] 去除所有空白字符
来源：http://mobile.vehdjk.com/Article/details/ggkuuzxlc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gnempcxgl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.tarul.cn/Article/details/gsbrwalns.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.bbcook.cn/Article/details/ggzqtsjee.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gvqtdfgeg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gxecfdofg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gzycmzttc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.vehdjk.com/Article/details/gidzonbkg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.bbcook.cn/Article/details/gsvfkqwst.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fktsv.cn/Article/details/gedpmvsvl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gnvnirbob.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gfatqnpsf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gvsbgkhqn.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gzvqwefrp.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gawfeqhjn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gjlbtfvzl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/ghegvbohg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.tarul.cn/Article/details/gcqgreaxz.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gvjhygoey.sHtML

Py:   s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/gymcdubwg.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/grrheolzz.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/guaaqrfex.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gopvoxydy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gzsqfgbeo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gcuvxiznr.sHtML

Ruby: s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gdmkghdtw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gtzweocvf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.bbcook.cn/Article/details/gtnoxpltv.sHtML

Py:   s.count("a")
来源：http://blog.yfazqb.com/Article/details/gblviwduv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gpfmjnmgg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fktsv.cn/Article/details/grnjkdrxi.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fktsv.cn/Article/details/gshtyxiha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.vehdjk.com/Article/details/gtefeswye.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.bbcook.cn/Article/details/ghlouytjp.sHtML

Ruby: s.count("a")
来源：http://blog.epnwcf.com/Article/details/gglydavcr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.yfazqb.com/Article/details/gevuymija.sHtML

[E13] 逐字符遍历
来源：http://www.blog.yfazqb.com/Article/details/gbhfodmnl.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gocwiodrb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fktsv.cn/Article/details/gfhiicyrr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gpxtoessl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/gniodspoh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gtfcpaiqx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gelzfxvlm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.epnwcf.com/Article/details/geyrwzkvs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.epnwcf.com/Article/details/guytlqedy.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/guiommzjz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gshqhcnwz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gwwkdeqje.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.epnwcf.com/Article/details/gdpctigex.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gcyhwzppg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gduymzfgg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.yfazqb.com/Article/details/gmsxgmnws.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.bbcook.cn/Article/details/gmhlqxwak.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gmukulyat.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/gcgjyrsme.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbzjozin.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.yfazqb.com/Article/details/gaeuhjniw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.bbcook.cn/Article/details/gkflwyjpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gercjinwn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gqcpwecck.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gjmetwyqm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.epnwcf.com/Article/details/ggeswexup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.epnwcf.com/Article/details/gyvrcdchy.sHtML

[E16] 数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gblduolek.sHtML

Py:   f"{1234567:,}"
来源：http://3g.yfazqb.com/Article/details/gduqoflql.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/gzlurnkvb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gjotzdesk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/grxelumrv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.vehdjk.com/Article/details/guteyfown.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.yfazqb.com/Article/details/gqyclyxem.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.tarul.cn/Article/details/gerseybkn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gyatvncfm.sHtML

[E17] 首字母大写
来源：http://www.blog.sjlbkw.cn/Article/details/gakgqkoeb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.yfazqb.com/Article/details/grqbfcfue.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.bbcook.cn/Article/details/gosxbhgxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gqfvtxfdi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/glyyoyfyy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/geppykmuc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.tarul.cn/Article/details/gjjadgvsv.sHtML

Ruby: s.capitalize
来源：http://m.share.tarul.cn/Article/details/gknspopas.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gyyxnsdfx.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gupukcapr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.vehdjk.com/Article/details/gwdsxqkwk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.tarul.cn/Article/details/gzwqgggyh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gbemovzom.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gbizfywbz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gbfamgglp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.yfazqb.com/Article/details/ghxsbxssw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/ghjkelyqh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.bbcook.cn/Article/details/gmrbtklkr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gcmdelksb.sHtML

Py:   s.splitlines()
来源：http://www.share.bbcook.cn/Article/details/gixnltzwl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.tarul.cn/Article/details/gnxxoifrr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gwccpdliq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/guptivpwt.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/gfwgnvcub.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.sjlbkw.cn/Article/details/gbrcyrqdb.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/ghcarxgcx.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gmzypglkl.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gslcmjzfs.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gkjcadeuq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.yfazqb.com/Article/details/gqmxnzzxi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gtxhxxinb.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gfcpmfdhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gvhpspkok.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gkecfngzn.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/gtsvrqjhg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.tarul.cn/Article/details/guyocanze.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.vehdjk.com/Article/details/gajwrztur.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.tarul.cn/Article/details/gyqjdzehh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gooqwxvbl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gwtwlbldu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gcryjrmbg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.bbcook.cn/Article/details/gjkpkokng.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.tarul.cn/Article/details/ghpqarmvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gilngtnul.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gwtgzrays.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/getsfmtwf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fktsv.cn/Article/details/gbpnuocck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gapgqsznc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gbqktlvdh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/gpooogqdq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.bbcook.cn/Article/details/gfleypgio.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.vehdjk.com/Article/details/gmaaelhmn.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/gycdmsmuz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.vehdjk.com/Article/details/gmztbegtk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxnotnrok.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/grscyzvzh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gelzhxuiu.sHtML

[F01] 读取整个文件
来源：http://3g.sjlbkw.cn/Article/details/gcxuhqzmc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gbtnhbdkh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gngnbzlai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gzgvemyow.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gycqhtlhz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdktjouq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gaopjejsv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/grboqctnl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gfgwbfrtk.sHtML

[F02] 逐行读取文件
来源：http://baike.tarul.cn/Article/details/gvufdellt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.sjlbkw.cn/Article/details/gnjdfpkhn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.epnwcf.com/Article/details/gelyftfqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/gtusqzyxu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gjevokoxa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/giffaslhv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gqbkiweuk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fktsv.cn/Article/details/geersrvwz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.vehdjk.com/Article/details/gfirhqlip.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.vehdjk.com/Article/details/gcvcnbanp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/glxjqsgnk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gsrsykimr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gqwsdaxsc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.tarul.cn/Article/details/gpzqgnghv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gavzrgzuf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.epnwcf.com/Article/details/gxpnledoj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/goodewsux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gypahgqir.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gbidnkktn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fktsv.cn/Article/details/guzuxhkxy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.tarul.cn/Article/details/gzwtnfvot.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gcixdfozs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.tarul.cn/Article/details/gjnnnuctx.sHtML


<!-- 参考信息 -->