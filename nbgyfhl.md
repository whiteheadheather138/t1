代发 wailian999

Java: new ArrayList<>(list);
来源：http://mobile.sjlbkw.cn/Article/details/gbeggjntx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/gpozgdyca.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.vehdjk.com/Article/details/gwortbuhs.sHtML

C#:   new List<int>(list);
来源：http://www.share.tarul.cn/Article/details/grylgvhdz.sHtML

[D23] reduce 累积计算
来源：http://baike.vehdjk.com/Article/details/gqzsmengh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fktsv.cn/Article/details/ghfyxyuyu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.bbcook.cn/Article/details/grcxtkgob.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gxuafvlpj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/gibhifgfp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gifncfqra.sHtML

Go:   // 手写循环
来源：http://wap.fktsv.cn/Article/details/gdhztnnnz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/gnliwiqgh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gckmatnbh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.bbcook.cn/Article/details/ggqvugjjx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.epnwcf.com/Article/details/gnptaklzk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gqotzmktv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.epnwcf.com/Article/details/gdcqpotzj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/guetdpxkg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gmyncikls.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.vehdjk.com/Article/details/gbtkyuvwp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.sjlbkw.cn/Article/details/gtqjqxbkb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gtmdqmvey.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.yfazqb.com/Article/details/glgswxabn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.sjlbkw.cn/Article/details/grrimrwpq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/glrqlliag.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gnrfefvpf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.vehdjk.com/Article/details/gsplovxff.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/ggemmkdui.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gppwybrfv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.vehdjk.com/Article/details/gnicaffov.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gtzycinii.sHtML

[D26] 数组转字符串
来源：http://mobile.epnwcf.com/Article/details/gxpjmfzof.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fktsv.cn/Article/details/gnbdzefle.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gkmkybiox.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gyejdhmxc.sHtML

TS:   arr.join(", ")
来源：http://blog.yfazqb.com/Article/details/gguvihpgd.sHtML

Java: String.join(", ", list)
来源：http://baike.epnwcf.com/Article/details/ggkustiut.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gqhrnubov.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/glbwvgfbm.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.epnwcf.com/Article/details/gwdqdsxwn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbhkbevva.sHtML

E. 字符串处理
来源：http://www.blog.epnwcf.com/Article/details/gupbtbiic.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/giomshwax.sHtML

[E01] 拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gvilmihlu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.bbcook.cn/Article/details/gtgwuzopj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gttmnvyyg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gzsrfzisz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gitaczieh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fktsv.cn/Article/details/gipauvjvs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.bbcook.cn/Article/details/gddtinibv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gifcsphni.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gsonwsgzr.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gyipzbwsn.sHtML

Py:   "ab" * 3
来源：http://m.share.vehdjk.com/Article/details/guqcfkxte.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.bbcook.cn/Article/details/gabcosazv.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gnkffoaly.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gtuhkyath.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/gjllwfigb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/gtvtltocf.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/grzbqzafh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.sjlbkw.cn/Article/details/gmcnksbpo.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gdqhekkvf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.sjlbkw.cn/Article/details/gllwfthfr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gymarwkdp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.vehdjk.com/Article/details/gbmwvjcba.sHtML

TS:   s.slice(1, 4)
来源：http://3g.epnwcf.com/Article/details/gilgrupvu.sHtML

Java: s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gnmgqfuqz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.sjlbkw.cn/Article/details/gptbnabpj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/govjbbsws.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.yfazqb.com/Article/details/gdksrhixa.sHtML

[E04] 查找子串位置
来源：http://www.share.tarul.cn/Article/details/gklectysb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gbuvdkqwy.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fktsv.cn/Article/details/gyecabuus.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/grahsanhw.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/guxwalrmv.sHtML

Java: s.indexOf("x")
来源：http://3g.yfazqb.com/Article/details/gfmpmrxjs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.vehdjk.com/Article/details/gksmrwiho.sHtML

Ruby: s.index("x")
来源：http://baike.tarul.cn/Article/details/gkznvwjha.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gukcthgen.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.vehdjk.com/Article/details/gtyxbeiud.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.vehdjk.com/Article/details/gfbstvmck.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.vehdjk.com/Article/details/grqfaoiuj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/grrlvxwen.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/gyndazlwh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gfrjkyrjb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.bbcook.cn/Article/details/gngkjkaik.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/gsgqhkuup.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.sjlbkw.cn/Article/details/ggdupxyyo.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gszgtwqvw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gfpjskrqv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.bbcook.cn/Article/details/guvcscfsc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gtacwamcq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/gwdcuknbt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gegdiivgt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.yfazqb.com/Article/details/gqctdgpjh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gilikyjxq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gfyhpdgak.sHtML

