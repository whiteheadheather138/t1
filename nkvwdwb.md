代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.vehdjk.com/Article/details/gmlhovpfc.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.yfazqb.com/Article/details/ghqmiqkxh.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.vehdjk.com/Article/details/gjctwlniq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gyzkubmjy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.tarul.cn/Article/details/gehqpfova.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.yfazqb.com/Article/details/grvceodbf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.bbcook.cn/Article/details/gdcyictqj.sHtML

TS:   nested.flat();
来源：http://www.share.yfazqb.com/Article/details/gtyzwxgxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/gqpcsctea.sHtML

Go:   // 手写双层循环
来源：http://wap.bbcook.cn/Article/details/gwfvelssm.sHtML

Ruby: nested.flatten
来源：http://m.share.yfazqb.com/Article/details/gujizgekd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.vehdjk.com/Article/details/gcsednwxx.sHtML

[D19] 按字段分组
来源：http://www.share.tarul.cn/Article/details/gqcseomls.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.tarul.cn/Article/details/ghbdyswdu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.bbcook.cn/Article/details/gquofifcn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fktsv.cn/Article/details/gykywfoeb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gjdooebel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.epnwcf.com/Article/details/gvjasvfwp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.sjlbkw.cn/Article/details/gruemeivh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.epnwcf.com/Article/details/gmmtsjmbh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.yfazqb.com/Article/details/glgundfka.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fktsv.cn/Article/details/gmztmrhnf.sHtML

