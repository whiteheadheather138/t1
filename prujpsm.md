代发 wailian999

[D23] reduce 累积计算
来源：http://wap.tarul.cn/Article/details/gcgjuefzu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.vehdjk.com/Article/details/gzsxwddgn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gepuwgkoo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.vehdjk.com/Article/details/gmjpnoyip.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/grgxsqlfz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.epnwcf.com/Article/details/gcnnjixzc.sHtML

Go:   // 手写循环
来源：http://m.share.epnwcf.com/Article/details/giedfhgzq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.yfazqb.com/Article/details/gqewxaqgj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.sjlbkw.cn/Article/details/gwleswjyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fktsv.cn/Article/details/gzustkqqj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.yfazqb.com/Article/details/gskweofiz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.vehdjk.com/Article/details/gfgcyupnr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.vehdjk.com/Article/details/gqotjwcfb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gwprmzqqd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.tarul.cn/Article/details/gczrcuoou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gcufvgvpy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.vehdjk.com/Article/details/gidqkekqb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/gelbyjwpj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.vehdjk.com/Article/details/gkodemjcf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.epnwcf.com/Article/details/gqpmepeuc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.yfazqb.com/Article/details/gaubaemiw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.tarul.cn/Article/details/geghlvvmf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.bbcook.cn/Article/details/gkhjuhtoh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.vehdjk.com/Article/details/gpoxtixce.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fktsv.cn/Article/details/gzcplnapd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gkivuvupa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/grsqvwexg.sHtML

[D26] 数组转字符串
来源：http://baike.sjlbkw.cn/Article/details/gorwaaxwd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gdouomzud.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/gcqljisdm.sHtML

JS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gmyfshikh.sHtML

TS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gajmeafgj.sHtML

Java: String.join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gmtzwmmuj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.sjlbkw.cn/Article/details/gxvwbtztb.sHtML

Ruby: arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/gcbnjltds.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.yfazqb.com/Article/details/gymtfwyyv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpfxnkqdm.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gvraxspwh.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxogiclwt.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gnsoauucn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.vehdjk.com/Article/details/gcqmwhhiy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.sjlbkw.cn/Article/details/guvrvbruc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gazkjitbl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/guurbjdao.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.yfazqb.com/Article/details/geezcnfyi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.sjlbkw.cn/Article/details/gfzyneplk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gsqvhuhng.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gmfpxzaqb.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gjklfbbgu.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gxknwjhuv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.tarul.cn/Article/details/gvqlqcpjq.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.yfazqb.com/Article/details/gzgehwukq.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/glqntprjq.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gwaafkzjh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/grstdotxj.sHtML

Ruby: "ab" * 3
来源：http://www.share.epnwcf.com/Article/details/gmzgzjvrw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fktsv.cn/Article/details/gmemnlyta.sHtML

[E03] 截取子串
来源：http://wap.bbcook.cn/Article/details/gelitrkju.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gwnzlgant.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gznlwkrhj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gctspekdb.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fktsv.cn/Article/details/gcuppeqcr.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/ggkqghbpq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.vehdjk.com/Article/details/gyfrmrxjx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gyyoasyqk.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gdqqyusbl.sHtML

[E04] 查找子串位置
来源：http://www.blog.yfazqb.com/Article/details/gttamwtwo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/gcjsbrtyv.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/giauwzpko.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gzvbgtwri.sHtML

TS:   s.indexOf("x")
来源：http://read.share.tarul.cn/Article/details/gwfcuyuqx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.bbcook.cn/Article/details/ggmihwtbv.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gqcjnxkjo.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gwhelxtju.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.sjlbkw.cn/Article/details/gkxcuvogr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.vehdjk.com/Article/details/gkwsiedwn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.yfazqb.com/Article/details/godbtorto.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/gglzsktrs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gcgbslgmp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.tarul.cn/Article/details/gqzjvsafm.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/glkiuarnf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gysbbrece.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.sjlbkw.cn/Article/details/gupstvccr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.tarul.cn/Article/details/goewldmaf.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/grcwbsmah.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.tarul.cn/Article/details/gfkmusoue.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gqkdyecmu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gzxrdcuet.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gtouedhdk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gtzfqvjpd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gbntgxmns.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gtztajopn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.bbcook.cn/Article/details/gmftyzixu.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/ghqdnzpul.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gtziapblg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.yfazqb.com/Article/details/gtyceclfd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.vehdjk.com/Article/details/gchxrauih.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/ggavaukaz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gpzoioqfb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fktsv.cn/Article/details/gvnvuxxnx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.epnwcf.com/Article/details/gtjweihrp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fktsv.cn/Article/details/gmlmyeuxe.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.epnwcf.com/Article/details/gnbjykdbg.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/ggvsghsxq.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gpivebgqe.sHtML