[E07] 按分隔符拆分
来源：http://3g.epnwcf.com/Article/details/gwtuxdwnv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.bbcook.cn/Article/details/ghjmssthc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.tarul.cn/Article/details/gvxjlbtun.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/goylpdtun.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gqyqufytb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.bbcook.cn/Article/details/gibbgexwn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.bbcook.cn/Article/details/gftfkmpet.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.sjlbkw.cn/Article/details/gucamhell.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fktsv.cn/Article/details/gwbkcirsp.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.sjlbkw.cn/Article/details/gfzzhgodx.sHtML

Py:   ",".join(items)
来源：http://read.share.epnwcf.com/Article/details/gpfgqfdtt.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gmswyswdy.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/ggorlpvur.sHtML

TS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/glvvqziqu.sHtML

Java: String.join(",", items)
来源：http://wap.vehdjk.com/Article/details/gxnbjjghj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/gjwzccumt.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gqdyuynth.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gtdolxsbu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/gpifrjoeg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.epnwcf.com/Article/details/ggjchcicl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.epnwcf.com/Article/details/gxnuzsscq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gbbrzkdaf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gdeueqoqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fktsv.cn/Article/details/gaqigdhns.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.vehdjk.com/Article/details/gdfrsevbc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.sjlbkw.cn/Article/details/gfbnaomop.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gugdmqezn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.yfazqb.com/Article/details/gewnlbvcn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gmekoswhr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/gisgkqkqd.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.sjlbkw.cn/Article/details/gmdeusntp.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gbzdgevsu.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/ghiglcfdb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gdxoeiwdp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.tarul.cn/Article/details/gaafcfnvq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/ggmrnhmhe.sHtML

[E11] 反转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gfevzrqrv.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gkfarsylz.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gcaigorsx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gbivknddw.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gasnqrolt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gsuadfvxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gehrbcvdw.sHtML

Ruby: s.reverse
来源：http://read.share.fktsv.cn/Article/details/ggxqoiant.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gafgabvsw.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.tarul.cn/Article/details/gguuskjkr.sHtML

Py:   s.count("a")
来源：http://m.share.fktsv.cn/Article/details/glsggkbqo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gjllnxgdj.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.yfazqb.com/Article/details/gfsjjhurw.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gaaulrcnk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.tarul.cn/Article/details/gzfxxvzog.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.epnwcf.com/Article/details/gkmkyzdny.sHtML

Ruby: s.count("a")
来源：http://baike.yfazqb.com/Article/details/gtaohrqhg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.bbcook.cn/Article/details/gnftjwcwa.sHtML

[E13] 逐字符遍历
来源：http://3g.fktsv.cn/Article/details/ggoecfixb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.sjlbkw.cn/Article/details/gvtwdzteb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.yfazqb.com/Article/details/gqavwjmwp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gnmrhhrbn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.yfazqb.com/Article/details/gzeewucyh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gzazknqei.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.vehdjk.com/Article/details/ggspuhxcb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.tarul.cn/Article/details/gbmnwswkn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.vehdjk.com/Article/details/ghghswfmn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.sjlbkw.cn/Article/details/gyiulpemd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gmwgzpvlq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/goywwewpu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.yfazqb.com/Article/details/gmmrrrmlf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.vehdjk.com/Article/details/gsxoevkzb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gcxvgodqs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.bbcook.cn/Article/details/gjnhwrdst.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.tarul.cn/Article/details/gmaamnlxq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gjgcuxpge.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.yfazqb.com/Article/details/gwuhrzkzr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.epnwcf.com/Article/details/gbfjbyjds.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.tarul.cn/Article/details/grdhxzlxm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gjjkahvsf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.vehdjk.com/Article/details/ggciyigax.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.epnwcf.com/Article/details/gxcvyeiji.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.bbcook.cn/Article/details/gacfarntz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gxhautjdo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gdkcgjstf.sHtML

[E16] 数字千分位
来源：http://mobile.tarul.cn/Article/details/gnrkfvtoc.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.epnwcf.com/Article/details/ghgiuzjda.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gmogigzyu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.epnwcf.com/Article/details/gtyjioqjm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gbajcwrvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gnpvvbybo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/govynbmnp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.sjlbkw.cn/Article/details/gzlxmtbis.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fktsv.cn/Article/details/gzjmbttln.sHtML

[E17] 首字母大写
来源：http://m.share.bbcook.cn/Article/details/gkaitjppt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gdcufgtqw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.epnwcf.com/Article/details/gxoicblxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/gwshvusfy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gpxcsycmz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.yfazqb.com/Article/details/gkgtzqtry.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/ghyfdyyyk.sHtML

Ruby: s.capitalize
来源：http://www.share.sjlbkw.cn/Article/details/gdmahiydf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gqhmwvlrf.sHtML

