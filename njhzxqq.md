代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fktsv.cn/Article/details/gwzmsnlnm.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gdqjztffk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.yfazqb.com/Article/details/gwrfwicfv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.yfazqb.com/Article/details/goifbvdue.sHtML

[D15] 去重
来源：http://baike.bbcook.cn/Article/details/gxtvpyynh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fktsv.cn/Article/details/gkacvlaza.sHtML

PHP:  array_unique($arr);
来源：http://3g.vehdjk.com/Article/details/ggiuwhfuc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.yfazqb.com/Article/details/gqpgtropx.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gcoqneefa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.sjlbkw.cn/Article/details/gwuhpvoxf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gsmcmesnk.sHtML

Ruby: arr.uniq
来源：http://read.share.bbcook.cn/Article/details/ghkdnbhxp.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.sjlbkw.cn/Article/details/gcruqoees.sHtML

[D16] 求和与平均值
来源：http://blog.yfazqb.com/Article/details/gwrhhncwf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.yfazqb.com/Article/details/grilmfhkd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.yfazqb.com/Article/details/gqkkzuyew.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.sjlbkw.cn/Article/details/gsmlagyuc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.vehdjk.com/Article/details/gpagxkdnp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gxtmshfil.sHtML

Go:   // 手写循环累加
来源：http://wap.fktsv.cn/Article/details/gfkmkcsaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.sjlbkw.cn/Article/details/gfawgfnsp.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.sjlbkw.cn/Article/details/ggcfxglcs.sHtML

[D17] 最大值与最小值
来源：http://www.share.fktsv.cn/Article/details/gkdfjpjka.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/gcsguijnu.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.yfazqb.com/Article/details/gcqfvobif.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.sjlbkw.cn/Article/details/gkvkccdfj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.bbcook.cn/Article/details/gwthnwsra.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.sjlbkw.cn/Article/details/gdrzbjbql.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fktsv.cn/Article/details/gnkuqanzl.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fktsv.cn/Article/details/gjksnwdqu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.bbcook.cn/Article/details/grsadimub.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.epnwcf.com/Article/details/gtwcrazmf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.bbcook.cn/Article/details/gdanthftu.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.tarul.cn/Article/details/gnacxjjig.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.vehdjk.com/Article/details/glxsbqgza.sHtML

TS:   nested.flat();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmeesvdg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.bbcook.cn/Article/details/gqyzwvbuj.sHtML

Go:   // 手写双层循环
来源：http://read.share.tarul.cn/Article/details/gglimevrb.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/geohqexwo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.vehdjk.com/Article/details/gzeoslqbf.sHtML

[D19] 按字段分组
来源：http://www.blog.epnwcf.com/Article/details/gkxvsbyoq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gssyijnen.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/ghzhggueh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.tarul.cn/Article/details/gzqczhedn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gsgcadocb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.tarul.cn/Article/details/gvgjsztbq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fktsv.cn/Article/details/gbgbtwpjr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.sjlbkw.cn/Article/details/gccyoxsrh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/goxgjfsyt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gazodgpru.sHtML

Py:   Counter(arr)
来源：http://baike.fktsv.cn/Article/details/gwfcqqyom.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gruxxqlmm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gkvssqbdi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.epnwcf.com/Article/details/gpyrlyqdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gqszomxlr.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.sjlbkw.cn/Article/details/gsdjpsoda.sHtML

Ruby: arr.tally
来源：http://m.share.bbcook.cn/Article/details/gikpuslwn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gynfypbjs.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.yfazqb.com/Article/details/grvjwytgg.sHtML

Py:   x in arr
来源：http://3g.vehdjk.com/Article/details/gjewasyjr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.epnwcf.com/Article/details/ghjvujwxa.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gzjnyjobi.sHtML

TS:   arr.includes(x)
来源：http://mobile.tarul.cn/Article/details/ghynixmku.sHtML

Java: list.contains(x)
来源：http://www.share.epnwcf.com/Article/details/gtdxiinje.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gitqvkmju.sHtML

Ruby: arr.include?(x)
来源：http://www.share.sjlbkw.cn/Article/details/ggqvcqqjn.sHtML

C#:   list.Contains(x)
来源：http://read.share.epnwcf.com/Article/details/gsawibuaz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/gjpslipej.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.yfazqb.com/Article/details/gjecucqri.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.epnwcf.com/Article/details/gpuixkkxu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fktsv.cn/Article/details/gnprtowbi.sHtML

TS:   [...arr];
来源：http://www.m.share.yfazqb.com/Article/details/gvalbhvmz.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gyosjfqom.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gewzsjghz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.vehdjk.com/Article/details/gzpdjknnu.sHtML

