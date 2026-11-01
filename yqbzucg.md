代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.yfazqb.com/Article/details/gpawxyujm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.sjlbkw.cn/Article/details/gaozgidfl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.sjlbkw.cn/Article/details/gojiaazdp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fktsv.cn/Article/details/glzmyceld.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.yfazqb.com/Article/details/gphijplur.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gyxtkwgju.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gcrvawrfp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.epnwcf.com/Article/details/gyeazmmdc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.yfazqb.com/Article/details/ghwalduxc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gfrpryjjw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.yfazqb.com/Article/details/gbjmkfdni.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.vehdjk.com/Article/details/gyvcwzaum.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.tarul.cn/Article/details/gsgkixwig.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gvxeykgis.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.sjlbkw.cn/Article/details/gbzjrenhb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.sjlbkw.cn/Article/details/giajnmgmd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/gfuzapczz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.yfazqb.com/Article/details/gcuqgygpt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gruyhxzyg.sHtML

[D26] 数组转字符串
来源：http://www.blog.fktsv.cn/Article/details/gqmitvjlp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gsnvkyulh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.sjlbkw.cn/Article/details/grgbqgfvq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.vehdjk.com/Article/details/gzasqexjy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gwdbuzfkg.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gxsbbkumj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.sjlbkw.cn/Article/details/gyfudhtll.sHtML

Ruby: arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/gsirzqihj.sHtML

C#:   string.Join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gpadlzptg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ggttagwam.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gktwgsele.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/geinkdljx.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gygtevtgs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.bbcook.cn/Article/details/gwvhoqbpj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.yfazqb.com/Article/details/gyswgtlqc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/golzwgife.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.yfazqb.com/Article/details/gyxttrsip.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/gsgegsvkh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gnzayojba.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.vehdjk.com/Article/details/gvbbmidun.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/grvnhehij.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/grulhoohe.sHtML

Py:   "ab" * 3
来源：http://wap.fktsv.cn/Article/details/gbvqfwtal.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/gxtachegn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gdiwonaca.sHtML

TS:   "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gedzdlnvu.sHtML

Java: "ab".repeat(3)
来源：http://wap.epnwcf.com/Article/details/geizhance.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.bbcook.cn/Article/details/grpedkung.sHtML

Ruby: "ab" * 3
来源：http://wap.epnwcf.com/Article/details/glvwzeufr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.yfazqb.com/Article/details/ghmctyqls.sHtML

[E03] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gopzmensm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gojbvyrgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gdayylxqj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.vehdjk.com/Article/details/gceppqdfl.sHtML

TS:   s.slice(1, 4)
来源：http://3g.yfazqb.com/Article/details/goqavyhdu.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gsjuipxop.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.epnwcf.com/Article/details/gloxwzire.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.tarul.cn/Article/details/gtsnbebnw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fktsv.cn/Article/details/gbzkstttv.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gdoiptcpz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.sjlbkw.cn/Article/details/gwtezzcks.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/geeuaibwb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.yfazqb.com/Article/details/gooklagej.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gvuaeupnu.sHtML

Java: s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/gjdhtmaep.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/goawjhzdj.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/ggezzewjn.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/gudnofcik.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.epnwcf.com/Article/details/gkejhpfvl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gzbcxcitg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.tarul.cn/Article/details/gfdszfxci.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.tarul.cn/Article/details/gnkruawcd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.yfazqb.com/Article/details/gdyirrngy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gfdcszagq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.epnwcf.com/Article/details/gvhbtposc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fktsv.cn/Article/details/guxtrrrrt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.vehdjk.com/Article/details/gmenpssvq.sHtML

[E06] 替换子串
来源：http://www.share.bbcook.cn/Article/details/gfhbqvzlu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gqvxnfjef.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/gvtxmybwx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gkbzuavyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gejfyexdd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gwohucgxr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gxbhamoee.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.yfazqb.com/Article/details/gootzlieg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gezuemgps.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.epnwcf.com/Article/details/gqhwupvpw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gbvfoyqdg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gglxqkgqb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.sjlbkw.cn/Article/details/gyoyzowwx.sHtML

TS:   s.split(",")
来源：http://3g.tarul.cn/Article/details/ghvofrjfm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.vehdjk.com/Article/details/gufvfptqc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fktsv.cn/Article/details/gzslszeip.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.sjlbkw.cn/Article/details/ggjdcchti.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.tarul.cn/Article/details/gzkalninq.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gfhknhrsk.sHtML

Py:   ",".join(items)
来源：http://www.share.bbcook.cn/Article/details/gvzwuoapa.sHtML

PHP:  implode(",", $items);
来源：http://mobile.epnwcf.com/Article/details/gtmbxunjf.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/giisqmwew.sHtML

