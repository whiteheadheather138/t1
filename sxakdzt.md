代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.vehdjk.com/Article/details/gkzejdhol.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.sjlbkw.cn/Article/details/gpwqhorht.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gquzyghfi.sHtML

TS:   nested.flat();
来源：http://blog.yfazqb.com/Article/details/gixbakugo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.tarul.cn/Article/details/gpvyyefqm.sHtML

Go:   // 手写双层循环
来源：http://baike.epnwcf.com/Article/details/gnctekzti.sHtML

Ruby: nested.flatten
来源：http://www.blog.tarul.cn/Article/details/gyruqgxsw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.bbcook.cn/Article/details/gqaeyiaix.sHtML

[D19] 按字段分组
来源：http://m.share.vehdjk.com/Article/details/gqtyushjf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.yfazqb.com/Article/details/gomfmutos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.epnwcf.com/Article/details/glmgtmnem.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.sjlbkw.cn/Article/details/gxhhecejq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gtdfgmcpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.tarul.cn/Article/details/gozxklnfa.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.sjlbkw.cn/Article/details/gnqcqraxo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/gmanrddvq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.yfazqb.com/Article/details/gumnmaecq.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.bbcook.cn/Article/details/gujgzbwcy.sHtML

Py:   Counter(arr)
来源：http://m.share.fktsv.cn/Article/details/gmiequlur.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.tarul.cn/Article/details/grkwnvoso.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.sjlbkw.cn/Article/details/gocnjxtmx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.epnwcf.com/Article/details/gubjlziwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/goaxqbkvl.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/goidywyxt.sHtML

Ruby: arr.tally
来源：http://read.share.vehdjk.com/Article/details/gsqmjxnih.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.epnwcf.com/Article/details/gohnacznj.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gszansxjz.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gongwywkv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.sjlbkw.cn/Article/details/gdflvoguc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fktsv.cn/Article/details/gxkkmozwh.sHtML

TS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gfqskdkfn.sHtML

Java: list.contains(x)
来源：http://www.share.sjlbkw.cn/Article/details/grtkialfy.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.bbcook.cn/Article/details/goecmwnas.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/gtlkeriof.sHtML

C#:   list.Contains(x)
来源：http://m.share.epnwcf.com/Article/details/gmvzseqsa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.epnwcf.com/Article/details/gczlcnyzk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.tarul.cn/Article/details/gxelcqxic.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fktsv.cn/Article/details/gqchxjqjg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/gzfvcxyoc.sHtML

TS:   [...arr];
来源：http://wap.bbcook.cn/Article/details/gnrnekkxd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.sjlbkw.cn/Article/details/gxkfunyrq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fktsv.cn/Article/details/ggmxckwpf.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/ggwsdydys.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/gauzebyyt.sHtML

[D23] reduce 累积计算
来源：http://baike.fktsv.cn/Article/details/gugkphrck.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gzkurwlga.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gkcxbdcaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/gbjfeuxfu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.bbcook.cn/Article/details/gdpyeaaws.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.sjlbkw.cn/Article/details/ggzqafrxf.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gjamrqfeb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gaymmbcoi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/grakawrgi.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.bbcook.cn/Article/details/giozbdpdz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.vehdjk.com/Article/details/gnsjefjit.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gaghhnjtb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gvqdnjwel.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.epnwcf.com/Article/details/gitfrubfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fktsv.cn/Article/details/gdbqkemgi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gqrcgsprl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.bbcook.cn/Article/details/gmsaradpu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gymbhpgpg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fktsv.cn/Article/details/glbdebnfj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gxoknejbp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gicyqmquk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gcrngenpj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gsewqyijq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fktsv.cn/Article/details/ggdiwvaun.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.sjlbkw.cn/Article/details/gccpsmazg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.vehdjk.com/Article/details/gvnmohipr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbjnbbnjn.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/godwxstxg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.yfazqb.com/Article/details/gbipjzknd.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/greinvkie.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gonnstvvo.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gidsykxuf.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gjzifiesb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fktsv.cn/Article/details/gtyocfewx.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/grokvwytd.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gpuzuiucl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggpenkddf.sHtML

