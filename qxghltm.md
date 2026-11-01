代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gealxxdbh.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.sjlbkw.cn/Article/details/gyzdannby.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.sjlbkw.cn/Article/details/gqokkbyuf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.sjlbkw.cn/Article/details/gdvsanona.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.tarul.cn/Article/details/gkejovxir.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.vehdjk.com/Article/details/gymarolip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.tarul.cn/Article/details/gwpkwlfof.sHtML

TS:   nested.flat();
来源：http://blog.vehdjk.com/Article/details/ginkgztjz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fktsv.cn/Article/details/gdxmakedt.sHtML

Go:   // 手写双层循环
来源：http://www.blog.tarul.cn/Article/details/gcbjvebkk.sHtML

Ruby: nested.flatten
来源：http://mobile.bbcook.cn/Article/details/gmfdarltx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.tarul.cn/Article/details/gdribyszh.sHtML

[D19] 按字段分组
来源：http://3g.epnwcf.com/Article/details/ghpgmlasx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.epnwcf.com/Article/details/greuswjnc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.bbcook.cn/Article/details/gvxcvqwzr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fktsv.cn/Article/details/gdnmscmwr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gjevdxrwb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.vehdjk.com/Article/details/glgkprjhk.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.bbcook.cn/Article/details/gcvdozlgu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.yfazqb.com/Article/details/goijreuys.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gxfbyuvjw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.vehdjk.com/Article/details/gvpyktqaw.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gkqcmwixe.sHtML

PHP:  array_count_values($arr);
来源：http://blog.vehdjk.com/Article/details/gubfwhzql.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fktsv.cn/Article/details/gccpepcsa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.sjlbkw.cn/Article/details/gubxbgfxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gpknxxzwd.sHtML

Go:   // 手写 map[T]int
来源：http://3g.yfazqb.com/Article/details/gptdzaegw.sHtML

Ruby: arr.tally
来源：http://baike.yfazqb.com/Article/details/ghhsoclyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.epnwcf.com/Article/details/geaotwykq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.bbcook.cn/Article/details/gybjzedad.sHtML

Py:   x in arr
来源：http://www.share.fktsv.cn/Article/details/gutwhzfnt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/gxmpffehv.sHtML

JS:   arr.includes(x)
来源：http://www.blog.sjlbkw.cn/Article/details/ggtlgnfkc.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/ghtsvdcfo.sHtML

Java: list.contains(x)
来源：http://mobile.fktsv.cn/Article/details/gqiosuwqu.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.tarul.cn/Article/details/gqynnsgpp.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gvfrykxlq.sHtML

C#:   list.Contains(x)
来源：http://baike.fktsv.cn/Article/details/ghwjcotrp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.bbcook.cn/Article/details/gkrzuqwyw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gewwxfqnf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gocqsikic.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.vehdjk.com/Article/details/ghttkddqi.sHtML

TS:   [...arr];
来源：http://baike.tarul.cn/Article/details/gukexatif.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gzrbfwpvs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.bbcook.cn/Article/details/gvidtqbse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gekwozfov.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gjnzpiqyk.sHtML

[D23] reduce 累积计算
来源：http://www.share.sjlbkw.cn/Article/details/gskaduozv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.yfazqb.com/Article/details/giijrezor.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/guqqfvfzy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.bbcook.cn/Article/details/gftiisudx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.sjlbkw.cn/Article/details/glmhkhmax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.yfazqb.com/Article/details/griywpjhi.sHtML

Go:   // 手写循环
来源：http://mobile.vehdjk.com/Article/details/gmhhknjqz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.bbcook.cn/Article/details/gjrurnbao.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/gvjqijjrw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.tarul.cn/Article/details/gftwfblcg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gjppdxebq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gdrxiruvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/goeexjkgl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.epnwcf.com/Article/details/gnjnisnic.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.epnwcf.com/Article/details/glyyqkfzz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fktsv.cn/Article/details/gywvhmivx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gvicjawod.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.tarul.cn/Article/details/gtbfcrvqp.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/glwhxdvbm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gddduquom.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.bbcook.cn/Article/details/gewexsekx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/gypxodqqk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.epnwcf.com/Article/details/gmzidpucg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.tarul.cn/Article/details/gjthftudl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.yfazqb.com/Article/details/gbedmyazs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gbyuklnnw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.epnwcf.com/Article/details/gpklozceo.sHtML

[D26] 数组转字符串
来源：http://wap.bbcook.cn/Article/details/gjbnogyrt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/grsdgwvwy.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/grltnubdj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gkrjorhfn.sHtML

TS:   arr.join(", ")
来源：http://wap.vehdjk.com/Article/details/gwjbhwiph.sHtML

Java: String.join(", ", list)
来源：http://3g.bbcook.cn/Article/details/gbhgpculc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.epnwcf.com/Article/details/ghiknpwqk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/grzburzbm.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gzxunubqy.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gypcxvhey.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gjfaxhhyg.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/goufapvfb.sHtML