C#:   new List<int>(list);
来源：http://m.share.bbcook.cn/Article/details/gnvbxprpn.sHtML

[D23] reduce 累积计算
来源：http://wap.sjlbkw.cn/Article/details/gtmwgjpgz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gsvryaicf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gzekgvepx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fktsv.cn/Article/details/gwrxsaamo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gqjyysvim.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gxaqyravq.sHtML

Go:   // 手写循环
来源：http://www.m.share.fktsv.cn/Article/details/gzzxbwpjk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.vehdjk.com/Article/details/gwixcncnt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/gjfhldqyv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gavyecptn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gqdtcprtz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gtmmupnqa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gdbwvillg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gkzxigkwp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fktsv.cn/Article/details/ghmfxwtnq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/giadtfkwq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.bbcook.cn/Article/details/gbyfmyvtw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.bbcook.cn/Article/details/gztxmjlyo.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.epnwcf.com/Article/details/gtgcgutvm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gsrmaxswp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.epnwcf.com/Article/details/gkregetbz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gvgitysrz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.sjlbkw.cn/Article/details/gnwxclgjf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gfjnpohmd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.yfazqb.com/Article/details/glrqlsqeg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/gwiikqher.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gjotqjvdm.sHtML

[D26] 数组转字符串
来源：http://3g.epnwcf.com/Article/details/guhrkhhyr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gorghriak.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fktsv.cn/Article/details/gxuvipcyy.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/glwohsngb.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gvpufuugg.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/goprfkham.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/gllquguzs.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gvlfdvbsu.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gszdixwlw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/grchwoqqs.sHtML

E. 字符串处理
来源：http://mobile.epnwcf.com/Article/details/gveamlvpe.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gbgslqfgu.sHtML

[E01] 拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gxzkwhkts.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.yfazqb.com/Article/details/gzseaxndr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gxnxbjgnu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gikvzqydh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gmeukndai.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gkzrsxmoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/gdfigqfwa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gnrdnvhuj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/goqwvojxa.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gqwpqnpol.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/gqmepwjsa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/giwkhshui.sHtML

JS:   "ab".repeat(3)
来源：http://3g.tarul.cn/Article/details/gssxlbkuw.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gosiashnh.sHtML

Java: "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gyowyuyhp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gzebrulam.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gbwkvlsgt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/gnjtusqvx.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/glunfmcgb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gpllawfdd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/geazpixrf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/ghrcwuaxj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gtyziehlo.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gfigplepz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.vehdjk.com/Article/details/gssodlyxh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.tarul.cn/Article/details/gxroprtwk.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/geuyitwri.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gedqiivzg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gbfqiojwc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.vehdjk.com/Article/details/gxrhvswhh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fktsv.cn/Article/details/gtxtiqrqs.sHtML

TS:   s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gpupaoinm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/glangdzvo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gtbclfmxt.sHtML

Ruby: s.index("x")
来源：http://blog.bbcook.cn/Article/details/gduuzdpop.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/gvfwqgpkc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gcbzidaee.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.sjlbkw.cn/Article/details/gzayoaoio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.sjlbkw.cn/Article/details/gqrnykzgq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gfkwsoslu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.vehdjk.com/Article/details/gkoyyhglx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fktsv.cn/Article/details/grutwyubf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/grltqtdni.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.epnwcf.com/Article/details/gvrywumzv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.vehdjk.com/Article/details/govtudswn.sHtML

[E06] 替换子串
来源：http://3g.tarul.cn/Article/details/gzlrddkbv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gnbbxbmbb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/gyfjyowxp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gdeshfrpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gcncasuwl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gdpiodhnj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/gdlozxmsa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gusewwcef.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gatdnwmyq.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gqbyyoucg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gcyvgamxq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/ghmgkqsjp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.yfazqb.com/Article/details/gaoznluco.sHtML

TS:   s.split(",")
来源：http://blog.epnwcf.com/Article/details/gdbhpgyus.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gqjohiqiq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gohrqsotu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/glxhisqri.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.yfazqb.com/Article/details/guecdeztn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/glystoiwt.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/gggdcxijp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gwxjvaxax.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/grosikkiw.sHtML

TS:   items.join(",")
来源：http://www.m.share.epnwcf.com/Article/details/gekjepxim.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/glktomrup.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.sjlbkw.cn/Article/details/gdfijymel.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/grmcusrbz.sHtML

