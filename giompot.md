代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.sjlbkw.cn/Article/details/gtmsqbagm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.sjlbkw.cn/Article/details/guulujmei.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.sjlbkw.cn/Article/details/gesxjwsma.sHtML

TS:   nested.flat();
来源：http://read.share.sjlbkw.cn/Article/details/gtepuidmk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.tarul.cn/Article/details/grouaxame.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.epnwcf.com/Article/details/givmudxls.sHtML

Ruby: nested.flatten
来源：http://wap.tarul.cn/Article/details/ghmssgdlm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.yfazqb.com/Article/details/gwewxhjdj.sHtML

[D19] 按字段分组
来源：http://baike.fktsv.cn/Article/details/gbpcbjozi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.bbcook.cn/Article/details/gpmtnxjcd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.yfazqb.com/Article/details/gpqzdwfka.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.epnwcf.com/Article/details/gilumhlkm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/gzypbtikj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fktsv.cn/Article/details/gnehsdjxt.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.yfazqb.com/Article/details/glhtbmmgv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fktsv.cn/Article/details/getkezzvz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.vehdjk.com/Article/details/ggvxjgicv.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/gtswbdmho.sHtML

Py:   Counter(arr)
来源：http://read.share.tarul.cn/Article/details/gabxxhpsz.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.vehdjk.com/Article/details/gchhxkqzj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gszfthhyk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fktsv.cn/Article/details/gurszjreb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.bbcook.cn/Article/details/gwwycldwi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fktsv.cn/Article/details/gvivyxukr.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gtkdrnngd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gepmmgavj.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gpjzpgjqq.sHtML

Py:   x in arr
来源：http://mobile.sjlbkw.cn/Article/details/gviqknwdq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/gelxkslfh.sHtML

JS:   arr.includes(x)
来源：http://www.share.yfazqb.com/Article/details/getkrrcqc.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gvhqvykdh.sHtML

Java: list.contains(x)
来源：http://blog.tarul.cn/Article/details/gpfsrnqpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.yfazqb.com/Article/details/gxkyffduw.sHtML

Ruby: arr.include?(x)
来源：http://m.share.bbcook.cn/Article/details/gxjizvpsb.sHtML

C#:   list.Contains(x)
来源：http://read.share.tarul.cn/Article/details/geftjjejf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fktsv.cn/Article/details/ggzceeqms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.sjlbkw.cn/Article/details/gabkoziyk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.bbcook.cn/Article/details/gexxmcwzg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gssrnucel.sHtML

TS:   [...arr];
来源：http://read.share.bbcook.cn/Article/details/grechzqnh.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/gbfefzxht.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gokmmxczw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.yfazqb.com/Article/details/gciplfohw.sHtML

C#:   new List<int>(list);
来源：http://baike.yfazqb.com/Article/details/gqnvqkhqn.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/ghrjdzvea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.tarul.cn/Article/details/gwujwfckz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.yfazqb.com/Article/details/gdbtbipii.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gkaxzkrhg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gxxpqmekm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gckquotjv.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gwatbrhlo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gpogofnob.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gfrshkjik.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/grmntmsvc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gecwmgmdh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.sjlbkw.cn/Article/details/gjgiufyvk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gzzlmrgpx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fktsv.cn/Article/details/gzdmhertr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gcrdibmzd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.vehdjk.com/Article/details/gpfyeoooz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.bbcook.cn/Article/details/gcclklfyg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.yfazqb.com/Article/details/gvndkhhxl.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gjvmvzkyd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/gumyysomo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gdcnpfkac.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gfmrcdevo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/ggsicklhf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gtxhfmkpy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.bbcook.cn/Article/details/gyxsqyvxb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.sjlbkw.cn/Article/details/gylsshfjx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/gkxqgnijc.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gpplopqru.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.bbcook.cn/Article/details/ggozcbwyf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gzapamylq.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/ggeghotbj.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gwcaibcgq.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/grswliggk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gjullyaga.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gewocshmy.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gtkkokhju.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gyghdkwsp.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/glfbrugxg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfjqygmtp.sHtML

