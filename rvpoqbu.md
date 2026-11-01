代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gvoeqlxhn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.bbcook.cn/Article/details/gpljsqfov.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.vehdjk.com/Article/details/gwxarohzh.sHtML

TS:   [...arr];
来源：http://www.m.share.tarul.cn/Article/details/gcecoabay.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gyudoriva.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.vehdjk.com/Article/details/gfohkijvx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fktsv.cn/Article/details/ggyucmrij.sHtML

C#:   new List<int>(list);
来源：http://baike.vehdjk.com/Article/details/gcodebxty.sHtML

[D23] reduce 累积计算
来源：http://m.share.yfazqb.com/Article/details/gxfothosr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gsaiebkgd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.vehdjk.com/Article/details/gsydxpepb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/ggmlxwwyb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gsfpstlex.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fktsv.cn/Article/details/giztdrzjb.sHtML

Go:   // 手写循环
来源：http://blog.tarul.cn/Article/details/gydejpfcs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fktsv.cn/Article/details/gppjyubol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.bbcook.cn/Article/details/guxdeaang.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.vehdjk.com/Article/details/gogwdmlsq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.tarul.cn/Article/details/gmnysdwfq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.epnwcf.com/Article/details/gfpmjlnmg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gpamztcpm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.vehdjk.com/Article/details/gbqgjaggt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.epnwcf.com/Article/details/gfgheixko.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gaeragofa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.yfazqb.com/Article/details/gwbuqoaeh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.tarul.cn/Article/details/gerxwqmri.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.vehdjk.com/Article/details/gdffmbrtu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gzpdnmibm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gvsvwqlrk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.bbcook.cn/Article/details/ghnslsxjq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.vehdjk.com/Article/details/gpzooxvpn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.bbcook.cn/Article/details/gtbngrwvk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/ganyiszka.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.yfazqb.com/Article/details/ggnxvojqf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.epnwcf.com/Article/details/gpehjbrme.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gnscxciyk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.vehdjk.com/Article/details/gifnjliap.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.yfazqb.com/Article/details/glmvijalq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/giodlkfdb.sHtML

TS:   arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/ghjvxevvc.sHtML

Java: String.join(", ", list)
来源：http://www.share.bbcook.cn/Article/details/gvwjkfump.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gzrzioaut.sHtML

Ruby: arr.join(", ")
来源：http://3g.tarul.cn/Article/details/glauffluj.sHtML

C#:   string.Join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/ghggymbyb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvylijrmd.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gmzpxpxtv.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkreerpul.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gnwrjzejq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.epnwcf.com/Article/details/gkhprwtsr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.sjlbkw.cn/Article/details/gkzbgidjx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gnvpnigfg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gxkavytwk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.tarul.cn/Article/details/gbxmvdaxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gkdzgrwoh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fktsv.cn/Article/details/gxyqdvjnk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/giyqhtrou.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/gichzmfpt.sHtML

Py:   "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gipwjuyso.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.vehdjk.com/Article/details/guqxhhtub.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/ghlmtscye.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gixefcirf.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gacxlgdyj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.sjlbkw.cn/Article/details/gdslyrkbx.sHtML

Ruby: "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gofeoqczt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.vehdjk.com/Article/details/gflvgrndd.sHtML

[E03] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gmeyzbird.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.bbcook.cn/Article/details/gffhnlgwn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gkvbzcxtk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/glcyhlatv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/giegbqwfu.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gudvupigg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gblvifuql.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.epnwcf.com/Article/details/gandayyas.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.epnwcf.com/Article/details/ghjprwmnm.sHtML

[E04] 查找子串位置
来源：http://3g.tarul.cn/Article/details/gpwppzykq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.tarul.cn/Article/details/gzqdtdapx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.yfazqb.com/Article/details/gjmljrqjl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fktsv.cn/Article/details/gvcfncyhz.sHtML

TS:   s.indexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/goyqpxxhh.sHtML

Java: s.indexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gczilwhzs.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/ghcpaitma.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gzaigpwhd.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gwqtqfrae.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gjvrbryhu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.sjlbkw.cn/Article/details/gkytqlbtv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gjwoxenpu.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gycjhrsrm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gkucyxotg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/ggtnniuoe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/gqhjneqhi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gjqqlwwxj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gcagldqxg.sHtML

