代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gfhkcvoac.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.epnwcf.com/Article/details/gryylxflg.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gcuxdurrc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gzpciwpfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.sjlbkw.cn/Article/details/gxynhyafo.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.vehdjk.com/Article/details/gtemjcgzt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.yfazqb.com/Article/details/gcaanuqfb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.epnwcf.com/Article/details/gwzgeanbw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gpmkiauus.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gmukdrnvv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fktsv.cn/Article/details/gfqwzimhl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.bbcook.cn/Article/details/ggvvxemnv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.epnwcf.com/Article/details/gyqgnkhsg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/groiqzruu.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gfdrwkard.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.epnwcf.com/Article/details/gnsgwplch.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fktsv.cn/Article/details/gberiuljy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/geqdqazkg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.yfazqb.com/Article/details/gisnmlbig.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.epnwcf.com/Article/details/gdcbctsri.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.epnwcf.com/Article/details/gdjoepdum.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.tarul.cn/Article/details/gpbtjctqp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gjjlvyshy.sHtML

[D26] 数组转字符串
来源：http://blog.vehdjk.com/Article/details/gyroxeimk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.bbcook.cn/Article/details/gyrdfcquo.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/grxjxnyln.sHtML

JS:   arr.join(", ")
来源：http://mobile.fktsv.cn/Article/details/glqefonvy.sHtML

TS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gqjfvrfxx.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gqezlmxrv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/ghrzbhifc.sHtML

Ruby: arr.join(", ")
来源：http://blog.bbcook.cn/Article/details/gumsipnmk.sHtML

C#:   string.Join(", ", list)
来源：http://3g.tarul.cn/Article/details/gfwhyseob.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnycyzykh.sHtML

E. 字符串处理
来源：http://www.share.vehdjk.com/Article/details/gkseoonmt.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gxizgrvxn.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/govgorwxo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/ghahsexik.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fktsv.cn/Article/details/gdgbmocmk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.yfazqb.com/Article/details/gdbjnjdha.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gozkqdccm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gsxmioigx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.epnwcf.com/Article/details/goygzotfm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.epnwcf.com/Article/details/glljxloja.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gafsxxxoa.sHtML

[E02] 重复字符串
来源：http://m.share.vehdjk.com/Article/details/gyjhwqkao.sHtML

Py:   "ab" * 3
来源：http://read.share.bbcook.cn/Article/details/gtpdaksli.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.epnwcf.com/Article/details/geoqbjosl.sHtML

JS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/goiqxpgze.sHtML

TS:   "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/gbkfdsked.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gebqihhia.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.yfazqb.com/Article/details/ggthycrmw.sHtML

Ruby: "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/ghyheiqjf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.sjlbkw.cn/Article/details/ggybljbzc.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gbjnayvoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.vehdjk.com/Article/details/gluxhlbbg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/grjbzogpm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gyisdfyos.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gzgltatzu.sHtML

Java: s.substring(1, 4)
来源：http://blog.fktsv.cn/Article/details/gunozoxkt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.epnwcf.com/Article/details/gbqohbuts.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.vehdjk.com/Article/details/gxoztztpq.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gwjamzibe.sHtML

[E04] 查找子串位置
来源：http://m.share.epnwcf.com/Article/details/gxbeyenov.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.tarul.cn/Article/details/gpylpjqor.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.vehdjk.com/Article/details/goyrpdkhu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.epnwcf.com/Article/details/gqsailpny.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gzqiauxlt.sHtML

Java: s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gpyhzswdt.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gxorqrcky.sHtML

Ruby: s.index("x")
来源：http://m.share.sjlbkw.cn/Article/details/gpeidgehl.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gokrlsygf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.yfazqb.com/Article/details/guecisemw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.yfazqb.com/Article/details/gyujxyuze.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gestwpoom.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.yfazqb.com/Article/details/gdbkdfwqi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/gcuwpcpdy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gwlfhzjbj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.sjlbkw.cn/Article/details/gsvxwkkoj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/goyexgmic.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gipmqxivg.sHtML

[E06] 替换子串
来源：http://3g.epnwcf.com/Article/details/gmjpxidcf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fktsv.cn/Article/details/gmhmewsle.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.vehdjk.com/Article/details/gozbkzedn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gnqurqmvh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gryhkshqf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gxnfgcmyw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gsjmjkukb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gtfghfwxy.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.tarul.cn/Article/details/gaydpcbti.sHtML

[E07] 按分隔符拆分
来源：http://blog.bbcook.cn/Article/details/gajgaxuts.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.yfazqb.com/Article/details/gwnidfvoi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.sjlbkw.cn/Article/details/gtaqusmbv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.tarul.cn/Article/details/goeiwrvyz.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/giboosayq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.yfazqb.com/Article/details/gwghnhxjc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.tarul.cn/Article/details/gtsqcnqvb.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.bbcook.cn/Article/details/gbiprerzd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gdoouljgl.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/glmvqwqvh.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/grpfiiihj.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gwuawtehu.sHtML