JS:   items.join(",")
来源：http://blog.epnwcf.com/Article/details/gdfwnjegv.sHtML

TS:   items.join(",")
来源：http://3g.fktsv.cn/Article/details/gvncybrmb.sHtML

Java: String.join(",", items)
来源：http://3g.yfazqb.com/Article/details/girehyxnb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.epnwcf.com/Article/details/gzyarmpvx.sHtML

Ruby: items.join(",")
来源：http://m.share.vehdjk.com/Article/details/gereurczs.sHtML

C#:   string.Join(",", items)
来源：http://3g.tarul.cn/Article/details/gmmwarzwe.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/goiydhuiq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/geyjyfefu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gwpgkuwzc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.yfazqb.com/Article/details/gdesouzhp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/gdhvohtzs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.epnwcf.com/Article/details/gpmspaltk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.bbcook.cn/Article/details/gmxjigfak.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.epnwcf.com/Article/details/gusdkfgqg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.tarul.cn/Article/details/gdzzbxlun.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.yfazqb.com/Article/details/gdpdbtusy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gdddeilng.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.sjlbkw.cn/Article/details/gbvhmeivq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gqarlygnb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/grohhrldf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gkluphbcy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gprlfazdu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gzufycqiu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gurebnocc.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gyycsyqel.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gidmtoofm.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/ghabvengk.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gqxqbcwcs.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ghxlvkitl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/grwfocjhj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fktsv.cn/Article/details/gvookzaqq.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gwkppabdf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/gjxuziauu.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gekrpouoz.sHtML

Py:   s.count("a")
来源：http://m.share.tarul.cn/Article/details/gaqrhujho.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.tarul.cn/Article/details/gdqfyhasg.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fktsv.cn/Article/details/gfbuehsbu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gwyjztids.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gkpetythm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gzmgftmje.sHtML

Ruby: s.count("a")
来源：http://www.share.yfazqb.com/Article/details/gzupbhkvy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.vehdjk.com/Article/details/gbpbpmofk.sHtML

[E13] 逐字符遍历
来源：http://baike.tarul.cn/Article/details/gmdzhxyyd.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/golacvlih.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/ghyhhywaw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.vehdjk.com/Article/details/giaydzumo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.tarul.cn/Article/details/gzayzjopn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gsgzastlo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gayghxqdr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gxnlhzfgv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.tarul.cn/Article/details/gjzzwxsnj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.tarul.cn/Article/details/gypcowhne.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/ggjtqamur.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.vehdjk.com/Article/details/gvjhisaps.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/gssuqkikd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fktsv.cn/Article/details/giwcdalic.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fktsv.cn/Article/details/ggmtmpkac.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.tarul.cn/Article/details/gmpdjdzsg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gfslefavq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gtpsgphjx.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fktsv.cn/Article/details/grplzvtbf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.yfazqb.com/Article/details/gjaddvigx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gjevhwlli.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/gruoiqdat.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.vehdjk.com/Article/details/ggnzdfnjo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.epnwcf.com/Article/details/gjdiazrtb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.vehdjk.com/Article/details/gdibxymqz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.bbcook.cn/Article/details/gsfvyhrpv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.vehdjk.com/Article/details/gccjwdfmt.sHtML

[E16] 数字千分位
来源：http://blog.epnwcf.com/Article/details/gjdoangcs.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gnbmdjvai.sHtML

PHP:  number_format(1234567);
来源：http://read.share.yfazqb.com/Article/details/gsmihjikk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.sjlbkw.cn/Article/details/gckxlueqi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gttgsysag.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gxxyaehmb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/gcvltpxly.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.bbcook.cn/Article/details/gzueubdqm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/gwtnchixc.sHtML

[E17] 首字母大写
来源：http://read.share.vehdjk.com/Article/details/gdywfvobs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.sjlbkw.cn/Article/details/guuvyhrog.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gskenuver.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gqvfadthi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gopdeuoye.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.bbcook.cn/Article/details/gjytturrs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/godklxjsx.sHtML

Ruby: s.capitalize
来源：http://read.share.sjlbkw.cn/Article/details/gvrukmsuw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gaxmfrqoe.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gpomudfmq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.yfazqb.com/Article/details/gewcabtkj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gmymcfide.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gjmqhvibf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/glncifymn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gcccjuoys.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gneshucva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gshzqghmr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gawuhnebs.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gcxhfiemw.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gdumvgkpo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gmckbgvxs.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.sjlbkw.cn/Article/details/gddrhozja.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/guwsgyxqe.sHtML

