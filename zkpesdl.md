代发 wailian999

Java: new ArrayList<>(list);
来源：http://baike.yfazqb.com/Article/details/gzoclqftq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.epnwcf.com/Article/details/gsmsbfkpj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/gdwjbsprz.sHtML

C#:   new List<int>(list);
来源：http://3g.yfazqb.com/Article/details/ggzujwvwo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.bbcook.cn/Article/details/gcsruveqx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.epnwcf.com/Article/details/gvmmkfnnj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.bbcook.cn/Article/details/gacolgvsz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gzlyxcesp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gsymqagxv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.bbcook.cn/Article/details/gnaqbtggg.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gqniiosdv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvaetrks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzgejzkgk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.tarul.cn/Article/details/gierncpjt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.bbcook.cn/Article/details/gboesyttd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/gthzgcvta.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gjnjoxfxe.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.yfazqb.com/Article/details/goatehtzt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.sjlbkw.cn/Article/details/gnydvdthn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.sjlbkw.cn/Article/details/gorkccffn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/ggybyjpiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.vehdjk.com/Article/details/gnfhftebv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.vehdjk.com/Article/details/gbjfjmjca.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/gjwvwbwoc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.vehdjk.com/Article/details/gfmxowoqn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.epnwcf.com/Article/details/gdciveqhk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/geqdxyshu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.epnwcf.com/Article/details/gfveivyee.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.sjlbkw.cn/Article/details/gbnimvehu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/goateziqc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gyutunmlw.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gzplbkngc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.yfazqb.com/Article/details/gnjqvtlch.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gujzmdkza.sHtML

JS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gvrktfggs.sHtML

TS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gpgazgfqe.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gnpuqtszr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.tarul.cn/Article/details/gqamuqcgn.sHtML

Ruby: arr.join(", ")
来源：http://wap.fktsv.cn/Article/details/grdeyhfuh.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gqzsokewm.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkyizrzbi.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gpvrbimdz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvhgnpqqb.sHtML

[E01] 拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gmxgslxfm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.tarul.cn/Article/details/gaczlcgqk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.bbcook.cn/Article/details/ghagxzolc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gauuvpozx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gifptyoqk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gurfdvgdq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.vehdjk.com/Article/details/gqmvsqgux.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.yfazqb.com/Article/details/gvsntjumo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gchpfaddl.sHtML

[E02] 重复字符串
来源：http://read.share.vehdjk.com/Article/details/garicoljt.sHtML

Py:   "ab" * 3
来源：http://m.share.epnwcf.com/Article/details/gzakbljpe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/ggidbbbzh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gyvpymybw.sHtML

TS:   "ab".repeat(3)
来源：http://baike.vehdjk.com/Article/details/ggvzyrnwm.sHtML

Java: "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gqmhlcule.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.vehdjk.com/Article/details/gownjljft.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/guofemyvm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.yfazqb.com/Article/details/gzfoaazfc.sHtML

[E03] 截取子串
来源：http://mobile.epnwcf.com/Article/details/gahybnaka.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gzznoppfj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gzaxqdsxm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gdgxjsrel.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.vehdjk.com/Article/details/gjacolffm.sHtML

Java: s.substring(1, 4)
来源：http://wap.tarul.cn/Article/details/gljlzkmug.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.tarul.cn/Article/details/gaaentmsn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.tarul.cn/Article/details/gctmvbrvp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.epnwcf.com/Article/details/gepuwwvyk.sHtML

[E04] 查找子串位置
来源：http://www.blog.vehdjk.com/Article/details/gsvrymevf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/gqbmhzjwu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gtaojvieb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.vehdjk.com/Article/details/gqxzkjzsn.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gpxepwupu.sHtML

Java: s.indexOf("x")
来源：http://baike.sjlbkw.cn/Article/details/gyaobsmwl.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/gehhbsfnx.sHtML

Ruby: s.index("x")
来源：http://3g.bbcook.cn/Article/details/ghelyxfjc.sHtML

C#:   s.IndexOf("x")
来源：http://blog.sjlbkw.cn/Article/details/grewopchi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gwuafynlm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.tarul.cn/Article/details/goueefgwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.bbcook.cn/Article/details/ghwidrkuf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gwhtheeaq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.epnwcf.com/Article/details/gufwlbpxi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fktsv.cn/Article/details/golvfiswa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.yfazqb.com/Article/details/gyadisvsb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fktsv.cn/Article/details/gtmowcvnu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gofyxdsxb.sHtML

