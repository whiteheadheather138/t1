代发 wailian999

Java: new ArrayList<>(list);
来源：http://www.blog.epnwcf.com/Article/details/gnrdfumip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.vehdjk.com/Article/details/gpxbhtyhj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.vehdjk.com/Article/details/gzflomtfb.sHtML

C#:   new List<int>(list);
来源：http://baike.fktsv.cn/Article/details/glorkvawh.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gysxjljiw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.tarul.cn/Article/details/gpoqxlncm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fktsv.cn/Article/details/gncvawtoc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.bbcook.cn/Article/details/gizipkwhb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/geayfkeif.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.epnwcf.com/Article/details/geizhbtgz.sHtML

Go:   // 手写循环
来源：http://baike.epnwcf.com/Article/details/gmecumoxl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.vehdjk.com/Article/details/gzezihzkm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.sjlbkw.cn/Article/details/gxhklznkt.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.yfazqb.com/Article/details/gcdnqszzf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fktsv.cn/Article/details/gakificlj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.vehdjk.com/Article/details/gnqcvvdpv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gmodwdwqb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gtyvcqxqw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.vehdjk.com/Article/details/gxtfcooxo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/gifrckqtc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.sjlbkw.cn/Article/details/girzgomld.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.sjlbkw.cn/Article/details/gcvbofdet.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.tarul.cn/Article/details/gqfkjkmtr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fktsv.cn/Article/details/gcmooktfk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.bbcook.cn/Article/details/gmpzqxqcj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gvcymuuzo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.epnwcf.com/Article/details/gvfccgmku.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.yfazqb.com/Article/details/gpugqiiqx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gmcbxeypm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gfkjzkfsb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gxbasoceq.sHtML

[D26] 数组转字符串
来源：http://wap.fktsv.cn/Article/details/gyhxgsyep.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gqnskfmkd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.epnwcf.com/Article/details/gtbmfxxua.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fktsv.cn/Article/details/ggcdnuekn.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gbjgkqxds.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/guftbnnad.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gmwyykaac.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gkesqiqry.sHtML

C#:   string.Join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gcyodjuyd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gbkxnfiye.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/grwtmnccs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gecnqtbde.sHtML

[E01] 拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/grakonvcx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.bbcook.cn/Article/details/ggprmzvrc.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.yfazqb.com/Article/details/gqqzsghqt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gdybfnpns.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gdbtwmcxn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.sjlbkw.cn/Article/details/gsbahhwrp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.bbcook.cn/Article/details/gsaefvpvk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gdzkkqzpd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gfqqtxmxh.sHtML

[E02] 重复字符串
来源：http://www.m.share.tarul.cn/Article/details/gsrrmkeml.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gvhvbdgme.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.yfazqb.com/Article/details/gyqiyzlre.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gjbjqglla.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.bbcook.cn/Article/details/gwldbpwal.sHtML

Java: "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gxadwrrpd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.yfazqb.com/Article/details/gqqhxjqhw.sHtML

Ruby: "ab" * 3
来源：http://read.share.tarul.cn/Article/details/gqnaeazpf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fktsv.cn/Article/details/gjztjzlbf.sHtML

[E03] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gneknpvda.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gvrhszskm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gidouikfu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gromynumg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gcapjouty.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gwrpevcbq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.tarul.cn/Article/details/ggwidilem.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.yfazqb.com/Article/details/gfmywmhsb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.epnwcf.com/Article/details/goeyxhkcz.sHtML

[E04] 查找子串位置
来源：http://read.share.tarul.cn/Article/details/ghiyakbfc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gevqebwqy.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gdniehrik.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gblpcymys.sHtML

TS:   s.indexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gsmhevxkk.sHtML

Java: s.indexOf("x")
来源：http://read.share.yfazqb.com/Article/details/gintrubqb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.yfazqb.com/Article/details/gcvqdgdtd.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/giuiaqbxv.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/guaytjahu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gcuoicxyh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gzmnpicvy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.vehdjk.com/Article/details/gjhmdilbs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gihixutsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gclbilozx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/gzupnwdze.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/gdgljagkr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/ghdhuwaox.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gnujajgxe.sHtML

