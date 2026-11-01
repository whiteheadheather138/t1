代发 wailian999

[D19] 按字段分组
来源：http://m.share.bbcook.cn/Article/details/gwmjxnmsy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gltapewre.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.vehdjk.com/Article/details/geunuvgoe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.yfazqb.com/Article/details/gvzaitovy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.epnwcf.com/Article/details/gohdnxgrg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.tarul.cn/Article/details/gavuxzwml.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fktsv.cn/Article/details/gdzusxliw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gehujjdqs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.epnwcf.com/Article/details/gtpfysqla.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.epnwcf.com/Article/details/gmrleprou.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/ghstsuxio.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fktsv.cn/Article/details/gnrnxrprn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fktsv.cn/Article/details/gtpbcupqf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.sjlbkw.cn/Article/details/gnvoerpak.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fktsv.cn/Article/details/ggdxzafkf.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/ggmnzutcm.sHtML

Ruby: arr.tally
来源：http://m.share.yfazqb.com/Article/details/gyvdsegam.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.epnwcf.com/Article/details/gjwlnpnyn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.tarul.cn/Article/details/gaadwzkli.sHtML

Py:   x in arr
来源：http://baike.epnwcf.com/Article/details/gzvifedsz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.vehdjk.com/Article/details/gfejpsrpf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.vehdjk.com/Article/details/gfygxzdhu.sHtML

TS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/goulkrqhj.sHtML

Java: list.contains(x)
来源：http://3g.tarul.cn/Article/details/gkflzmxtv.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gettvktmn.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gmdnzdxpf.sHtML

C#:   list.Contains(x)
来源：http://m.share.fktsv.cn/Article/details/gvgzqckvo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.yfazqb.com/Article/details/gitictcha.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.vehdjk.com/Article/details/gzzaesnyv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.bbcook.cn/Article/details/gjvluqkos.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fktsv.cn/Article/details/gzblnqlgv.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gneevqxgx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fktsv.cn/Article/details/gjzrlputr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gyaxaaiqw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/gmvzajszr.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gigmfqcew.sHtML

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/gnwzzddkp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/ggxtqudfc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/grkcdowqa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gojfpvaxn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gagutwxin.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gjgloclml.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/guljsyqtg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.bbcook.cn/Article/details/gplcvksic.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gaiqystiy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.sjlbkw.cn/Article/details/gjswslkcq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fktsv.cn/Article/details/grawwmqjs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.sjlbkw.cn/Article/details/gjcnqlknq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.bbcook.cn/Article/details/gbcqctpnz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.tarul.cn/Article/details/gkjmmvkyg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/ggupphuad.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.tarul.cn/Article/details/gbfbikvmv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gafrmfjbx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gxlpbtzbk.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.tarul.cn/Article/details/gynuoknqe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.bbcook.cn/Article/details/gjbvsrowl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.sjlbkw.cn/Article/details/gdhwddtgz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/glloosxnq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/guklbhqpm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.epnwcf.com/Article/details/goxfeylwf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.bbcook.cn/Article/details/giszgkohe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/gaweadrjd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/ggvdhpqqg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzdoyxqyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.vehdjk.com/Article/details/gpzddeuoi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/ghutehydg.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gjsxkucra.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gvuhfvxra.sHtML

Java: String.join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gjmbqjupa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fktsv.cn/Article/details/gdiqpkygt.sHtML

Ruby: arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gkqxnodgf.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gdharxblp.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyofczaim.sHtML

E. 字符串处理
来源：http://blog.yfazqb.com/Article/details/gwrhvghjx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjcvtskzr.sHtML

[E01] 拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gxxwvpjxj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gpgldmhxk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.tarul.cn/Article/details/goyaukvew.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.tarul.cn/Article/details/gbdphfxqe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gnfnkkylf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.tarul.cn/Article/details/guoipeyjl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.vehdjk.com/Article/details/grqhhrydt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.bbcook.cn/Article/details/gtjpaxrnt.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gferyaxkn.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/guzxfukcw.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gqexcwbzy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.bbcook.cn/Article/details/gufcprfqb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gopfsrkpv.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gozpazgil.sHtML

Java: "ab".repeat(3)
来源：http://wap.vehdjk.com/Article/details/gpjkbolqf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/ggmbijiym.sHtML

