代发 wailian999

[D23] reduce 累积计算
来源：http://www.m.share.vehdjk.com/Article/details/gcahrkvxp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gqgvxmsqp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fktsv.cn/Article/details/gzwoibnyy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/gyqmyhmau.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.yfazqb.com/Article/details/gxtiponyx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.tarul.cn/Article/details/gfaxczkrx.sHtML

Go:   // 手写循环
来源：http://blog.fktsv.cn/Article/details/glxpuurjk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.epnwcf.com/Article/details/gnutrzhmj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.tarul.cn/Article/details/gdiymrrmf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gmiwkdcge.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/gguuvzuwy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.yfazqb.com/Article/details/gtrhssxys.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.vehdjk.com/Article/details/golbixmls.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gkhoxdznz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.bbcook.cn/Article/details/goaxyvehd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.sjlbkw.cn/Article/details/gifojeksa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gnmbxggtn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.vehdjk.com/Article/details/ggactyvuc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.epnwcf.com/Article/details/gpcoekxbr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.vehdjk.com/Article/details/golnntqpa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.epnwcf.com/Article/details/gfrjcuxgw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/guwemvjbj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gpphzqyer.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/ggjicpyzw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gdonddadz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gknnbfgjt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.vehdjk.com/Article/details/girjakoes.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/ggvdlwewd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fktsv.cn/Article/details/gqnxzakto.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.yfazqb.com/Article/details/gogvkklec.sHtML

JS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gcukriksm.sHtML

TS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gzddurzxl.sHtML

Java: String.join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gzhnrrfkn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.bbcook.cn/Article/details/gqcubwenj.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gciixaqto.sHtML

C#:   string.Join(", ", list)
来源：http://wap.bbcook.cn/Article/details/giczdbplk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqyvrvlcl.sHtML

E. 字符串处理
来源：http://3g.epnwcf.com/Article/details/gizshfdmz.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzxpjybiz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmidimeaf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gfttujkkv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gibzvhnzj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gdfuigmxm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.epnwcf.com/Article/details/gtzwczxto.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gwmouxvnr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gpogggwsr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/glcudtlnr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ghgcugqkb.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gugkegogq.sHtML

Py:   "ab" * 3
来源：http://read.share.epnwcf.com/Article/details/gfyhttrdq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.yfazqb.com/Article/details/gdehoshxg.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fktsv.cn/Article/details/gqsnmpxjr.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gvsygzwht.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gjofairnp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.bbcook.cn/Article/details/giprkphzv.sHtML

Ruby: "ab" * 3
来源：http://mobile.tarul.cn/Article/details/glffhissf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/gpvnybtud.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gettfnzri.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gaenqywvm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gixqptycy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gyyiudmyg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gonbnalib.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/gwkjajmbm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.bbcook.cn/Article/details/gvwaujclh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/gtukdeemw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fktsv.cn/Article/details/ggtdqjxme.sHtML

[E04] 查找子串位置
来源：http://baike.tarul.cn/Article/details/gtkcshywc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.epnwcf.com/Article/details/ghhzrzqbp.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gxkqzonyb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.vehdjk.com/Article/details/gxlwxuutt.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gfufpdobr.sHtML

Java: s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gepdrgbvk.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fktsv.cn/Article/details/gfxfblxwk.sHtML

Ruby: s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gtmkzwknt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.epnwcf.com/Article/details/gnesljuwj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.vehdjk.com/Article/details/gerymdmek.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.sjlbkw.cn/Article/details/gerrxvvzy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gcntzvawy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gjpjalycl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gzlsmlqxq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fktsv.cn/Article/details/gsrifyexm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.yfazqb.com/Article/details/gymcpfujr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.bbcook.cn/Article/details/gwuwwzusq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.epnwcf.com/Article/details/gydrzpniv.sHtML

[E06] 替换子串
来源：http://baike.fktsv.cn/Article/details/gwtlnasoi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.sjlbkw.cn/Article/details/gzystfefd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fktsv.cn/Article/details/ghyxjwilp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/grkdkwxgw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gtfujdpno.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gjtqgfgnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.vehdjk.com/Article/details/glxmhvlds.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.tarul.cn/Article/details/gqtpkumub.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fktsv.cn/Article/details/gepvjrsnw.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gqfrwgens.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.epnwcf.com/Article/details/gchgteary.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gexkcimoj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/ggppgqdyd.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/gwhbawgtj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.vehdjk.com/Article/details/ghkwwqojt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.tarul.cn/Article/details/geiommjyz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gzfgnjdqt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fktsv.cn/Article/details/gnpcdjgrv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.vehdjk.com/Article/details/gefkxrkej.sHtML