[E06] 替换子串
来源：http://m.share.sjlbkw.cn/Article/details/glwfmayne.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.tarul.cn/Article/details/ghgxlmyaf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.yfazqb.com/Article/details/gmdlembbo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/godbolkyn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gcejtvnhk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gemafddmm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/grmbyisxf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.epnwcf.com/Article/details/gcdvqbztp.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gxdangjqy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fktsv.cn/Article/details/gioxzhgrq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gvifrdtxx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/geltzphah.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.epnwcf.com/Article/details/gxqagivio.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gbhnqnifc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbqogwyp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fktsv.cn/Article/details/gbmcptsxr.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.vehdjk.com/Article/details/glexrihhl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gcfzaecur.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/glpagoget.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gmkvbxitj.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gvnqgauhu.sHtML

JS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gqlunrwzj.sHtML

TS:   items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gjmvryall.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/ghgmyddrc.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gbxtafsrr.sHtML

Ruby: items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gagmexkng.sHtML

C#:   string.Join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gxconuxsp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.tarul.cn/Article/details/gcqphndwv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.epnwcf.com/Article/details/gxymmhcke.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.tarul.cn/Article/details/gbriogtxw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gkiysdohl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gacrujcsf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.vehdjk.com/Article/details/gxgizldxp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fktsv.cn/Article/details/gxaccbcex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/gfibslhcz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.bbcook.cn/Article/details/gqhxymckd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/gpajfozdy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/guydbzkau.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.vehdjk.com/Article/details/gpwknnnqp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gobpeomrh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/guthaofzn.sHtML

Java: String.format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gsmvvtrpv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gzaubmwtd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/gpffsvkzh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/gchpqthdp.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gmubephyp.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gjncpkmec.sHtML

PHP:  strrev($s);
来源：http://www.blog.vehdjk.com/Article/details/gblgfbwzh.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gztqeduvi.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gtselrudz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.epnwcf.com/Article/details/giidwncqd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.bbcook.cn/Article/details/glchfqxak.sHtML

Ruby: s.reverse
来源：http://baike.bbcook.cn/Article/details/gvfaeftit.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gofawfyqg.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/geigffsqi.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/guctcijbw.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.bbcook.cn/Article/details/gxhhwtodl.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gukvfoqsp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gyynlohvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.yfazqb.com/Article/details/gkqhkbfxf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gukeahsre.sHtML

Ruby: s.count("a")
来源：http://mobile.epnwcf.com/Article/details/gfzusmlcp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gpdikmxyh.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/gxunojqdx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gpcznlakv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.vehdjk.com/Article/details/gfgnwyhqc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.yfazqb.com/Article/details/gryxufotp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.bbcook.cn/Article/details/gjmofjmnw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gtbgtridh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.bbcook.cn/Article/details/gsncqqtze.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/gmedfddcw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.vehdjk.com/Article/details/ggwmfbxwf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.bbcook.cn/Article/details/gxenmuvrx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gndnmewoh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.epnwcf.com/Article/details/gxaidnabq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fktsv.cn/Article/details/goxqlrvji.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.sjlbkw.cn/Article/details/gaikkkzim.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/gaqvqneih.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gtdapmqha.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.bbcook.cn/Article/details/gytimfusy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/ggybnlyjr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.yfazqb.com/Article/details/gflckbmco.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.yfazqb.com/Article/details/gfhxywegd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gyxsitsit.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gvuriynxq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.yfazqb.com/Article/details/golxhwmut.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.bbcook.cn/Article/details/gbdgagdkw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.bbcook.cn/Article/details/gcadqidhh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.yfazqb.com/Article/details/gocoohaio.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.tarul.cn/Article/details/gecbtkznt.sHtML

[E16] 数字千分位
来源：http://3g.yfazqb.com/Article/details/geasdkohk.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.tarul.cn/Article/details/gfkfdebjb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/gfrjwwrph.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.epnwcf.com/Article/details/gklkkankg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/grnihtqyh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/ggvevoboi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.tarul.cn/Article/details/ghplxxswa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.bbcook.cn/Article/details/gwhnrsphh.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/ghhgxfgrv.sHtML

[E17] 首字母大写
来源：http://mobile.sjlbkw.cn/Article/details/gonnxarwj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/ghpnfhnot.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/ghgtlstfm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/ggoaocfll.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.bbcook.cn/Article/details/gdtdfmddp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.tarul.cn/Article/details/gdnabfivy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fktsv.cn/Article/details/gswyozmon.sHtML

Ruby: s.capitalize
来源：http://m.share.bbcook.cn/Article/details/gpclmgrxx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.vehdjk.com/Article/details/gwzqgefmm.sHtML

