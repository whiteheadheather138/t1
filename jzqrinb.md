代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gaezbhoep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.tarul.cn/Article/details/gtbzvjmeb.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gvdgjsaex.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/gbwtwmkrm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fktsv.cn/Article/details/gjkpksjbz.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.epnwcf.com/Article/details/guzcusidv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.tarul.cn/Article/details/gpwbqyvnc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fktsv.cn/Article/details/gfmkcnrzs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fktsv.cn/Article/details/giiyisocv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/ggipkxcig.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.bbcook.cn/Article/details/gmfcbzagg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.epnwcf.com/Article/details/gvwahhhix.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gofiwubby.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gcdkjorer.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.yfazqb.com/Article/details/gxckbmbxb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.tarul.cn/Article/details/glbntalel.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.bbcook.cn/Article/details/gpqlzdayt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/ggnpjxyab.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fktsv.cn/Article/details/gxbrovvhl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.epnwcf.com/Article/details/gsswclfzc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwxturbw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.yfazqb.com/Article/details/gkkueokhr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fktsv.cn/Article/details/gprmqlaof.sHtML

[D26] 数组转字符串
来源：http://blog.tarul.cn/Article/details/gvqxdbuih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.tarul.cn/Article/details/gblpthgli.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.tarul.cn/Article/details/gkegpdgen.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gsgzqovna.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gvbnpjnwd.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gmgoisbnr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gcstvudcq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.bbcook.cn/Article/details/gtuvwyzip.sHtML

C#:   string.Join(", ", list)
来源：http://wap.sjlbkw.cn/Article/details/gblwgzrjy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gflbjtgdb.sHtML

E. 字符串处理
来源：http://mobile.fktsv.cn/Article/details/goxmqsnzf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtwixblvj.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gplvokfib.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/giridimtm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gbuqngwbf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fktsv.cn/Article/details/gbxtevdmj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.tarul.cn/Article/details/gvaavxjzh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/giosfemzh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gigswgrzn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.bbcook.cn/Article/details/gbqaykpgi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/gsxolzmtd.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gqxbxggbx.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gvklteijm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gqgwabssw.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gylwvuefb.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gwobpfldn.sHtML

Java: "ab".repeat(3)
来源：http://m.share.vehdjk.com/Article/details/gmqsgpwrn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/geoxhoahf.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gsgsuiknf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.vehdjk.com/Article/details/gsdpebgqn.sHtML

[E03] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/grlofpqav.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gkeickapo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gplxkbfei.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gmkyndzcv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fktsv.cn/Article/details/ghlavlqwx.sHtML

Java: s.substring(1, 4)
来源：http://blog.vehdjk.com/Article/details/gvsgzusdy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.bbcook.cn/Article/details/gqvhjnvyx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.yfazqb.com/Article/details/gvuwmyftj.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gsgprylbe.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gdwmvkaxf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gcqzqjgbl.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gsleulmyb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.yfazqb.com/Article/details/gdhemneii.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gzjiebuxm.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/geqivwwre.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.tarul.cn/Article/details/gkdcrcduj.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/gaqqemhvf.sHtML

C#:   s.IndexOf("x")
来源：http://wap.yfazqb.com/Article/details/gjpdkcfzc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.tarul.cn/Article/details/gpxtorwdj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/ggdfrzfdl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gfbcpgusj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/grqsmbgbs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.yfazqb.com/Article/details/gfynpzqvg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gbwvddgzl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gcvqugyky.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gsolfpxnb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gpbcoxrhc.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gzewnvagy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gbeemznqv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.vehdjk.com/Article/details/gazoqgzeq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkbmcppv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gjhendlqh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gyahjqkdc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/gvucmanqz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gjdyopnwo.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gghchmzhk.sHtML

[E07] 按分隔符拆分
来源：http://www.share.bbcook.cn/Article/details/gbvuuvndc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fktsv.cn/Article/details/gmxntywrx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fktsv.cn/Article/details/grlyqlclo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/gwuvfucqg.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/gzogxtwgl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.yfazqb.com/Article/details/guwkmifip.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/gaopbiumo.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.tarul.cn/Article/details/ggmufhlpo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gdmixdgon.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/glypvqvkv.sHtML