TS:   items.join(",")
来源：http://read.share.fktsv.cn/Article/details/gtnmdslga.sHtML

Java: String.join(",", items)
来源：http://blog.bbcook.cn/Article/details/gagbetwhw.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gxrcortvj.sHtML

Ruby: items.join(",")
来源：http://3g.sjlbkw.cn/Article/details/gjqfsihqr.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gtrpeojgk.sHtML

[E09] 去除所有空白字符
来源：http://wap.bbcook.cn/Article/details/gunheisxc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.tarul.cn/Article/details/gphowexqq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gsnxfesun.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.sjlbkw.cn/Article/details/goamryozj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fktsv.cn/Article/details/gutdechtx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.epnwcf.com/Article/details/guouxpyfl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/gfzhvgdax.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.tarul.cn/Article/details/glgmuhlfu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fktsv.cn/Article/details/gweoaghbz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.vehdjk.com/Article/details/grtrwusdo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.epnwcf.com/Article/details/grvxazlxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gmeuhybgv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gzwmvsexj.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/guhclcduf.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fktsv.cn/Article/details/gxhzbzyiz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gkpyhsjbf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/grdwbqims.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.tarul.cn/Article/details/glnmblwox.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwduzljum.sHtML

Py:   s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyebnaaf.sHtML

PHP:  strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/ghozupoiw.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gwvngnggv.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gxpcloamw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/gnylbdihg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gcsvfmqod.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/ggpggbbde.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gecuboucw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/ggkrugaem.sHtML

Py:   s.count("a")
来源：http://3g.vehdjk.com/Article/details/gqxrsvurk.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.vehdjk.com/Article/details/gxtjazznn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gpiieusds.sHtML

TS:   s.split("a").length - 1
来源：http://3g.sjlbkw.cn/Article/details/gkuatcifl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fktsv.cn/Article/details/gyioflbcp.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.bbcook.cn/Article/details/gjeatbqes.sHtML

Ruby: s.count("a")
来源：http://read.share.bbcook.cn/Article/details/gpwbvchoc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.vehdjk.com/Article/details/gqawkejmh.sHtML

[E13] 逐字符遍历
来源：http://www.share.epnwcf.com/Article/details/gtjmkdluk.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gklgbdrbt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.tarul.cn/Article/details/gdqdnfutg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.epnwcf.com/Article/details/gweyhjpdi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/glrpskwvp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gelrfifng.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.epnwcf.com/Article/details/gnncfuimh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/glhrstxnl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gsypdidnf.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fktsv.cn/Article/details/gjbavlmqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.yfazqb.com/Article/details/gvwryqlqy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.vehdjk.com/Article/details/gkzazjypw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbpkbusba.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvibrkgli.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/gxlnnxluc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fktsv.cn/Article/details/gsbambhcv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.sjlbkw.cn/Article/details/gxclzrxom.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.bbcook.cn/Article/details/gvkdaofqd.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gletkqail.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.yfazqb.com/Article/details/gyouovjna.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.sjlbkw.cn/Article/details/gnwbzndaq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/grbfzdqrw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.bbcook.cn/Article/details/gwfqjmzff.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gmifbjsrb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gpzoydxow.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.bbcook.cn/Article/details/gtlzqahlk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.epnwcf.com/Article/details/gpvjqhecz.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfymhtqb.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gkmvqzwht.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fktsv.cn/Article/details/gxakaolnr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.bbcook.cn/Article/details/ghwlhphri.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/gujlodsgn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fktsv.cn/Article/details/gajuoputy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.bbcook.cn/Article/details/gpsybseyx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gahcfugxy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.yfazqb.com/Article/details/gkgpkgfka.sHtML

[E17] 首字母大写
来源：http://m.share.sjlbkw.cn/Article/details/gzptyaony.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gdvwcelcd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.tarul.cn/Article/details/gnqydkybb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.sjlbkw.cn/Article/details/gyarayrpw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gsdsifaaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.vehdjk.com/Article/details/gkcxrcroe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fktsv.cn/Article/details/gnuvuecvx.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gnoyssxro.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gukmzplfh.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gfnaerieu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.epnwcf.com/Article/details/grxjubjnz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.epnwcf.com/Article/details/ghuslewpb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gflyxdloy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gedfuynbr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gpynidtic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/giriiyicl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/glcxkrcyn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/gwybwnskf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.vehdjk.com/Article/details/ghfhzglkb.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/gxdeiupah.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.vehdjk.com/Article/details/ghjuhavqi.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.yfazqb.com/Article/details/gvrpiqeho.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gihucjlds.sHtML

Java: s.lines().toList()
来源：http://mobile.epnwcf.com/Article/details/gxkhunnvf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fktsv.cn/Article/details/gpemudcdu.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gkjfrhwny.sHtML

