代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gyvheynun.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.tarul.cn/Article/details/gngzwvtnp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.sjlbkw.cn/Article/details/gvugkjeoy.sHtML

TS:   nested.flat();
来源：http://read.share.tarul.cn/Article/details/gynmpttpf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.bbcook.cn/Article/details/ghdiocvhe.sHtML

Go:   // 手写双层循环
来源：http://wap.sjlbkw.cn/Article/details/gqzfsuxgx.sHtML

Ruby: nested.flatten
来源：http://mobile.yfazqb.com/Article/details/guhhpjbhy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fktsv.cn/Article/details/gctgvumoq.sHtML

[D19] 按字段分组
来源：http://baike.fktsv.cn/Article/details/ggipqrflv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gxevexydw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.sjlbkw.cn/Article/details/ghjihuadd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gpznepslp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/gzpfnbxtn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gweqiyxiq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/gxavmtilq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gtfqrvcvw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fktsv.cn/Article/details/glmbfubei.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.tarul.cn/Article/details/gfridctnd.sHtML

Py:   Counter(arr)
来源：http://blog.fktsv.cn/Article/details/gggskkwbi.sHtML

PHP:  array_count_values($arr);
来源：http://baike.bbcook.cn/Article/details/gthlsnaxe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/gwuachhde.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.sjlbkw.cn/Article/details/gthtqrwna.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.sjlbkw.cn/Article/details/gdvazpiqf.sHtML

Go:   // 手写 map[T]int
来源：http://blog.tarul.cn/Article/details/gqcrhtpvr.sHtML

Ruby: arr.tally
来源：http://www.share.tarul.cn/Article/details/gzygpwjii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.vehdjk.com/Article/details/gesxwmnrg.sHtML

[D21] 判断是否包含某元素
来源：http://wap.bbcook.cn/Article/details/gynqbkxov.sHtML

Py:   x in arr
来源：http://read.share.sjlbkw.cn/Article/details/gxfhlsicl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.bbcook.cn/Article/details/gkhvcsmfd.sHtML

JS:   arr.includes(x)
来源：http://baike.tarul.cn/Article/details/gjegchwib.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.epnwcf.com/Article/details/galcosqmd.sHtML

Java: list.contains(x)
来源：http://mobile.tarul.cn/Article/details/gzegjrkqh.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gzekuxrac.sHtML

Ruby: arr.include?(x)
来源：http://baike.vehdjk.com/Article/details/gkxilwhph.sHtML

C#:   list.Contains(x)
来源：http://read.share.bbcook.cn/Article/details/gotssfrml.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gtpozdqeu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/gjrfkjzwa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gsxdjicuf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gsdirwlvo.sHtML

TS:   [...arr];
来源：http://www.m.share.vehdjk.com/Article/details/geneepxws.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.bbcook.cn/Article/details/gnyuerbdl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fktsv.cn/Article/details/gycrkoekg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.bbcook.cn/Article/details/gfoemkqmh.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gnpwalvuy.sHtML

[D23] reduce 累积计算
来源：http://blog.fktsv.cn/Article/details/grrorkxzx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.yfazqb.com/Article/details/guynyopma.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fktsv.cn/Article/details/gfarxfnkt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/glhctwtxt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gmesgpnkt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gubrqoyrk.sHtML

Go:   // 手写循环
来源：http://www.blog.sjlbkw.cn/Article/details/gmyetwlif.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.bbcook.cn/Article/details/gdzvbgiqv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.sjlbkw.cn/Article/details/gjqyckkjx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/ghbzpnuqj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gpnfyulxc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fktsv.cn/Article/details/gekzbdrnx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fktsv.cn/Article/details/grhkkisbw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gazbaylqs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.sjlbkw.cn/Article/details/goesnlney.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gvvtixddu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gitfhstcc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.bbcook.cn/Article/details/gvkowbvux.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.tarul.cn/Article/details/gwsrxifwt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gpuhrbgpz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.vehdjk.com/Article/details/gspxloqei.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gtvhbabrl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/glwouwgta.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gcueechhn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/ghdaykyld.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fktsv.cn/Article/details/gvmudwuxj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/ggpnoziwl.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gqlgoduyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gkcqnfbyu.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gpmifbqdl.sHtML

JS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gpemqihye.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gnuolwqrp.sHtML

Java: String.join(", ", list)
来源：http://m.share.yfazqb.com/Article/details/gawihyejr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.epnwcf.com/Article/details/gwrctdapz.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gfteeocgt.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fktsv.cn/Article/details/gdsvvijsk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxfjpaugo.sHtML

