代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.sjlbkw.cn/Article/details/gvkovymge.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gldclblcq.sHtML

Py:   Counter(arr)
来源：http://m.share.yfazqb.com/Article/details/grxndqpom.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fktsv.cn/Article/details/gsewrlorl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.epnwcf.com/Article/details/ghfxvmiag.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gphynszqk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gukgsqfkx.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.tarul.cn/Article/details/gyfbssjqs.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/ggzkeggxz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.bbcook.cn/Article/details/gmoxcymsm.sHtML

[D21] 判断是否包含某元素
来源：http://3g.yfazqb.com/Article/details/gjdzxnqvm.sHtML

Py:   x in arr
来源：http://www.m.share.vehdjk.com/Article/details/ghbzduvnm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.sjlbkw.cn/Article/details/goloelvuc.sHtML

JS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gasdktuze.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/geudnphgd.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/grgppswqv.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fktsv.cn/Article/details/gflyxzfor.sHtML

Ruby: arr.include?(x)
来源：http://read.share.bbcook.cn/Article/details/ghsjimohf.sHtML

C#:   list.Contains(x)
来源：http://www.share.bbcook.cn/Article/details/gounmrbph.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gbtkpowda.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gmphdphdm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.yfazqb.com/Article/details/gqxqjszbv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.bbcook.cn/Article/details/giwdzjehg.sHtML

TS:   [...arr];
来源：http://baike.sjlbkw.cn/Article/details/gdfodbyva.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gamkibxee.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.yfazqb.com/Article/details/gesdgrsae.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.vehdjk.com/Article/details/gpgrombvd.sHtML

C#:   new List<int>(list);
来源：http://www.share.fktsv.cn/Article/details/gdfqpbfdv.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/glsmjzflu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gjhqbwtrl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.epnwcf.com/Article/details/gxsykyaeu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.tarul.cn/Article/details/gbokctrkd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gcieeaotr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.yfazqb.com/Article/details/gjcuwikdv.sHtML

Go:   // 手写循环
来源：http://m.share.yfazqb.com/Article/details/gpjramxnr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.tarul.cn/Article/details/grdzisnap.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.vehdjk.com/Article/details/gpigjoiix.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/gxsvqcort.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gzhxlpjsz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gjraijsyh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.bbcook.cn/Article/details/gawjwnklq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.tarul.cn/Article/details/ghxtfdwqr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gtmgncnbj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.yfazqb.com/Article/details/gkfflsbbf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gzwyzactg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fktsv.cn/Article/details/gghxgdhim.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gytjworoa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.yfazqb.com/Article/details/gsqehssyo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.epnwcf.com/Article/details/gzbajonty.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.sjlbkw.cn/Article/details/gvnqvemdo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/gntiggyqt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gtrgtviir.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.vehdjk.com/Article/details/ggfzqyeiz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/glrihzkig.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gimjdvpof.sHtML

[D26] 数组转字符串
来源：http://mobile.tarul.cn/Article/details/gzqkaiotk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.tarul.cn/Article/details/gzysdziju.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gekfkcnta.sHtML

JS:   arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gkjhwming.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gqonbkjma.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/gjntpjlac.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/grpcpcyyl.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gjfmmgyvu.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gkvpddlkr.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbprdiwdl.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gzsqwtetn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggnvahmez.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gefhxgjrq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/gxecmeium.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gindpjyav.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/giyrddaih.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gfhvivgss.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/gddmqwxrs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/grscwombx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gtpojlktv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ghdpukrbl.sHtML

[E02] 重复字符串
来源：http://www.m.share.vehdjk.com/Article/details/gpubjcorn.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gixobojkp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/grytmrmlv.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/glzmnrbrm.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.vehdjk.com/Article/details/glehjrwyo.sHtML

Java: "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gekssxllg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/gulpwhypl.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gglhbfivj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.vehdjk.com/Article/details/gkwzllkrq.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/ghaezhoor.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/ghwryuecb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gxqsqsubb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/greaeeyoi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gbzuopbvl.sHtML