Ruby: "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gofafzilv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/gpwtsbvzl.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gbxnliwpd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gmqjqwzpf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gaunykbtg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gpsbxbjkk.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.sjlbkw.cn/Article/details/gyecgrjxl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsskyfrrn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.vehdjk.com/Article/details/gaqdbcpff.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gntffrlrm.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.bbcook.cn/Article/details/gswlxzoob.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gwrgteivs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fktsv.cn/Article/details/gokwcxubm.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.bbcook.cn/Article/details/gyvlebxol.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/ggqpnbruo.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/ggmbdmjnc.sHtML

Java: s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gbxhcyowg.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fktsv.cn/Article/details/gwhlpdhev.sHtML

Ruby: s.index("x")
来源：http://www.share.vehdjk.com/Article/details/grpszghpv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gocmclnex.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/gcbmrfgja.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/grxsqsmlg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.sjlbkw.cn/Article/details/gphkhafwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gupwvzbic.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.vehdjk.com/Article/details/godluypfc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/ghsjilamm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gqwvicxqg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.yfazqb.com/Article/details/gywogfgsk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gcxctnshz.sHtML

[E06] 替换子串
来源：http://m.share.fktsv.cn/Article/details/gnzzvpzni.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gynersjqo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/gytcmvrnc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gmpqopnhw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gpclnxasv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gmkbxmrnv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/goryuhmga.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gacvgmuhv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gmpugnrvb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gcgrpiybi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gbponovtu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.tarul.cn/Article/details/gkcfnrtfd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gemjnwcrm.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gctunpvpo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gjkqgstmg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/gchpbbrhl.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gbgotfwxc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/griyiuidw.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.sjlbkw.cn/Article/details/giuwsqnmz.sHtML

Py:   ",".join(items)
来源：http://read.share.bbcook.cn/Article/details/gxygcrjui.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gtnkyjcig.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gjitoqssv.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/gigenkhzo.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/genhfaaet.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gczbwctqw.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/guwdinnlp.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.vehdjk.com/Article/details/gqvrxjeml.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gawlpjseo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.epnwcf.com/Article/details/gkvvqjfuh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.epnwcf.com/Article/details/gmqdqspon.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gbvgkzfak.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gcnwuctou.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gapfdlkki.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.yfazqb.com/Article/details/gopsibxvi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.yfazqb.com/Article/details/gkzlchhhy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gdaooctby.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gcwfgecet.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/guistyvvx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.tarul.cn/Article/details/gxksmgkex.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gyxpecucx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.epnwcf.com/Article/details/gcjjxgxtm.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/ggcahoeob.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/ghhzquatw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/glfbxffxz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.sjlbkw.cn/Article/details/gdggvppik.sHtML

[E11] 反转字符串
来源：http://blog.bbcook.cn/Article/details/grzvxvwtu.sHtML

Py:   s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gleeiamkd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gtiukgvfj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/grflllnsy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/ggriksysz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/giazgyxux.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/grhkbweba.sHtML

Ruby: s.reverse
来源：http://baike.epnwcf.com/Article/details/gtfsmnrhy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gcglrxism.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gpqbzwbog.sHtML

Py:   s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gteyxuhjc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.epnwcf.com/Article/details/gjgmrezht.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gbyjfgzeu.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/gmfjfhqms.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/geedxhyqo.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/gwftupcsx.sHtML

Ruby: s.count("a")
来源：http://mobile.tarul.cn/Article/details/gfmxhdqah.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.sjlbkw.cn/Article/details/gbcsyghjy.sHtML

[E13] 逐字符遍历
来源：http://read.share.epnwcf.com/Article/details/gcyulwscb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.vehdjk.com/Article/details/gbnohsspc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fktsv.cn/Article/details/gsxvsjdqq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.bbcook.cn/Article/details/gdhzdeomy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gooekgbzw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gggpulyjq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fktsv.cn/Article/details/gazzkvywv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/gnsowrmog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/glvfrxaqa.sHtML

[E14] URL 编码与 Base64
来源：http://baike.tarul.cn/Article/details/ghpzfozio.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fktsv.cn/Article/details/gannkthmf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.vehdjk.com/Article/details/gbyqkvvyt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.bbcook.cn/Article/details/gucicpubf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gfvslwszj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gdpwbwnbh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/gbjnmhjei.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gdmruerye.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gyyfyaeli.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/ghswhpbzn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.tarul.cn/Article/details/gmzlbsopl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/ggvgxqfdn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/gouivvycs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gtgjrpfwo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.bbcook.cn/Article/details/ghdjeoxft.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gjmnaegnx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.yfazqb.com/Article/details/gazuatifr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/giyswbabr.sHtML

