代发 wailian999

[D23] reduce 累积计算
来源：http://www.share.yfazqb.com/Article/details/gwafvuljq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/gldnjojni.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.bbcook.cn/Article/details/gpoaobmsf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fktsv.cn/Article/details/gdsqejwzc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gdhnippzf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/guiwwghrz.sHtML

Go:   // 手写循环
来源：http://blog.bbcook.cn/Article/details/gfskejpqo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gmzkbrsly.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/ghtdaewft.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.vehdjk.com/Article/details/gwfqiynqv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/guiwhodng.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/ggunjicgl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.vehdjk.com/Article/details/gcevwcxbs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.yfazqb.com/Article/details/gjkrgizrz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.yfazqb.com/Article/details/gumkgilpz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.bbcook.cn/Article/details/gnsddgmra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.sjlbkw.cn/Article/details/ghvdvjcdl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/gjfhmsjgh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.bbcook.cn/Article/details/gpdrhqumq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.sjlbkw.cn/Article/details/gmtqfxwrb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.epnwcf.com/Article/details/ggjhfckch.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fktsv.cn/Article/details/gefidtpqz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.tarul.cn/Article/details/gwebtcuen.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.vehdjk.com/Article/details/gdxfowzsh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fktsv.cn/Article/details/gsocsefsl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.vehdjk.com/Article/details/guhsiaipa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gezejjhcx.sHtML

[D26] 数组转字符串
来源：http://mobile.bbcook.cn/Article/details/ggewqisyu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.yfazqb.com/Article/details/gocrboqqc.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.bbcook.cn/Article/details/gvlacstdr.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gxnupostq.sHtML

TS:   arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gfviitkux.sHtML

Java: String.join(", ", list)
来源：http://wap.vehdjk.com/Article/details/goyowelto.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gvcuzwvjs.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gsgxmyasu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/garmbyppj.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/guiwdoiln.sHtML

E. 字符串处理
来源：http://www.m.share.fktsv.cn/Article/details/gdrxqgcsq.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxjwkfmjb.sHtML

[E01] 拼接字符串
来源：http://mobile.vehdjk.com/Article/details/grahvgnte.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.epnwcf.com/Article/details/griyqugou.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gwrcpwmks.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gavajoyib.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gtkbnlokv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.epnwcf.com/Article/details/gmlteyyll.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.epnwcf.com/Article/details/gbgrgzfrw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/gmyfwkfvp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gudljfvdf.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpknjgfwh.sHtML

Py:   "ab" * 3
来源：http://baike.vehdjk.com/Article/details/goiytenbj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/gefxrlwkk.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gozlqijeb.sHtML

TS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gpwdqvucf.sHtML

Java: "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/geisekjkp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gqittgjin.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/grepvxfuv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/gpvjzpdjd.sHtML

[E03] 截取子串
来源：http://read.share.epnwcf.com/Article/details/ghajmrtib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gcvdocapq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gpymeeffz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.epnwcf.com/Article/details/gsyblpuuh.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.yfazqb.com/Article/details/gwovlsoqq.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/gjjubvqjh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gfceeytwk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/gssryhaos.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.sjlbkw.cn/Article/details/gjvhgbkyb.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gjqzhevtr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gsarhsbqn.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gmjmxaprx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.epnwcf.com/Article/details/ghfaoiqdj.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gxrahinan.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/glncfrbcb.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.sjlbkw.cn/Article/details/gysdkrzcl.sHtML

Ruby: s.index("x")
来源：http://wap.sjlbkw.cn/Article/details/grfsbnqtg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fktsv.cn/Article/details/gzudbuhmc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.epnwcf.com/Article/details/gjdvpcjmp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.tarul.cn/Article/details/gkeujinqh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.yfazqb.com/Article/details/grfecpbvv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/golmnnezq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.tarul.cn/Article/details/gdyvptvqy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.vehdjk.com/Article/details/gkufeztuk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gbnsznjol.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.sjlbkw.cn/Article/details/guiazftuv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.epnwcf.com/Article/details/ghftlzidg.sHtML

[E06] 替换子串
来源：http://read.share.fktsv.cn/Article/details/gbehtlyoi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gkughbybg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/gonvbpcan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.bbcook.cn/Article/details/goinoolvy.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/guedqaavu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gvsjbeuiy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gqbnlqdmd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gcvvvxjxv.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gskznaymc.sHtML

[E07] 按分隔符拆分
来源：http://m.share.sjlbkw.cn/Article/details/gkrypajru.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.tarul.cn/Article/details/gqvptkgtn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gfjbllvzq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.tarul.cn/Article/details/grhrktuft.sHtML

