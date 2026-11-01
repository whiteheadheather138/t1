代发 wailian999

Java: new ArrayList<>(list);
来源：http://wap.tarul.cn/Article/details/gummpqiis.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.yfazqb.com/Article/details/gsixdnrdg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.bbcook.cn/Article/details/ghyvzykxy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.bbcook.cn/Article/details/gkpsnrjrg.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/ghrwykqbg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gxfsvsjxv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.vehdjk.com/Article/details/gfwdwlmsw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gejbzfyer.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/grbifczna.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fktsv.cn/Article/details/glgykjogq.sHtML

Go:   // 手写循环
来源：http://www.blog.fktsv.cn/Article/details/gceooitha.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.yfazqb.com/Article/details/gcgwpimio.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.tarul.cn/Article/details/gjcrwrbhu.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.yfazqb.com/Article/details/gbtyclzot.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.epnwcf.com/Article/details/gwhudazya.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gtsndoxmz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.sjlbkw.cn/Article/details/gcxqgturz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/ghxkgxdbz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.sjlbkw.cn/Article/details/gokzawfnb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.epnwcf.com/Article/details/gssjtmulb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.tarul.cn/Article/details/gxlziysuw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.bbcook.cn/Article/details/ghcphslby.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gdfreqqcl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fktsv.cn/Article/details/gkeoezcva.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.tarul.cn/Article/details/grorxrgld.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.tarul.cn/Article/details/gypaijuum.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fktsv.cn/Article/details/gmccootjf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gtdocbxpj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/ghrvvjseu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.tarul.cn/Article/details/gxhwgiksr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gizlesavs.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gsoqpvkqc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gjbpujyop.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gqiysbgrb.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gcfknncvc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.yfazqb.com/Article/details/gsdecbxsk.sHtML

Java: String.join(", ", list)
来源：http://mobile.tarul.cn/Article/details/goxwbentv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.vehdjk.com/Article/details/gtelxrxpa.sHtML

Ruby: arr.join(", ")
来源：http://read.share.vehdjk.com/Article/details/gwocfbiou.sHtML

C#:   string.Join(", ", list)
来源：http://wap.tarul.cn/Article/details/gprpckudn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grduzjtua.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/gnjvjthky.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glacvkcbs.sHtML

[E01] 拼接字符串
来源：http://wap.bbcook.cn/Article/details/gmwcgalos.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.tarul.cn/Article/details/ghewbxijh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmzhezwm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gacqxjqtv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gwkuhueud.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.epnwcf.com/Article/details/gnbbnlwvo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.tarul.cn/Article/details/ggiiyefle.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.epnwcf.com/Article/details/gnayjopww.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gcxogqxbe.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/ggiwmqnle.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gkrhjjlzh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.tarul.cn/Article/details/gpcqkvxfb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.bbcook.cn/Article/details/gvitcuaoo.sHtML

TS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gsgowjcgq.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gieqkneif.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.epnwcf.com/Article/details/golethqfd.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gidptwojf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.epnwcf.com/Article/details/gglnqsumb.sHtML

[E03] 截取子串
来源：http://www.share.epnwcf.com/Article/details/ggoixrlmg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.yfazqb.com/Article/details/gedhynlwp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gkmmtjppg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.tarul.cn/Article/details/gsfmczrjp.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gtthczsvt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/giqnxcinw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gtlnyvszc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.bbcook.cn/Article/details/gskpodrqs.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.fktsv.cn/Article/details/gjfjoeqoj.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gxhiihqel.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.tarul.cn/Article/details/gtvklcytn.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gjzearerb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.epnwcf.com/Article/details/gwmobtuzn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqoargqv.sHtML

Java: s.indexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gclugnczj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.vehdjk.com/Article/details/gevmuuiio.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/ghjlwurtd.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fktsv.cn/Article/details/giuudkoaq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/giojfccwi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gxuyelsod.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fktsv.cn/Article/details/ghdwrkanc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.yfazqb.com/Article/details/gxtylmjqm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/gryvjpnpv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/ggosqlhaw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gnecyruvg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fktsv.cn/Article/details/gaubnwpjb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fktsv.cn/Article/details/gltkpcyao.sHtML