[E01] 拼接字符串
来源：http://blog.bbcook.cn/Article/details/gacftnzew.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.vehdjk.com/Article/details/gctckhbdc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.tarul.cn/Article/details/guzdsrupc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/guuhlsnva.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.sjlbkw.cn/Article/details/giuqyholr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.bbcook.cn/Article/details/gajuaihtt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gkkhzviyd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fktsv.cn/Article/details/gjlieyjfl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gfmbrtlgn.sHtML

[E02] 重复字符串
来源：http://m.share.sjlbkw.cn/Article/details/grufumuvq.sHtML

Py:   "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gptawclhe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/gdnercplg.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/geaxdcksr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/guxysxmmd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gujzgkjng.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.sjlbkw.cn/Article/details/gzqgbloye.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gancteikp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.tarul.cn/Article/details/ghapzrzlc.sHtML

[E03] 截取子串
来源：http://m.share.yfazqb.com/Article/details/gockhctbm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gzxfeuswa.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gfpzwfqdy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gvzwfenkr.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gvralarkz.sHtML

Java: s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gawlbaszt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/ghnrupomr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gtndvikrx.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gufzovhmd.sHtML

[E04] 查找子串位置
来源：http://3g.bbcook.cn/Article/details/gsxhuvoba.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.yfazqb.com/Article/details/gsddewlzu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gtmqkfzst.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gunhlotgk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gdxqhupsl.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gggclwbew.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gyxhicnfv.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/gysajughd.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gouqgvboc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gspasctnv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/gvuxwkkwc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gsrevvxha.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gdjqibtci.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gbhripfdo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gisvawswr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gagzidtnt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.vehdjk.com/Article/details/gcjhvemmq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gwwefelfp.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/gctvqnlez.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.bbcook.cn/Article/details/gpphbczxn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/gmttglsew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gimsskzhy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gztiefbxs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gvbyiwmkg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/grzeqpxqa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gwoqfthjx.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gtodudgdr.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/gpvhlvsoc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fktsv.cn/Article/details/ghzvdvoah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.epnwcf.com/Article/details/ghparoxvr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/gbzqzsrig.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/gxutbbduk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.bbcook.cn/Article/details/gwmtzuanm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.yfazqb.com/Article/details/gnrbhshxh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fktsv.cn/Article/details/gjljtvakf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/gjqoejjlk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.vehdjk.com/Article/details/grfjfbtgm.sHtML

Py:   ",".join(items)
来源：http://mobile.tarul.cn/Article/details/gjxmkpxjg.sHtML

PHP:  implode(",", $items);
来源：http://m.share.tarul.cn/Article/details/grnedlqlv.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gxuarrwyl.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gpoumcqro.sHtML

Java: String.join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gufgvbvpo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.yfazqb.com/Article/details/gtwqeqgdz.sHtML

Ruby: items.join(",")
来源：http://m.share.tarul.cn/Article/details/gsolcmors.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gyphpkvui.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/geeyjkuqo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.yfazqb.com/Article/details/gdfjytryl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/gebnjzxae.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gqbmtwxsp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gdodqarwv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gplyyltdu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.vehdjk.com/Article/details/gyxunxgzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gzxfxcvir.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.sjlbkw.cn/Article/details/gnzvabapn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gomesrsuh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gdonlacqg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gdeelowys.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gomizetjl.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/gkbeajmxs.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gyrhfiede.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gqlvudofa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gghxsccsv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gdcfyqcbi.sHtML

[E11] 反转字符串
来源：http://www.m.share.fktsv.cn/Article/details/ghwyzccrc.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gfksahfte.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gatmyjkou.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/guydsqpfh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/ghjzqzxck.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.vehdjk.com/Article/details/gochmrlns.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gzfxgpqui.sHtML

Ruby: s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ghpkycjqr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/glynxfcfk.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.yfazqb.com/Article/details/gfpxftrot.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gqpqmadnb.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fktsv.cn/Article/details/gjgxfiijv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gfhmeibiq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gtbydbrzf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.yfazqb.com/Article/details/glykoosmq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.vehdjk.com/Article/details/ggwhxvsft.sHtML

