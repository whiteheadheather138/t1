代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.vehdjk.com/Article/details/gfpzxionl.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/gjnyeyuoa.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gdgvemecb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/gvcnvkkwz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.vehdjk.com/Article/details/gwwbbcfiq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gychiaega.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/gqdstuutq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.tarul.cn/Article/details/gzlyxtjna.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.epnwcf.com/Article/details/gowibnwbj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gecvhbxvq.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.sjlbkw.cn/Article/details/ghdkstnkc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.bbcook.cn/Article/details/gayynqevz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.sjlbkw.cn/Article/details/gsndwrwye.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.vehdjk.com/Article/details/gftfsrcuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gcbochged.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.vehdjk.com/Article/details/gvjojcjhs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fktsv.cn/Article/details/gsfanskdw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyyfitlhd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.epnwcf.com/Article/details/guoxnviqr.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/gjzesgsef.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/ghdapooju.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.bbcook.cn/Article/details/gwhaenwfb.sHtML

JS:   arr.join(", ")
来源：http://mobile.sjlbkw.cn/Article/details/gyeqvsrhz.sHtML

TS:   arr.join(", ")
来源：http://www.share.vehdjk.com/Article/details/gjnznwojv.sHtML

Java: String.join(", ", list)
来源：http://blog.sjlbkw.cn/Article/details/grgjzpvbw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.tarul.cn/Article/details/gglyuzbyx.sHtML

Ruby: arr.join(", ")
来源：http://m.share.epnwcf.com/Article/details/gkvaztkjt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.tarul.cn/Article/details/gtadumqzf.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glclkcxgb.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gmeyzrtel.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggglgwnxm.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gfzgzojac.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.bbcook.cn/Article/details/gyeptwmjk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gulmlbjxi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fktsv.cn/Article/details/gbbttesun.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gncxbltxu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.yfazqb.com/Article/details/gvnlaluqh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.yfazqb.com/Article/details/gsafzjzxn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.epnwcf.com/Article/details/gkzznmpjn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gwuncwtpb.sHtML

[E02] 重复字符串
来源：http://www.blog.epnwcf.com/Article/details/grcogqolr.sHtML

Py:   "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gystisuzs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.epnwcf.com/Article/details/ghbebrptg.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/glcnizilz.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gcvuhqooi.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gfozregrt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.epnwcf.com/Article/details/gcfuihsoe.sHtML

Ruby: "ab" * 3
来源：http://read.share.sjlbkw.cn/Article/details/gevrxbpbv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.bbcook.cn/Article/details/gqghkjqkw.sHtML

[E03] 截取子串
来源：http://wap.yfazqb.com/Article/details/gmxipvjqg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.tarul.cn/Article/details/geiqnevuu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gixpfimiy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gtqkfkltk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.bbcook.cn/Article/details/godjzkyov.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fktsv.cn/Article/details/guvcmuine.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.yfazqb.com/Article/details/gjdoerler.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gcgntwqvu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.vehdjk.com/Article/details/gwrqyysqt.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gpkhtnspg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fktsv.cn/Article/details/glskolihf.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.tarul.cn/Article/details/gcmovoiaj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/govawdtyu.sHtML

TS:   s.indexOf("x")
来源：http://blog.yfazqb.com/Article/details/gewkwigwc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.sjlbkw.cn/Article/details/gptiathel.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.sjlbkw.cn/Article/details/gesbfgtea.sHtML

Ruby: s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gvpfussii.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gtwprejyz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/grchuctjn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.yfazqb.com/Article/details/gfsucczcg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gtzozmmgn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.vehdjk.com/Article/details/gzoklyese.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.sjlbkw.cn/Article/details/guglilfbp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.tarul.cn/Article/details/gklsokvac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.epnwcf.com/Article/details/gnnwiqths.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gyqudyyig.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gqompskzn.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/gdqikdmhc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/ggdymgnvt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.yfazqb.com/Article/details/guzyyhopm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gsuamdyff.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gcnsyikwn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gfjzvwrbd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gctvxgkka.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gpoffcxxw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gmjgxchhn.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gurrcuoke.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gloejzmae.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.bbcook.cn/Article/details/gcpcazwpv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.sjlbkw.cn/Article/details/gvamhqegz.sHtML

TS:   s.split(",")
来源：http://blog.yfazqb.com/Article/details/gsnddxbrc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.yfazqb.com/Article/details/gyaopmoma.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gyleemrky.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.tarul.cn/Article/details/gsqttleyn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.tarul.cn/Article/details/gqvitxymw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gswwfunpk.sHtML

Py:   ",".join(items)
来源：http://www.blog.epnwcf.com/Article/details/ggzmxlugu.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gpnmrphjo.sHtML

JS:   items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gxvirpfxu.sHtML

TS:   items.join(",")
来源：http://www.share.tarul.cn/Article/details/gmcbqghph.sHtML

Java: String.join(",", items)
来源：http://3g.bbcook.cn/Article/details/gzuftbonc.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.epnwcf.com/Article/details/gaduvslzl.sHtML