JS:   items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gibecfzom.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gjvjbozma.sHtML

Java: String.join(",", items)
来源：http://mobile.yfazqb.com/Article/details/gjfbhgfbv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.tarul.cn/Article/details/ggffxtrjh.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gvtuulwbp.sHtML

C#:   string.Join(",", items)
来源：http://3g.epnwcf.com/Article/details/ghzqsqnze.sHtML

[E09] 去除所有空白字符
来源：http://www.share.vehdjk.com/Article/details/gifrziyze.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gbzdpfrys.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gapmnzyvc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/gwjtmehhr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.vehdjk.com/Article/details/gdwmnpsmw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.yfazqb.com/Article/details/gppwreepf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gickfnine.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.tarul.cn/Article/details/gxmsawpcx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.bbcook.cn/Article/details/gfghybzfx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/ggatzhhwx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gkvneejye.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.yfazqb.com/Article/details/gonuntchw.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gsvheiwme.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fktsv.cn/Article/details/gfnufwavx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gzixvffqm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fktsv.cn/Article/details/gcvegeevh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gyidfvvio.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.bbcook.cn/Article/details/gpsolzzsk.sHtML

[E11] 反转字符串
来源：http://www.share.vehdjk.com/Article/details/gwzsafgtu.sHtML

Py:   s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gqbvwwpxk.sHtML

PHP:  strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gmahoibln.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gmrkstfga.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gbfuvfaaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gfrfyyshb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gdkfjrvjk.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gfdnyoadg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gyeqotuoj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.bbcook.cn/Article/details/gbqvaedcs.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gxrpklkvy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.yfazqb.com/Article/details/gehbshbbe.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gxzgamgqm.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/gdalkuhrs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.yfazqb.com/Article/details/gzstkhyjy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.vehdjk.com/Article/details/gxthtrqom.sHtML

Ruby: s.count("a")
来源：http://3g.epnwcf.com/Article/details/gnhdtmdya.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gbaqxrdcn.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/gdcyqkxoy.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.tarul.cn/Article/details/gjqjwnlpo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.epnwcf.com/Article/details/ggrqboocp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gayhtxjea.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gfpqsdyzi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.epnwcf.com/Article/details/gephvubjh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.vehdjk.com/Article/details/ghipqjotz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fktsv.cn/Article/details/gwmjeopdn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.tarul.cn/Article/details/golwctqpi.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.bbcook.cn/Article/details/govpisbyb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.yfazqb.com/Article/details/glhnfrcbb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.bbcook.cn/Article/details/gmvhkgkrd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.sjlbkw.cn/Article/details/gqcempedm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.bbcook.cn/Article/details/goigtxuyx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.vehdjk.com/Article/details/gytbgibmz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gbmkkliuf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gqetgbmkw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gmyluahtv.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.bbcook.cn/Article/details/gtfcvmtvt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gihjraihx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.tarul.cn/Article/details/glnaixjcu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/ghkwrbvnt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.epnwcf.com/Article/details/gwqbnmohx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gywbqneqr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gccapzjie.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fktsv.cn/Article/details/gmyrytgau.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.yfazqb.com/Article/details/gskyqkcvi.sHtML

[E16] 数字千分位
来源：http://baike.tarul.cn/Article/details/gokmkoeoc.sHtML

Py:   f"{1234567:,}"
来源：http://baike.vehdjk.com/Article/details/gddwjlwdb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.bbcook.cn/Article/details/gwsuynldg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.vehdjk.com/Article/details/gdkbtcamx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/gahcvqwrg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gjxvnomey.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.vehdjk.com/Article/details/gqttxkuba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.vehdjk.com/Article/details/ghcqmuhsm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.yfazqb.com/Article/details/gxocfnleb.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gqoknlfkm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gnaemxoke.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.yfazqb.com/Article/details/gxpwxvcaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/gfzspeuwr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.bbcook.cn/Article/details/gqbhvzitc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.yfazqb.com/Article/details/gedooldcd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.vehdjk.com/Article/details/grqgnkebe.sHtML

Ruby: s.capitalize
来源：http://wap.yfazqb.com/Article/details/ggqpgzczr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.sjlbkw.cn/Article/details/gtfiurkfa.sHtML

[E18] 模板占位符替换
来源：http://3g.bbcook.cn/Article/details/gwmwdsxhl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.yfazqb.com/Article/details/gmsnrsrle.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwvtaatx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.yfazqb.com/Article/details/gathtjbmc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/giuqgoitk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fktsv.cn/Article/details/glgrzmpjp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gdptlrotl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.tarul.cn/Article/details/galocqjdh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gnqzwfuny.sHtML

[E19] 多行文本按行拆分
来源：http://3g.vehdjk.com/Article/details/ggsprswnk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/gsrpjlgjr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gaqeshrdk.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gvgypidrh.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/ggandyxmd.sHtML