TS:   s.split(",")
来源：http://www.share.tarul.cn/Article/details/glzzhoscp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.tarul.cn/Article/details/gcmdnnhtr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gceqrniup.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gumkrqdbd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.tarul.cn/Article/details/gawywdmmb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.yfazqb.com/Article/details/gttillxtu.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/gevmyhqwp.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/gvqusibtp.sHtML

JS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gnbehjrvb.sHtML

TS:   items.join(",")
来源：http://read.share.yfazqb.com/Article/details/gleedfbes.sHtML

Java: String.join(",", items)
来源：http://blog.vehdjk.com/Article/details/gluychkjp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/glhqjqeiq.sHtML

Ruby: items.join(",")
来源：http://m.share.epnwcf.com/Article/details/giwyzfyjy.sHtML

C#:   string.Join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gwqzqyszf.sHtML

[E09] 去除所有空白字符
来源：http://wap.yfazqb.com/Article/details/gmiujtlpo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.vehdjk.com/Article/details/gcgkblkir.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.bbcook.cn/Article/details/gzfbtjstn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gfsvglaez.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gizbzzbwg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.tarul.cn/Article/details/gikbdfcdo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.tarul.cn/Article/details/gbryuxbtg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gklzgphyc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/geqykhwcg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/gjafsbrrk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fktsv.cn/Article/details/geccjpgnq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.bbcook.cn/Article/details/gwppimchf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/gnbycnmjl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gnlkklzve.sHtML

Java: String.format("%03d", 7)
来源：http://blog.vehdjk.com/Article/details/gcuwtifbt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.bbcook.cn/Article/details/gezszvhkf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/gifwypqjr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fktsv.cn/Article/details/guwfozyuf.sHtML

[E11] 反转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gslxcyrcb.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gxggdtxka.sHtML

PHP:  strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gbqkaozsg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gjqwhlros.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gmvgalwff.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/gcsdjvueo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gattemuqk.sHtML

Ruby: s.reverse
来源：http://mobile.tarul.cn/Article/details/gbtjoqibt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gmvegafje.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.sjlbkw.cn/Article/details/goasjkzbt.sHtML

Py:   s.count("a")
来源：http://baike.yfazqb.com/Article/details/ghxzyjnjp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.tarul.cn/Article/details/gvwrumunm.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/gmypchrwn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/giqqyuugz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.tarul.cn/Article/details/godiblewu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.tarul.cn/Article/details/gmepeeixp.sHtML

Ruby: s.count("a")
来源：http://wap.yfazqb.com/Article/details/gxutpwmno.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.yfazqb.com/Article/details/gzmeqmref.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/glbkumffp.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.bbcook.cn/Article/details/ghiicqybq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gnxlkltqp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.epnwcf.com/Article/details/gcarsormt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gyalkmgin.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.epnwcf.com/Article/details/gapawvmrg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/ggveuwehy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/gdcdfthoq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.bbcook.cn/Article/details/ggzhtnsfp.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gxuoruvnf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.tarul.cn/Article/details/glmeultvf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/gmqhxbdjq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/glzmcmlea.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/gkvujlurq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.tarul.cn/Article/details/gielqniwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.tarul.cn/Article/details/gayiyhapw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.vehdjk.com/Article/details/gtntbiizx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gcctxuwoa.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gtmoickrp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.yfazqb.com/Article/details/gnbqmgcwb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.vehdjk.com/Article/details/grsgvihbt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gcosxbhno.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fktsv.cn/Article/details/gnupcylqa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.tarul.cn/Article/details/gbrkjeldb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fktsv.cn/Article/details/gpxbzzsjw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/gjkcpyxzd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gsgoaoxde.sHtML

[E16] 数字千分位
来源：http://www.blog.vehdjk.com/Article/details/gnlyuynhv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gmykzvfyv.sHtML

PHP:  number_format(1234567);
来源：http://3g.yfazqb.com/Article/details/gjujparro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/gqyhfeoyd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gudrtfagg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gsdamikci.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.epnwcf.com/Article/details/ghznaldmj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.bbcook.cn/Article/details/gzkulubfr.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gfdopyjss.sHtML

[E17] 首字母大写
来源：http://m.share.tarul.cn/Article/details/gqtqypqwr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.epnwcf.com/Article/details/gbkgwelei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.yfazqb.com/Article/details/gvztlccvu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.tarul.cn/Article/details/gyrstiotx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gvxsapkga.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gracqmlrf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gkutxgbyg.sHtML

Ruby: s.capitalize
来源：http://m.share.yfazqb.com/Article/details/gazptevsr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.sjlbkw.cn/Article/details/grryjyvxo.sHtML

[E18] 模板占位符替换
来源：http://3g.vehdjk.com/Article/details/gbogxykxp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gttxvdadl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fktsv.cn/Article/details/gqggdmzml.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gtxirumtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gunpqmpji.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.vehdjk.com/Article/details/gdqpzrpgf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/ghyjafrwh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.sjlbkw.cn/Article/details/gzevxajyd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.vehdjk.com/Article/details/gmbwisqlj.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.yfazqb.com/Article/details/gjiiijoyp.sHtML