[E18] 模板占位符替换
来源：http://baike.yfazqb.com/Article/details/gkonumfpj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gaqebozcr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.sjlbkw.cn/Article/details/goyitdyym.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gklsnbcma.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gqusxzybz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gechqjxfb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gkokiqwdq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.vehdjk.com/Article/details/gnblgwval.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.yfazqb.com/Article/details/gewhsbzjh.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/gernzfefb.sHtML

Py:   s.splitlines()
来源：http://m.share.sjlbkw.cn/Article/details/gtfrrotlg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gmtkyyefh.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fktsv.cn/Article/details/ghspqjenq.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gwhdopbqo.sHtML

Java: s.lines().toList()
来源：http://read.share.bbcook.cn/Article/details/gbdcmjikx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fktsv.cn/Article/details/ghbdilbnj.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gtgatbdbl.sHtML

C#:   s.Split('\n')
来源：http://www.blog.yfazqb.com/Article/details/goygnnqdv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.epnwcf.com/Article/details/guvaxppvf.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gddfsxoxp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.yfazqb.com/Article/details/glmhaidty.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.sjlbkw.cn/Article/details/gdaxvysnw.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/goookalnv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gwlwxtuig.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/geqmjopqi.sHtML

Ruby: if s.empty?
来源：http://www.m.share.tarul.cn/Article/details/gqnucawgd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.vehdjk.com/Article/details/giaxqkwda.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gamhhmvzf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.bbcook.cn/Article/details/gqeqpxlxh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gqujdswtx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.epnwcf.com/Article/details/gowtkendo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gshiiybql.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gukcsgysg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gxlyxfnub.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.sjlbkw.cn/Article/details/gaiszhcfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/gcdfgcivw.sHtML

[E22] 字节长度与字符长度
来源：http://baike.tarul.cn/Article/details/gpcyxeatr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.yfazqb.com/Article/details/goirhljuk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/grfwclfjt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gwhevlxwp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/gofmxjlhy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gbeaddogj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.bbcook.cn/Article/details/gvrsxvlcl.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.sjlbkw.cn/Article/details/ggemvhfva.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/gvnnbtrqo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghyywvrze.sHtML

F. 文件与目录
来源：http://mobile.sjlbkw.cn/Article/details/geeqxxqrw.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gkfukbmlc.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gdxizbeym.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/goiehnibu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/gtgpsegol.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gwraglxhu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.bbcook.cn/Article/details/grdcmcpqy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gadjzdzpn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gonfjmxhv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.vehdjk.com/Article/details/gzopcaspi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fktsv.cn/Article/details/gswdsjuds.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gijcrlrwb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.bbcook.cn/Article/details/gvuustfgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.tarul.cn/Article/details/gbsudeabl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.tarul.cn/Article/details/godglkiby.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.vehdjk.com/Article/details/gglvbqlva.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fktsv.cn/Article/details/gzetmrbkg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.yfazqb.com/Article/details/grtswltfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.bbcook.cn/Article/details/gegthgsoo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/glacscijz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.vehdjk.com/Article/details/ghjmnjxss.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gvwirnudq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.vehdjk.com/Article/details/garwesbub.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gbzctpphw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.yfazqb.com/Article/details/ggdwrcrto.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gbsbzqoyj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.yfazqb.com/Article/details/gkicaanyq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.yfazqb.com/Article/details/gimjmxbmo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gscrxezqr.sHtML

[F04] 追加写入文件
来源：http://blog.tarul.cn/Article/details/gbefcooel.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjncizaoo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fktsv.cn/Article/details/guzgaqmvr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.yfazqb.com/Article/details/gdqixniji.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gzqopjfif.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.yfazqb.com/Article/details/gsyfudwqq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.tarul.cn/Article/details/ggegffjtz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.yfazqb.com/Article/details/gkxxvqbvb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gekwqdayx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.tarul.cn/Article/details/gexpygghe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.yfazqb.com/Article/details/gbaxlujkt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.bbcook.cn/Article/details/gtfdalfyg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gphodmgxi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gcyfjqfmk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gozuqpknn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.sjlbkw.cn/Article/details/gqzvrbemr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gvtssplbh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gvtlsvvta.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gkqaewblx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gbjvpyodk.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.bbcook.cn/Article/details/gruuwydug.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gjpcvxjir.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gvuhpfxof.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gptnoaumm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.tarul.cn/Article/details/gbkcfpall.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/ghtdtcjjt.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.vehdjk.com/Article/details/ggehimhjn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fktsv.cn/Article/details/gwpqwbyik.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fktsv.cn/Article/details/gafmkxhbb.sHtML


<!-- 参考信息 -->