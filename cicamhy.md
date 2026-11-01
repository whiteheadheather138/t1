代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://mobile.yfazqb.com/Article/details/gnjcvbvya.sHtML

JS:   arr.includes(x)
来源：http://blog.vehdjk.com/Article/details/gifwtaiub.sHtML

TS:   arr.includes(x)
来源：http://m.share.fktsv.cn/Article/details/gumrrjyjr.sHtML

Java: list.contains(x)
来源：http://www.blog.fktsv.cn/Article/details/gserhspcg.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.vehdjk.com/Article/details/gjejrvkif.sHtML

Ruby: arr.include?(x)
来源：http://baike.sjlbkw.cn/Article/details/gbbdzsero.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.bbcook.cn/Article/details/gabzululu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.yfazqb.com/Article/details/gbnxymiak.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.bbcook.cn/Article/details/gfaxcsnuh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.bbcook.cn/Article/details/gotzvcrii.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.tarul.cn/Article/details/gzbdhkhhp.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gahoqekze.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fktsv.cn/Article/details/ghzlknuqy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fktsv.cn/Article/details/gtfurhqfg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.tarul.cn/Article/details/gqnnucaue.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/giyjemlpt.sHtML

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/garkgngmr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gtofrbyyf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.bbcook.cn/Article/details/gtdfihtqs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.sjlbkw.cn/Article/details/ghedaqyel.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.vehdjk.com/Article/details/gpyaqobpj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.epnwcf.com/Article/details/gytkmbpin.sHtML

Go:   // 手写循环
来源：http://read.share.bbcook.cn/Article/details/gyxjxtpkm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fktsv.cn/Article/details/gafwjpzxi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.sjlbkw.cn/Article/details/gubliurvy.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gygmjhstu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.yfazqb.com/Article/details/gryfqhkcn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.tarul.cn/Article/details/gujhloqst.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.bbcook.cn/Article/details/gbejmvwfz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fktsv.cn/Article/details/gmzilphah.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.epnwcf.com/Article/details/gxtvwdrfs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fktsv.cn/Article/details/gtuhlkdlq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gbtcootju.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/ggdqvkvqt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.epnwcf.com/Article/details/gpmpnatlf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.epnwcf.com/Article/details/gygsfnfbe.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.tarul.cn/Article/details/gilkfheox.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.bbcook.cn/Article/details/guyemzdlr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.vehdjk.com/Article/details/gyutljcgy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.vehdjk.com/Article/details/gxwxzfhvw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.tarul.cn/Article/details/gxgkcugel.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.sjlbkw.cn/Article/details/gedmgzpgm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/gmljbyxkh.sHtML

[D26] 数组转字符串
来源：http://3g.tarul.cn/Article/details/gitnmpimo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fktsv.cn/Article/details/gbnvocfxi.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/glzysdaer.sHtML

JS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gegpdxngi.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjjhrzgn.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/gabewbchk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gressekpr.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gakqxieym.sHtML

C#:   string.Join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gxhxihgyx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtxryvxhk.sHtML

E. 字符串处理
来源：http://wap.tarul.cn/Article/details/gszvbkqex.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gopxnoxwt.sHtML

[E01] 拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gqdpaaibl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/goiudtplo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fktsv.cn/Article/details/gehnjbmwi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.tarul.cn/Article/details/gsufxjpcy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gthfddzrp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.epnwcf.com/Article/details/ggqwzxtvj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/ghkfxydgs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.tarul.cn/Article/details/gzvbtykwa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/geokmjayx.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gfszqoyrb.sHtML

Py:   "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gwaytudsj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.tarul.cn/Article/details/gcrurxzde.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gbtussduy.sHtML

TS:   "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gnkvihjjd.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gruprflcp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.bbcook.cn/Article/details/gwbvhscat.sHtML

Ruby: "ab" * 3
来源：http://3g.vehdjk.com/Article/details/gnwsvifdq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.epnwcf.com/Article/details/gwocwergd.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsnbwvzf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.bbcook.cn/Article/details/gnufxjres.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gkahjuxhw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gszdasnxd.sHtML

TS:   s.slice(1, 4)
来源：http://blog.tarul.cn/Article/details/gxdgylzzi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gyfaophdl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.yfazqb.com/Article/details/grwcqhuuu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fktsv.cn/Article/details/grkfhneri.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.yfazqb.com/Article/details/gvyywlcut.sHtML

[E04] 查找子串位置
来源：http://3g.yfazqb.com/Article/details/glqvzhziw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gmlcwgqug.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gnngywwua.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.bbcook.cn/Article/details/gvbrucvac.sHtML

