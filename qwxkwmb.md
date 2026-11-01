代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.sjlbkw.cn/Article/details/goaaiyars.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.sjlbkw.cn/Article/details/grscfdera.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/gkkwycyfq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.epnwcf.com/Article/details/gnaagwccx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.yfazqb.com/Article/details/gjzxrteei.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.bbcook.cn/Article/details/gjltxricb.sHtML

Py:   Counter(arr)
来源：http://wap.epnwcf.com/Article/details/glzlkstdi.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.yfazqb.com/Article/details/gemgkwijk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gkfbtmtqv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.yfazqb.com/Article/details/gpmgbycme.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.epnwcf.com/Article/details/gznqfstds.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fktsv.cn/Article/details/gmyozbngd.sHtML

Ruby: arr.tally
来源：http://blog.yfazqb.com/Article/details/ggnxrkakn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.sjlbkw.cn/Article/details/gtyflfdjw.sHtML

[D21] 判断是否包含某元素
来源：http://baike.yfazqb.com/Article/details/gezlndabw.sHtML

Py:   x in arr
来源：http://baike.yfazqb.com/Article/details/gnnmgdvfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/grzhmoiwn.sHtML

JS:   arr.includes(x)
来源：http://read.share.epnwcf.com/Article/details/ggjqmtlgt.sHtML

TS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gughseqon.sHtML

Java: list.contains(x)
来源：http://www.share.yfazqb.com/Article/details/guugajdwx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gnenhxldw.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gwsqlooxf.sHtML

C#:   list.Contains(x)
来源：http://m.share.bbcook.cn/Article/details/gbrtekmrx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.tarul.cn/Article/details/gkrbcghmi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gillioizb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gywvarezv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.yfazqb.com/Article/details/gkqgnasio.sHtML

TS:   [...arr];
来源：http://m.share.yfazqb.com/Article/details/gejfohiii.sHtML

Java: new ArrayList<>(list);
来源：http://blog.yfazqb.com/Article/details/goozcloqe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gicyidvdv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gqxecnvdq.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gwfjylweo.sHtML

[D23] reduce 累积计算
来源：http://baike.sjlbkw.cn/Article/details/gvdmbigvh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gommylhtw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gctjkhgex.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/grkujkuno.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gglhmnxsr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gdxfhdibi.sHtML

Go:   // 手写循环
来源：http://read.share.epnwcf.com/Article/details/gcvimqfki.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/gfdnidjjc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.yfazqb.com/Article/details/gziwoorfy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.tarul.cn/Article/details/gaerwktjh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gazpyvidw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/gwfxsmjwr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbesvcdfk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gvemqwsal.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gozvhfukn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gznpxxbfs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.vehdjk.com/Article/details/gdmzbcqha.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gkeginrkd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.bbcook.cn/Article/details/gynqgsgdm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gjeoqtoxb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gjnspudbw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/ghxpcffpj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.epnwcf.com/Article/details/gcuvduxxm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/gvjvnshrv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gnclxcrsh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gswtnsnqy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.epnwcf.com/Article/details/gemutsaip.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gnayksqnm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gssywxkzr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gwavihjgf.sHtML

JS:   arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/ggtcgyfgq.sHtML

TS:   arr.join(", ")
来源：http://wap.sjlbkw.cn/Article/details/gphruhiyg.sHtML

Java: String.join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/gtcssakad.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gilolznke.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/gkmoeeflz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeupnimg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/giktoghnp.sHtML

E. 字符串处理
来源：http://read.share.epnwcf.com/Article/details/garmfzbnb.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpgwdhjrn.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gqrwppsrw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.sjlbkw.cn/Article/details/gnoonnkif.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.bbcook.cn/Article/details/guypgkarg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gzlskqouu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gzvocghwo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fktsv.cn/Article/details/gudlcojxp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.bbcook.cn/Article/details/gpwubnpum.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.epnwcf.com/Article/details/gzighzgfe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fktsv.cn/Article/details/giwsmvsqu.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/grealtggh.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gyfgqyiyc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gveowzxrn.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/gdwukzalb.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/ggbqhibiy.sHtML

Java: "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gblnrmjvl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxhaghni.sHtML

