代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/gkeihhzni.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.yfazqb.com/Article/details/getilpotq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.yfazqb.com/Article/details/glagfhbui.sHtML

Go:   // 手写循环累加
来源：http://read.share.epnwcf.com/Article/details/gbokqzggh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fktsv.cn/Article/details/gyhslycbe.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.vehdjk.com/Article/details/ggrvgtqkd.sHtML

[D17] 最大值与最小值
来源：http://blog.vehdjk.com/Article/details/ggfmjdbuh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fktsv.cn/Article/details/gxxgpuozy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.yfazqb.com/Article/details/gkrkowukh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fktsv.cn/Article/details/gezhbobln.sHtML

TS:   Math.max(...arr);
来源：http://baike.epnwcf.com/Article/details/ggbtzitmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.bbcook.cn/Article/details/gouddomli.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.vehdjk.com/Article/details/gqvrdfydp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.vehdjk.com/Article/details/gdcnarlmp.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.tarul.cn/Article/details/gvgrwhzzt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.bbcook.cn/Article/details/guebegszb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.bbcook.cn/Article/details/grsktadqj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.yfazqb.com/Article/details/grgwrllrp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.epnwcf.com/Article/details/geikncrpj.sHtML

TS:   nested.flat();
来源：http://www.m.share.fktsv.cn/Article/details/glroiviul.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.vehdjk.com/Article/details/glwybcvpn.sHtML

Go:   // 手写双层循环
来源：http://m.share.fktsv.cn/Article/details/gewooozvk.sHtML

Ruby: nested.flatten
来源：http://www.share.yfazqb.com/Article/details/gayyjppje.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fktsv.cn/Article/details/gqlciggfb.sHtML

[D19] 按字段分组
来源：http://www.m.share.vehdjk.com/Article/details/gpqjyddxo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fktsv.cn/Article/details/guurfeaha.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.sjlbkw.cn/Article/details/gzfoanems.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/glidswuej.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.tarul.cn/Article/details/gojynnrbk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fktsv.cn/Article/details/gmldyzcpt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.tarul.cn/Article/details/gzengtrrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.sjlbkw.cn/Article/details/gagamzxsb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fktsv.cn/Article/details/ggqdcqfxx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gmaawvcpr.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gzgwyiqym.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.bbcook.cn/Article/details/gameyhaqa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.yfazqb.com/Article/details/gusghrswo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/ggkdnibpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/gwnjemqtl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.yfazqb.com/Article/details/gjypjnsug.sHtML

Ruby: arr.tally
来源：http://mobile.epnwcf.com/Article/details/gqjfbpnci.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.yfazqb.com/Article/details/gjgsvwjbs.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.bbcook.cn/Article/details/gycljpvlk.sHtML

Py:   x in arr
来源：http://baike.bbcook.cn/Article/details/gwvpwgace.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/glovprmgm.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/ggwrtqyeo.sHtML

TS:   arr.includes(x)
来源：http://read.share.sjlbkw.cn/Article/details/gcohfykee.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gowbdsfkq.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gyqvwgbld.sHtML

Ruby: arr.include?(x)
来源：http://3g.fktsv.cn/Article/details/gitmjhhcb.sHtML

C#:   list.Contains(x)
来源：http://baike.bbcook.cn/Article/details/gkalsqgvy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.bbcook.cn/Article/details/gbywromif.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.epnwcf.com/Article/details/gtkpicgmt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.sjlbkw.cn/Article/details/gcsvshztv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.bbcook.cn/Article/details/gzxnvaymk.sHtML

TS:   [...arr];
来源：http://mobile.vehdjk.com/Article/details/gmweopvst.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.sjlbkw.cn/Article/details/goxhdtjun.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fktsv.cn/Article/details/gpnhjhxyf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gucgwpnfe.sHtML

C#:   new List<int>(list);
来源：http://3g.tarul.cn/Article/details/gqkbfwqce.sHtML

[D23] reduce 累积计算
来源：http://www.blog.epnwcf.com/Article/details/gnbdmckuw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.tarul.cn/Article/details/ggdxzvlei.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.tarul.cn/Article/details/gddduflyp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gljhzzrpy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gfvpwwotn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/glgairnnj.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gzwhzumuc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.epnwcf.com/Article/details/ggnnytjby.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gxjtyyahs.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fktsv.cn/Article/details/grdzvbtur.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.epnwcf.com/Article/details/gafekubnm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.sjlbkw.cn/Article/details/ghziprvry.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.tarul.cn/Article/details/gzyvhocje.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gsjwjqtbv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.yfazqb.com/Article/details/garixuvyz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gdnpkoqkx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fktsv.cn/Article/details/gfrfhglzw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/gbhutefvv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gccmmabqa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gimbanksd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.epnwcf.com/Article/details/gmcdjxovq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.epnwcf.com/Article/details/gjcddjpie.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gerrinvsa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.tarul.cn/Article/details/gfhtghsde.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.sjlbkw.cn/Article/details/gpvkleuyp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fktsv.cn/Article/details/guxqldcfd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.vehdjk.com/Article/details/gootbqipl.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gfadcckuv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gfodervls.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.yfazqb.com/Article/details/gcfhdsmro.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/giteilusb.sHtML