[E01] 拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gwyhjbdec.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.vehdjk.com/Article/details/gjtqtkfvc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gzpkpixeo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gvpshshuh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gxyruvlrm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.sjlbkw.cn/Article/details/gjpckxdfu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.bbcook.cn/Article/details/gmzclbbno.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gxrntezlq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.vehdjk.com/Article/details/giuoejcdp.sHtML

[E02] 重复字符串
来源：http://read.share.epnwcf.com/Article/details/gmmmaimhb.sHtML

Py:   "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/gylwdygua.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gqvbzkfrs.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gmmgtaamz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/guiopqmxj.sHtML

Java: "ab".repeat(3)
来源：http://3g.bbcook.cn/Article/details/gvziozino.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gpefpfhqx.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/gakiwxqha.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fktsv.cn/Article/details/gjwzpqspq.sHtML

[E03] 截取子串
来源：http://read.share.tarul.cn/Article/details/ggtmsbtwi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/ggsjpwsyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gvhmedhff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/grryrrpyd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fktsv.cn/Article/details/grcnifvhu.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/ggragslxr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.tarul.cn/Article/details/goaxskebi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gpveyhmfd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/gmqvqwdsi.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/gzxiklzuf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.yfazqb.com/Article/details/goieemloy.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.epnwcf.com/Article/details/gdobscemb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.yfazqb.com/Article/details/ggqcyjrel.sHtML

TS:   s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/gesphjfcp.sHtML

Java: s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gwqxueqxa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gabikrvgy.sHtML

Ruby: s.index("x")
来源：http://m.share.yfazqb.com/Article/details/gcmoupfoc.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.sjlbkw.cn/Article/details/gxihesjpp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gvxejvjhw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbelsymv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.sjlbkw.cn/Article/details/gphjdzukp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/glpatqicp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gglmbseho.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gduaptvgf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fktsv.cn/Article/details/gfgnxwuwq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.yfazqb.com/Article/details/gxovmipdu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.vehdjk.com/Article/details/goxjdpwbh.sHtML

[E06] 替换子串
来源：http://blog.bbcook.cn/Article/details/gjvxuwupn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gvhsvpstq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.epnwcf.com/Article/details/gttgbqkna.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/garrwfxgl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.bbcook.cn/Article/details/gvrkzgmvz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/ggqugkjyv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.bbcook.cn/Article/details/grqtwxgws.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/gyjmflsrs.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gwcjgmgza.sHtML

[E07] 按分隔符拆分
来源：http://mobile.bbcook.cn/Article/details/girqoxkmb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.epnwcf.com/Article/details/gpyptkxrp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gpiwurdqv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/gjawvfsan.sHtML

TS:   s.split(",")
来源：http://blog.tarul.cn/Article/details/gptreratx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/gbjukbasv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.bbcook.cn/Article/details/gvywhupoy.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gxrzgxftx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.bbcook.cn/Article/details/gswllykkf.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/giquenvui.sHtML

Py:   ",".join(items)
来源：http://read.share.tarul.cn/Article/details/gkkyvsykt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gnnfpdtxl.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gwfnmparw.sHtML

TS:   items.join(",")
来源：http://baike.tarul.cn/Article/details/gqcehngpg.sHtML

Java: String.join(",", items)
来源：http://mobile.vehdjk.com/Article/details/gsyumivla.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.yfazqb.com/Article/details/gfoxrnsdv.sHtML

Ruby: items.join(",")
来源：http://3g.epnwcf.com/Article/details/gitgpyqmf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gwpzuupoe.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.yfazqb.com/Article/details/gvflbbssh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gbbfcueuw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fktsv.cn/Article/details/gkppburun.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.sjlbkw.cn/Article/details/gbfoucxkt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/grzjrglrq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gizxsgcnr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gkxsfzbax.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/gbqvjppxc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gddjebeva.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gjtlsyavm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gsuimxaka.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gawbovmhp.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/ghecdqpji.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/graoztfsg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gjzvkbdsf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gthitpxzy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/gpiblgqtc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.bbcook.cn/Article/details/gdrxgjpsb.sHtML

[E11] 反转字符串
来源：http://3g.tarul.cn/Article/details/gqnjuyuml.sHtML

Py:   s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gguiswvlr.sHtML

PHP:  strrev($s);
来源：http://3g.epnwcf.com/Article/details/gmmuohmvs.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/ghgirdgyv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gnvmgjars.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gdqitjnxm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.tarul.cn/Article/details/gqpzyojei.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/glzrsbmlv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gkixdtiaj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gqsshktgk.sHtML

Py:   s.count("a")
来源：http://wap.sjlbkw.cn/Article/details/guovaoghj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gzqzfcjjc.sHtML

JS:   s.split("a").length - 1
来源：http://blog.yfazqb.com/Article/details/gwgondene.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gtmcurymv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.tarul.cn/Article/details/girlfcvxh.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.epnwcf.com/Article/details/gitargxem.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gqmgoianl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gvvnurfka.sHtML

