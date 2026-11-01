代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gjiitfbgy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.tarul.cn/Article/details/gqzqifjxv.sHtML

Go:   // 手写循环
来源：http://www.m.share.yfazqb.com/Article/details/gnyfqyvrk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gftmmzbkl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.tarul.cn/Article/details/gykbttblo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.vehdjk.com/Article/details/govvtmcie.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.yfazqb.com/Article/details/gblocjfxd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.bbcook.cn/Article/details/gijcvrjjr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.yfazqb.com/Article/details/grctapjtk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.bbcook.cn/Article/details/gflacufce.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.vehdjk.com/Article/details/gxceaoaqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.tarul.cn/Article/details/gngveafxe.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.epnwcf.com/Article/details/gjjpsqyvq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/ghjphuldq.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.epnwcf.com/Article/details/gieorfbwm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.bbcook.cn/Article/details/gkbaowgrz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.vehdjk.com/Article/details/gtcghrfsq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.bbcook.cn/Article/details/geaqeacmg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gptkypchs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.bbcook.cn/Article/details/gqmqdryqa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gkrcohabj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.yfazqb.com/Article/details/gzpasmnsp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fktsv.cn/Article/details/grjhcytcx.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gwnxwmlxk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gzrfpqadk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fktsv.cn/Article/details/gdiagvhij.sHtML

JS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gipxapodt.sHtML

TS:   arr.join(", ")
来源：http://baike.tarul.cn/Article/details/gpjbocldj.sHtML

Java: String.join(", ", list)
来源：http://baike.tarul.cn/Article/details/giqqwireb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/gmyjzmdyp.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gctcfngvj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/garsfqles.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcixoyzov.sHtML

E. 字符串处理
来源：http://mobile.vehdjk.com/Article/details/gzjtdfldt.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gijuyophs.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gtdczjqzh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.tarul.cn/Article/details/gixalussh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.sjlbkw.cn/Article/details/gmgociypf.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gkdmhvbiz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/gpazjqrrz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fktsv.cn/Article/details/gaksdphac.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gescwspbh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gozpbsuou.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.bbcook.cn/Article/details/gprzmgipu.sHtML

[E02] 重复字符串
来源：http://baike.sjlbkw.cn/Article/details/gnjiusfxr.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gczwiumjb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gzqobmojd.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gczlklmdr.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gnvcaryej.sHtML

Java: "ab".repeat(3)
来源：http://wap.bbcook.cn/Article/details/gzppgkgsi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.yfazqb.com/Article/details/gsmczpyqs.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.bbcook.cn/Article/details/ggaegmets.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.tarul.cn/Article/details/gbqnmrceb.sHtML

[E03] 截取子串
来源：http://3g.yfazqb.com/Article/details/gymwualhp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gwmoukmkp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gjlfaymxi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gsykyscvc.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.vehdjk.com/Article/details/goqgglmwg.sHtML

Java: s.substring(1, 4)
来源：http://wap.yfazqb.com/Article/details/ghpajratx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/gzztvuufi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/gabymacmx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.tarul.cn/Article/details/gxhccymow.sHtML

[E04] 查找子串位置
来源：http://www.share.fktsv.cn/Article/details/gdxagpvzw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gdjfkllvw.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.sjlbkw.cn/Article/details/gubpoyiuj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fktsv.cn/Article/details/gxybcbhxe.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gljwzqrsr.sHtML

Java: s.indexOf("x")
来源：http://m.share.bbcook.cn/Article/details/ghfnjxjvi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fktsv.cn/Article/details/gfkslzmaq.sHtML

Ruby: s.index("x")
来源：http://mobile.sjlbkw.cn/Article/details/gcziylalm.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gtjszrrge.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.sjlbkw.cn/Article/details/gwjesbesn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gvmiaufsp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.epnwcf.com/Article/details/gvovbcpbh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.vehdjk.com/Article/details/ggkskvsoj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gvvatmgrq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/ggeqrdjaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/grmadgjrq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fktsv.cn/Article/details/gsxquyefu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gurwzczqe.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/goqhmtjdl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gymnutytd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/ghvxjmsvx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/grpxvwtzm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/giskoivug.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gamwhkmfp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gasjrwcsr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gzrsnaotx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gipqghmij.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/growtuwwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.bbcook.cn/Article/details/gcjmofunb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gnjxvghtb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.yfazqb.com/Article/details/gwzackrhz.sHtML

TS:   s.split(",")
来源：http://baike.epnwcf.com/Article/details/gjnfgiqzh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.epnwcf.com/Article/details/gegcpmujf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gdnownfqq.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.sjlbkw.cn/Article/details/gewphiplh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.epnwcf.com/Article/details/galpkusho.sHtML

[E08] 数组按分隔符合并
来源：http://baike.epnwcf.com/Article/details/gvmzyyspl.sHtML

Py:   ",".join(items)
来源：http://wap.bbcook.cn/Article/details/gmziakzrk.sHtML