TS:   arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/gutlbvvyt.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gaxmfjukw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.bbcook.cn/Article/details/ggvashitp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fktsv.cn/Article/details/ggfgeeaup.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gjzvsxpka.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxguqkcix.sHtML

E. 字符串处理
来源：http://www.blog.yfazqb.com/Article/details/gmzjshail.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/genstuyqw.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwlhkmxym.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.tarul.cn/Article/details/gwzuugaly.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gdecndbvl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/grfpzenps.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gcsyaphzn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwzopxrj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/gubyjscth.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gisblvqer.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.yfazqb.com/Article/details/gnegpqcgm.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gryfwkcvz.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gnwbhoujr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/ghkppscbs.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fktsv.cn/Article/details/gfjdoqnkk.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/ggonopeds.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gqaxbshut.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fktsv.cn/Article/details/gvzvscpvc.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/guamsycuf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.yfazqb.com/Article/details/gnvggaopn.sHtML

[E03] 截取子串
来源：http://www.blog.bbcook.cn/Article/details/ggcwqthme.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.vehdjk.com/Article/details/gcajtvyja.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gpmpqaatj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gwnuzgjpf.sHtML

TS:   s.slice(1, 4)
来源：http://3g.vehdjk.com/Article/details/gsuzlankq.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gfmvveqfb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.sjlbkw.cn/Article/details/giktvsypa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.sjlbkw.cn/Article/details/gfxshkijs.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gypyufbgw.sHtML

[E04] 查找子串位置
来源：http://wap.tarul.cn/Article/details/gnboqzlxr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gumikmsxt.sHtML

PHP:  strpos($s, "x");
来源：http://blog.vehdjk.com/Article/details/glhzjjivy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.yfazqb.com/Article/details/grkwzccts.sHtML

TS:   s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gmykucvrl.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gjaburbsm.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gptdluhpb.sHtML

Ruby: s.index("x")
来源：http://baike.vehdjk.com/Article/details/gtoipxtnf.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.vehdjk.com/Article/details/gsuocfvxe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/giaksumgg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gnjcetbip.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/gwrjnquwy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/ggwudzitc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.vehdjk.com/Article/details/gxthdderc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gfrztmizh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.tarul.cn/Article/details/gmrjhyaiw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gnmfzgqyq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gtuvwnlkm.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gdvyuehhs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.sjlbkw.cn/Article/details/gayvzwloj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fktsv.cn/Article/details/gutqjrxsu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gaxmjqluo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gpiuyeavw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gnvcupdhn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gxexwwtcm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gudyehfry.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gxzcrjuot.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gszbqathn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gbnaxyeqm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.vehdjk.com/Article/details/gcxhmzlsv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.tarul.cn/Article/details/gdbuwplqw.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gpudsuupd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.tarul.cn/Article/details/gjbqtktsy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.vehdjk.com/Article/details/gskdtggcn.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.vehdjk.com/Article/details/gsxevxcah.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fktsv.cn/Article/details/geesmyvdm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fktsv.cn/Article/details/gejtwkmfh.sHtML

Py:   ",".join(items)
来源：http://www.share.sjlbkw.cn/Article/details/ggzgoaort.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gzpnryesj.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gwrnwuaun.sHtML

TS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gkfjlmwvq.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gdwsmcire.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gqbzoyggs.sHtML

Ruby: items.join(",")
来源：http://baike.bbcook.cn/Article/details/gbetxooqr.sHtML

C#:   string.Join(",", items)
来源：http://www.share.tarul.cn/Article/details/ggnrfufho.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gwnkpcusz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/gobtwgeor.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.epnwcf.com/Article/details/gqjjejxeg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/goxcynwcm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.yfazqb.com/Article/details/gkbpfjxdb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.bbcook.cn/Article/details/ggwlkzauj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.tarul.cn/Article/details/gwrdrrlwo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.vehdjk.com/Article/details/gasyzqimc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.tarul.cn/Article/details/gimyakvyg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.sjlbkw.cn/Article/details/garqbkuig.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.bbcook.cn/Article/details/gyekqvtgc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.bbcook.cn/Article/details/gpyrsphwk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gfymfofem.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gfyqavubh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gzvbopumd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gnvvyqnks.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gbevthsmo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/gjbrnosjp.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/grwsusyru.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gpieurnrs.sHtML