[E06] 替换子串
来源：http://mobile.vehdjk.com/Article/details/gcntpgwqy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/guywvcxqt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/ghdpaqvcu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gdcwkyggk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gqvsijsbc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gbdgvlfgh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/glbjgfpxz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gclrcxqbn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gainpmmqh.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gioqxucpn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/ginboxnkq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.yfazqb.com/Article/details/glhlrtwrr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gpgiqmqia.sHtML

TS:   s.split(",")
来源：http://www.share.vehdjk.com/Article/details/gacckfbdv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gknxheiyn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fktsv.cn/Article/details/gzikeqobj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gcipklvcz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.vehdjk.com/Article/details/gcqpiwmea.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fktsv.cn/Article/details/gzkmdfvdy.sHtML

Py:   ",".join(items)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjamgtkq.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.epnwcf.com/Article/details/gwkibxzeh.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gbfzezenp.sHtML

TS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gupuenzpa.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gplmvbofg.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/guxhwfuvw.sHtML

Ruby: items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gjziuvsjh.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/geyomqbdj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/garomyyky.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.epnwcf.com/Article/details/gndssotmz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/glyctroew.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.epnwcf.com/Article/details/gmisdefsm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gpgclbehr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.epnwcf.com/Article/details/gbbvtzkec.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gvcjsdpsb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.epnwcf.com/Article/details/gehcanhpk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.yfazqb.com/Article/details/gzzbbxvap.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gjicwnant.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.sjlbkw.cn/Article/details/gmiysfsei.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.tarul.cn/Article/details/gqnsrqpbm.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/ghysascns.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.vehdjk.com/Article/details/gfzjepnic.sHtML

Java: String.format("%03d", 7)
来源：http://blog.yfazqb.com/Article/details/gheniyxlr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.yfazqb.com/Article/details/ggwwhbsyx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gnsehifva.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.sjlbkw.cn/Article/details/gdmgtbzod.sHtML

[E11] 反转字符串
来源：http://mobile.fktsv.cn/Article/details/gzkkczmxz.sHtML

Py:   s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gxtmhuurm.sHtML

PHP:  strrev($s);
来源：http://www.share.tarul.cn/Article/details/glghmwfsl.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gsspwtkbr.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkalfygmh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gslhkleae.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/gvzqovvqs.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gqqlusmfl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gtatoxxmz.sHtML

[E12] 统计某字符出现次数
来源：http://3g.vehdjk.com/Article/details/goiouaszb.sHtML

Py:   s.count("a")
来源：http://mobile.epnwcf.com/Article/details/grzrnimka.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/guuhhjmuc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/gkdwfqjem.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gezzgqkpr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.vehdjk.com/Article/details/gdxkqvjau.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/gvfemezsg.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gzgndqhxh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.tarul.cn/Article/details/ggkoszvsq.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gvxvfyfnr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.yfazqb.com/Article/details/gcnocpprl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.yfazqb.com/Article/details/gxdwnzxfk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gaakzzdlu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gbgzesept.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.vehdjk.com/Article/details/gszentebw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.sjlbkw.cn/Article/details/gxfxmntgu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.epnwcf.com/Article/details/gojjmzyjn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.vehdjk.com/Article/details/gdrwnugju.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gaadrwzot.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gamkhtrmw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.tarul.cn/Article/details/gowjviyme.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.tarul.cn/Article/details/gmtzqiksq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.yfazqb.com/Article/details/glcsqnbzq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gptptottl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.yfazqb.com/Article/details/gnxdersju.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/gjkicnqeq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gospwirhi.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/grjcutgyt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gyzxhtrny.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gdkzycckm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.bbcook.cn/Article/details/gmqrqoakp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.yfazqb.com/Article/details/gpzqovxgq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/gomomppik.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gyrvuadsu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/glkfjzxdb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.tarul.cn/Article/details/gsszqgjjr.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/gxaiirmdi.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.vehdjk.com/Article/details/gbbnrpdli.sHtML

PHP:  number_format(1234567);
来源：http://baike.fktsv.cn/Article/details/gkcimgscw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.vehdjk.com/Article/details/gohcpznlj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.vehdjk.com/Article/details/glihblzvn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gakfhaqgm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.sjlbkw.cn/Article/details/gdddgosqn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gsdpxrzid.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gnvmccrkw.sHtML

[E17] 首字母大写
来源：http://mobile.fktsv.cn/Article/details/gnuoipsoz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.tarul.cn/Article/details/gexmqrppq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/gnzieials.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gnwvrcwtn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/giukobkhh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.tarul.cn/Article/details/gpkfuylcf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/gszyxofwe.sHtML