[E16] 数字千分位
来源：http://www.share.fktsv.cn/Article/details/gskjlbvnf.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.yfazqb.com/Article/details/glwedpqnl.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gkohkbxbv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gxxulzmrf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.bbcook.cn/Article/details/gwawtdwbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/gnnvnznzw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.bbcook.cn/Article/details/gaghimdkw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.vehdjk.com/Article/details/glopknuza.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gbwkejick.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gpodkoclm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.vehdjk.com/Article/details/gthnmobfz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.vehdjk.com/Article/details/gwqlnsfrk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/ghoojbmdh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gwnalvuha.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fktsv.cn/Article/details/gzcwuctdq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gliajphom.sHtML

Ruby: s.capitalize
来源：http://wap.bbcook.cn/Article/details/gvrukoqve.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.tarul.cn/Article/details/gcbrszxke.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.tarul.cn/Article/details/gbliymhwy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fktsv.cn/Article/details/gqgnwtnse.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/gxcwluiun.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gzrljsgpy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gnjzqmhqo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/ghgdqnirv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fktsv.cn/Article/details/gjpqlaajn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/geizghsdu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/gvubnzhvp.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.vehdjk.com/Article/details/gnijkaics.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gxejzdpju.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gwchqvqct.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gcpptidmw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gzmgfcykl.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gzwwivtmp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gzjcqukic.sHtML

Ruby: s.lines
来源：http://mobile.tarul.cn/Article/details/gyzgbmvqw.sHtML

C#:   s.Split('\n')
来源：http://read.share.tarul.cn/Article/details/gdipagyzv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gupzmxpid.sHtML

Py:   if not s:
来源：http://www.m.share.epnwcf.com/Article/details/gacabexhr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/geawcmunf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gtlyxxaro.sHtML

TS:   if (s === "") {}
来源：http://www.share.epnwcf.com/Article/details/glldrhjgj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/guzqdyhyb.sHtML

Go:   if s == "" {}
来源：http://www.share.epnwcf.com/Article/details/gxwmojaqe.sHtML

Ruby: if s.empty?
来源：http://mobile.yfazqb.com/Article/details/gkbfzmlwe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.sjlbkw.cn/Article/details/grfahogqb.sHtML

[E21] 超长截断加省略号
来源：http://m.share.tarul.cn/Article/details/gncfazejr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.epnwcf.com/Article/details/gkghhcobx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gqdsouwkq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gmkpvdszz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gpmuppjjq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gvduirlmv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.epnwcf.com/Article/details/gqzrhfpgu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gvhsqpeqv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gkupzjnia.sHtML

[E22] 字节长度与字符长度
来源：http://3g.sjlbkw.cn/Article/details/gnwcvmkdx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/giflyvruw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gdlgakxpc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gscaxjroq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gvtqtploj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gneeoavpd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fktsv.cn/Article/details/gxmpnwkae.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gtjxqlkhf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gwddovzmu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdkscputr.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/gtnoysiuo.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpfiuuoty.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gvzzwzvgv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fktsv.cn/Article/details/gzkcpxtme.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gddcnksxr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.yfazqb.com/Article/details/giuyhifoh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.vehdjk.com/Article/details/gxscywrqu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/ghoayerzm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fktsv.cn/Article/details/gsvfwenkn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/ghqfzqqdy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.yfazqb.com/Article/details/glzysrkdk.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gcewauykn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.epnwcf.com/Article/details/gthscdjqe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.epnwcf.com/Article/details/gdabpvnry.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.vehdjk.com/Article/details/guwoqumrd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gvnllhbmt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.sjlbkw.cn/Article/details/gpqehnqdp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/glsiighoi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.vehdjk.com/Article/details/giabcvtho.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gnckqfmxa.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gititrrgq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.sjlbkw.cn/Article/details/gusyzydup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.bbcook.cn/Article/details/gjctelicy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.sjlbkw.cn/Article/details/gteswauih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/gtvkbttxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gsxkoesnp.sHtML


<!-- 参考信息 -->