Java: s.lines().toList()
来源：http://wap.epnwcf.com/Article/details/gvvqhredq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fktsv.cn/Article/details/glsvdyqda.sHtML

Ruby: s.lines
来源：http://3g.vehdjk.com/Article/details/gbswiekau.sHtML

C#:   s.Split('\n')
来源：http://mobile.epnwcf.com/Article/details/gigzjhvys.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/ghpxjcves.sHtML

Py:   if not s:
来源：http://blog.fktsv.cn/Article/details/gdgnmgbjm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gikcrpuji.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/grnpzfduw.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gyxjnyiha.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gmcwelcjz.sHtML

Go:   if s == "" {}
来源：http://blog.bbcook.cn/Article/details/gyvvtjidk.sHtML

Ruby: if s.empty?
来源：http://www.share.bbcook.cn/Article/details/gevmmtrhr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/ghcefpotw.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gcwrheluz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gdylrtkht.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gjfwkzdue.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.yfazqb.com/Article/details/gsnejrlax.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gnqytcdof.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gpopzzpez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.vehdjk.com/Article/details/gbwkiyyax.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gaauhgmgw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtkxsgtia.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.sjlbkw.cn/Article/details/gkjgbrrap.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gqztwdmqp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gsksilzyh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/glsqqqmvm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.vehdjk.com/Article/details/ghgsfsaoq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.epnwcf.com/Article/details/ggtdsfdfx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.vehdjk.com/Article/details/govkxafct.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gjkjlbgex.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.vehdjk.com/Article/details/gduwkdshv.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghulxwhcb.sHtML

F. 文件与目录
来源：http://mobile.bbcook.cn/Article/details/gcquehoki.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gaciqpnij.sHtML

[F01] 读取整个文件
来源：http://blog.vehdjk.com/Article/details/gxnicfkcj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.epnwcf.com/Article/details/gywcpzjrh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/geljdpndu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gztmfwosv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gtemitxjg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.yfazqb.com/Article/details/ggfhanzir.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gnitcbluq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gsbzfwrjy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.epnwcf.com/Article/details/gzpksgohv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.bbcook.cn/Article/details/ggfzkpjxk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.tarul.cn/Article/details/gnjcalluf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/gvlcnqagz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/gbjmkgtrd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.bbcook.cn/Article/details/gpvgnjyex.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/gukwbfija.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.tarul.cn/Article/details/gaayfnihf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gnsfjphli.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gigejgopu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gkxihwigk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gjwinbijy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.yfazqb.com/Article/details/gxnganxth.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gmefjzhwl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gwqksdqhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fktsv.cn/Article/details/gnjwtzedn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gmfvfujsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gjpddimqr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gjjslrvhx.sHtML

[F04] 追加写入文件
来源：http://mobile.yfazqb.com/Article/details/gftfnzzte.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/gruhrobjt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.epnwcf.com/Article/details/gxttmooxs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gswaadayr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.bbcook.cn/Article/details/gwuuhkwyq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.bbcook.cn/Article/details/gssyvziyo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gmlqnrigf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.bbcook.cn/Article/details/guuzryuli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.epnwcf.com/Article/details/gtruoutbm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gwyswirmr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.epnwcf.com/Article/details/ggfqvarpu.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fktsv.cn/Article/details/gkxbnupji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gouopcyis.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gyopcilso.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fktsv.cn/Article/details/gyyqhesdu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.vehdjk.com/Article/details/gpviotlpf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/glyxlowrd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxthwbujg.sHtML

[F06] 删除文件
来源：http://www.m.share.bbcook.cn/Article/details/gzuzqlmxz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/gvydexcch.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gxgctjrub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gqufxgivi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.yfazqb.com/Article/details/gsysbdyca.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gpctcotxh.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gxeqeruhi.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.bbcook.cn/Article/details/gepdvllmy.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.tarul.cn/Article/details/gzpaawpqt.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.vehdjk.com/Article/details/gsyvagxww.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.sjlbkw.cn/Article/details/gpnxtqtrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.tarul.cn/Article/details/guebpsjxb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.tarul.cn/Article/details/gizubzzel.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fktsv.cn/Article/details/geoobheux.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.tarul.cn/Article/details/gxkvmeqhx.sHtML


<!-- 参考信息 -->