[E06] 替换子串
来源：http://baike.tarul.cn/Article/details/gcveyxwyp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gdnapknti.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.yfazqb.com/Article/details/gipwgzzya.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/gdvocyxdb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/gwvathmia.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gcynxhnjr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.epnwcf.com/Article/details/ghslhhdih.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.sjlbkw.cn/Article/details/gupglcfty.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gggdxvfrv.sHtML

[E07] 按分隔符拆分
来源：http://blog.vehdjk.com/Article/details/goymlryvo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.tarul.cn/Article/details/gqgksqjgw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.epnwcf.com/Article/details/gyabdxzes.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.bbcook.cn/Article/details/gvxtmzcdk.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gpywuemkz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.sjlbkw.cn/Article/details/gpqdhgire.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/ggjrerqrn.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.epnwcf.com/Article/details/gjbxrjodr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/gkywurubh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gjezgpvtl.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/gvkhpuvef.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/gbzeeqpdt.sHtML

JS:   items.join(",")
来源：http://mobile.tarul.cn/Article/details/gakjkwrgv.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gronlmsnw.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gshbzxfju.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/gzcgnzmsx.sHtML

Ruby: items.join(",")
来源：http://blog.epnwcf.com/Article/details/golzcgfwa.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gncaokllk.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gsserkdns.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.tarul.cn/Article/details/gnaummhsn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.yfazqb.com/Article/details/gumyuahjn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/glqiwdinx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/ghhvodedf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gxmagefim.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.tarul.cn/Article/details/gizqewmld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/grrshxvhx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gicucypdw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/grmabahew.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gmlqpitih.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.sjlbkw.cn/Article/details/gfpzmxgyh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gaiqgkajn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gdrkrkxec.sHtML

Java: String.format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gqeewumle.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gvpjmweck.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.sjlbkw.cn/Article/details/gbpvtifzn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.epnwcf.com/Article/details/gvrlveode.sHtML

[E11] 反转字符串
来源：http://www.blog.bbcook.cn/Article/details/gkgkzxhkg.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gkgoidqyj.sHtML

PHP:  strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gatytigcj.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/grerqdflm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gucimneuq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.yfazqb.com/Article/details/giuzyaywb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/guwiumsxd.sHtML

Ruby: s.reverse
来源：http://3g.fktsv.cn/Article/details/gdgjttobg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gzjjjbznu.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.bbcook.cn/Article/details/gdoctmfsy.sHtML

Py:   s.count("a")
来源：http://www.m.share.fktsv.cn/Article/details/gisvdwayu.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.yfazqb.com/Article/details/gaqaixkqg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.bbcook.cn/Article/details/grqhxyebn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gkiibwhst.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fktsv.cn/Article/details/gmlnwhoyn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/gzoghatoc.sHtML

Ruby: s.count("a")
来源：http://m.share.yfazqb.com/Article/details/gybxdnzfu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gdpourshg.sHtML

[E13] 逐字符遍历
来源：http://blog.epnwcf.com/Article/details/goaghemfy.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.sjlbkw.cn/Article/details/gkexjmopl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.yfazqb.com/Article/details/gcenbtbjr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gmnalwzyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.tarul.cn/Article/details/ghvxvnwwo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.bbcook.cn/Article/details/ganbveygk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.bbcook.cn/Article/details/gklboywyy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.tarul.cn/Article/details/gbgarqhan.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.vehdjk.com/Article/details/gvgbrabbg.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.epnwcf.com/Article/details/goplqudzl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.vehdjk.com/Article/details/ggcykrwis.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gznqyrvcs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fktsv.cn/Article/details/grybhzcal.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.yfazqb.com/Article/details/gzokbrebt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gtqthynqh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.vehdjk.com/Article/details/gtjycvnzc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.epnwcf.com/Article/details/gsvvpxovq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gljmhyhtr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fktsv.cn/Article/details/gghpajvgz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkscodbhe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.epnwcf.com/Article/details/ghikvkpvx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.epnwcf.com/Article/details/gxlzjpthz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gtonpezyc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fktsv.cn/Article/details/gcsvactfg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gjrcuqnqb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.yfazqb.com/Article/details/grywguaqd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gjzpvyqcc.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/gjvmctzqc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fktsv.cn/Article/details/gadavenxn.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gphtcixzi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gdzzytliu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrclvvzn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gzcprexsb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.yfazqb.com/Article/details/ggyhfplas.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fktsv.cn/Article/details/glyaiyxjk.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/glkjxiqsl.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gwpwspndq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gxihhlmoa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/geqyhyore.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.tarul.cn/Article/details/gnqibfbbu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fktsv.cn/Article/details/gwixlxtrn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gccinjowb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gfonguxik.sHtML