Ruby: "ab" * 3
来源：http://www.blog.tarul.cn/Article/details/gkqvtliay.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.sjlbkw.cn/Article/details/gwetewufe.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gmldhsoxi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.yfazqb.com/Article/details/gboxxdhwp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gbpstadxg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.bbcook.cn/Article/details/gwgkvypey.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gbikglmju.sHtML

Java: s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/govizhrkc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.bbcook.cn/Article/details/gkyjyrhto.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gfcpvcynl.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gylbupato.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gjgancpoq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gxixchmgg.sHtML

PHP:  strpos($s, "x");
来源：http://wap.bbcook.cn/Article/details/givrzijvc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.sjlbkw.cn/Article/details/glgpkumlo.sHtML

TS:   s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gbwwouleq.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gzhljlpet.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gscpohrbk.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gkafithnn.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gsqeqxxsj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.vehdjk.com/Article/details/gtrebgqvu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gpqzhwwge.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/gmxuatuqt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gnnadtzce.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.bbcook.cn/Article/details/gsashmeue.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/grjkwwzlk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gkmkxtldn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gwsomlcau.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gztywybfy.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gsnjdqctj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.yfazqb.com/Article/details/gmouxupga.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.tarul.cn/Article/details/gdxudbsgy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/guvxiimqn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gabtijqvo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/grrdjvxsr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/goorvcgzz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/gsmvuzlru.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gckqzrnam.sHtML

[E07] 按分隔符拆分
来源：http://mobile.tarul.cn/Article/details/gjtnbvkmg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gihkggfjc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/gabwmbpgm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.tarul.cn/Article/details/gbnrfxdcn.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gszubhupo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.vehdjk.com/Article/details/gxrdeojhy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gqzpcbtvm.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.epnwcf.com/Article/details/gdkuqrmbp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.sjlbkw.cn/Article/details/gnfwltxrr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fktsv.cn/Article/details/gfmzaqpxy.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gsvbtpjmv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.epnwcf.com/Article/details/gprbprlmd.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gdvlqtqyo.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/ghdcxmfdh.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/geqwkoykw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gccqdiouj.sHtML

Ruby: items.join(",")
来源：http://mobile.epnwcf.com/Article/details/gktrphfhf.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/gzbngbtoc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fktsv.cn/Article/details/gnynwzcwb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gdtttxnpd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fktsv.cn/Article/details/gquqakwxw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.sjlbkw.cn/Article/details/gwnvvzbua.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gyvfsmyls.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.bbcook.cn/Article/details/ggbpiqqjj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/glypskasi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gpmfdxare.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.epnwcf.com/Article/details/ghfoqwyhe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gahgokcbg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.vehdjk.com/Article/details/gscnjdoty.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gvfjxcuhu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/giupccmmd.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.yfazqb.com/Article/details/gowfygoxf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.sjlbkw.cn/Article/details/gtddfwrip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gcegpyssx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gwlpxbfth.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gystlnhpu.sHtML

[E11] 反转字符串
来源：http://www.share.bbcook.cn/Article/details/gxhrxijnv.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gplukvxsg.sHtML

PHP:  strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gwwlysyll.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gsqznlhlh.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gpmzjpbqo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.tarul.cn/Article/details/gfhpfobhx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fktsv.cn/Article/details/gkxcultbv.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gniknhnyt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/gfkhjgvda.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gwllcuarx.sHtML

Py:   s.count("a")
来源：http://3g.tarul.cn/Article/details/gfqdeljer.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/grxmsukve.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gvehvsibe.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.vehdjk.com/Article/details/gkffgkarc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gfbqeefpt.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.vehdjk.com/Article/details/gccmccjnh.sHtML

Ruby: s.count("a")
来源：http://m.share.sjlbkw.cn/Article/details/gztqhdvcg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/grjgmnerh.sHtML