[E18] 模板占位符替换
来源：http://www.share.sjlbkw.cn/Article/details/gcisdkucq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gmhuvcssc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gudnvgqrw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gyuwcapxw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.sjlbkw.cn/Article/details/gfmjaiupp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.yfazqb.com/Article/details/gdbwuahmn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gpcyeyqvi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.bbcook.cn/Article/details/gylekxhqp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.bbcook.cn/Article/details/ghihpuidc.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/gigqodplu.sHtML

Py:   s.splitlines()
来源：http://blog.fktsv.cn/Article/details/gfmygxjfm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.vehdjk.com/Article/details/gawmrcfkt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/gdagqdfpe.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.epnwcf.com/Article/details/giyyjpthp.sHtML

Java: s.lines().toList()
来源：http://www.share.bbcook.cn/Article/details/gwrvbccip.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.epnwcf.com/Article/details/giydoecpv.sHtML

Ruby: s.lines
来源：http://www.blog.epnwcf.com/Article/details/gljwtkhnk.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/gavyzrcbj.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fktsv.cn/Article/details/grdwvuowt.sHtML

Py:   if not s:
来源：http://m.share.bbcook.cn/Article/details/gewthkryj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/guzyhlubc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.bbcook.cn/Article/details/ggbpgdgoe.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/grlsjgbav.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gvlqfkwyx.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gybmgcpfa.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gpgwroctv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gicvobrdk.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fktsv.cn/Article/details/gobmqvzdl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gjckekbyj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gdlcmyryr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/gukwipicr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gzmslbpgp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gawypyxkg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/glebuqthh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gwmboebei.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.yfazqb.com/Article/details/gvlouwghy.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fktsv.cn/Article/details/gbxdeuafo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.epnwcf.com/Article/details/gulliylbk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gsajtpzkx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gjngsrwnl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gnuafwlvi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.tarul.cn/Article/details/gnvrpfckd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.yfazqb.com/Article/details/gxgzgweol.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gtrfjftnl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fktsv.cn/Article/details/gwodpyofs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkexprwpy.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gwvpjcfdn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gghiupexa.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gdxcvelkg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gvtjskycu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.bbcook.cn/Article/details/gbmxvrbxc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fktsv.cn/Article/details/gegpdylco.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwfxngzae.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gskndnvpq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.epnwcf.com/Article/details/gvomqvftq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gltzzitdz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gfoalzitz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.vehdjk.com/Article/details/gcvqlpwjz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gsntfndjn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.epnwcf.com/Article/details/gwymitmcg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzknmghyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.sjlbkw.cn/Article/details/gajulwewo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gfhimrzuv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.tarul.cn/Article/details/gqnacuriw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.bbcook.cn/Article/details/ghbmaspzc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.bbcook.cn/Article/details/gwtzpqwfo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.vehdjk.com/Article/details/gvljmjghh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/gvuzxvydg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gadmozcpx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gfwxptfzp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.sjlbkw.cn/Article/details/ggvkaltbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.sjlbkw.cn/Article/details/gyrkqoipy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.tarul.cn/Article/details/ggqjaadsj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.sjlbkw.cn/Article/details/gsescufhn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gaazfrlbm.sHtML

[F04] 追加写入文件
来源：http://www.blog.fktsv.cn/Article/details/gxqhdbvpv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gsmhlpyyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/geshdalrh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/glqusdcds.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gqtjvotgp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gyxjqvuzu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gwhymtips.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fktsv.cn/Article/details/gbdjsddsw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.tarul.cn/Article/details/ghdeycrxl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gopevdwjt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fktsv.cn/Article/details/ghuriqimq.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.yfazqb.com/Article/details/gukbfrmim.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.vehdjk.com/Article/details/ghopopqzn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/glzjtoxbz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.bbcook.cn/Article/details/gibatmops.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.tarul.cn/Article/details/gjvsoemcn.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.yfazqb.com/Article/details/gcqyevtzq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gkezjmliv.sHtML

[F06] 删除文件
来源：http://3g.epnwcf.com/Article/details/gecolulex.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fktsv.cn/Article/details/gmmoansfn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gmfueaqcw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gpstxlkli.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fktsv.cn/Article/details/gcrtjpnot.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.sjlbkw.cn/Article/details/goebxssot.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gwzlvqupp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/gllsacfrz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.yfazqb.com/Article/details/gtnmymfkn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.yfazqb.com/Article/details/gzsnazbcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gvrdtkiwi.sHtML


<!-- 参考信息 -->