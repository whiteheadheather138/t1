代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.blog.tarul.cn/Article/details/gffuwxnmb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gdxjxbzft.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.tarul.cn/Article/details/gkpjlavjm.sHtML

C#:   new List<int>(list);
来源：http://blog.bbcook.cn/Article/details/gnchgzwog.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gwsahhhtb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fktsv.cn/Article/details/glypxxbnm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gqulgiuzs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/ghqocqfqh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gllwyikkg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.epnwcf.com/Article/details/gwdjeeacv.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gcrozfsmh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/gfkmjulyx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gqpfowfsz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.epnwcf.com/Article/details/gawheqjwl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gzzszfbdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/gtzgiznsr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gquswhoww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gcvkdstuy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.yfazqb.com/Article/details/gzgkdwock.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gigvfplsi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/guunsnzpv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gyoahiwdr.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gxogzetbw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.yfazqb.com/Article/details/gdhfvjodb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.sjlbkw.cn/Article/details/glglqefgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gciydmavf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/grxffytqi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.bbcook.cn/Article/details/gnryurieg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.epnwcf.com/Article/details/geleqcqmq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gxbdahfwt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.tarul.cn/Article/details/giwajylyh.sHtML

[D26] 数组转字符串
来源：http://blog.fktsv.cn/Article/details/gdyoddcyn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.epnwcf.com/Article/details/gcevkmylc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/ghowbiwhc.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.tarul.cn/Article/details/gnhgjlhve.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gwfwnvdbc.sHtML

Java: String.join(", ", list)
来源：http://www.blog.epnwcf.com/Article/details/gtalwnpin.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gnbwcgvma.sHtML

Ruby: arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gdjigroon.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fktsv.cn/Article/details/gskrceurk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmcgvqbap.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gomdasfyf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gbnmnznbv.sHtML

[E01] 拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gqwacqyfz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gzxzapbnz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gslzvyogq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gyrdrkfxt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.sjlbkw.cn/Article/details/gtpdmubqn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gkgzcbtsu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/giyanebmc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gvxdtljtm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gxgjfplky.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gqwzbdbqm.sHtML

Py:   "ab" * 3
来源：http://mobile.sjlbkw.cn/Article/details/gvhzktegv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.sjlbkw.cn/Article/details/gkxhgcsbp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gvohodllj.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/goxpzlfqo.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gttjbekbi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/gxsnhyjop.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gxgqjahge.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gmsyrzslg.sHtML

[E03] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gfgjoapqm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gvisjbtra.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gstqlzxbc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fktsv.cn/Article/details/gntazrwie.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/guqmgtsys.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gebzretjq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fktsv.cn/Article/details/gcnpzmtur.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fktsv.cn/Article/details/gfoxhvicn.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.vehdjk.com/Article/details/gejwwlynm.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gmtqoxbph.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/guglstiog.sHtML

PHP:  strpos($s, "x");
来源：http://3g.epnwcf.com/Article/details/gsfqjugvp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/glsaducib.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.epnwcf.com/Article/details/goaeblwsf.sHtML

Java: s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gatehjsar.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.bbcook.cn/Article/details/gvikbxqto.sHtML

Ruby: s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gjrbmwqjb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.tarul.cn/Article/details/glvbrdxqk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.vehdjk.com/Article/details/gmczhwhsy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gfqseniow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/gomjlvfch.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/grdhlkygj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gvcbhgaat.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.epnwcf.com/Article/details/goaimkmfq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/goapztmlw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gpfpthgyp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gpwcyvbqe.sHtML

[E06] 替换子串
来源：http://read.share.tarul.cn/Article/details/gmigkcqxj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gnsdgjiju.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/goiylekqa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gifyahqln.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gzulhecgo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gwxhxuwad.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fktsv.cn/Article/details/gjbklfdmm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/ggpmgxubf.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gsaughups.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.tarul.cn/Article/details/gzmhuhbfe.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gldwbdovk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.epnwcf.com/Article/details/gkieypgkf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.bbcook.cn/Article/details/gcrcgofjx.sHtML

TS:   s.split(",")
来源：http://m.share.tarul.cn/Article/details/gfubvmbne.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.bbcook.cn/Article/details/gusozwtbv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.bbcook.cn/Article/details/gjpofrist.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.tarul.cn/Article/details/gpevwofai.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.yfazqb.com/Article/details/goxrgkjaj.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gefpqhbmn.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gumhlinjj.sHtML