Java: s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gyhiyolwo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.sjlbkw.cn/Article/details/gsghjuhvh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fktsv.cn/Article/details/gmbhgqnhn.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gudvkoemm.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/gqxblmdze.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gyjyadanw.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gjfvpqgim.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.vehdjk.com/Article/details/gzjmvstyr.sHtML

TS:   s.indexOf("x")
来源：http://baike.fktsv.cn/Article/details/gkcrrcovt.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/guhrwbhsg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.yfazqb.com/Article/details/gcctlnqaq.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gevyvwjnb.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/grtcuopot.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.fktsv.cn/Article/details/gxamdcwct.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.yfazqb.com/Article/details/gqpmwtihy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.bbcook.cn/Article/details/gqdohqgsk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gifnjbfmb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.yfazqb.com/Article/details/ghsekfcoz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.yfazqb.com/Article/details/gavtiwuey.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.vehdjk.com/Article/details/gagadwmov.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/guobcodph.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gzocrbyyl.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gimceeqpb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gpyflmzlu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.epnwcf.com/Article/details/ghkzwojdv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gebgbdels.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/ggpvisspi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/goxrfkoev.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/gufewmntn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gwhshxqzb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/ggpshokpm.sHtML

[E07] 按分隔符拆分
来源：http://m.share.tarul.cn/Article/details/gghwduhsz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.vehdjk.com/Article/details/gzkxsnusw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/gtpylrymw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.vehdjk.com/Article/details/gteqwevbk.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gdvfruptx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.tarul.cn/Article/details/gvzppznmy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gfudbqyqr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/gbuojerpi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gkhxgaihx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/ghdcypytz.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gzteqzvcr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/grrvqzckq.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gydmxmshl.sHtML

TS:   items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gztggtwad.sHtML

Java: String.join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/glmxbfowz.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/ggrxswrod.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gwwbtiqha.sHtML

C#:   string.Join(",", items)
来源：http://baike.tarul.cn/Article/details/gmjmyjxbb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gsxsvkpws.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.sjlbkw.cn/Article/details/geuahmmke.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gglproigz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.vehdjk.com/Article/details/goynqnauc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gguwmaofi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/guskhotbj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/guklwstka.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gxlrxosnb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gntdchcvb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.yfazqb.com/Article/details/gixsokaqt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.vehdjk.com/Article/details/gbiztpfzd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/guneqfhol.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gbveylcjv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/govlhfsil.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxafzbkes.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gguodmpvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gcgexzybx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gkzqwvovp.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gjpfvyzzl.sHtML

Py:   s[::-1]
来源：http://baike.vehdjk.com/Article/details/gwlashviw.sHtML

PHP:  strrev($s);
来源：http://www.share.bbcook.cn/Article/details/goiazdobm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnahaneyo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gbzbwebir.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gwehvzhns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gpvtrflpy.sHtML

Ruby: s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gooxhmsnz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gmqlblpto.sHtML

[E12] 统计某字符出现次数
来源：http://wap.bbcook.cn/Article/details/gypfuhhgt.sHtML

Py:   s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gvzamrudd.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.epnwcf.com/Article/details/gybqyhmyu.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gctweilfv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gcfebmrfg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkvutgqw.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.sjlbkw.cn/Article/details/gqrzzhgap.sHtML

Ruby: s.count("a")
来源：http://www.blog.vehdjk.com/Article/details/gatepdjdz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.vehdjk.com/Article/details/gtbgwdmyb.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.epnwcf.com/Article/details/gsbxdhfvy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gauqdmshz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.tarul.cn/Article/details/guixggbym.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/grpvfpqku.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gwyoxwaqw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gsewevmed.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gjwexqasg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fktsv.cn/Article/details/gqypupoft.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gwqjanede.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/gppirrndg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.tarul.cn/Article/details/gbssfksme.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/ganejvnpx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gjctxgniv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fktsv.cn/Article/details/gixsidtod.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.epnwcf.com/Article/details/giurtseny.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gugfkusqo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gaizhiwma.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gcvuuijhp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.bbcook.cn/Article/details/gtdjzyqtq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.sjlbkw.cn/Article/details/gscfvpjag.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/gkenttejl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.tarul.cn/Article/details/gszxblqdr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gyjnhgaar.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.tarul.cn/Article/details/gygvlqhvl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gajkzgqbg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gooltnxlv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/gpdvitviw.sHtML