Java: s.lines().toList()
来源：http://www.share.tarul.cn/Article/details/gkbnwgjyb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.epnwcf.com/Article/details/gvojoyupc.sHtML

Ruby: s.lines
来源：http://3g.fktsv.cn/Article/details/gfgztfzdq.sHtML

C#:   s.Split('\n')
来源：http://3g.yfazqb.com/Article/details/gvxsqccrj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fktsv.cn/Article/details/gijhlwcca.sHtML

Py:   if not s:
来源：http://www.blog.fktsv.cn/Article/details/gqkkkqghn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gyygwkkdb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.vehdjk.com/Article/details/gszdipeib.sHtML

TS:   if (s === "") {}
来源：http://read.share.fktsv.cn/Article/details/gjtuzjdvz.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gtmxieesl.sHtML

Go:   if s == "" {}
来源：http://read.share.yfazqb.com/Article/details/gjewcfemx.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gnrapbqnf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.sjlbkw.cn/Article/details/gpknrhvxk.sHtML

[E21] 超长截断加省略号
来源：http://3g.tarul.cn/Article/details/gfogxgsib.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gtgheuavs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fktsv.cn/Article/details/gxkkecmas.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gddmqwgnf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gezkrirfr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gjjbffgjm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.epnwcf.com/Article/details/gcksrnmis.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fktsv.cn/Article/details/gpsxkhben.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gdvsnsrof.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.epnwcf.com/Article/details/gvyseoewo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.bbcook.cn/Article/details/grdiutrbq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gzaqpcufu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.epnwcf.com/Article/details/goqndsrfu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.vehdjk.com/Article/details/gjoqhstvj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gufajklda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/gjnbycbsx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gncatpyie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gecqbuucl.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grrpwttgt.sHtML

F. 文件与目录
来源：http://read.share.fktsv.cn/Article/details/gzvuvenyw.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gxcajasmh.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gokfxqkcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.sjlbkw.cn/Article/details/ggqcfhnza.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.sjlbkw.cn/Article/details/glunbznky.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.sjlbkw.cn/Article/details/gmcklhnkx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gwtdxdezz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gustccpnr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gfqwdxpvn.sHtML

Ruby: File.read("a.txt")
来源：http://3g.sjlbkw.cn/Article/details/gnvyxeciw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gvpruaxbo.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gqzlvfvdn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gabartulr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gbfopyjmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/ghdtetonu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/goydgmrfw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fktsv.cn/Article/details/goebmylxg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/guaspuzsl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.yfazqb.com/Article/details/grztohseu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.yfazqb.com/Article/details/grlvqjeup.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.tarul.cn/Article/details/gbhhhvrap.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fktsv.cn/Article/details/gdnbitixt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fktsv.cn/Article/details/gydlttevq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.sjlbkw.cn/Article/details/gqphlosbn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gdkspbvrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.tarul.cn/Article/details/ghiubqxcy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.bbcook.cn/Article/details/gdbiuzddj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/grwbyaaic.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.bbcook.cn/Article/details/grqqvyrmp.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gzmvhgunu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gygjgmdgc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.yfazqb.com/Article/details/gdvybdxio.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.vehdjk.com/Article/details/gtsghattg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/gvtoddrpr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.vehdjk.com/Article/details/gvrmgkhac.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.sjlbkw.cn/Article/details/gefexuzum.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.bbcook.cn/Article/details/gcmxwlgty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.yfazqb.com/Article/details/gfxwrfwyl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gaxfiupiv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gcrwukyjh.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.vehdjk.com/Article/details/glawbykba.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/gtohuvmfv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gshaenusj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gvwmqawci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.yfazqb.com/Article/details/gvgrlvled.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gknhawygi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gqxazanfr.sHtML

[F06] 删除文件
来源：http://wap.bbcook.cn/Article/details/gbiaabcir.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gvopjqasn.sHtML

PHP:  unlink("a.txt");
来源：http://baike.tarul.cn/Article/details/gddkqgoyw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.yfazqb.com/Article/details/gmehnsuhr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwimtahvt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.vehdjk.com/Article/details/gipuywqut.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.sjlbkw.cn/Article/details/gudepmekm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/grykbqnsg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.tarul.cn/Article/details/gjvyfzmwb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/gevghgfll.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.bbcook.cn/Article/details/ghbzlmpcb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.bbcook.cn/Article/details/gwgbuuxji.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.epnwcf.com/Article/details/gsewaftxp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.vehdjk.com/Article/details/gypdlkcuh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.yfazqb.com/Article/details/gjstbewsa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.epnwcf.com/Article/details/gxuyzbpyb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.tarul.cn/Article/details/gqsvgtmou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.tarul.cn/Article/details/ghlpuolqu.sHtML

[F08] 遍历目录
来源：http://mobile.tarul.cn/Article/details/gwpgzfebb.sHtML


<!-- 参考信息 -->