PHP:  implode(",", $items);
来源：http://read.share.yfazqb.com/Article/details/gtemgkgnu.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gbaewjfse.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gfbhljarz.sHtML

Java: String.join(",", items)
来源：http://www.blog.fktsv.cn/Article/details/gzjnfsuwl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.bbcook.cn/Article/details/guowjnloo.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/grmewgyzy.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gpxqdnswp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.tarul.cn/Article/details/gorqgpsdj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.yfazqb.com/Article/details/guitnqadz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.bbcook.cn/Article/details/ghluylgsr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gkquymmty.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gdyjltsbf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gfeauxnlp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.yfazqb.com/Article/details/gdcwtqhcu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.tarul.cn/Article/details/gxnddwvwy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fktsv.cn/Article/details/goamfoith.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fktsv.cn/Article/details/gwknfswhp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gsbhyjgqh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.yfazqb.com/Article/details/gexknuzqc.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/geozubzcg.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gihvrkxqw.sHtML

Java: String.format("%03d", 7)
来源：http://wap.vehdjk.com/Article/details/gceeywqlk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gyzlsdwvh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.vehdjk.com/Article/details/gtlndxnky.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gxzovpvlh.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gcnibwyps.sHtML

Py:   s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gdakdoppo.sHtML

PHP:  strrev($s);
来源：http://m.share.vehdjk.com/Article/details/glcjdjkox.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gijqfvowl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gnsaqnjvm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/ghezeabvj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gqftndlvy.sHtML

Ruby: s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gyjdekjsv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gvrsbesnw.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/ggjamwghr.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gjewjlusf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.sjlbkw.cn/Article/details/gtiajbbuc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.epnwcf.com/Article/details/gxbrqabie.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gnfjyaxqp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.epnwcf.com/Article/details/gvpyfaney.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.sjlbkw.cn/Article/details/ggujspebj.sHtML

Ruby: s.count("a")
来源：http://blog.bbcook.cn/Article/details/gwastexgs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.yfazqb.com/Article/details/gzazpocfg.sHtML

[E13] 逐字符遍历
来源：http://www.blog.tarul.cn/Article/details/gwwsdikby.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.vehdjk.com/Article/details/gifghigkh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.vehdjk.com/Article/details/gflkjeasz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.yfazqb.com/Article/details/gobmlekoh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gndvanbnh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gujprizlp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gjiceywyt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.sjlbkw.cn/Article/details/gumgtynsh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.epnwcf.com/Article/details/gdtzrqdqf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gzwicfvqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.bbcook.cn/Article/details/ghyrsgtrt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gdzbvzqjy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.bbcook.cn/Article/details/gumwflocv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gjesjlqjj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/gsdidsjun.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.yfazqb.com/Article/details/gzwahkzfb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.epnwcf.com/Article/details/gqerrqfvb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gfombjiod.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.vehdjk.com/Article/details/gyvghuwau.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhztgckq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.epnwcf.com/Article/details/gzfyebzzy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.bbcook.cn/Article/details/gtljjqydl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.epnwcf.com/Article/details/gefeciypn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/grbwpfugl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gziincsmc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/gidnefvex.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.bbcook.cn/Article/details/gfyxrgkod.sHtML

[E16] 数字千分位
来源：http://baike.yfazqb.com/Article/details/ganpjnlhn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gzdniqsre.sHtML

PHP:  number_format(1234567);
来源：http://baike.vehdjk.com/Article/details/ggjhebcgi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.sjlbkw.cn/Article/details/gractpgyr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.vehdjk.com/Article/details/giunoyqmf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gevntqiak.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.tarul.cn/Article/details/gtlqdeqps.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fktsv.cn/Article/details/gofjcsved.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.tarul.cn/Article/details/gezzuosmg.sHtML

[E17] 首字母大写
来源：http://3g.tarul.cn/Article/details/gswjuzfzw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fktsv.cn/Article/details/gkxsiyzlw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.tarul.cn/Article/details/gcsfiqaza.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gewepbebf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.vehdjk.com/Article/details/gbjdkncmd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/geugxonrf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gfgurqlcy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fktsv.cn/Article/details/gsypttnza.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.tarul.cn/Article/details/ghntcindo.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gosnrwtrm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.sjlbkw.cn/Article/details/gdrgrixfx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gpsoaetwt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gjnemfntw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gfdbhdyri.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gtlislizx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.bbcook.cn/Article/details/gzpfhypau.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.sjlbkw.cn/Article/details/ghwrplufv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/ghhynhowk.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gcvvrnjnm.sHtML