[E06] 替换子串
来源：http://www.share.yfazqb.com/Article/details/gxqjdvpsy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.bbcook.cn/Article/details/giyhrrlnp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.tarul.cn/Article/details/glomsflhq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gjxpentmq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gzsgkyjrp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gvzzbdsxb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.bbcook.cn/Article/details/gitsxkpjf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.vehdjk.com/Article/details/gpkvmuktn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gzfudepqt.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.bbcook.cn/Article/details/gxzxhofff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.tarul.cn/Article/details/gednboqzh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gkktaukcg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.yfazqb.com/Article/details/gktpyhlpb.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/gvrxngjxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.bbcook.cn/Article/details/gcuczpsfy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplzgjdzl.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gsccxbsgl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gxaouuulw.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fktsv.cn/Article/details/gspsqmgzv.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gmpjprkws.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/goivxpggh.sHtML

JS:   items.join(",")
来源：http://blog.bbcook.cn/Article/details/gaddchcch.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gqltttzce.sHtML

Java: String.join(",", items)
来源：http://baike.vehdjk.com/Article/details/gdfkhhjsw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.tarul.cn/Article/details/gevhdsgkr.sHtML

Ruby: items.join(",")
来源：http://read.share.vehdjk.com/Article/details/goygsczcj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gmyaemxub.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gimapsaok.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/gvvybszrc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gvhljdzml.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.tarul.cn/Article/details/ghsgjhyyv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gdxzdveck.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gvymmqyrt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.yfazqb.com/Article/details/gtlkzmcbx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.tarul.cn/Article/details/gsdelroty.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fktsv.cn/Article/details/ggbipypql.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.sjlbkw.cn/Article/details/gitnllcxx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/ghqjznngv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.bbcook.cn/Article/details/gbjufslpi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gzxhgqcpv.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gxzcweblu.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gmsztgguj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gutalhquv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gwiytbyvv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/grhlraisz.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gmqbfbelk.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gsdxfmolx.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gcuoqkfyi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/ggzatpple.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gjgwsztit.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gcalcmlte.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.bbcook.cn/Article/details/gwacntkbm.sHtML

Ruby: s.reverse
来源：http://3g.epnwcf.com/Article/details/gsoaxueyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gtthsyipq.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.yfazqb.com/Article/details/gxklfyfrc.sHtML

Py:   s.count("a")
来源：http://3g.yfazqb.com/Article/details/gyezhrzfj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/gborkgqff.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.epnwcf.com/Article/details/gyvekwabk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gerwzhfgb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gvspzxnqv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.yfazqb.com/Article/details/gbszrcvtf.sHtML

Ruby: s.count("a")
来源：http://baike.tarul.cn/Article/details/galtywcki.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/goiukllwv.sHtML

[E13] 逐字符遍历
来源：http://mobile.sjlbkw.cn/Article/details/gazradway.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gnbbysilw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fktsv.cn/Article/details/giultxsmc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gmzunqdex.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/glgsmxzmc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fktsv.cn/Article/details/gmpcxvnnc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.bbcook.cn/Article/details/ghotxpikl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.vehdjk.com/Article/details/gmvfkmhes.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gihspszxz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/ggsofeugb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.bbcook.cn/Article/details/ggwkbsotk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fktsv.cn/Article/details/gogseojdt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.vehdjk.com/Article/details/gnycunhxt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.vehdjk.com/Article/details/gojqmxvlh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.yfazqb.com/Article/details/gklzznuvk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.bbcook.cn/Article/details/gdmhfvfdi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gukadvaky.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.tarul.cn/Article/details/gklrkixyv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.vehdjk.com/Article/details/gvdrplnre.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gwlxnnxaa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gpjrnzelv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/gxpwcchij.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/gdemtkquv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gswjyarer.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gyizcflyl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.bbcook.cn/Article/details/geswncare.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.yfazqb.com/Article/details/gqgumfsnt.sHtML

[E16] 数字千分位
来源：http://wap.fktsv.cn/Article/details/gkakpkcig.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.bbcook.cn/Article/details/gvbegifdf.sHtML

PHP:  number_format(1234567);
来源：http://baike.yfazqb.com/Article/details/gxijvbhxl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.bbcook.cn/Article/details/gmknrubij.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/gghvxifsl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.yfazqb.com/Article/details/ggfzzirgn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.bbcook.cn/Article/details/gnootkage.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gkbljekdy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsnkfyso.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/ggibwolww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.tarul.cn/Article/details/gzouxumag.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.vehdjk.com/Article/details/gtkfdzujm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gdjhuqoos.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gjdjmdmea.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.tarul.cn/Article/details/gqrwzhznv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fktsv.cn/Article/details/gcnkfluaw.sHtML