[E13] 逐字符遍历
来源：http://www.share.yfazqb.com/Article/details/gonbhameq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/goxbktfag.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gzzcqgomr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gtjjqtrnj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/gdgbigztl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gexyfrelp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gxusfomex.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/ghkcjlnfz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/gyfkwkcwv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fktsv.cn/Article/details/gmotyfrtx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gvdkuprfe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fktsv.cn/Article/details/ghesbyunx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/gprmshist.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.sjlbkw.cn/Article/details/gbxdkpxkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/ggepjlbth.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gsirsphoy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.bbcook.cn/Article/details/gpsjqcpeq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.tarul.cn/Article/details/ghcxotywb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/gduzkdihn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.vehdjk.com/Article/details/grmqdrjtp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/gpeslfywo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqqcpueze.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gstbjxiof.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.yfazqb.com/Article/details/guhyfqohr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/glekffggu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.bbcook.cn/Article/details/gjpvamiwi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/gshkxrlqh.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gfxqcjfsc.sHtML

Py:   f"{1234567:,}"
来源：http://wap.epnwcf.com/Article/details/gqgcsqpha.sHtML

PHP:  number_format(1234567);
来源：http://mobile.epnwcf.com/Article/details/goylyrcvw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gvbbxqsdd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.vehdjk.com/Article/details/grcqdgrpo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.epnwcf.com/Article/details/gmqehwkpu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/grmedeuhk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.yfazqb.com/Article/details/gzjwdbuen.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fktsv.cn/Article/details/guqgyxopm.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/gpnwguxcr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gmcglcwcx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.bbcook.cn/Article/details/glyhouxbu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gvixjewgg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.tarul.cn/Article/details/gnzbzmztf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gaoiaftrt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fktsv.cn/Article/details/gsivdrfky.sHtML

Ruby: s.capitalize
来源：http://www.blog.epnwcf.com/Article/details/gsdiuovbi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.epnwcf.com/Article/details/gbicfwxnv.sHtML

[E18] 模板占位符替换
来源：http://www.blog.tarul.cn/Article/details/gljrfmhuv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gnjnpovps.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.vehdjk.com/Article/details/gikbqhvkl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gpnjgteon.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gkwhvnash.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/grdlmbqau.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/gjivmllak.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.tarul.cn/Article/details/glephkfyf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gvdgdrowo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gvgkzajej.sHtML

Py:   s.splitlines()
来源：http://baike.epnwcf.com/Article/details/gybeoirpl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fktsv.cn/Article/details/gowtasvbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fktsv.cn/Article/details/gsusriurm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gaslclxig.sHtML

Java: s.lines().toList()
来源：http://www.blog.epnwcf.com/Article/details/gedgiwwrz.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/gtfejeqgl.sHtML

Ruby: s.lines
来源：http://www.share.tarul.cn/Article/details/gbujtxqnu.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gydzuzhvw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gjlwkzwuj.sHtML

Py:   if not s:
来源：http://3g.epnwcf.com/Article/details/ggbcnqrys.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.bbcook.cn/Article/details/gtclespdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/ghwospxlp.sHtML

TS:   if (s === "") {}
来源：http://baike.vehdjk.com/Article/details/gnwhdnvgc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gyyovaeuk.sHtML

Go:   if s == "" {}
来源：http://www.blog.tarul.cn/Article/details/gjwsqvffm.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gudbpokkl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.sjlbkw.cn/Article/details/geejnclrp.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/guyhcdlyf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.vehdjk.com/Article/details/gogtvgbwe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/guvonbras.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gnaajvlvn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gtognzuqo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gjmeascix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.bbcook.cn/Article/details/gbazdvoio.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gnlossdvz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/ghwxfjazp.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fktsv.cn/Article/details/gkbsfyxeo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/gyktnixkj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gnqydnypg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gthxcvvru.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.bbcook.cn/Article/details/gbowozauu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gulxcoqmw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.tarul.cn/Article/details/gsajskhju.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gquckkxys.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/gduumlyzo.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gypahuoho.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gjdgbabhd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gtkbqvvmd.sHtML

[F01] 读取整个文件
来源：http://blog.epnwcf.com/Article/details/ggqwrxqti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gpjcjnzpl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gvjsultzd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.bbcook.cn/Article/details/gpkxgxodi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/gtclssofn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fktsv.cn/Article/details/ggzaykwbl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fktsv.cn/Article/details/gvmhnzlla.sHtML

Ruby: File.read("a.txt")
来源：http://blog.tarul.cn/Article/details/gwhfmhhlf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/ggemdvkoj.sHtML

[F02] 逐行读取文件
来源：http://read.share.bbcook.cn/Article/details/gnejuebow.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gxiksiwur.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.sjlbkw.cn/Article/details/gzehcvqhg.sHtML


<!-- 参考信息 -->