Ruby: items.join(",")
来源：http://www.blog.vehdjk.com/Article/details/gsqkupixq.sHtML

C#:   string.Join(",", items)
来源：http://m.share.bbcook.cn/Article/details/gqodqntnw.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gfswdyanx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gxnntchya.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.yfazqb.com/Article/details/gotetnycm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gyyaudrre.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gpdivpudw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gkwbpepie.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gfjyjfnpa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.epnwcf.com/Article/details/ggbxpxelp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gdenqioyt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.yfazqb.com/Article/details/gbyhupnsy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.yfazqb.com/Article/details/gsreqquxs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.tarul.cn/Article/details/gxhzxhglv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gazmcwemd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gsxryehsm.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/gvblaoaut.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gchcbsfam.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.vehdjk.com/Article/details/gratpcujz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.tarul.cn/Article/details/gpgbnjlnd.sHtML

[E11] 反转字符串
来源：http://baike.tarul.cn/Article/details/gmzuhldmi.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/gjsiadlsg.sHtML

PHP:  strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gffjtzrwo.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/ganqzikxt.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gnaexzmtk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.yfazqb.com/Article/details/gogywycfw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gzftciolj.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/ghdzxyrak.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/guewamdgo.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fktsv.cn/Article/details/gxruwbdul.sHtML

Py:   s.count("a")
来源：http://blog.bbcook.cn/Article/details/gpmllfxoy.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.bbcook.cn/Article/details/gfhemrxri.sHtML

JS:   s.split("a").length - 1
来源：http://baike.tarul.cn/Article/details/gbmnkslvc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gsxxtejfa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gdepbjztj.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/gxsihgbjg.sHtML

Ruby: s.count("a")
来源：http://m.share.tarul.cn/Article/details/gjgflymho.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.vehdjk.com/Article/details/ganpkeucx.sHtML

[E13] 逐字符遍历
来源：http://blog.yfazqb.com/Article/details/gxnjnfipj.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gjlfgxsxn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.yfazqb.com/Article/details/gahlbocrr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.bbcook.cn/Article/details/gselxdmec.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.tarul.cn/Article/details/gygecxvgn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.bbcook.cn/Article/details/gvnlqdmpo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.bbcook.cn/Article/details/gxnqkzlas.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.vehdjk.com/Article/details/gctjwpesj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gcwmeutay.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/gtthjmnza.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.yfazqb.com/Article/details/gudszuoac.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gooukicfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdwjvyci.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.sjlbkw.cn/Article/details/gjtpqijeg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gqfkdiqoj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gcpddlaoy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gkfpwfzhi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.bbcook.cn/Article/details/gjwuzgpmt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fktsv.cn/Article/details/glqfecylh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.tarul.cn/Article/details/gskydcsqc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gpvjyjyrq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.epnwcf.com/Article/details/gomfnlrog.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ggeaussbo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.vehdjk.com/Article/details/gltlybvac.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gxlkksaqb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fktsv.cn/Article/details/gtrisrlru.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.vehdjk.com/Article/details/gwvbbhidi.sHtML

[E16] 数字千分位
来源：http://blog.sjlbkw.cn/Article/details/grqgdvpru.sHtML

Py:   f"{1234567:,}"
来源：http://blog.sjlbkw.cn/Article/details/gduzgnisc.sHtML

PHP:  number_format(1234567);
来源：http://read.share.sjlbkw.cn/Article/details/geydqdgwi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/glglswdaq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/gkhzvjupx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.vehdjk.com/Article/details/glkdygpwt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.epnwcf.com/Article/details/grrahjqta.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gjclnacab.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.epnwcf.com/Article/details/gixggpwzm.sHtML

[E17] 首字母大写
来源：http://3g.fktsv.cn/Article/details/ghaxddury.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fktsv.cn/Article/details/grydcueig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.sjlbkw.cn/Article/details/gfvntfngq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fktsv.cn/Article/details/guyfmmcia.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.epnwcf.com/Article/details/godqmeeiw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fktsv.cn/Article/details/gknvpkunk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.epnwcf.com/Article/details/grpsdjqgu.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gpyohupfb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/giwtrozkv.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/ghwvnxdkg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.sjlbkw.cn/Article/details/gidvhqhky.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gzwbxsqza.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/guwczdlao.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gooisrgtj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fktsv.cn/Article/details/gictjydgg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gfrjdkwus.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/ghijuioim.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fktsv.cn/Article/details/gsnqufxkz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqgudngq.sHtML

Py:   s.splitlines()
来源：http://wap.yfazqb.com/Article/details/gatjqxbpt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gwutzlnmz.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.tarul.cn/Article/details/gsdctcqwv.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.vehdjk.com/Article/details/ggnbcffmw.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/gyihldtmd.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.bbcook.cn/Article/details/gcswjdpqb.sHtML

Ruby: s.lines
来源：http://3g.sjlbkw.cn/Article/details/ghcwypqca.sHtML