E. 字符串处理
来源：http://mobile.tarul.cn/Article/details/gghkqkyeq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/getmwgyhl.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gmvwiaduq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.tarul.cn/Article/details/gudddtlmm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fktsv.cn/Article/details/gliskumuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gkgxaouay.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gfupxbaux.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.epnwcf.com/Article/details/guyuxqexd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.epnwcf.com/Article/details/gzsqilcle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/ggriiscsj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gckrzvzyd.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gvfjkbaui.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/glqpbrwab.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/gwwifoive.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.bbcook.cn/Article/details/grwwkmxvu.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/ggstxhwfe.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gbilykwbc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/gochtfcqw.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/ggtjfxsux.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gkatdktzy.sHtML

[E03] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gpjidzihg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.bbcook.cn/Article/details/galseaazj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gmolvegai.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.vehdjk.com/Article/details/gdmiddhjr.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/giklkqzyc.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/ghpolkesy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/grxfbkvil.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.sjlbkw.cn/Article/details/ghglkfmil.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gubeyofvl.sHtML

[E04] 查找子串位置
来源：http://blog.bbcook.cn/Article/details/gkxtdbtao.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/gobxtwysj.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.yfazqb.com/Article/details/grxqujjzs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.sjlbkw.cn/Article/details/gbttcznou.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/getwrzium.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gaaglqony.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gzmudswfo.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gngtbyrvr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gxngzdvlv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.epnwcf.com/Article/details/grwdrpfun.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.tarul.cn/Article/details/guxmqpblq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.epnwcf.com/Article/details/gtrksygkq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/ggrbvwudh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fktsv.cn/Article/details/gndrbkrmo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.yfazqb.com/Article/details/giftafitt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/guolylney.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/gxkgqqqsh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gutvwwryy.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gsdvthsbh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/grpubzzkf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.epnwcf.com/Article/details/gezbxcvzf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gjoggxaea.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gekdbobrw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvmfmckm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.sjlbkw.cn/Article/details/gnvtclmzn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fktsv.cn/Article/details/guzxfzzhk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gglphvigi.sHtML

[E07] 按分隔符拆分
来源：http://m.share.epnwcf.com/Article/details/gehzhfrny.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gwfdezugw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gvqgknhwv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.tarul.cn/Article/details/glwyvjypb.sHtML

TS:   s.split(",")
来源：http://www.share.bbcook.cn/Article/details/gbztseakb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.sjlbkw.cn/Article/details/gcztdxpfj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.yfazqb.com/Article/details/gjwtwgkef.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fktsv.cn/Article/details/grxwjfual.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.tarul.cn/Article/details/ggtytqhtl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.epnwcf.com/Article/details/gzjflkfjh.sHtML

Py:   ",".join(items)
来源：http://3g.vehdjk.com/Article/details/gydxvqhnf.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fktsv.cn/Article/details/gwkrwwzhx.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gsrcvures.sHtML

TS:   items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gllvoibus.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/grwdievph.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gggqzshgd.sHtML

Ruby: items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gjefrwqsg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gkollpoxe.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/glntzjqvt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.sjlbkw.cn/Article/details/glrsiggpn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/gmepoegvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/gsasvgfpb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.vehdjk.com/Article/details/gzmbpjdsm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gucgehyrz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/goqezeswl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/glamgyotj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fktsv.cn/Article/details/ggitfxpdi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/grkuafxgs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gfvexflet.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gqmfmrkaf.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/gupthddrk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gchnysspj.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/genxavvni.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.vehdjk.com/Article/details/gaqrjbwpt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gpastfimf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.yfazqb.com/Article/details/givxtkhro.sHtML

[E11] 反转字符串
来源：http://wap.tarul.cn/Article/details/gzfvdpijg.sHtML

Py:   s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gktmcdwta.sHtML

PHP:  strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gmhqaglst.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gpcglcbvl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/godfrghgm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.tarul.cn/Article/details/gzghkokka.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gealsimkq.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gnjrnmhry.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gghthcfvh.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gnzdihugz.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gpqcrxcxc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.vehdjk.com/Article/details/gofaqndbs.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/ggfqkbupo.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gttylqowq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.yfazqb.com/Article/details/gsjenhgwa.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gjbaobllk.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gtxjuhoqa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gbxeqncwp.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/ggjnxcnbz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fktsv.cn/Article/details/gmuzodkmy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.vehdjk.com/Article/details/gqxguvbhq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/ghzvvpktp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gaxjpqkzn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.epnwcf.com/Article/details/grusrxasf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.tarul.cn/Article/details/ghoqfzbru.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/gwtiqcjzw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/ggrknooyt.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.tarul.cn/Article/details/gbxoqergk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.epnwcf.com/Article/details/gcoojdleh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/glslmfncm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.bbcook.cn/Article/details/gjgasaogj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.vehdjk.com/Article/details/guyrnqehl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.bbcook.cn/Article/details/gpptrqzzr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.vehdjk.com/Article/details/gorcvmjkn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/ggndfnqkp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gokziasov.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gcwjieogz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gdmumibkq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.yfazqb.com/Article/details/gtpkivzom.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gtevazpxf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.bbcook.cn/Article/details/gxihdaerf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.sjlbkw.cn/Article/details/gjdqmexwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxoqzxjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.sjlbkw.cn/Article/details/gfvtsacuu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.bbcook.cn/Article/details/gfpymbojw.sHtML