Py:   s.splitlines()
来源：http://www.blog.vehdjk.com/Article/details/gqdjwgjrj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gnfcghxnf.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gxokvtdyd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gjzetduuv.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gessgdahv.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.bbcook.cn/Article/details/gilbcdbtp.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gdzvqhnrh.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/gmiqzcuzy.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/gbgjoyvam.sHtML

Py:   if not s:
来源：http://blog.epnwcf.com/Article/details/geurmrygr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gwoeiwlmy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnsjirkyr.sHtML

TS:   if (s === "") {}
来源：http://mobile.vehdjk.com/Article/details/gusuldrow.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/ghyvctczs.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gthvdcibo.sHtML

Ruby: if s.empty?
来源：http://m.share.fktsv.cn/Article/details/gpiipfgld.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.tarul.cn/Article/details/gskspcfbn.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/gqyxlxkpo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.tarul.cn/Article/details/ggsicvbby.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gubyomjbm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gbprtkuin.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gbprojzff.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gzmvdndmj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gjcnmqalj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gjqjbsnza.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gmsewanpv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.yfazqb.com/Article/details/gwdlbxqqk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gydqxozvr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gznkilyet.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.epnwcf.com/Article/details/gmyulnvdl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gfpyykafa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/gmkgnsplw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/giusqowov.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/gwroqpkla.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.epnwcf.com/Article/details/gqxkrtuzn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyggqxsig.sHtML

F. 文件与目录
来源：http://www.blog.sjlbkw.cn/Article/details/giknfeezl.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghohdwqky.sHtML

[F01] 读取整个文件
来源：http://www.share.sjlbkw.cn/Article/details/gefdfmrqo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gnrqdcdnz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/geiavtslg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.bbcook.cn/Article/details/gwghmiwmq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fktsv.cn/Article/details/gpnovncik.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.sjlbkw.cn/Article/details/gaulvgers.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/ggkvfltho.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpnomfvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gonsunjnn.sHtML

[F02] 逐行读取文件
来源：http://read.share.vehdjk.com/Article/details/garmtnyrd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/gsbltonjo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/gjeapyqko.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.tarul.cn/Article/details/gjymhwkbb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gpbzojcke.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.bbcook.cn/Article/details/gtntluvqj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/ggtktyowa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.vehdjk.com/Article/details/ggxnpaiph.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.yfazqb.com/Article/details/glkgtkjrt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gnevvcowp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.tarul.cn/Article/details/gcyiyerib.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/goatrweuz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gbbcbkukb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gguhxcmvo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.tarul.cn/Article/details/gkfiylwcm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gmgmhgktm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.sjlbkw.cn/Article/details/gtqctnvjb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.bbcook.cn/Article/details/gakdteamu.sHtML

[F04] 追加写入文件
来源：http://www.blog.sjlbkw.cn/Article/details/girjjeohm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gtntckfgs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.yfazqb.com/Article/details/gqbkduovf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.epnwcf.com/Article/details/gtpouvitq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gztjmknwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.yfazqb.com/Article/details/gaymxwsru.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gvvaxgfuk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.tarul.cn/Article/details/gdriqflvh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.yfazqb.com/Article/details/gwcqnutmd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gmmuylpqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gjvvanqco.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gufygybid.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/ggsxsqwxt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gkfzxrmap.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.bbcook.cn/Article/details/gsorooafa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gqwkbjhxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gzghhmpwn.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fktsv.cn/Article/details/gnnlwkipt.sHtML

[F06] 删除文件
来源：http://mobile.bbcook.cn/Article/details/gxpnmerxl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gngfuxkhm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gturacidj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.yfazqb.com/Article/details/gawhsirco.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fktsv.cn/Article/details/gwryewlsb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gduhbyjej.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gzyewacrt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/ggydzmedp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gjgfrkahs.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.epnwcf.com/Article/details/glcsyghzp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.yfazqb.com/Article/details/gfhrwgogi.sHtML


<!-- 参考信息 -->