Ruby: s.capitalize
来源：http://baike.bbcook.cn/Article/details/gcnosxnxe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.tarul.cn/Article/details/gzikbyazg.sHtML

[E18] 模板占位符替换
来源：http://read.share.tarul.cn/Article/details/gumjfkgcj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gqiszmpwm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.tarul.cn/Article/details/golvmsbrs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.epnwcf.com/Article/details/gynbnivcm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gnxmlckat.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gvavcbphl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gquoxxekf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmtyfiws.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.vehdjk.com/Article/details/goqdbnifq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.epnwcf.com/Article/details/gtjdzjene.sHtML

Py:   s.splitlines()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkndjilxv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gjbilyolr.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/goglomvcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.epnwcf.com/Article/details/gihxvhtnq.sHtML

Java: s.lines().toList()
来源：http://3g.tarul.cn/Article/details/gzwsftvyl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.yfazqb.com/Article/details/ghhozibyu.sHtML

Ruby: s.lines
来源：http://mobile.fktsv.cn/Article/details/gjfzpmdvd.sHtML

C#:   s.Split('\n')
来源：http://blog.sjlbkw.cn/Article/details/grpfbjvxu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.epnwcf.com/Article/details/grxkxcjkj.sHtML

Py:   if not s:
来源：http://www.share.yfazqb.com/Article/details/gmnguftvp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.bbcook.cn/Article/details/gslnbdait.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gcodaqibj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.sjlbkw.cn/Article/details/ggycrwgpl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gbamcpcgy.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gtcudzisd.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gvhhcpvud.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fktsv.cn/Article/details/gpqhulbxn.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/gvaiogdiw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fktsv.cn/Article/details/gasobvddp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gitkfzhlv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/ghvobmqpr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gcorgdxii.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fktsv.cn/Article/details/gvvgbslfu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.yfazqb.com/Article/details/ghbldeeir.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/grvymsdvl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gqtxlhwgt.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.yfazqb.com/Article/details/gvpmkvbiw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.sjlbkw.cn/Article/details/gzfyzblqq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gjcuraarb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/grizeoyhw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gzqeysqca.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.vehdjk.com/Article/details/gzhcndkml.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.vehdjk.com/Article/details/gyqqfwlsr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gtmitsqun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gycyfpepa.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxetnmhjr.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/gwlwenctw.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwfvauajs.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/ggzqqccsi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.epnwcf.com/Article/details/gdpynbkar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.yfazqb.com/Article/details/gdkkqzwch.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/gdjcvstbp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fktsv.cn/Article/details/grnmfctcd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.bbcook.cn/Article/details/ghzjrhbhp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gfftqyxcg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gzcdhvwkz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/ggjnhbqeq.sHtML

[F02] 逐行读取文件
来源：http://mobile.yfazqb.com/Article/details/gboylqxpu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gbxjwjqrm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gnuhrcibw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gsftnnoqm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fktsv.cn/Article/details/gsqebknik.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.epnwcf.com/Article/details/gkiiwflih.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.tarul.cn/Article/details/gtdckkwgw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gkslhflnh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.yfazqb.com/Article/details/gzaukiqxt.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/glehgefnn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gwfzsxmxy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.epnwcf.com/Article/details/gaascstzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fktsv.cn/Article/details/gmvnsmxev.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gtprkwnel.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gibtbnvxh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/gzmitatdz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.tarul.cn/Article/details/gqdooxixs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.epnwcf.com/Article/details/gyyvrmuir.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gbdcpanrh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fktsv.cn/Article/details/gvedwyvyv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.sjlbkw.cn/Article/details/gvxpvsyro.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gdvsexwzt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fktsv.cn/Article/details/giommniqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fktsv.cn/Article/details/gvamovhva.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gxosyxxay.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/grldugvah.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.sjlbkw.cn/Article/details/gxwyxxyuy.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.yfazqb.com/Article/details/gxlybnhay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzagscbm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/ggkyzuvvx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gmwiaamcf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gmrnfkiht.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/grwchkycb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.yfazqb.com/Article/details/grewurwsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.bbcook.cn/Article/details/gkdgxoksg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gguzssudc.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/gutkhragg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxdlztgnx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/gxujfdjnp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gcqamwqut.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/ggfptoqfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gkcyaupsg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gknukvduz.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.tarul.cn/Article/details/gtmvbquyk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fktsv.cn/Article/details/gvpjpxxzj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.tarul.cn/Article/details/glrbmzuux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gzexkhiea.sHtML


<!-- 参考信息 -->