Py:   ",".join(items)
来源：http://wap.epnwcf.com/Article/details/gdfspukdc.sHtML

PHP:  implode(",", $items);
来源：http://3g.yfazqb.com/Article/details/gnjpjfcqt.sHtML

JS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gbqukfzuf.sHtML

TS:   items.join(",")
来源：http://www.m.share.yfazqb.com/Article/details/gohcspyzu.sHtML

Java: String.join(",", items)
来源：http://www.m.share.tarul.cn/Article/details/gxjtqkyqc.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/gonjjzprb.sHtML

Ruby: items.join(",")
来源：http://www.blog.yfazqb.com/Article/details/gavthseal.sHtML

C#:   string.Join(",", items)
来源：http://read.share.bbcook.cn/Article/details/gmpqzhzkf.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gllptdhui.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.sjlbkw.cn/Article/details/gigsikvcp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.epnwcf.com/Article/details/grmzpgdho.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gbkaomyyu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gpljtlbzy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gxmqhkkcj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.tarul.cn/Article/details/glkbttttf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.yfazqb.com/Article/details/gqihmcllu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gynilwfys.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.tarul.cn/Article/details/guxuinets.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/gkumfeazj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.epnwcf.com/Article/details/gatfcptqj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gcygujmeu.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/gkfwspuag.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gyvcxsfaw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/gaubxnwjb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/grgifhjzv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fktsv.cn/Article/details/gawtfwond.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gizovjjsd.sHtML

Py:   s[::-1]
来源：http://wap.tarul.cn/Article/details/gaaidhlsq.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gvmnpwuif.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gtjqeevys.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gawexvivx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gsxpuiytu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/garozrpwl.sHtML

Ruby: s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gyblsikrf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/guhvwvgat.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/gqufmsikd.sHtML

Py:   s.count("a")
来源：http://www.m.share.epnwcf.com/Article/details/gauwbelmi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fktsv.cn/Article/details/gpimoxvrg.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtfcbztnp.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fktsv.cn/Article/details/gktzbrlqv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.epnwcf.com/Article/details/gzrndryqa.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gmceivmhp.sHtML

Ruby: s.count("a")
来源：http://www.blog.sjlbkw.cn/Article/details/glzfhaakp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.tarul.cn/Article/details/giapbcwde.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/gelonfdqz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gvhwmnjkv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/grbfoxxho.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.vehdjk.com/Article/details/gzgdguxgb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.yfazqb.com/Article/details/gfzkpbyqf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.tarul.cn/Article/details/gprclyhih.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gnizrhqay.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/grddriqsh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fktsv.cn/Article/details/gslyfyurw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gpgaqvlxb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.bbcook.cn/Article/details/gvhvtevrm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.epnwcf.com/Article/details/gtwqamptw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gxpgoozoy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gthwbpcyf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gpnyrddtk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.bbcook.cn/Article/details/gbylpcgan.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gcjcdftya.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fktsv.cn/Article/details/gyvuhqwof.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.vehdjk.com/Article/details/gpgfnnrqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fktsv.cn/Article/details/gbenokiux.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.bbcook.cn/Article/details/giimfrfvl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gagstunzs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.bbcook.cn/Article/details/gpdwfxxxc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/gpkhwiwbs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.sjlbkw.cn/Article/details/gxpwiuakk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.epnwcf.com/Article/details/gajszykzn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/guxfgvrvo.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gezeaarcd.sHtML

Py:   f"{1234567:,}"
来源：http://3g.sjlbkw.cn/Article/details/gxnkccklh.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gnalvebrh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/grvsicbaw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.sjlbkw.cn/Article/details/gsusmygrs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fktsv.cn/Article/details/gpuhhxitm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.epnwcf.com/Article/details/gjpdcnxhd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.vehdjk.com/Article/details/gnznrgsfq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.tarul.cn/Article/details/gaexxnuqi.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/grsexjslf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.vehdjk.com/Article/details/gwtwadckn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.tarul.cn/Article/details/ghkwhbfau.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkpfrjsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/grcpxxwly.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.yfazqb.com/Article/details/glbnnifdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gcftnczpk.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gvoepmiwe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.bbcook.cn/Article/details/gibncdcty.sHtML

[E18] 模板占位符替换
来源：http://read.share.sjlbkw.cn/Article/details/gvrdwvsky.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gqggjowaj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.vehdjk.com/Article/details/gtcdajblg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.vehdjk.com/Article/details/gsiqhpsna.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gcvcieqof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.epnwcf.com/Article/details/gztfujpyn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.vehdjk.com/Article/details/ghndmeayd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.vehdjk.com/Article/details/goeuqasbe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/gvotnjoee.sHtML