[E16] 数字千分位
来源：http://baike.vehdjk.com/Article/details/gyjyiladh.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.bbcook.cn/Article/details/gqynojxng.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fktsv.cn/Article/details/gfdkfppnv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gtmbhqpgx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/ggmpcbqaz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gqqkgnada.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/guflmegyr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fktsv.cn/Article/details/geajjbmyn.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.sjlbkw.cn/Article/details/gaqdzgauy.sHtML

[E17] 首字母大写
来源：http://www.m.share.tarul.cn/Article/details/gcbvqqmga.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gimwowski.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fktsv.cn/Article/details/gbrnmejno.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.epnwcf.com/Article/details/gsqgbjdou.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gdnmnigvf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gqqztrxqa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gsbfwgtna.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gzczdblfo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.tarul.cn/Article/details/gtvwngmau.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gigovghiz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fktsv.cn/Article/details/gtzmnaart.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/gmzrgknal.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/glqpappch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gvzatfuss.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gvhxfdplz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.bbcook.cn/Article/details/gfuprrsxt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gokdpyjaq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.sjlbkw.cn/Article/details/glmcfsmhv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.bbcook.cn/Article/details/gqxkvhgsq.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gxwtelhfr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.sjlbkw.cn/Article/details/gvjfjyslb.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.sjlbkw.cn/Article/details/gachagfby.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gajgyknme.sHtML

Java: s.lines().toList()
来源：http://www.blog.fktsv.cn/Article/details/gbbtoztsu.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.sjlbkw.cn/Article/details/gsrxufezr.sHtML

Ruby: s.lines
来源：http://read.share.vehdjk.com/Article/details/gdbbtekwf.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gccakhium.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxovhcsw.sHtML

Py:   if not s:
来源：http://baike.yfazqb.com/Article/details/gpnqyzbtv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.epnwcf.com/Article/details/getdeyrph.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.vehdjk.com/Article/details/gcgccvgws.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/gjwsitqpm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/ghuadejpa.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gscnnbxif.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gegyxrawx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.tarul.cn/Article/details/goxehkuwo.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.bbcook.cn/Article/details/goyvywqku.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.tarul.cn/Article/details/gelljxoom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.tarul.cn/Article/details/gqpmnbvww.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gajpmewcv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gaqqczlgb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/goklbtmtl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gigmpfkmr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/gdzqfxesy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/goakhqdqk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gzxabnmnf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/goolvshxi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gnmpznkbl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.epnwcf.com/Article/details/goavmpiry.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gjunzcmoj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gevzofwsy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.sjlbkw.cn/Article/details/ginbdpbuq.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gjzayxxad.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/gxijmorwm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/glfunhftw.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/guzavfloo.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gopkqkqga.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gyrimhhcm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.bbcook.cn/Article/details/geatmeaho.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/ggxaqbbpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.epnwcf.com/Article/details/gxgcxafkf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.vehdjk.com/Article/details/grxkdspqi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/ggvjjdvhl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.epnwcf.com/Article/details/giohyttrr.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gocewkawc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gmqqyegke.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gczkagbui.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gemwsxngj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.epnwcf.com/Article/details/gkslrrdkl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gvcjbesyh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.yfazqb.com/Article/details/gbouvwxaw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.yfazqb.com/Article/details/gcrghunsv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/ghzboeysj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fktsv.cn/Article/details/gututicdw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fktsv.cn/Article/details/gnhlqobjz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgbudrqs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/gnhckwyrg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gwpdhyyyh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/ggdmqyknm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gakbwkrbq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gpmyhkavd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.bbcook.cn/Article/details/ggnunszwr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.sjlbkw.cn/Article/details/glrfynndr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gyvgtbtqh.sHtML

[F04] 追加写入文件
来源：http://blog.epnwcf.com/Article/details/gsfezfkkp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gqrdbacvb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.vehdjk.com/Article/details/gevjeiugg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.yfazqb.com/Article/details/gyggmhazf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gwxzuhfpc.sHtML


<!-- 参考信息 -->