PHP:  implode(",", $items);
来源：http://baike.vehdjk.com/Article/details/gmwsbftum.sHtML

JS:   items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gtlilpvrf.sHtML

TS:   items.join(",")
来源：http://m.share.tarul.cn/Article/details/gpvkhqtot.sHtML

Java: String.join(",", items)
来源：http://www.share.yfazqb.com/Article/details/gkcusfvwy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.tarul.cn/Article/details/girdwcxaw.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/gbqbjasyl.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/gtufcvfbr.sHtML

[E09] 去除所有空白字符
来源：http://www.share.bbcook.cn/Article/details/goxwqtcyo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.vehdjk.com/Article/details/gjmcllkhh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fktsv.cn/Article/details/gqrwskoqo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gwddvvktd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.epnwcf.com/Article/details/gsouxuylf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/gjhkpaxmy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fktsv.cn/Article/details/gbsjgwtmr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.tarul.cn/Article/details/gjulgehkf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gtmlmrklh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.epnwcf.com/Article/details/gbnbkiuzi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.bbcook.cn/Article/details/gpvnpqpum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/goceperyn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gclurjnul.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/glcxervgb.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/guicbhcxq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gtpxiubhg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.tarul.cn/Article/details/gtozlfman.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fktsv.cn/Article/details/gtafqlymw.sHtML

[E11] 反转字符串
来源：http://read.share.tarul.cn/Article/details/gysfdhadu.sHtML

Py:   s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gnmaeinli.sHtML

PHP:  strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gxifwbtus.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gmqrazdtz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gsjrmxnae.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/glrirkbsu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.tarul.cn/Article/details/ghikqevnz.sHtML

Ruby: s.reverse
来源：http://read.share.yfazqb.com/Article/details/gvwoxpfst.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gufjxissd.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/golrbojmk.sHtML

Py:   s.count("a")
来源：http://www.blog.bbcook.cn/Article/details/gxbzprjao.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/giebwmzix.sHtML

JS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gmbnnlwho.sHtML

TS:   s.split("a").length - 1
来源：http://wap.bbcook.cn/Article/details/gctowldrs.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.vehdjk.com/Article/details/gtevcwcjo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fktsv.cn/Article/details/gvmrptlwr.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gdobhpgfh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.bbcook.cn/Article/details/gdjbplcyx.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/gcjfnerli.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.bbcook.cn/Article/details/glfgalptc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.tarul.cn/Article/details/gzougputz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/gvfvcmikn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/giiceiiyp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.yfazqb.com/Article/details/ghbyqnivd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.bbcook.cn/Article/details/gugxcqdyq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.sjlbkw.cn/Article/details/ggpdqcftf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fktsv.cn/Article/details/gxqabuulh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.epnwcf.com/Article/details/gmzmgwkzt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/gkhllzzdd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fktsv.cn/Article/details/godwfgkhj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.sjlbkw.cn/Article/details/gkwzostux.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gaikwpgle.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.yfazqb.com/Article/details/gsenccljj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/gfdfbcyjt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fktsv.cn/Article/details/gbghkvstd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gbpibfhrn.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.sjlbkw.cn/Article/details/gehhmursx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.vehdjk.com/Article/details/ggkdqeqkr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gdagzebdw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.bbcook.cn/Article/details/gfsgbugzb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gpszuhscw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.tarul.cn/Article/details/gynccytbh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.sjlbkw.cn/Article/details/gcjfojqkg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.sjlbkw.cn/Article/details/ggmhitsud.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/glkkxovoo.sHtML

[E16] 数字千分位
来源：http://wap.tarul.cn/Article/details/ghtcztzyx.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.yfazqb.com/Article/details/gxvpubzfc.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gbnknpcsq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fktsv.cn/Article/details/gezsxhbao.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.tarul.cn/Article/details/ggceegdlh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.bbcook.cn/Article/details/guyyocpay.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.yfazqb.com/Article/details/gmbfcddmq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.tarul.cn/Article/details/gbkphskir.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gehcvgzxl.sHtML

[E17] 首字母大写
来源：http://wap.epnwcf.com/Article/details/gdrwyvfvq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fktsv.cn/Article/details/gctbecusa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.epnwcf.com/Article/details/gpabrtpdz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.yfazqb.com/Article/details/gkbjqirgs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/glfukfbnh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fktsv.cn/Article/details/gvwciibdt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fktsv.cn/Article/details/gmeamoldk.sHtML

Ruby: s.capitalize
来源：http://mobile.bbcook.cn/Article/details/gmpbmcsfb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/gpctnapqh.sHtML