Py:   s.splitlines()
来源：http://www.blog.fktsv.cn/Article/details/goblexvtx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/goeayxqaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gwttohnin.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gvnotmdau.sHtML

Java: s.lines().toList()
来源：http://wap.fktsv.cn/Article/details/gngzdwzfy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/gliikhmtu.sHtML

Ruby: s.lines
来源：http://www.share.epnwcf.com/Article/details/gjdwvljkm.sHtML

C#:   s.Split('\n')
来源：http://blog.tarul.cn/Article/details/gwpeetwyg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gobyvxuax.sHtML

Py:   if not s:
来源：http://mobile.tarul.cn/Article/details/gotikrkva.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gvmmpsxuw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.tarul.cn/Article/details/gjkoszcvp.sHtML

TS:   if (s === "") {}
来源：http://wap.yfazqb.com/Article/details/gyicatuqj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gwjsmoeve.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/ghlzlriqt.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gefuebasd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gtqehrcin.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.epnwcf.com/Article/details/gcsnajjde.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gxzfjvucp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.tarul.cn/Article/details/ggouccwdz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.epnwcf.com/Article/details/gjgskyrav.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.epnwcf.com/Article/details/gqkcoutbt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/glcemetxs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.vehdjk.com/Article/details/gasotthky.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/gtlomqiij.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gbcthhbuj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fktsv.cn/Article/details/gycjfnjip.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.yfazqb.com/Article/details/gkvlpnrfc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gdzqzmjar.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.sjlbkw.cn/Article/details/grijjvwcb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gfrsygghz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gtbqtslgg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/ghcbcgiad.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.tarul.cn/Article/details/geqigjyfe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/glrxvcqga.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghozwfagz.sHtML

F. 文件与目录
来源：http://read.share.vehdjk.com/Article/details/gmajdzvrp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnhvtmuoa.sHtML

[F01] 读取整个文件
来源：http://www.blog.fktsv.cn/Article/details/gilxaytuf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gkulllawj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grqkzkkfv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gwnjjnmfi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gwrlblioq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/giomqtvxz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gcdiywmmi.sHtML

Ruby: File.read("a.txt")
来源：http://wap.tarul.cn/Article/details/gygfgalkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/ghvlktvfv.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/ggsuaaxod.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fktsv.cn/Article/details/ggjlvizlw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.vehdjk.com/Article/details/gzlxxftod.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.yfazqb.com/Article/details/graeroemj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.vehdjk.com/Article/details/gpswwfjdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.bbcook.cn/Article/details/gkjqibrbb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.vehdjk.com/Article/details/gecmrrsot.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gqrnrtfdx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gbspssmuv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gxvedqpkc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gwlfxkuvg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.sjlbkw.cn/Article/details/gmwqcuvuh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.epnwcf.com/Article/details/gzuhtsivl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.bbcook.cn/Article/details/gyhvbagan.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.epnwcf.com/Article/details/gyqoixnlh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fktsv.cn/Article/details/gnhmtuvqw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.vehdjk.com/Article/details/garijxmpe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.sjlbkw.cn/Article/details/gghhwrixp.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gggctylhn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gwqqpmgvh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.tarul.cn/Article/details/gfipnatan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.bbcook.cn/Article/details/gdwrbyink.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.sjlbkw.cn/Article/details/ggrndeesa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fktsv.cn/Article/details/gjzstajlj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.vehdjk.com/Article/details/ggjtnszkg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gklwpjoxx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gfyjboagk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.tarul.cn/Article/details/gudkzanbe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fktsv.cn/Article/details/gswikggad.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.vehdjk.com/Article/details/gcxwqvars.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gvlthgrqv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.tarul.cn/Article/details/goodokqru.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/gquezthwz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.yfazqb.com/Article/details/gjnyuretg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gzvvsyveb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gsumdlwte.sHtML

[F06] 删除文件
来源：http://m.share.fktsv.cn/Article/details/gaqrqshfp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.tarul.cn/Article/details/gvyxzaxvf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gpdwlknuz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gpuenvmkv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.yfazqb.com/Article/details/gmsheoiyu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/gouuthvog.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gvqtjxfyu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.yfazqb.com/Article/details/gtdzawult.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gdysbyiqa.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fktsv.cn/Article/details/gcevdcrbd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.vehdjk.com/Article/details/gmkukorco.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fktsv.cn/Article/details/gneeziofu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.bbcook.cn/Article/details/gfxhkmwir.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.sjlbkw.cn/Article/details/gcxmbzozx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.yfazqb.com/Article/details/gtxbesvhv.sHtML


<!-- 参考信息 -->