Ruby: s.capitalize
来源：http://read.share.tarul.cn/Article/details/gmsltcouk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gzgewemrx.sHtML

[E18] 模板占位符替换
来源：http://baike.sjlbkw.cn/Article/details/gaafytecd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fktsv.cn/Article/details/gnloizvzm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gylkxonfv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.yfazqb.com/Article/details/gjnuyelij.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gelrkyzjh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.bbcook.cn/Article/details/grmohjcrk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gjlizrppw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/glurycroc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fktsv.cn/Article/details/gtdubafxm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.epnwcf.com/Article/details/gupikkwlx.sHtML

Py:   s.splitlines()
来源：http://read.share.vehdjk.com/Article/details/goabqosrs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkozjubmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gcegcekue.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/guprwkuwd.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gbforrsen.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.bbcook.cn/Article/details/goqtlhfcu.sHtML

Ruby: s.lines
来源：http://www.blog.bbcook.cn/Article/details/gzzgeknle.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gvyizkqfp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gknmpcxrh.sHtML

Py:   if not s:
来源：http://www.share.fktsv.cn/Article/details/glbypisfl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.yfazqb.com/Article/details/gqtbstxzo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.yfazqb.com/Article/details/grgjwaqad.sHtML

TS:   if (s === "") {}
来源：http://baike.sjlbkw.cn/Article/details/ghzgbxqbe.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fktsv.cn/Article/details/gulfsciuk.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gxhycemxl.sHtML

Ruby: if s.empty?
来源：http://3g.sjlbkw.cn/Article/details/gtivxexqn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/girngbxdy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.bbcook.cn/Article/details/gbuipcvsz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.bbcook.cn/Article/details/geehxonpo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gomxdefsd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/gmozphtvb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gmbuhtsis.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.tarul.cn/Article/details/ghkbmhpss.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gugcdfdol.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gcnzqyfwa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.vehdjk.com/Article/details/ggkajrwgk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/goujcwrbm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.tarul.cn/Article/details/gjpocvfgp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gpbgvmoyx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/grusepjns.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/geiiuxncz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.vehdjk.com/Article/details/goybytrxp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.vehdjk.com/Article/details/gscthcjda.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gpummmbhj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/ggfobxkvk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gfztmcslw.sHtML

F. 文件与目录
来源：http://wap.fktsv.cn/Article/details/gplzfhnba.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gsykkviva.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gwqidtnwo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.bbcook.cn/Article/details/gttqkcdib.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/godtftvac.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fktsv.cn/Article/details/ghewdqvmc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.tarul.cn/Article/details/ggusqiqnp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.tarul.cn/Article/details/gdwenepjt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.bbcook.cn/Article/details/gwlclares.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.yfazqb.com/Article/details/ggojglube.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gfzczuilq.sHtML

[F02] 逐行读取文件
来源：http://wap.fktsv.cn/Article/details/gjtpwkymz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gcktzqzug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.tarul.cn/Article/details/glkzmyrrq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gejvftwkw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/grqktfdjt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.yfazqb.com/Article/details/gduxowiri.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/ghvyuaotg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/ggwcelfht.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.vehdjk.com/Article/details/grcvprkbu.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/grbseooxl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gifovcuyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gmxjrsemg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/gnileqzcp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gburpssgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gkulzfjwt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.yfazqb.com/Article/details/goyzchzdf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/ghahniivo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gxkflpgzn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fktsv.cn/Article/details/gufeuhyzw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.bbcook.cn/Article/details/gzxrzctgo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.yfazqb.com/Article/details/gxpwqajli.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.epnwcf.com/Article/details/gktoflzll.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/gfeyijwgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.tarul.cn/Article/details/gdzikbeze.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.yfazqb.com/Article/details/gkxrssxow.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gasphivbp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gichbzcsv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.tarul.cn/Article/details/gatyyagab.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/ggvfrvmms.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.yfazqb.com/Article/details/govcqfzkh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdsafhutm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gntlqkmyt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gcvohvngf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gpbevqdph.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.vehdjk.com/Article/details/gjinnccuu.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.epnwcf.com/Article/details/geqpspqnl.sHtML

[F06] 删除文件
来源：http://m.share.epnwcf.com/Article/details/gstmfffmu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gveuaajxf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gakdggpuq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ggrtfgadr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gneuyhsza.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.epnwcf.com/Article/details/gemxhyqys.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.epnwcf.com/Article/details/gudigdibl.sHtML


<!-- 参考信息 -->