[E13] 逐字符遍历
来源：http://blog.vehdjk.com/Article/details/getfrpxfl.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/ggphkrvle.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gkdwqrxng.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gvovwemsl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.epnwcf.com/Article/details/gjebxnglh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gssrqjwuj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gdmpzqvwo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/geruuwjgp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/ghqdioose.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/ggvtqxsdf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.vehdjk.com/Article/details/gdinsoumg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gftihiurs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gdmkpqwoh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gewftdgcf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.tarul.cn/Article/details/gndknobfx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gudqadkbd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/gezewjgwc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.yfazqb.com/Article/details/gnisyiors.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdmawlef.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.tarul.cn/Article/details/gkynrazaq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.tarul.cn/Article/details/gmickepue.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.bbcook.cn/Article/details/gaiwmgnpm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fktsv.cn/Article/details/gfkuammkp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fktsv.cn/Article/details/gtmrlcwmy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gyylqtxqs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/guzksvria.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gmnzjrnkm.sHtML

[E16] 数字千分位
来源：http://read.share.bbcook.cn/Article/details/gkyeewmfu.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.tarul.cn/Article/details/gfqyctxmv.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/ggaaznzjj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/grcqsjani.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gjhhlcqia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjiwlfuep.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gazovxaki.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gtshqnzvt.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/grktyortx.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gwvzongqq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/gdjdwjort.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.sjlbkw.cn/Article/details/gvxscwqww.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/geaombeak.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gdgcniiiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.sjlbkw.cn/Article/details/gxnfgqvrl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/grdqrgbpg.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gdziftigz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.vehdjk.com/Article/details/gjqextmlk.sHtML

[E18] 模板占位符替换
来源：http://mobile.bbcook.cn/Article/details/gnmcbmvti.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.yfazqb.com/Article/details/gswbfavsq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fktsv.cn/Article/details/gjnteqspb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gmvtaubnz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/ghnhaxztj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gzmpqkema.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.yfazqb.com/Article/details/glyfgidvy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/giaytzrbw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.bbcook.cn/Article/details/gkkkvjdzi.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/giuhwdicq.sHtML

Py:   s.splitlines()
来源：http://mobile.bbcook.cn/Article/details/gkonzytnu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.bbcook.cn/Article/details/gplhztzhf.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.tarul.cn/Article/details/gcsnggpsw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.tarul.cn/Article/details/geyurzura.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gbrhiqfdz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gbgjtonfc.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gwoeyhtap.sHtML

C#:   s.Split('\n')
来源：http://www.blog.bbcook.cn/Article/details/gfykaxjdc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gmywhqddg.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gefwvuhoh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gnneoxonp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.bbcook.cn/Article/details/glkovkjql.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gqjxhmnel.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/ggfpjldgi.sHtML

Go:   if s == "" {}
来源：http://www.blog.fktsv.cn/Article/details/gpyczcjck.sHtML

Ruby: if s.empty?
来源：http://baike.sjlbkw.cn/Article/details/gnxhzdgdy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/glcfhxrzt.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/gzbtkhuis.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fktsv.cn/Article/details/ggyibavym.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/ggtpeslgk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/giguibknt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gdglihlip.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gncydzzzh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.epnwcf.com/Article/details/gpwhqljzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gvoppgvdm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gmbfrlywv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/givhbuaiv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.epnwcf.com/Article/details/gjfiskgvh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/ggakrofiy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gjumknoey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gapdjinkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gqqeoaxuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gvljzyhei.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.epnwcf.com/Article/details/gxjitczaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gisdickrc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/geusazwjm.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/gowuryqxn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gsjvkujat.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gyyjqwbuq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/gszzvstza.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gavalocrx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.bbcook.cn/Article/details/gtbyfytkh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/gvvlupeqy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gqjiauubf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.tarul.cn/Article/details/gtlvtmaob.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gcgpaieqw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gfflhkjol.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/gdrchclic.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gmrywcwru.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.vehdjk.com/Article/details/gkkvrnkze.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gfmuugpdw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gkrcuzvgj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.tarul.cn/Article/details/gjfyxshld.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gjbniihwm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fktsv.cn/Article/details/gqzyghnku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gpldcowcn.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.bbcook.cn/Article/details/goushgdab.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gqiezmicm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/ggnqwjlpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gdjobqvah.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.yfazqb.com/Article/details/gfbqkobau.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gtzxwnuot.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.vehdjk.com/Article/details/gxlslgbjr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.bbcook.cn/Article/details/gtfsflpxl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.bbcook.cn/Article/details/gyrvnijev.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gaantnmkk.sHtML


<!-- 参考信息 -->