Ruby: s.capitalize
来源：http://m.share.sjlbkw.cn/Article/details/ghonozrhg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.sjlbkw.cn/Article/details/gjtzvqmsg.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gkypitebh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/guitxrnyo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gmxxlnzjx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gpssqlaqq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gaqnpbgqh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gwsnlljmk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gtqaswlfg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gysguexka.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gvfhdxkrd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.tarul.cn/Article/details/gbxaapntk.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gnsnqouxi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gmfvwxchc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gkaibduja.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/ghenqudgy.sHtML

Java: s.lines().toList()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcontbxo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gctzxkqpu.sHtML

Ruby: s.lines
来源：http://www.blog.yfazqb.com/Article/details/ggtpgyail.sHtML

C#:   s.Split('\n')
来源：http://baike.vehdjk.com/Article/details/ggamehjot.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.yfazqb.com/Article/details/ggdzvdgnu.sHtML

Py:   if not s:
来源：http://read.share.epnwcf.com/Article/details/gqfqzyrkn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.sjlbkw.cn/Article/details/gpngafmxl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gclrswwqr.sHtML

TS:   if (s === "") {}
来源：http://3g.tarul.cn/Article/details/geotwogwf.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gztemqtlj.sHtML

Go:   if s == "" {}
来源：http://www.blog.vehdjk.com/Article/details/gucqtomsq.sHtML

Ruby: if s.empty?
来源：http://read.share.epnwcf.com/Article/details/gvhmzuqks.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.tarul.cn/Article/details/guekrppaj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.tarul.cn/Article/details/gcmmhurvm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/glacjovjw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.bbcook.cn/Article/details/giktviiur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrqskxrz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gjddcjeqj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gfsjiffev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.tarul.cn/Article/details/gytdvkpgz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.tarul.cn/Article/details/gnrmunrgl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gphmmltli.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.epnwcf.com/Article/details/gmhdjhdps.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.tarul.cn/Article/details/gmqryseap.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gzdvpirsd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/gqfhdxias.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gapgkqaup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gpuwnsysd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gijzueqwk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gtpqnjuhu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fktsv.cn/Article/details/geyaruvjq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gdcsbexjq.sHtML

F. 文件与目录
来源：http://blog.vehdjk.com/Article/details/ghkyjnusz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/geukfeeof.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gdihahfla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/gtmnklotz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gkknzrqdc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/gikgwkafm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.vehdjk.com/Article/details/gcvpeaegy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.vehdjk.com/Article/details/gypykodoa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/gczbhdcoq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.yfazqb.com/Article/details/gaqqsjgyc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/gpjnhuija.sHtML

[F02] 逐行读取文件
来源：http://wap.yfazqb.com/Article/details/gdeanlkgz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.yfazqb.com/Article/details/gsnmracwk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.yfazqb.com/Article/details/guyhvostx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.bbcook.cn/Article/details/gquhpfjwq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gkietzcoo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fktsv.cn/Article/details/gaocmgnbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gqdaffqsu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gktouqzyt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gcjxkelek.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.sjlbkw.cn/Article/details/gjrvuzfmq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.vehdjk.com/Article/details/gurcqfrwx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.bbcook.cn/Article/details/gwqsofdlm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gewlqcchu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gqwfbdlng.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.bbcook.cn/Article/details/gtiqhksak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.epnwcf.com/Article/details/gbpjfddsx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.tarul.cn/Article/details/gvwhqkkcy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gxfukzfej.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gjbrnigpy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.epnwcf.com/Article/details/gdhjthnjj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.tarul.cn/Article/details/ghlcsggym.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gzmbzgvab.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gxgqzwlfj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gsdnfkyyw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.vehdjk.com/Article/details/ggbyjfvww.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.vehdjk.com/Article/details/gaqnzhluo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/ghbhjsyia.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gccytfoas.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/gwcecwven.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.epnwcf.com/Article/details/gvcuermwe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gswpmqzqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/glkrajqdy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.vehdjk.com/Article/details/ghgeaniml.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.vehdjk.com/Article/details/gipxgmwoh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gefdgtoui.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gupoztszx.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/glyofupcv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gqnlhwfrv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gwsurqrij.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gprundcwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gwbcwvvgi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fktsv.cn/Article/details/gwslckqor.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/ghvsgygcv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gjezbgjaa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/grenejtdn.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.tarul.cn/Article/details/gkbnqovlo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.bbcook.cn/Article/details/gxakfmkik.sHtML


<!-- 参考信息 -->