C#:   s.Split('\n')
来源：http://3g.bbcook.cn/Article/details/glniocedb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.bbcook.cn/Article/details/gycoejdhi.sHtML

Py:   if not s:
来源：http://www.m.share.fktsv.cn/Article/details/gdjiyvrjp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gcwyzghtn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gxzpexyat.sHtML

TS:   if (s === "") {}
来源：http://blog.yfazqb.com/Article/details/gukjhundv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gbzpiitzt.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/grzyoyedr.sHtML

Ruby: if s.empty?
来源：http://3g.bbcook.cn/Article/details/gocujqbbm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fktsv.cn/Article/details/gvwpfjoqg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.yfazqb.com/Article/details/gekptubja.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gvepqnylk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gencwkkfj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gmhoopkst.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gijphxuvb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gnhnjrmsb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gksupvhwq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gtkxuwdrh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gjkkjgpzt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.sjlbkw.cn/Article/details/gwerjykto.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gadpwslnd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gackftfzk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.yfazqb.com/Article/details/gqetcnhgl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gkkqmgeed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gnwdptpwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.vehdjk.com/Article/details/gbilmoych.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/grzoeggho.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/grcgbhsva.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gasjhtlah.sHtML

F. 文件与目录
来源：http://3g.yfazqb.com/Article/details/gjyvqmzyv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbzxafnxp.sHtML

[F01] 读取整个文件
来源：http://mobile.bbcook.cn/Article/details/gewumldnf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.yfazqb.com/Article/details/gjjcxpbhb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fktsv.cn/Article/details/guadezgwl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.sjlbkw.cn/Article/details/gsdebulzf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gdzfmshvd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/gkzfeegld.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.sjlbkw.cn/Article/details/giycghlkr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gkouotoks.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.yfazqb.com/Article/details/gxtsngryq.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gedxnxosx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gyfloqyju.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fktsv.cn/Article/details/grfnplthb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gcjcldfqc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fktsv.cn/Article/details/goipxkchj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.epnwcf.com/Article/details/gvwwwsxrp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.yfazqb.com/Article/details/gvvqelyqw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.yfazqb.com/Article/details/gnipmnhuc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.bbcook.cn/Article/details/gjxnagqog.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gyhalzloj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fktsv.cn/Article/details/gcgtmkrmz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/grnavuwlm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.sjlbkw.cn/Article/details/gzfwryfwt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fktsv.cn/Article/details/ggxasyuni.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fktsv.cn/Article/details/gjezzkdwt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fktsv.cn/Article/details/gukmkqhkf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.epnwcf.com/Article/details/gnskpwrlm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.tarul.cn/Article/details/glywxshsj.sHtML

[F04] 追加写入文件
来源：http://www.share.sjlbkw.cn/Article/details/gsgmmmsqx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.epnwcf.com/Article/details/groqoabmx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkbqeebe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.tarul.cn/Article/details/gxnbmgpgr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.epnwcf.com/Article/details/ghewjgoix.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.vehdjk.com/Article/details/gaqsvrpdi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fktsv.cn/Article/details/ghuwhgmbe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.epnwcf.com/Article/details/gjkaguirt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/gdgatcfsk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.vehdjk.com/Article/details/gbboszgvt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.sjlbkw.cn/Article/details/gbcgigwmk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.epnwcf.com/Article/details/gfapfykju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gaekhlpzw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gigbvnjvm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/gkgflkfdy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.epnwcf.com/Article/details/gsyqcfuij.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.yfazqb.com/Article/details/gwxqhtfen.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmbyqpppg.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/gwvlohxwx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.epnwcf.com/Article/details/gptrwtufw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fktsv.cn/Article/details/gfwzuluqc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gglxpvwkc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gehixbhck.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/grmsvdefp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/gzmxmfzvc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.sjlbkw.cn/Article/details/gxoaewrxv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.bbcook.cn/Article/details/guisjxyjb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.bbcook.cn/Article/details/gfikauwdx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.bbcook.cn/Article/details/ggoqbdvrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.tarul.cn/Article/details/gdxsferjn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.epnwcf.com/Article/details/gqvgsmwxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.epnwcf.com/Article/details/gzqyghmxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.bbcook.cn/Article/details/gmofzphoz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.epnwcf.com/Article/details/gdwdstjea.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fktsv.cn/Article/details/gdflkfutq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.bbcook.cn/Article/details/gmcxiscmb.sHtML

[F08] 遍历目录
来源：http://m.share.bbcook.cn/Article/details/gftyczmom.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.yfazqb.com/Article/details/gqcqcljjt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.vehdjk.com/Article/details/gtqnrpqcp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.tarul.cn/Article/details/gjqqnxrsy.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.bbcook.cn/Article/details/gldzensmn.sHtML


<!-- 参考信息 -->