E. 字符串处理
来源：http://www.blog.fktsv.cn/Article/details/gwudzrfcj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gqfczwlif.sHtML

[E01] 拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gdtlduynb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.tarul.cn/Article/details/gbfukpbqk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gyleugzrz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.vehdjk.com/Article/details/gitaoeuay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gpacaesht.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.sjlbkw.cn/Article/details/gpfhzgmby.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.yfazqb.com/Article/details/grnieaqcx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.yfazqb.com/Article/details/gtytybdjr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.vehdjk.com/Article/details/guqpfonbk.sHtML

[E02] 重复字符串
来源：http://read.share.bbcook.cn/Article/details/gvonesutj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gmqhnbfoi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gebcklwop.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gbebruvvr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gtsdmckkz.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gqlpgvdku.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gwooypevc.sHtML

Ruby: "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gopmgxtbc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gemdtttcv.sHtML

[E03] 截取子串
来源：http://blog.vehdjk.com/Article/details/glyrtwysz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.epnwcf.com/Article/details/grsdnwlbt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gvnsmeepq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.epnwcf.com/Article/details/gacqhdnbm.sHtML

TS:   s.slice(1, 4)
来源：http://3g.tarul.cn/Article/details/gzsizfwxx.sHtML

Java: s.substring(1, 4)
来源：http://read.share.bbcook.cn/Article/details/gehxfupzg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gorwokltr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/gkmeanfvy.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gspmybook.sHtML

[E04] 查找子串位置
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtqefnei.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gpmuuwgkc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.epnwcf.com/Article/details/gubizjicv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.yfazqb.com/Article/details/gnjfertdv.sHtML

TS:   s.indexOf("x")
来源：http://blog.vehdjk.com/Article/details/gukoqinwa.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gzjlsgxcx.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.vehdjk.com/Article/details/gakzlhdmj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/grzcoroop.sHtML

C#:   s.IndexOf("x")
来源：http://blog.bbcook.cn/Article/details/gsyatasfn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gfnqsadmm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fktsv.cn/Article/details/gskgvvjzl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gavxdqryq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gospqqemj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gfkrfdyoc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gxvzgtsvu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.vehdjk.com/Article/details/geznesajb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.vehdjk.com/Article/details/glsrzuyhu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/gegifxpwc.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gkwjsnjfv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.yfazqb.com/Article/details/gaydtifys.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gjocdislv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gljbcpodg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gpddadpwj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gklcmstse.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gcfahbdqp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gnhduktjv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.tarul.cn/Article/details/gtjdewbyr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fktsv.cn/Article/details/glzxscumk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gocrkevej.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.vehdjk.com/Article/details/gfwckysrj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.epnwcf.com/Article/details/gepfnbcie.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gxzdyfbds.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.vehdjk.com/Article/details/gajzwpmga.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.bbcook.cn/Article/details/gpqtpdoru.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/gdprhcdki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fktsv.cn/Article/details/gpugqlmhw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gslwdfbmt.sHtML

Py:   ",".join(items)
来源：http://3g.sjlbkw.cn/Article/details/gwyostsdv.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/gijefpevd.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gjstlvyhv.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gbvgdmjgr.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gaaofglhm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.tarul.cn/Article/details/goknhsjhq.sHtML

Ruby: items.join(",")
来源：http://read.share.tarul.cn/Article/details/gwvnkfybm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fktsv.cn/Article/details/gojykzycq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gorppozdv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/gxzkmswje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/ggrhbiroa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/gcvhliktj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gfklmfeci.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/gqbbizeba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/gnwuxtmxx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/ggiiiogjq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gsicqfyoe.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/geqiqjdwk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gimeuwmbk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gyualxjcw.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gzdqxtzow.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/glomzgnyt.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gsmndppvl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gehqzhrkz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gfprrwzwa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fktsv.cn/Article/details/gudavglwd.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/gfhidmtxd.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/giglqpyzx.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gcaddxaks.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gzgqqxyvy.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gmgghhmmq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fktsv.cn/Article/details/gqjotbzvx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gtbnmojty.sHtML

Ruby: s.reverse
来源：http://m.share.yfazqb.com/Article/details/gikoiwmxw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gbjrogqax.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gbqqqlash.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gmqqncnxn.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.tarul.cn/Article/details/gycctztsq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.yfazqb.com/Article/details/gujfpjlya.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gpygvainq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gltkmhuhd.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gmgejkthy.sHtML

Ruby: s.count("a")
来源：http://www.blog.tarul.cn/Article/details/grovsiptv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.bbcook.cn/Article/details/gudfiixni.sHtML