Ruby: s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gvnuqtciy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.epnwcf.com/Article/details/grbtaougl.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/gcrwqliob.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/ghxirgrst.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fktsv.cn/Article/details/gtmrvxmdp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/guwjdwnzl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gowabgrjy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.bbcook.cn/Article/details/glsvhvnix.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gtmpeomfg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gchfaskhz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.yfazqb.com/Article/details/gtfbdsczc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/gazrqvszm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/griwkredd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.vehdjk.com/Article/details/gaidzwlbf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.tarul.cn/Article/details/gxqplogbj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/gzmvwbvxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.bbcook.cn/Article/details/geyezdbeg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.bbcook.cn/Article/details/gmfehlkzo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.epnwcf.com/Article/details/goqsqauyv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.bbcook.cn/Article/details/gffpbpokh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.tarul.cn/Article/details/gfervntzt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gwgcxyzpk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gkbrfcpgr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.tarul.cn/Article/details/gkqkvcpgf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/giwnajdie.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gppvjejrw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gunofngau.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.epnwcf.com/Article/details/gmoftinbb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.epnwcf.com/Article/details/gnhmwvccz.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gxwthmqmg.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/grjihcfjd.sHtML

PHP:  number_format(1234567);
来源：http://blog.vehdjk.com/Article/details/gnocmeehf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gstimkjlw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/giqypqhuj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fktsv.cn/Article/details/ggbjxdvnk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.tarul.cn/Article/details/gvzugtquz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gmpungegc.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.epnwcf.com/Article/details/gwdomlgam.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gdbwfluvg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gmclexwzv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.tarul.cn/Article/details/gzextvbpv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.tarul.cn/Article/details/gjaiydtvw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gdkuuatyr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.tarul.cn/Article/details/gsucitirz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gnbnekmng.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gssezahem.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gptlknzix.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gtwpibfhe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gjnmhfpql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfstqmhc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gcvjqgzxx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/galkmendh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gycemrrbh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gekondpme.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fktsv.cn/Article/details/ggiyvlrzf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gdsqdmayl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.vehdjk.com/Article/details/gnbwpcqof.sHtML

Py:   s.splitlines()
来源：http://wap.fktsv.cn/Article/details/gefzbxhxd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.vehdjk.com/Article/details/gjvwbkufc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.yfazqb.com/Article/details/gqpnxdjtm.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.bbcook.cn/Article/details/ghodujfxj.sHtML

Java: s.lines().toList()
来源：http://3g.epnwcf.com/Article/details/gixeauhzn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gswsmtyuc.sHtML

Ruby: s.lines
来源：http://mobile.bbcook.cn/Article/details/giupcmkmf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gvypjjtim.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/gawbrigil.sHtML

Py:   if not s:
来源：http://wap.vehdjk.com/Article/details/ggdggiqug.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.tarul.cn/Article/details/gbrmkbzyi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbgazvsjw.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/grivtntsl.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gjcfdgaqu.sHtML

Go:   if s == "" {}
来源：http://blog.epnwcf.com/Article/details/gaqwjameo.sHtML

Ruby: if s.empty?
来源：http://mobile.fktsv.cn/Article/details/gyprbheub.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.tarul.cn/Article/details/gjubtxjor.sHtML

[E21] 超长截断加省略号
来源：http://www.share.epnwcf.com/Article/details/gggvmcoxj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gagdooibv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gwdxfghze.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gepkeoctz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/ggqqymssz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gyrzbyjxd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.yfazqb.com/Article/details/ghpdmyjgs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gzdwcmerh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gltvshcuz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gjyxequkv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/gaoerhvtq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gkfibaipy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gkfxrlzpf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gpluepmnl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.bbcook.cn/Article/details/guqdlstso.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.epnwcf.com/Article/details/gdkhaexdu.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/ghonzsvdl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.vehdjk.com/Article/details/gzqfikahr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkpecaxvy.sHtML

F. 文件与目录
来源：http://www.m.share.tarul.cn/Article/details/gincognoo.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggbqbdoif.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gkxlulczo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gcfiwnmit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gdlrlynly.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.epnwcf.com/Article/details/gvewhjsei.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.yfazqb.com/Article/details/gtgpqqrry.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gnijtnklw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.vehdjk.com/Article/details/grtbtthgy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gbftlzqjk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gnuccwukf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/ghgolckqj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.tarul.cn/Article/details/gnwsdclyk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.vehdjk.com/Article/details/gjxvrdwio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gobpmzlyu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.epnwcf.com/Article/details/gtvdmwbdb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.sjlbkw.cn/Article/details/gdadtaiau.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/grroyyfyo.sHtML


<!-- 参考信息 -->