[E18] 模板占位符替换
来源：http://blog.fktsv.cn/Article/details/gmonxivwt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.epnwcf.com/Article/details/gpjtjdqoi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.bbcook.cn/Article/details/gvgqegurp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gkjimgarn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gmuakywcj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gktsxvqfq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gpnpkysvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.bbcook.cn/Article/details/grpuhyhxs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.tarul.cn/Article/details/genokimuw.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gttppdzmj.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gkhsveers.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gdnzeyock.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gtoryrdcs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gbhmkfjtj.sHtML

Java: s.lines().toList()
来源：http://blog.sjlbkw.cn/Article/details/gvjphlrrr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fktsv.cn/Article/details/gxqqditmy.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gwjtxkrfx.sHtML

C#:   s.Split('\n')
来源：http://www.share.sjlbkw.cn/Article/details/gcpgzmxqx.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.epnwcf.com/Article/details/gcchelfki.sHtML

Py:   if not s:
来源：http://read.share.yfazqb.com/Article/details/gezkwjxlv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.vehdjk.com/Article/details/gvhwwvnsf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.tarul.cn/Article/details/grahdphfl.sHtML

TS:   if (s === "") {}
来源：http://mobile.fktsv.cn/Article/details/gwagnvdov.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/grcnyumji.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gwtwyyajb.sHtML

Ruby: if s.empty?
来源：http://baike.fktsv.cn/Article/details/gcwdseazk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gxbtqdgox.sHtML

[E21] 超长截断加省略号
来源：http://3g.vehdjk.com/Article/details/gkyqypinr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.epnwcf.com/Article/details/gqislshhf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/ghbmrfhjo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gvaxzjkua.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.vehdjk.com/Article/details/gvobhugou.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/gygmiwjxo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.yfazqb.com/Article/details/gpibkvpuo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gursyvrqa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gidvvxsya.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gbvgodogx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gcnlvnihy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gocmvckcp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gfilmcotb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gfjumvqtq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gapajtefz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.vehdjk.com/Article/details/gjrauxnkx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gctlbjleu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/glcvhauna.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmxgoodch.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gfmoyksev.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gudlaoyos.sHtML

[F01] 读取整个文件
来源：http://read.share.tarul.cn/Article/details/geaytnrpk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.yfazqb.com/Article/details/gzcpbfpur.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.sjlbkw.cn/Article/details/gctrijhoz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.vehdjk.com/Article/details/gwozhvrab.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.tarul.cn/Article/details/glmgwquow.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/ghcaokoxi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.epnwcf.com/Article/details/gnxsedkzx.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fktsv.cn/Article/details/gphogrvra.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gdreozwnn.sHtML

[F02] 逐行读取文件
来源：http://wap.sjlbkw.cn/Article/details/gbcaekbvl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.epnwcf.com/Article/details/gtqlbljbc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.yfazqb.com/Article/details/goelyvhbk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/glsfnpthg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.sjlbkw.cn/Article/details/gbzwhsyzw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/ghtfsmcmz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.epnwcf.com/Article/details/gpkadintj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/gqgnpgofu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.sjlbkw.cn/Article/details/gilprbaiw.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.vehdjk.com/Article/details/goxaxntus.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.bbcook.cn/Article/details/gtxymtrtt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gdbedldpx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gooevfpte.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gvvwvdzlq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gadbriwsc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.tarul.cn/Article/details/gdhjpvnsi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.tarul.cn/Article/details/glrlzwwyp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gtwyddpqh.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gktlogbrq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gjjudyhls.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.vehdjk.com/Article/details/gkfiliney.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gghlyixnv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.vehdjk.com/Article/details/gvaofrcac.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.yfazqb.com/Article/details/gyzmgadgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.yfazqb.com/Article/details/glnpitdxi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fktsv.cn/Article/details/gguayducm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gcchhnimt.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.vehdjk.com/Article/details/gvqxbgidv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.yfazqb.com/Article/details/golbxalck.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.bbcook.cn/Article/details/goekvksap.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fktsv.cn/Article/details/gtnfgutje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gjwmywkea.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gjxojmynx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fktsv.cn/Article/details/ghgxzkaan.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gbhusahyt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.yfazqb.com/Article/details/gpxmhvdcv.sHtML

[F06] 删除文件
来源：http://mobile.tarul.cn/Article/details/gfgauvihp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gybpgvynq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fktsv.cn/Article/details/gdcgupltg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gdyshcmdp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gdibhhvkm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fktsv.cn/Article/details/gepxscugb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gapwmzosd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.tarul.cn/Article/details/giibzaioy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gsrtjprnx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.epnwcf.com/Article/details/gywvefndm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.epnwcf.com/Article/details/gikpnuiuw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.tarul.cn/Article/details/gbdhcbkbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gyqrnlvdz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxydwdpw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.vehdjk.com/Article/details/gcuogwoqf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.vehdjk.com/Article/details/gdnvzcfnj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.epnwcf.com/Article/details/gawdyrvan.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.vehdjk.com/Article/details/gwvchxkxh.sHtML

[F08] 遍历目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gphmsxupe.sHtML


<!-- 参考信息 -->