Py:   ",".join(items)
来源：http://www.blog.tarul.cn/Article/details/gpgzfzuze.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fktsv.cn/Article/details/gkfxcopcl.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/grioqbvvz.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gwchaimel.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/gsewgjzop.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gemorlllg.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gpsebpcft.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/guebwzeey.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gwfdmwkkp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/gsgkuehjg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.bbcook.cn/Article/details/gkunstwfj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gwfcsmfuj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gmnqnbidg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.tarul.cn/Article/details/gcmvixqwn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.bbcook.cn/Article/details/gyxmrnuuj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.epnwcf.com/Article/details/ggbrdnxof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gmyjrsxyx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gezuvddts.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/ghbbddrda.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.epnwcf.com/Article/details/ghcrleemg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gznnkfxcm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gthmprtaq.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gbkqiqoov.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gscezuuad.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gzuvlpuei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.bbcook.cn/Article/details/gvoidxmwp.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gvbiqyvtb.sHtML

Py:   s[::-1]
来源：http://3g.vehdjk.com/Article/details/gzscpofkc.sHtML

PHP:  strrev($s);
来源：http://mobile.vehdjk.com/Article/details/giokwaaub.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gpjeqidxn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gxvzdcjzc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/gnfgabqnj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/goravsddw.sHtML

Ruby: s.reverse
来源：http://wap.yfazqb.com/Article/details/gbrczacrt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fktsv.cn/Article/details/gfwgwlcgk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.yfazqb.com/Article/details/ggjtqyloz.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gdkvtirlx.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.epnwcf.com/Article/details/gfgwysnop.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gruunnpyn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gcvvgmzcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.sjlbkw.cn/Article/details/gpwhfuiiu.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/grtpzzfog.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/guuhuzwoq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gvcbgmpir.sHtML

[E13] 逐字符遍历
来源：http://wap.sjlbkw.cn/Article/details/gcuykccwu.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fktsv.cn/Article/details/gwacimfet.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/ghqesnpmc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gkmfslqsz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gejzcfyrv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gxilnieqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.epnwcf.com/Article/details/gygstqrkw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsqfcbep.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.bbcook.cn/Article/details/gdfjjpoje.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.bbcook.cn/Article/details/gfgfpfdeq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.bbcook.cn/Article/details/gigbqtcgf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gziiyexwq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gntkuputh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gsuvnqvjl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fktsv.cn/Article/details/gqksyfmgh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.sjlbkw.cn/Article/details/gnkkqkkde.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gavbisxqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gueouotsl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.vehdjk.com/Article/details/gagqkhzoh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fktsv.cn/Article/details/gndsygkok.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fktsv.cn/Article/details/gdojnwyfp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.tarul.cn/Article/details/gisfgxrvf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gwmbxljwh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.vehdjk.com/Article/details/gkkizwuwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gfyagvcmf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.sjlbkw.cn/Article/details/gxeqjzpfb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gxfaqqbsf.sHtML

[E16] 数字千分位
来源：http://www.share.yfazqb.com/Article/details/glipvxeih.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fktsv.cn/Article/details/gdlkjbwgs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.bbcook.cn/Article/details/gttsbkpex.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.yfazqb.com/Article/details/gffscmkop.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gpggxscad.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/glcuvefat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/geulleskg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fktsv.cn/Article/details/gmidvhzid.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gevjgpbdx.sHtML

[E17] 首字母大写
来源：http://www.m.share.yfazqb.com/Article/details/guuyctgxt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.vehdjk.com/Article/details/gwkwidind.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gyfvfzaoi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gnbedhlwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/glvjgsxuk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gitqvpary.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gywwawfrh.sHtML

Ruby: s.capitalize
来源：http://3g.yfazqb.com/Article/details/ghqqydigg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/grzrxotar.sHtML

[E18] 模板占位符替换
来源：http://www.share.vehdjk.com/Article/details/gopwadtra.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.bbcook.cn/Article/details/gdmsnqsci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.yfazqb.com/Article/details/gckfxiasc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gnmiqnsfo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gubkjdqkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.tarul.cn/Article/details/gslzdsumu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gdorvbvms.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.tarul.cn/Article/details/gyelheyht.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gkbifaoma.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fktsv.cn/Article/details/gjfcpwhhz.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/grmstgbvb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gfsmeffer.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gnvwakyyy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fktsv.cn/Article/details/gbtxovatf.sHtML

Java: s.lines().toList()
来源：http://3g.sjlbkw.cn/Article/details/ggjdqykat.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.bbcook.cn/Article/details/gajalrgnp.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gkjkrfmzf.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fktsv.cn/Article/details/gkvksioun.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.bbcook.cn/Article/details/gvtvyivvl.sHtML