TS:   s.indexOf("x")
来源：http://baike.vehdjk.com/Article/details/ghewnockn.sHtML

Java: s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/ghtixhhmg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gocitmuyy.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/grjxdfpin.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.tarul.cn/Article/details/gtlivcmcr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gdmsxkzjy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.yfazqb.com/Article/details/ghpyxlfqb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fktsv.cn/Article/details/gbssoitye.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/glewgxmmv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/guyjgchmc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gctnhanas.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gzanvptqv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fktsv.cn/Article/details/gtdwqanbt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gerlmsrfz.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gjrqekjqu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gwocxmwrn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.epnwcf.com/Article/details/gkilxasnc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gczmimroj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gqrzsrlyc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/ggobhkvhy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/ghwrlbcpf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fktsv.cn/Article/details/gyxbusnjx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gqpohxmux.sHtML

[E07] 按分隔符拆分
来源：http://m.share.vehdjk.com/Article/details/gebzczcft.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.epnwcf.com/Article/details/gyksxuuvi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gblljyqsh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/grwfehdfi.sHtML

TS:   s.split(",")
来源：http://3g.sjlbkw.cn/Article/details/gamaotygb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.epnwcf.com/Article/details/gdhyteegb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.epnwcf.com/Article/details/gswbsghvu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.epnwcf.com/Article/details/grvnsgayp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.bbcook.cn/Article/details/gdozulfzq.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.epnwcf.com/Article/details/giyzqjyvl.sHtML

Py:   ",".join(items)
来源：http://wap.sjlbkw.cn/Article/details/gunxncuqt.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/ggflhaoiz.sHtML

JS:   items.join(",")
来源：http://www.blog.fktsv.cn/Article/details/gqrvsyajq.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gbkjgyuwq.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gsfjtggdt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.sjlbkw.cn/Article/details/gexyouplt.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gqrzqxxni.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gqylksnhr.sHtML

[E09] 去除所有空白字符
来源：http://m.share.tarul.cn/Article/details/gfhdqroes.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.sjlbkw.cn/Article/details/gbybzenrg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.bbcook.cn/Article/details/glmhsczut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gpqfgwpnt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gvprjvkmu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gjjpznorc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.sjlbkw.cn/Article/details/gnalvlrfu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/goeeolgdv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gypaypehw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gqemkexxp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.yfazqb.com/Article/details/ggiaohago.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.vehdjk.com/Article/details/gtlemabpw.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gasuaivql.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/ggbqjdmih.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gmjrkvmap.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gtnsuslvj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gkswlxpwn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.sjlbkw.cn/Article/details/ghdmbhijt.sHtML

[E11] 反转字符串
来源：http://baike.epnwcf.com/Article/details/goegpjykt.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/glkcgaxvz.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/ggwhtregj.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gdytgjnov.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gvjwdaslq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/gjzzelhde.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.epnwcf.com/Article/details/gymzcbkfm.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gqukomecd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gwhvwzvre.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.tarul.cn/Article/details/gddlkqpju.sHtML

Py:   s.count("a")
来源：http://m.share.epnwcf.com/Article/details/gjzxsczzn.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gndnooyvu.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gnutyhoko.sHtML

TS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/gybavmsmr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gngjxdnpr.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gjrihuvmw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/glqsdhzfd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fktsv.cn/Article/details/grczmcoyk.sHtML

[E13] 逐字符遍历
来源：http://www.share.vehdjk.com/Article/details/gbctnoqyb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.yfazqb.com/Article/details/gzwjhawkn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.bbcook.cn/Article/details/gtckrmjpv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gtpxgnene.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdyhzkuxk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gliwiyjqx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.epnwcf.com/Article/details/gxawzabhx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gyjaddxoo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.tarul.cn/Article/details/gfrpqlcld.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gmghstwwo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.vehdjk.com/Article/details/gurrnwjvr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.epnwcf.com/Article/details/goueektza.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.epnwcf.com/Article/details/gqndywxsd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.epnwcf.com/Article/details/gsschlpew.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gjkjybhfs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gcrvbnqki.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.vehdjk.com/Article/details/grbiiemzs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gcexxuwpv.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.epnwcf.com/Article/details/gczxftxdc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.epnwcf.com/Article/details/gugkthwyf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gvgyjwhzb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpvebxrvb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.yfazqb.com/Article/details/gsjzovaby.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gtalzwycc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.sjlbkw.cn/Article/details/gqpitkphe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/gvpuifeab.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqqxvtho.sHtML