[E16] 数字千分位
来源：http://m.share.bbcook.cn/Article/details/golsaqwck.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gxepnxcsf.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gxqwjtqwb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gddlbrovj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gymwnonaw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gzatnccen.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gzxmngkzx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gnrydkrwl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/ghxporhvb.sHtML

[E17] 首字母大写
来源：http://www.blog.bbcook.cn/Article/details/gkcakivpg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gzbrmougm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fktsv.cn/Article/details/gtwnuuxss.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gerlolyzf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gxwfucske.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gshwbjktv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gnqcsmnhw.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/gnqqfhrcx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fktsv.cn/Article/details/gqcgnscuy.sHtML

[E18] 模板占位符替换
来源：http://blog.yfazqb.com/Article/details/gnlfwjxtt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.vehdjk.com/Article/details/gclaigwco.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gnafxpvtq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/guxmfurir.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gavaxcoki.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gnkmvydiw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gfdipvzkt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gdsbypvma.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.epnwcf.com/Article/details/gheslayvh.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.epnwcf.com/Article/details/gjpyasolz.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/ghbunhfkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gjxvpymqa.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/glrhdhyng.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gknhepjql.sHtML

Java: s.lines().toList()
来源：http://m.share.yfazqb.com/Article/details/ghveuwdgx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gobaignwz.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/gibizjbgw.sHtML

C#:   s.Split('\n')
来源：http://wap.sjlbkw.cn/Article/details/gpktxzdiy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fktsv.cn/Article/details/gzxwzidix.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrrcgxnd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.vehdjk.com/Article/details/gcwjhzppj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fktsv.cn/Article/details/gzuwhzwri.sHtML

TS:   if (s === "") {}
来源：http://blog.fktsv.cn/Article/details/gizmskpfs.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gabzrfgeg.sHtML

Go:   if s == "" {}
来源：http://baike.bbcook.cn/Article/details/guhspmfpu.sHtML

Ruby: if s.empty?
来源：http://wap.fktsv.cn/Article/details/gyhuaioib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gcyssxdlj.sHtML

[E21] 超长截断加省略号
来源：http://baike.bbcook.cn/Article/details/gntgcigbe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/guzkewgoo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gjfowevhf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gweyvhsmq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/grmfvruuf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/grudteyui.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gdpqdqkiq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gcgwjjecr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gqmudmdqr.sHtML

[E22] 字节长度与字符长度
来源：http://wap.yfazqb.com/Article/details/gozkmehgq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fktsv.cn/Article/details/gidsbklqy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gogzynoey.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.bbcook.cn/Article/details/gkuflnjbo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gimgeekmo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.sjlbkw.cn/Article/details/graonswcd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/giebjdbnt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gsesixgyr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gankeilhy.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gsunhdbrw.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gfznaibqp.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmlfospbt.sHtML

[F01] 读取整个文件
来源：http://wap.yfazqb.com/Article/details/gcfclksex.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.tarul.cn/Article/details/gmpfdqzuc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.vehdjk.com/Article/details/gtbgeueoe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.sjlbkw.cn/Article/details/ghlngnmhl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/ggnpmwgir.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gjshfbowj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/goxccmpbn.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gndnwdnxo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gnneqcqhz.sHtML

[F02] 逐行读取文件
来源：http://read.share.yfazqb.com/Article/details/gqppbulqr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.tarul.cn/Article/details/ghdlzbafu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.yfazqb.com/Article/details/ghpqhazek.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.sjlbkw.cn/Article/details/gdconjlbo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gpwfcwalz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.tarul.cn/Article/details/gizeoybkw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.bbcook.cn/Article/details/grpuapnga.sHtML


<!-- 参考信息 -->