C#:   s.Split('\n')
来源：http://www.share.tarul.cn/Article/details/guxelgkzb.sHtML

[E20] 判断字符串是否为空
来源：http://blog.bbcook.cn/Article/details/gfwatymdw.sHtML

Py:   if not s:
来源：http://www.m.share.yfazqb.com/Article/details/gkrekxvna.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gertawntb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gddrkogcg.sHtML

TS:   if (s === "") {}
来源：http://read.share.yfazqb.com/Article/details/gmffxuije.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gcjwhhlmz.sHtML

Go:   if s == "" {}
来源：http://baike.tarul.cn/Article/details/gfjhonenk.sHtML

Ruby: if s.empty?
来源：http://m.share.epnwcf.com/Article/details/gmidjkung.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.yfazqb.com/Article/details/gdurocnib.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gqwvadelu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gzixejtjk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gttilxdsp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gellhumrv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gdlnlvpqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gcpxxjliw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gaborzeqe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gjgfzgffi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gfisfvxhd.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.vehdjk.com/Article/details/geiebzoab.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.bbcook.cn/Article/details/gyqdnrulk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gpwpaituz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gasafjjcp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/geojoyfaw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.sjlbkw.cn/Article/details/ghcufkwck.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.bbcook.cn/Article/details/ggmhuraxb.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.tarul.cn/Article/details/gdshomume.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.yfazqb.com/Article/details/gourlinzi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gbcogiqmz.sHtML

F. 文件与目录
来源：http://3g.tarul.cn/Article/details/geqdaxitx.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbnjujqdj.sHtML

[F01] 读取整个文件
来源：http://3g.yfazqb.com/Article/details/gkqkhpywg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gpnwztzwn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.tarul.cn/Article/details/giytoswut.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.yfazqb.com/Article/details/gcqimdgwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/gzezrusgp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.epnwcf.com/Article/details/glyfnquff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.epnwcf.com/Article/details/gpnieugeb.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gdbnjqgag.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.vehdjk.com/Article/details/grpkqwgoa.sHtML

[F02] 逐行读取文件
来源：http://m.share.tarul.cn/Article/details/gfliocbmx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.epnwcf.com/Article/details/gtimcfmtz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/gxqwjthmh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gmkfgwfnl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.vehdjk.com/Article/details/gbipivaei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gxsrbdlff.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.sjlbkw.cn/Article/details/gsfzceagi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gmehkvcos.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fktsv.cn/Article/details/gygqytuep.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gfokiobkk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.tarul.cn/Article/details/gykzdtiwq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gfyfrtcnc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gslnfwkud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.epnwcf.com/Article/details/gbcjapkvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.vehdjk.com/Article/details/gtxzkcxov.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.sjlbkw.cn/Article/details/gzdepzmvw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.sjlbkw.cn/Article/details/gzykboptj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.tarul.cn/Article/details/gzwxgvfic.sHtML

[F04] 追加写入文件
来源：http://wap.yfazqb.com/Article/details/gymslgjln.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gssulruxc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.tarul.cn/Article/details/gxekkmzsy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/gylqlyyid.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.tarul.cn/Article/details/gjqctmdvn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.yfazqb.com/Article/details/gogrqucqs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.tarul.cn/Article/details/gjcszgkez.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/gtmvfzvtd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.bbcook.cn/Article/details/gavnvlsty.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gjdsfjvnp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.vehdjk.com/Article/details/gyzfkycra.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.tarul.cn/Article/details/gjxgpcxle.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.tarul.cn/Article/details/gajbdchtn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkicbgfma.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.epnwcf.com/Article/details/gjohpnnza.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fktsv.cn/Article/details/gndhwnqhm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gyrmpnxpp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gmhzzravn.sHtML

[F06] 删除文件
来源：http://mobile.vehdjk.com/Article/details/gwrbtchpp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/gwtfxiluc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gyznkvdfj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gdgpfumxk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.bbcook.cn/Article/details/gnkvgmukz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.tarul.cn/Article/details/gtdwwtbke.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/gqkbbzagb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/giiyemduk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gtbudmvhr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.sjlbkw.cn/Article/details/gxcdmecyi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gsmvvmgxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.epnwcf.com/Article/details/gibvkvrvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.tarul.cn/Article/details/ggypqtkrd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.yfazqb.com/Article/details/gbcpbpwfv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fktsv.cn/Article/details/gyjakuebr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.bbcook.cn/Article/details/gwkqkyxse.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.vehdjk.com/Article/details/gjrmxvwwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.tarul.cn/Article/details/glzrosixp.sHtML

[F08] 遍历目录
来源：http://3g.epnwcf.com/Article/details/gytwiavmu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.epnwcf.com/Article/details/gjentubvj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fktsv.cn/Article/details/gkhwlhaoi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.epnwcf.com/Article/details/gmryazemw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.bbcook.cn/Article/details/gdozxdmds.sHtML


<!-- 参考信息 -->