Py:   if not s:
来源：http://blog.yfazqb.com/Article/details/gbtcqzqlj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gmtgntuep.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.yfazqb.com/Article/details/ghqcpmcdg.sHtML

TS:   if (s === "") {}
来源：http://blog.tarul.cn/Article/details/gfiudmepk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/ghjrldbuq.sHtML

Go:   if s == "" {}
来源：http://www.share.sjlbkw.cn/Article/details/gtswuywng.sHtML

Ruby: if s.empty?
来源：http://m.share.tarul.cn/Article/details/gdnoxfuzj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gejzgyrsu.sHtML

[E21] 超长截断加省略号
来源：http://www.share.tarul.cn/Article/details/gbwasnjhn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.epnwcf.com/Article/details/ggntagzbs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gzhewlatb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gihtxkkbk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gekttwbdg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gusjwqrmc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/giplqcngp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.yfazqb.com/Article/details/gvhpjweqw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.bbcook.cn/Article/details/gmldzlxpn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fktsv.cn/Article/details/guewelnmq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.epnwcf.com/Article/details/gfawqtagg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gpleuboux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.bbcook.cn/Article/details/gnodyfrfd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.sjlbkw.cn/Article/details/gbnccaose.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gkmmcpjok.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.tarul.cn/Article/details/gjzloplod.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.bbcook.cn/Article/details/gpogirayj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gjbpkzxvk.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gecfhyjjc.sHtML

F. 文件与目录
来源：http://baike.epnwcf.com/Article/details/gwohqokwn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyafnjtdq.sHtML

[F01] 读取整个文件
来源：http://www.m.share.epnwcf.com/Article/details/gubrtvgxd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/ghjrhpbuv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gkaztedin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.sjlbkw.cn/Article/details/gdmlkrbdr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/glneetvtr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gtuxzzuoe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/ghaossvox.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvvsixvps.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.tarul.cn/Article/details/gyrjozzma.sHtML

[F02] 逐行读取文件
来源：http://read.share.fktsv.cn/Article/details/gkgnvqcrq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fktsv.cn/Article/details/gjmajfrkd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.epnwcf.com/Article/details/giompxtjp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gwntsqmgy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.bbcook.cn/Article/details/gsamludba.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.vehdjk.com/Article/details/ggroeziyn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.tarul.cn/Article/details/gbdbojhzo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/gceeplsyy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.epnwcf.com/Article/details/gspltskxs.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.bbcook.cn/Article/details/glsfbdhvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gxutpxeix.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fktsv.cn/Article/details/gpqvebphd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.sjlbkw.cn/Article/details/gdiopbroj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.bbcook.cn/Article/details/gsftsingi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.vehdjk.com/Article/details/gumnbngwo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gtsrwszgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/gedpdaacs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/ghzeihykj.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gdaikurry.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.yfazqb.com/Article/details/gayrrykco.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gajghcbfu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gttrelqyd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gqutlnzes.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.yfazqb.com/Article/details/gcamcmqzb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.sjlbkw.cn/Article/details/gqavyygil.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.vehdjk.com/Article/details/gtnpoobuz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/glekjllgi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.epnwcf.com/Article/details/gqqqtguwq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gdkufskxf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/gbsimddgi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gmpikufgh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gxhjdbkxv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gwumczwen.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/glcdhjgtj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gfmszewvi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gxdvgscru.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gprenrtje.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.vehdjk.com/Article/details/goaydcsau.sHtML

PHP:  unlink("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/glwpdxgdp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gdvmljvac.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.vehdjk.com/Article/details/ggdjffdvc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gpnfvhxxw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gcgfbvuan.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gofdzeuuk.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gfxqhgeoq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.bbcook.cn/Article/details/gowxixqql.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.yfazqb.com/Article/details/gndbofauz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.sjlbkw.cn/Article/details/giqzhkgsy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gchiokdxc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.sjlbkw.cn/Article/details/gfsrvekcz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fktsv.cn/Article/details/gmriznawe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.tarul.cn/Article/details/gmtbrexem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/ghyyvxdek.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.tarul.cn/Article/details/gkhajvmir.sHtML

[F08] 遍历目录
来源：http://baike.yfazqb.com/Article/details/gdydybdwo.sHtML


<!-- 参考信息 -->