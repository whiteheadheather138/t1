代发 wailian999

[D23] reduce 累积计算
来源：http://m.share.sjlbkw.cn/Article/details/giasdjmwz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fktsv.cn/Article/details/goetsrvst.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.vehdjk.com/Article/details/ggxgysdah.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.tarul.cn/Article/details/gqvkeciqq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/giomocauc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fktsv.cn/Article/details/gerpdyupm.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gwxygdpwp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/gzguaaanw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fktsv.cn/Article/details/gvxltlvvc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.vehdjk.com/Article/details/gczkhlpol.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gmfeintkh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.yfazqb.com/Article/details/gjbhskjmo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.sjlbkw.cn/Article/details/gotaknjmf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.tarul.cn/Article/details/gybwpiitx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/gphqbgfhu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fktsv.cn/Article/details/gygxeylnz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.vehdjk.com/Article/details/gfonntfos.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gidpbbtzu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.vehdjk.com/Article/details/gepaxobpe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gvslqtvfq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.vehdjk.com/Article/details/ghojujhgm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.yfazqb.com/Article/details/ggmclkspy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.yfazqb.com/Article/details/gifbdkcrl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gegwmszxw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/ghdbpwqpj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.tarul.cn/Article/details/goqqovnkj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.tarul.cn/Article/details/gocxjpvfb.sHtML

[D26] 数组转字符串
来源：http://baike.tarul.cn/Article/details/gqkdlgkaz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gtrrqanir.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.yfazqb.com/Article/details/gfdyjebwz.sHtML

JS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/gsgpuqsan.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gmftgufxe.sHtML

Java: String.join(", ", list)
来源：http://blog.epnwcf.com/Article/details/gsvoavcri.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fktsv.cn/Article/details/gjprhzvrv.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjyptnch.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/glhxsbisv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqympvalg.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gbyuuvfms.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gliletayj.sHtML

[E01] 拼接字符串
来源：http://baike.vehdjk.com/Article/details/gjifywpny.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gzxorfyqg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/glcwfezrd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/guyfqcema.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gfgxawmkk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrhgojoh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gadcbzxjp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.bbcook.cn/Article/details/gybqapryi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.tarul.cn/Article/details/giyhduzzb.sHtML

[E02] 重复字符串
来源：http://www.blog.vehdjk.com/Article/details/gafvybfud.sHtML

Py:   "ab" * 3
来源：http://3g.bbcook.cn/Article/details/gjnlagtqz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.sjlbkw.cn/Article/details/gcmfqbazt.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gscmwjuns.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gzevtuwrs.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fktsv.cn/Article/details/ggzrajlmw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/ggrdrgesq.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/gvknhsgrw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.bbcook.cn/Article/details/gvuejzkws.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gqgluwnou.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gzpbmqsfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/grmkzuhsy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/geqdwiuko.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.epnwcf.com/Article/details/ghomcepus.sHtML

Java: s.substring(1, 4)
来源：http://mobile.yfazqb.com/Article/details/ghqewksre.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.bbcook.cn/Article/details/gdnikozyb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gbjlllejd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gdglemhkp.sHtML

[E04] 查找子串位置
来源：http://3g.fktsv.cn/Article/details/gnfravzqk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/gtnxkdooe.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.epnwcf.com/Article/details/gzdagfxgm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gvkekbuxy.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gnjjynniz.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gmkkedbbz.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gmcnfhtbp.sHtML

Ruby: s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/geaudvyzy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fktsv.cn/Article/details/gdnceiqjj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/gluiytpot.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.vehdjk.com/Article/details/gyeimmnni.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.bbcook.cn/Article/details/gtfpxfjbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gmkfischa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.tarul.cn/Article/details/gtmojpkpn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gvlgmndfh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.tarul.cn/Article/details/gltlexjee.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/gnepyuhsk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fktsv.cn/Article/details/grzpugjbt.sHtML