PHP:  strrev($s);
来源：http://m.share.tarul.cn/Article/details/ggvgjlycq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gnlkpztwb.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gblolwbxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gtubjjkvj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.epnwcf.com/Article/details/guvcpctye.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gsduddeid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gyvljzein.sHtML

[E12] 统计某字符出现次数
来源：http://baike.yfazqb.com/Article/details/gfktuwlqz.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gubaqgecg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gvotwriek.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.yfazqb.com/Article/details/gezypawrf.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gukznishn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/gobrylluq.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gnwtpudyz.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ghymsgpat.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fktsv.cn/Article/details/gbmyveymr.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gnbjqwieu.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/gljbxlwjl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.yfazqb.com/Article/details/gbaagzvua.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gbpfwnvle.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gkpmukdzg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.yfazqb.com/Article/details/gkwiehzet.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gfhbelghb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.sjlbkw.cn/Article/details/gjuollgqq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.epnwcf.com/Article/details/glkdqeihy.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gijfrmkxz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.yfazqb.com/Article/details/glxvqckmr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.bbcook.cn/Article/details/gufwmnwyk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gzhlisego.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.yfazqb.com/Article/details/gvmtosrlh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.bbcook.cn/Article/details/ghnlrblbc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.vehdjk.com/Article/details/gbjlounwp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.yfazqb.com/Article/details/gewoflxap.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gikujdkut.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gsdfctzsx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gqbxkxaxb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gxsuneyaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gsufznugq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/gevevkoqi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.yfazqb.com/Article/details/guuwrotou.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fktsv.cn/Article/details/ghkgufmqj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.vehdjk.com/Article/details/gwvisdbyv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.tarul.cn/Article/details/ghmmfcwfr.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gwyuccozs.sHtML

Py:   f"{1234567:,}"
来源：http://3g.bbcook.cn/Article/details/gcroydwbe.sHtML

PHP:  number_format(1234567);
来源：http://blog.epnwcf.com/Article/details/gnspuggqh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gtfspojdz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gzlnylouc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gktaogrnm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.epnwcf.com/Article/details/gpvqmywfi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gaymrqvyl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fktsv.cn/Article/details/gfehvliei.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gnejcnrsm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gdolxcury.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gxgwjavur.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gjpgrfgtd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gpejzaztr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gimmwnapg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.sjlbkw.cn/Article/details/gdfuhywko.sHtML

Ruby: s.capitalize
来源：http://baike.yfazqb.com/Article/details/ggfffouun.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/growpdjnx.sHtML

[E18] 模板占位符替换
来源：http://baike.vehdjk.com/Article/details/gvmrlpzws.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gqyldhbnq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gygdujlwa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.epnwcf.com/Article/details/gpcosraak.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.tarul.cn/Article/details/gvoitiubm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.vehdjk.com/Article/details/gvwyyrrra.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/ghpwzhdsl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.epnwcf.com/Article/details/gbuaymjdj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gyqyzbpyx.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gnqlnucqd.sHtML

Py:   s.splitlines()
来源：http://www.share.epnwcf.com/Article/details/gpgdhlaku.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.bbcook.cn/Article/details/gulfvkvfk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gfgmbuxbp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.vehdjk.com/Article/details/gngztsckl.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fktsv.cn/Article/details/gmveptzxg.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gpjkwijdh.sHtML

Ruby: s.lines
来源：http://m.share.bbcook.cn/Article/details/ggyfvqero.sHtML

C#:   s.Split('\n')
来源：http://read.share.vehdjk.com/Article/details/gatkriqet.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gfvetpylb.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gqqjepdwv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/glxptpqiy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.vehdjk.com/Article/details/ggmhbuuyq.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gkaednoii.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gwzvjoijm.sHtML

Go:   if s == "" {}
来源：http://mobile.fktsv.cn/Article/details/gbmxkqftt.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gefzgclui.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gcvtwynvz.sHtML

[E21] 超长截断加省略号
来源：http://m.share.epnwcf.com/Article/details/gsfwhejdr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gqlozdnlz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gnvqaermf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/ggfdstybm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/gkmuykqgd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fktsv.cn/Article/details/godempdgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gmlaneoub.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gigwezwud.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gbzhrikrv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gwtbqnbqf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gyucukunh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gxlpdxpbs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/ghwdjliit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gobqtmogy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.epnwcf.com/Article/details/gqiphjits.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gqthxllxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.vehdjk.com/Article/details/gcmsagajl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/ghdpofcnn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/guwryoqru.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/gusluwrsl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gprnxqxtx.sHtML


<!-- 参考信息 -->