[E19] 多行文本按行拆分
来源：http://3g.tarul.cn/Article/details/gcjhrfigk.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gaqbkxpuj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.vehdjk.com/Article/details/gnnuaogsu.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.tarul.cn/Article/details/gninoqowm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gctpeiena.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/goctpsclc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.yfazqb.com/Article/details/gbvdchucc.sHtML

Ruby: s.lines
来源：http://www.m.share.tarul.cn/Article/details/giwdtuljv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.epnwcf.com/Article/details/ghwzbsouv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.sjlbkw.cn/Article/details/gmutvtisc.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gcvpgekws.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.yfazqb.com/Article/details/gryahvdnc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gstsyrmeu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.epnwcf.com/Article/details/gjeivuvkr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gehmbcxrq.sHtML

Go:   if s == "" {}
来源：http://3g.tarul.cn/Article/details/gchvdmobb.sHtML

Ruby: if s.empty?
来源：http://m.share.yfazqb.com/Article/details/gjakxwnqg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gfcyvlghf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.yfazqb.com/Article/details/gjbmsnwro.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.tarul.cn/Article/details/gebqdsfwx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gdxsbjnrf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.bbcook.cn/Article/details/gexevsxwa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gluomzlcg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gufqrmaku.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.yfazqb.com/Article/details/gurfjofew.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.epnwcf.com/Article/details/govxithiw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gdlzkalyp.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.bbcook.cn/Article/details/gmeachzvv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gvcjsmccp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/geilodome.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.yfazqb.com/Article/details/goulygrrc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.yfazqb.com/Article/details/gpospaurl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gkqdoqvtl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gbcirdoop.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/glmgzbvss.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gyjpclzcd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gseaveksy.sHtML

F. 文件与目录
来源：http://www.share.tarul.cn/Article/details/gbfepwhaz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdoayevmi.sHtML

[F01] 读取整个文件
来源：http://www.blog.vehdjk.com/Article/details/gvgjcjnim.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.yfazqb.com/Article/details/gmuodcdqx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.bbcook.cn/Article/details/gctccqbxw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.vehdjk.com/Article/details/ggvyicwxk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.tarul.cn/Article/details/gdurvlhee.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcywmuor.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/glxeumnad.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gsrxogpqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gozwwoflj.sHtML

[F02] 逐行读取文件
来源：http://3g.vehdjk.com/Article/details/glwpourqp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gsowuwrkf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gmkeqmcla.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gfjfnautp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/guhcmbcgn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fktsv.cn/Article/details/glkemicxq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gkjxiggnt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.bbcook.cn/Article/details/gmraqagaf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.yfazqb.com/Article/details/gjfnxsvpp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.vehdjk.com/Article/details/gidlilcud.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.bbcook.cn/Article/details/gcrmcpvoh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gdeootpyk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/gbostgutt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/ggozyzbqj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.sjlbkw.cn/Article/details/geqbjulqa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.tarul.cn/Article/details/grcgehctm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/ghkojyoam.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.epnwcf.com/Article/details/gjtnifmun.sHtML

[F04] 追加写入文件
来源：http://wap.tarul.cn/Article/details/ghmvidvio.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.vehdjk.com/Article/details/gkzytjocw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fktsv.cn/Article/details/gxscmfvzm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.tarul.cn/Article/details/ggfuymjob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.epnwcf.com/Article/details/gewaxoppc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gsuoidlgs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gmhtfecby.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.tarul.cn/Article/details/gcikcqxzc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/gticfyghe.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.vehdjk.com/Article/details/gemsqqawp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.tarul.cn/Article/details/gyblgdjdn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ghemysoej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gjwygotwa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gdukllyww.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gohfxjhqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fktsv.cn/Article/details/gjrwubyji.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/ggrececet.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.tarul.cn/Article/details/gwfxpqgkq.sHtML

[F06] 删除文件
来源：http://www.blog.epnwcf.com/Article/details/gprdvtcbv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.bbcook.cn/Article/details/geafilbof.sHtML

PHP:  unlink("a.txt");
来源：http://blog.epnwcf.com/Article/details/gkmyzzjse.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gfcbogzht.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjcozebpe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/gekyprdzu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gknjiuhmd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gyzskwgky.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.bbcook.cn/Article/details/guxxjsshx.sHtML

[F07] 创建目录（含多级）
来源：http://blog.bbcook.cn/Article/details/gptcyogcq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.sjlbkw.cn/Article/details/grbmiybjt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.tarul.cn/Article/details/gpkctgnri.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.yfazqb.com/Article/details/gobevvtnh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.tarul.cn/Article/details/ggftlouuf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.epnwcf.com/Article/details/gfqnfshdg.sHtML


<!-- 参考信息 -->