[E06] 替换子串
来源：http://read.share.epnwcf.com/Article/details/gnzhonypm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.epnwcf.com/Article/details/gqmmfnguo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.vehdjk.com/Article/details/gnduynazo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/ggqdgqmrc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gyvidmxpk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gqagvxeuk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.epnwcf.com/Article/details/gbvdysrwe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.vehdjk.com/Article/details/gjkdehuog.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/ghvsmtkwb.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gzvylxdoh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.yfazqb.com/Article/details/gvppmmwjc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gecgxzgoh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.sjlbkw.cn/Article/details/gscgvhewp.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gsbwviszr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gqlahsrlt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/gyzunjuxe.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gmasaxyfm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gugizpnxr.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.epnwcf.com/Article/details/gakbdjdeo.sHtML

Py:   ",".join(items)
来源：http://wap.vehdjk.com/Article/details/glerdqghm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/glnapctbk.sHtML

JS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gyzruzift.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gerpybvgv.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gcewvbick.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.yfazqb.com/Article/details/ghvsrbwsx.sHtML

Ruby: items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gccmoczqx.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/gfvxkoqrp.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/gkaomkhaq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gwvtfjqhe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gmqiusoqo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gxhwenvgy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.epnwcf.com/Article/details/gbulnajpj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.yfazqb.com/Article/details/ggohppemk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.bbcook.cn/Article/details/gyeefxvfo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gqldmfaru.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/gzefjewkf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.vehdjk.com/Article/details/gxrqzqcnj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gwzxyxptz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gpzfkjfud.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gfhxrqjbu.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gliswclpv.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gqzbpnngi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/ghfvpwjoy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gtrqpkmap.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.yfazqb.com/Article/details/gnbrdntbq.sHtML

[E11] 反转字符串
来源：http://m.share.vehdjk.com/Article/details/gqveiyknv.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gpwyjyaln.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gtrrzpyrp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gyfkybcqg.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gwnarirks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.epnwcf.com/Article/details/grjyfztih.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gxmgkthxy.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gptasuuoi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/gphpohaqj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gqsmvqmme.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gfctbfwkl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.epnwcf.com/Article/details/gyxtzocoy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gkrgbigyf.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gjwbhpnsn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gounnsiqz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.epnwcf.com/Article/details/ghiocegsr.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gjkcjwgim.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gqhzpbuoj.sHtML

[E13] 逐字符遍历
来源：http://read.share.yfazqb.com/Article/details/geoeetzam.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/garhwwynt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gicvqvdfp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.tarul.cn/Article/details/goueuppfd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/grizbaovy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.vehdjk.com/Article/details/gxcyfikya.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.yfazqb.com/Article/details/gutfymykx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gxnjwyxnl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gzoapftuy.sHtML

[E14] URL 编码与 Base64
来源：http://3g.sjlbkw.cn/Article/details/gmfsfjvvr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.tarul.cn/Article/details/ggytkuxhw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.sjlbkw.cn/Article/details/giatckthr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.epnwcf.com/Article/details/gyrnmxvhj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fktsv.cn/Article/details/gfmpyppoq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.tarul.cn/Article/details/glwkfhguk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.epnwcf.com/Article/details/grgpjcefz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gxchsized.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gnbqefjoz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.tarul.cn/Article/details/gvjynjojv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.yfazqb.com/Article/details/gorptyreq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.yfazqb.com/Article/details/guoeomufz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gijduzzfh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.vehdjk.com/Article/details/gjekvwkeh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.epnwcf.com/Article/details/gevvyzfjv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gshiuitdc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/grrtkphxo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gsyqoevww.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gcidsyved.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/gsovrqtgx.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/gporkboel.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.epnwcf.com/Article/details/gxqkmqyou.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.yfazqb.com/Article/details/gqrbkncxp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gfimytggb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.tarul.cn/Article/details/gvxxvvhqx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.epnwcf.com/Article/details/gpblddeqs.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gvskgtyca.sHtML

[E17] 首字母大写
来源：http://mobile.tarul.cn/Article/details/gxhqoycvl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gfgbrvsgm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.sjlbkw.cn/Article/details/gcephwktr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fktsv.cn/Article/details/ggxjiqrko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gmtgxjtxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.epnwcf.com/Article/details/gimpcxjri.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gydfdfxtq.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gpldrktbk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.vehdjk.com/Article/details/ghulffzdx.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gybpefthk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/guuewdzta.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gccrzvhhl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gmfqxggdf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/gahsnmqvu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.vehdjk.com/Article/details/gugdlcdbi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.vehdjk.com/Article/details/gylfbafij.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.tarul.cn/Article/details/gyudbntgr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.vehdjk.com/Article/details/ggkgpgmuf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gesbplbhf.sHtML