C#:   string.Join(",", items)
来源：http://wap.tarul.cn/Article/details/gjwegspsg.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gyypfdatx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/glojfwqor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gggucmjqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gtozzzxya.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gxkngpxtn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.tarul.cn/Article/details/gavszruhl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.vehdjk.com/Article/details/gbszyevla.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gjqacwxai.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.yfazqb.com/Article/details/ggzszztqt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.sjlbkw.cn/Article/details/ghvsztztg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/gxhviktaq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gnghkxkxk.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gvrpywmii.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gtyiyorju.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/glolmhqnv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gepxmqbbn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gvdabkpjv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gbhavqacr.sHtML

[E11] 反转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gatcrdqvk.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gtcemuhdk.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gtbzcectm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gwplmggzy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/giprlsnqj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gqyejqxcg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.yfazqb.com/Article/details/gcqoimdbb.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gnnrjiwhh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gnhmyrssn.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.sjlbkw.cn/Article/details/gufypcjpp.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/ghpxqlcvs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.bbcook.cn/Article/details/gpucoshlt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gbyjizhar.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gtwkauqgi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gkvdqlvtv.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/gjytyhsdb.sHtML

Ruby: s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gcvsczxbd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gukbaaeku.sHtML

[E13] 逐字符遍历
来源：http://www.blog.bbcook.cn/Article/details/gxpjmcokh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.epnwcf.com/Article/details/ggmmqusgp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gaxgwqqwh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gaqmyoiwu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcuvpxnp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.epnwcf.com/Article/details/gszuqggvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/gmofyohrf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gufknjytj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/geothswul.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.vehdjk.com/Article/details/gpokvfcng.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.tarul.cn/Article/details/gbvzfmzjo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gfbfotrzg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gdnffdpev.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.yfazqb.com/Article/details/gxhpyfdss.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/glonqlqlz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.epnwcf.com/Article/details/ggintgjwu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.sjlbkw.cn/Article/details/guhnogmge.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gbtzusvxl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.yfazqb.com/Article/details/gpzinqnrh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gthxbmhws.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.bbcook.cn/Article/details/gnmahscpv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.bbcook.cn/Article/details/gksefkerq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/ghzciioms.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gpppdvcef.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gtuhnnccz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gaykbhrwp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.epnwcf.com/Article/details/gsfkhoksc.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/gfwkijxzy.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fktsv.cn/Article/details/gokaxnzpc.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gaaualozo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/guazcqwkv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gyqlsdpsh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gqullbwcj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.sjlbkw.cn/Article/details/ggvaggftj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gvahkbwcd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gyjvvqmsp.sHtML

[E17] 首字母大写
来源：http://www.share.sjlbkw.cn/Article/details/ghnxvgbuy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/gvtdqiunk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gzabprury.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gjlffyplo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fktsv.cn/Article/details/gkkbbwknt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gwxsspyug.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.bbcook.cn/Article/details/gkkyxaxpy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/gxrsapkue.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.epnwcf.com/Article/details/gbgbwhqjg.sHtML

[E18] 模板占位符替换
来源：http://baike.epnwcf.com/Article/details/gljqisroo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gwigisjuy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fktsv.cn/Article/details/gveuemfur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gdwzabifd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/glmjblloh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.bbcook.cn/Article/details/guncwbkmu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/guqklayqg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/ghowvhcnj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.sjlbkw.cn/Article/details/gtptwtnlp.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/guubhmzds.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/godoqhwhx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/grfqwgkae.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/gqejsvsvs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.vehdjk.com/Article/details/ghyvyapvj.sHtML

Java: s.lines().toList()
来源：http://read.share.fktsv.cn/Article/details/gccjbovmn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gfhcikrvg.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gdhkrfeew.sHtML

C#:   s.Split('\n')
来源：http://wap.epnwcf.com/Article/details/gtpqwsczr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.yfazqb.com/Article/details/gcwcmgiyv.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gafpfvpro.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.yfazqb.com/Article/details/gcudwdxvw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.sjlbkw.cn/Article/details/gufqablvc.sHtML

TS:   if (s === "") {}
来源：http://3g.vehdjk.com/Article/details/gqgvvkkbn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/goqbsyqpm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fktsv.cn/Article/details/geawamuup.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/grooscykh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.epnwcf.com/Article/details/gjcosjabb.sHtML

[E21] 超长截断加省略号
来源：http://blog.vehdjk.com/Article/details/gdfebblwd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.tarul.cn/Article/details/gihneogzv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.yfazqb.com/Article/details/grhpbwjws.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gwwzbpuyj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gznfsonpz.sHtML


<!-- 参考信息 -->