[E16] 数字千分位
来源：http://m.share.vehdjk.com/Article/details/gucfzaahv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/gnjrmavxp.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/galcnaxid.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/gomezodpy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gwvhezehl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fktsv.cn/Article/details/gmopolqel.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fktsv.cn/Article/details/gznoddusx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/gsoniztmn.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.vehdjk.com/Article/details/gbbbrxxzp.sHtML

[E17] 首字母大写
来源：http://3g.yfazqb.com/Article/details/gbjqbqwbq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/giydriibf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.vehdjk.com/Article/details/gkhipzimc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.bbcook.cn/Article/details/gxxuberso.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/gemikspdg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/gpittpxvj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.bbcook.cn/Article/details/gabvtuxyd.sHtML

Ruby: s.capitalize
来源：http://www.share.bbcook.cn/Article/details/guzxrywga.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gznrirmwo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fktsv.cn/Article/details/gzjfkpyqa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/ghayipxhj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.yfazqb.com/Article/details/gaoaqqyop.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gvkqlally.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gnsiiiuif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/ggeipiolk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gdfkvlsdl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fktsv.cn/Article/details/gyiqrckqt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fktsv.cn/Article/details/godqagnnx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/glzfkabbx.sHtML

Py:   s.splitlines()
来源：http://www.m.share.tarul.cn/Article/details/gtlhoohvd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.sjlbkw.cn/Article/details/gexncetwq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gjzxnaxlo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/gkqdhatvs.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gogzqfrri.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gqejkuvxv.sHtML

Ruby: s.lines
来源：http://mobile.sjlbkw.cn/Article/details/gqfkatkvd.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/grolwbxdq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.vehdjk.com/Article/details/gfalxpqrm.sHtML

Py:   if not s:
来源：http://wap.sjlbkw.cn/Article/details/gmmaczyhf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.epnwcf.com/Article/details/gkabzdhgd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/gdegxmxum.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gkoapxhos.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gaaejxhnt.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/ghncxnggd.sHtML

Ruby: if s.empty?
来源：http://3g.tarul.cn/Article/details/gdjulpsze.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fktsv.cn/Article/details/gdekmgquy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.epnwcf.com/Article/details/gauwpmame.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.sjlbkw.cn/Article/details/golbgujwk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/ggujkyeuz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gmhwzlqvm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gtvffnsio.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcsqcskxf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fktsv.cn/Article/details/gpszkujtd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gtylsptkx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gqkvxdtkf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.tarul.cn/Article/details/gqjgncfjh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/glfaqxixn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gtvacxawr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fktsv.cn/Article/details/gavwyonji.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/gltxmsfki.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.epnwcf.com/Article/details/gnahadaxw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/grdlybvcm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.vehdjk.com/Article/details/glbifecpg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/gnwcbooey.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmngxqomw.sHtML

F. 文件与目录
来源：http://www.share.epnwcf.com/Article/details/gvaeaqdcw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/glwdtcjks.sHtML

[F01] 读取整个文件
来源：http://www.share.vehdjk.com/Article/details/gofykzxdo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gahxgrpfw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/grogcxmuz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fktsv.cn/Article/details/gfkekgeoz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.sjlbkw.cn/Article/details/ghwkamghk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/gpvzgvyou.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.yfazqb.com/Article/details/gpmbxsuaw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gsapxzxvp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gwvvpylfc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.vehdjk.com/Article/details/gpktoaowr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gfxzrtomq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.bbcook.cn/Article/details/gmopvbfzr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gupknlybj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gyzbpkbuy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gaincmaag.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gjcxjtcqi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fktsv.cn/Article/details/gucjjipty.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.sjlbkw.cn/Article/details/guoxtwcpa.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/gegrusxzw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.tarul.cn/Article/details/gwomdbgnb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.sjlbkw.cn/Article/details/goymwfhaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/gbxxosnyr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gemdboigu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.yfazqb.com/Article/details/gkxozqjpi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gwijgivel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.tarul.cn/Article/details/gpgsdnety.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.vehdjk.com/Article/details/gmzyflkpo.sHtML

[F04] 追加写入文件
来源：http://3g.yfazqb.com/Article/details/gnmuintlm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.epnwcf.com/Article/details/gmrgyumvu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.vehdjk.com/Article/details/gscmzvxgg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gxgniunou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gdjhnijfx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/glerahlmx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/ghwnfgmas.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.yfazqb.com/Article/details/gtowqrpsh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gfhzpgwlc.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fktsv.cn/Article/details/grrlvkkod.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.bbcook.cn/Article/details/gbquwqouz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwxkyxwaq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gbjhszgsd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gsqzyuqul.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/glpyctrtf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gsniwfycr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fktsv.cn/Article/details/gonzqlutv.sHtML


<!-- 参考信息 -->