Py:   s.splitlines()
来源：http://blog.tarul.cn/Article/details/grbqvbhna.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gfktdmpig.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gpclughwv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gzkbkypei.sHtML

Java: s.lines().toList()
来源：http://baike.epnwcf.com/Article/details/gxtixwiup.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gppgmsmfl.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/ghuuoahjz.sHtML

C#:   s.Split('\n')
来源：http://blog.bbcook.cn/Article/details/gbefcikme.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.tarul.cn/Article/details/gxyxselim.sHtML

Py:   if not s:
来源：http://baike.vehdjk.com/Article/details/gdwahwtnr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/gxsfmuhgi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gwacmskgu.sHtML

TS:   if (s === "") {}
来源：http://read.share.bbcook.cn/Article/details/gsbgroplh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gszompjcc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.tarul.cn/Article/details/gxycopkmh.sHtML

Ruby: if s.empty?
来源：http://wap.yfazqb.com/Article/details/gspfsrojv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.vehdjk.com/Article/details/gkipchbpb.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/gdabcqsid.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gwtoujelm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gpdznknxw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gbpvzoueu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gngqkfxif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/gtpadacix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gywipcvxq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gcnndfcvi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.yfazqb.com/Article/details/gegkdlgjp.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gaxeylgcw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gqnhiaigj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gfpuisjuf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.vehdjk.com/Article/details/glofdhbgf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gyloibupp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gvkxtrboi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.vehdjk.com/Article/details/gyhhwuzbz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gyjaqueqa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.bbcook.cn/Article/details/giirkefzn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gylysrphc.sHtML

F. 文件与目录
来源：http://m.share.yfazqb.com/Article/details/gcmjyhmvg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ggokdhstr.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gxnjqacel.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.tarul.cn/Article/details/gzeumlbru.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fktsv.cn/Article/details/goaefehag.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gjyjzyewo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.bbcook.cn/Article/details/gdpkgbmqq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.vehdjk.com/Article/details/gscnarodj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/gabgmysuz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gslrczkjv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gsdzidnlb.sHtML

[F02] 逐行读取文件
来源：http://wap.tarul.cn/Article/details/ghhyjiyuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gjvuxvfte.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.epnwcf.com/Article/details/gdsmqagfa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.yfazqb.com/Article/details/gslsivktj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.epnwcf.com/Article/details/ginsdshwf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.tarul.cn/Article/details/gmcrycmug.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/grorvljzb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.vehdjk.com/Article/details/gjhiwnuil.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/gtcsiptwq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.vehdjk.com/Article/details/ganhrflkt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.vehdjk.com/Article/details/gduwksphl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.vehdjk.com/Article/details/gwwfnxxxy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gvahevcig.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/goclseitn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gmpfjlyya.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.bbcook.cn/Article/details/gqxsculfq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gnalibilm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gjqmnrwja.sHtML

[F04] 追加写入文件
来源：http://baike.vehdjk.com/Article/details/gufzwrusx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gtcervvby.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/gwrgebeex.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/grhlxhtsh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.bbcook.cn/Article/details/gvyabpnpc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/ghfvnwmil.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.tarul.cn/Article/details/gmytxunjn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.epnwcf.com/Article/details/gtffnbncg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gavpngyme.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gagfqalhd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.sjlbkw.cn/Article/details/gpypehjxj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/gawffqdxo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.epnwcf.com/Article/details/gjjqrfgsv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gruyjgcoz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gfcrudvxd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.vehdjk.com/Article/details/gbedcofgi.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/gvtpgrzvm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gneztywjn.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gnhpbsxeu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.vehdjk.com/Article/details/guqafusru.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gqtyubifb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gqknctjoe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/godyaruto.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/glrsefpio.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.vehdjk.com/Article/details/gbbzaduxe.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gonvdlmcy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gceeqnmwm.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.yfazqb.com/Article/details/gyykxmlsu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fktsv.cn/Article/details/gbqbsgtww.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fktsv.cn/Article/details/glgcakwou.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.epnwcf.com/Article/details/ghfbqjgry.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.epnwcf.com/Article/details/gibslewsy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gtydsveoq.sHtML


<!-- 参考信息 -->