[E13] 逐字符遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gcyqmplfe.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.bbcook.cn/Article/details/gxmwjupyg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghhjagytn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gwkyhcmen.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.vehdjk.com/Article/details/govbmpqee.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gdjlxyulc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.tarul.cn/Article/details/gmtctygmt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.vehdjk.com/Article/details/gkptyutnu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/gqofwjzpv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.sjlbkw.cn/Article/details/gwwahujze.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fktsv.cn/Article/details/gnnjzzigj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.yfazqb.com/Article/details/gzkxrrgnh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.vehdjk.com/Article/details/gosmkmusl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/gjpcczxyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gkbdxszlv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gscbuposo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fktsv.cn/Article/details/gvtlqjuzw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.tarul.cn/Article/details/gghivbmhh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.tarul.cn/Article/details/gssyeanre.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/ghwfhwizx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fktsv.cn/Article/details/ggavhecaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.bbcook.cn/Article/details/gokdmwjoj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/gxpsslnqb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gdyjmwkto.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gygyfyhgx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.vehdjk.com/Article/details/ggyojdjrj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.sjlbkw.cn/Article/details/gqcdwydtz.sHtML

[E16] 数字千分位
来源：http://www.share.vehdjk.com/Article/details/gyqupsmlv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.vehdjk.com/Article/details/gdvvljhgl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.sjlbkw.cn/Article/details/gvvernkmc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gbwzndzak.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gzclolhxk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gjsrwiizm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.vehdjk.com/Article/details/gsbzmxewi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.yfazqb.com/Article/details/gldiscvcu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fktsv.cn/Article/details/gqdjtmsqa.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/gewwehvrf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.vehdjk.com/Article/details/gudafnays.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gqkyzywoz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gbnycbtah.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gumfthljm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.vehdjk.com/Article/details/gbsvqctwm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/ggwwidqxu.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gmcikokxh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/gdqrjhkxt.sHtML

[E18] 模板占位符替换
来源：http://mobile.vehdjk.com/Article/details/glhadorme.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gojqibgzt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/grjqyugot.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gywsvorhy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gnxtdlrdd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/ghqshugnb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbcrnftv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/ghimkdjub.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.yfazqb.com/Article/details/gedlnxhjn.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.yfazqb.com/Article/details/grfchbbym.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gvuxnrfjl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.bbcook.cn/Article/details/gceuurquf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gsqvwcmez.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gffgjmxyn.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gwrhxdtmx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.vehdjk.com/Article/details/grbmonkug.sHtML

Ruby: s.lines
来源：http://3g.yfazqb.com/Article/details/gazgktgao.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gxjyhjjeh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/goilcjsfi.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gejammitn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.epnwcf.com/Article/details/gjruyngbt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fktsv.cn/Article/details/gkjnsnqph.sHtML

TS:   if (s === "") {}
来源：http://baike.fktsv.cn/Article/details/gpmyasklo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/giplzjerz.sHtML

Go:   if s == "" {}
来源：http://baike.sjlbkw.cn/Article/details/gausabyti.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gixocxuim.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fktsv.cn/Article/details/gjzrotlrf.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gxvheljhx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.epnwcf.com/Article/details/geingbtdo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gpbezargt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/gxdyukaic.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/geidxqjxk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gynpfhvby.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fktsv.cn/Article/details/gswvrhhxb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.tarul.cn/Article/details/ggyaxfeav.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.bbcook.cn/Article/details/glxsvuqrw.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/gtyhwymyr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/gxivfcihh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gyjizqdlg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.tarul.cn/Article/details/gyrwyajbh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/gkxzksqgm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/gdbxttzod.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gvvhhfxmd.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gqubovqdk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fktsv.cn/Article/details/gzzpawhny.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkexcmqf.sHtML

F. 文件与目录
来源：http://read.share.epnwcf.com/Article/details/gzhhcplos.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkwduvpav.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/gwiceiorh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.tarul.cn/Article/details/gpfalzraa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.tarul.cn/Article/details/gxrxaqfwz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.yfazqb.com/Article/details/gffjzbrtl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/geywpwmml.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gcvwwtxjd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gsuaxcskl.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzvfgokhh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.epnwcf.com/Article/details/gzczgdoud.sHtML

[F02] 逐行读取文件
来源：http://m.share.sjlbkw.cn/Article/details/gkgpiclxb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gdeggzsub.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.sjlbkw.cn/Article/details/gncnvraoz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/ghscuceia.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gpmksikgk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fktsv.cn/Article/details/gsmjmlkfl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.sjlbkw.cn/Article/details/gakavlbhb.sHtML


<!-- 参考信息 -->