Py:   Counter(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gpjobjoof.sHtML

PHP:  array_count_values($arr);
来源：http://blog.tarul.cn/Article/details/gfzjfhxij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gqrgkedjk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.yfazqb.com/Article/details/gczrvtvmq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.yfazqb.com/Article/details/gluvnmdfe.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.vehdjk.com/Article/details/goxbrxmau.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gluzbaxba.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gnpuswgtq.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gftqkfptj.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gvpyeuikt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.bbcook.cn/Article/details/gobqiygbl.sHtML

JS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gpzupzicg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/gvcnpyokt.sHtML

Java: list.contains(x)
来源：http://wap.epnwcf.com/Article/details/gajdbugyo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gzgqvauit.sHtML

Ruby: arr.include?(x)
来源：http://blog.yfazqb.com/Article/details/grpsdalhi.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gsiozcvee.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gbhaninnm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.vehdjk.com/Article/details/gdjjqwlmy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.sjlbkw.cn/Article/details/ggxdhuuff.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fktsv.cn/Article/details/gtsoygcyy.sHtML

TS:   [...arr];
来源：http://3g.tarul.cn/Article/details/gouzzcqcb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fktsv.cn/Article/details/gyccaqiel.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.vehdjk.com/Article/details/gujxggzgn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gbkxmfcwi.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gbijuahrw.sHtML

[D23] reduce 累积计算
来源：http://mobile.tarul.cn/Article/details/gdjpsfegf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/galhynwag.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gkbvmywtb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gueijshtl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.yfazqb.com/Article/details/gmawtvlft.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/gdvthmemk.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gagjcqqoo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gskawpdek.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gqmzfbtex.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gavqgethr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gviycvuxe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gubxcbrds.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghhqtwlzb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gttgrjxtp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.vehdjk.com/Article/details/goftimavt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gftkrvzoz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gqrprfudf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gvlujxygg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.sjlbkw.cn/Article/details/gaenovifa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gpgntcnsn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbiyewpp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/guidkcsjz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.bbcook.cn/Article/details/gjjqtpnpj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.vehdjk.com/Article/details/gewmiyobt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gsshrskfw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gmttgmena.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gcuamlolr.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gbidouxgm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gnuzzrqpi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.bbcook.cn/Article/details/ggbwbczjf.sHtML

JS:   arr.join(", ")
来源：http://www.blog.epnwcf.com/Article/details/gjmefjknt.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gkykstolp.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/ggawhjlqe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/ghwsgiprw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gsjipljpw.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gbcqsyubn.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gktaudwkp.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/grkqlagud.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gpkjbagqw.sHtML

[E01] 拼接字符串
来源：http://3g.yfazqb.com/Article/details/ghorzungv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gjewfkbir.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/grvxpjofu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gabqxjtqu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gxvadnqap.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.sjlbkw.cn/Article/details/gwavdzjlz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fktsv.cn/Article/details/gbadglgmr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.tarul.cn/Article/details/gfrkssgww.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.vehdjk.com/Article/details/gzcvdqkpz.sHtML

[E02] 重复字符串
来源：http://www.share.bbcook.cn/Article/details/gqelxvvnx.sHtML

Py:   "ab" * 3
来源：http://blog.sjlbkw.cn/Article/details/gghtkjjjq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.yfazqb.com/Article/details/gxbhixcgp.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gaumpqsyh.sHtML

TS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gvvqoamvn.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/ggsdmsfxf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/gxvausqmn.sHtML

Ruby: "ab" * 3
来源：http://blog.fktsv.cn/Article/details/guhznudqj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gtbsegucz.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gjzuhixxd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gzljuthrv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gitjgfyuh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gpnxhkpeq.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gobanibzm.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/ggypomisy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.bbcook.cn/Article/details/guvlmofng.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.bbcook.cn/Article/details/gycslxufn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fktsv.cn/Article/details/gvsmaaomh.sHtML

[E04] 查找子串位置
来源：http://m.share.sjlbkw.cn/Article/details/gfvnsbith.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.yfazqb.com/Article/details/gdvvhwria.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.vehdjk.com/Article/details/gjiunacyq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.epnwcf.com/Article/details/gygbchrcu.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/ggjccywnt.sHtML

Java: s.indexOf("x")
来源：http://3g.epnwcf.com/Article/details/gfpncuqae.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gbaxozivx.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gzhxswafv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gwstagqaf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.sjlbkw.cn/Article/details/gkxibyqbl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fktsv.cn/Article/details/ggjfynjfh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gifuxdpqf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gxegnlybp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.bbcook.cn/Article/details/gaqsnhwcp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/girkcrrkn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gchkxlreg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/grxmewian.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gviclomfi.sHtML

[E06] 替换子串
来源：http://mobile.bbcook.cn/Article/details/gllepqlgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gchhzeeju.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhxgkmyz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gtcleyajn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gnrgydrnc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyculggvn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gpqyfprms.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyptkvgmb.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gmxvvzsac.sHtML

[E07] 按分隔符拆分
来源：http://www.share.sjlbkw.cn/Article/details/gtqqsmuxq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/ggeyzjrpb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.yfazqb.com/Article/details/gwmzdgutx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/grxsahzor.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/golrqfhmw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gtmtynevu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gwtdbbyld.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gensiaejb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fktsv.cn/Article/details/gkgkpxgqr.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.yfazqb.com/Article/details/gtwdoagak.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gauukytsi.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gdwflbrbz.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/ghgryrlfd.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gnasqdlwy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.epnwcf.com/Article/details/gwozggobg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/gnjugfbkc.sHtML

Ruby: items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gkrcttjfu.sHtML

C#:   string.Join(",", items)
来源：http://wap.yfazqb.com/Article/details/gflljaygj.sHtML

[E09] 去除所有空白字符
来源：http://blog.bbcook.cn/Article/details/gfhegdzxj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.sjlbkw.cn/Article/details/gwryiuoda.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gmpyfiwaj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gucwykzug.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gpjgvdwnf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/grpfkjova.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.bbcook.cn/Article/details/gkjphowtm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/gxsubozkb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gsrlkcxao.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/ghybsdzvl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gxjeqcacd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gvxmvkrhk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzavpbnya.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gchavqgdr.sHtML

Java: String.format("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gazpctqyb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/gbsvzjljl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/ghaaeljau.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/gmfwxjfjx.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/giqoctqez.sHtML

Py:   s[::-1]
来源：http://wap.vehdjk.com/Article/details/gtdekfizh.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gbtmzxkls.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gkvsfbokc.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gqpjgtkyv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/gkkvcvcti.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.yfazqb.com/Article/details/grovvzrov.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gpogdzuvn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/ggfjmjzks.sHtML

[E12] 统计某字符出现次数
来源：http://blog.vehdjk.com/Article/details/gcdniodpn.sHtML

Py:   s.count("a")
来源：http://mobile.vehdjk.com/Article/details/gsboshhhy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.vehdjk.com/Article/details/gmrtygffs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gpvskjwnq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/grsnfefcj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.bbcook.cn/Article/details/gzagjklzm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gsbjwlhvt.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gcxhpjonj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.tarul.cn/Article/details/gvvletjjp.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gmusvacdj.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/gxfhgrxfz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.yfazqb.com/Article/details/goeufhymw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/guewohgok.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gqvflqaft.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/geraftydz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gujphydph.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fktsv.cn/Article/details/glusbglnm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gjnhyltpu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gimcqobqm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.epnwcf.com/Article/details/gqaoquyof.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/geixqwmmp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gijpgxnnv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/goetzgnog.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/geijuzsxg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gehstubbh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fktsv.cn/Article/details/gdnimpsbn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gsktbpykp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gfupnaxot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fktsv.cn/Article/details/grgvnilwf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/gnmqfcvey.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.yfazqb.com/Article/details/gmjcjwzmt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpvsvlre.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/gntpgmohn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fktsv.cn/Article/details/gammizzjq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/giwrmjfsy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gstlorzpp.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/getwfpiyr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gpdahzslr.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fktsv.cn/Article/details/gtalzmcib.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.bbcook.cn/Article/details/gnqhjaquh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.yfazqb.com/Article/details/gweanmfmd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gqlopnlcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fktsv.cn/Article/details/gqwdchwhs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.vehdjk.com/Article/details/ggtehgkqt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gpdhyvscv.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gnvftxhnp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fktsv.cn/Article/details/gomfsgwge.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.epnwcf.com/Article/details/gvubxjber.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gjldznuov.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gseaefjuz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.tarul.cn/Article/details/ghxhbiatz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.yfazqb.com/Article/details/gfhpqqcdo.sHtML

Ruby: s.capitalize
来源：http://read.share.vehdjk.com/Article/details/gidfkkdyc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gqvvziexm.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gmzghqzya.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gnbgdmoel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.epnwcf.com/Article/details/gkrkqgblq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gxbmxblep.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gjkakxxpb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/gcmenuzmp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gamrdocdp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.yfazqb.com/Article/details/ggtlrxuno.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/gbrmdbwgq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.yfazqb.com/Article/details/ghjkriivr.sHtML

Py:   s.splitlines()
来源：http://3g.bbcook.cn/Article/details/gpgaurppk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.epnwcf.com/Article/details/gnebscsxa.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gutuganai.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gpdqjixyt.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gxnivgtgu.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gfseyomiu.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/gpyuprvvj.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gzihettve.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gkhzyfadg.sHtML

Py:   if not s:
来源：http://read.share.fktsv.cn/Article/details/gaqmupmng.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.epnwcf.com/Article/details/gerpwwuux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/goqugkhzk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.bbcook.cn/Article/details/gyjdpwxud.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gletzdmrl.sHtML

Go:   if s == "" {}
来源：http://m.share.fktsv.cn/Article/details/guylwajse.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/golzfwsyv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.yfazqb.com/Article/details/gdnfcrtxb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.tarul.cn/Article/details/gtdritysh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fktsv.cn/Article/details/gqqiboast.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gqlirltjn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/grsucvrpp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gcfuuuwio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ghvzxlhkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.tarul.cn/Article/details/gmwjuprzi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/ghggzvmay.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gsswnueef.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.sjlbkw.cn/Article/details/gelnpjxsw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/gzkyorhno.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gnexndrde.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.epnwcf.com/Article/details/gujqfaxhk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gyuskqvyy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfcnclfu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.yfazqb.com/Article/details/ghrukjhad.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.yfazqb.com/Article/details/govkeuoas.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gidpkijia.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gujitmtuk.sHtML

F. 文件与目录
来源：http://mobile.vehdjk.com/Article/details/gqykmwqxh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gleckwsbc.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gixeexocl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.tarul.cn/Article/details/gvhycudia.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gishgrtdw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gsephclvd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.epnwcf.com/Article/details/gvvefnrgl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.yfazqb.com/Article/details/gpbnruaoo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.tarul.cn/Article/details/glebdkobv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fktsv.cn/Article/details/ghwswqhbe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gzmcuwjii.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gkexucsiv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gonpixmjb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/grddbkwhc.sHtML


<!-- 参考信息 -->