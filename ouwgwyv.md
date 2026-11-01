代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.bbcook.cn/Article/details/gbttzwvxe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.yfazqb.com/Article/details/ghrbqxxqo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.vehdjk.com/Article/details/grxhxekzs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/glfojszmq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.tarul.cn/Article/details/geqzhshme.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.epnwcf.com/Article/details/gevstxgic.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.tarul.cn/Article/details/gdsepmeaq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.vehdjk.com/Article/details/gizxhrseu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.vehdjk.com/Article/details/grfzhlvou.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.epnwcf.com/Article/details/gelazkvpl.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fktsv.cn/Article/details/gzktcjqps.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.tarul.cn/Article/details/gzouniphw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.sjlbkw.cn/Article/details/gvuahrlxm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fktsv.cn/Article/details/ggtusbqmb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gdsnatysm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.bbcook.cn/Article/details/guiticibx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.vehdjk.com/Article/details/gshxrovtd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.vehdjk.com/Article/details/gatjispwb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/gixbvdfpl.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/gkwhsnqhh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.yfazqb.com/Article/details/gpjlmftga.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/ggowtvvmq.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/grsxatckz.sHtML

TS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gaxecgyyi.sHtML

Java: String.join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gvvttekjn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.epnwcf.com/Article/details/goqnojhdd.sHtML

Ruby: arr.join(", ")
来源：http://read.share.tarul.cn/Article/details/gvblqnhyl.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gdinhehmo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdvvgqkqx.sHtML

E. 字符串处理
来源：http://www.m.share.bbcook.cn/Article/details/gkmrepqre.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gatnilmoo.sHtML

[E01] 拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gxnzfnpbl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.bbcook.cn/Article/details/godcwaoal.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fktsv.cn/Article/details/gviovaaqx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.yfazqb.com/Article/details/gzllqgauu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gftdcvzay.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fktsv.cn/Article/details/gcnhomzfj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fktsv.cn/Article/details/gvglecnuf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gezywrtko.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gtomtherf.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/gzawxewnc.sHtML

Py:   "ab" * 3
来源：http://baike.yfazqb.com/Article/details/gkizwbfxw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fktsv.cn/Article/details/gbnklhaeg.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gllmzdtyz.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/geoxrzweu.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gonjkhkuv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fktsv.cn/Article/details/gdxerecly.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gbxrencsd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/giejpmcrd.sHtML

[E03] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gjajhwwuh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gmgxbdjln.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/ggxfxakvx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/ghvyxbldg.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gzoohddrs.sHtML

Java: s.substring(1, 4)
来源：http://baike.vehdjk.com/Article/details/gvkmkkfkz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.vehdjk.com/Article/details/gmzfttwpp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.vehdjk.com/Article/details/gavqllorh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.bbcook.cn/Article/details/gejszbhrd.sHtML

[E04] 查找子串位置
来源：http://www.m.share.yfazqb.com/Article/details/gsdqjrocg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.epnwcf.com/Article/details/gqyhymowa.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fktsv.cn/Article/details/gcpbkafpk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gtguokhug.sHtML

TS:   s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/ggpfugngc.sHtML

Java: s.indexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gxliixxyv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.epnwcf.com/Article/details/gkklgnmwv.sHtML

Ruby: s.index("x")
来源：http://www.m.share.bbcook.cn/Article/details/gmszrtnis.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.bbcook.cn/Article/details/ghmdhqhlb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.sjlbkw.cn/Article/details/gdijbhlzt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.bbcook.cn/Article/details/gbgorbynu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fktsv.cn/Article/details/gxrvgterb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.vehdjk.com/Article/details/gqmevplge.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.vehdjk.com/Article/details/gavklbedc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/ghfxxbknd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.bbcook.cn/Article/details/gbqsvlcem.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.vehdjk.com/Article/details/grdvelwpc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gnwyywwao.sHtML

[E06] 替换子串
来源：http://wap.sjlbkw.cn/Article/details/gzxmgdmxb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.sjlbkw.cn/Article/details/gvdoyxdbk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.epnwcf.com/Article/details/gqxikuwaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gidxkitdl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gohanqjdd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gbdlkiyvz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.vehdjk.com/Article/details/gpostreat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gbuzyykqi.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gxrcvmhbl.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gkukvafpk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fktsv.cn/Article/details/gequbznpf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.epnwcf.com/Article/details/gdflbhcoe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gnjlqssrg.sHtML

TS:   s.split(",")
来源：http://www.blog.tarul.cn/Article/details/gcgcbvuyu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.sjlbkw.cn/Article/details/gswnhxrmt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpacuvpfx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.sjlbkw.cn/Article/details/gtzudmuxo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gbrqqkrvv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gjurvmdiz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.bbcook.cn/Article/details/ggoapotew.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gecjnpzuq.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/ghgzlfygc.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/glraslqmw.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gzwekjulm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.yfazqb.com/Article/details/gyiojillj.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gfznuydqb.sHtML

C#:   string.Join(",", items)
来源：http://3g.fktsv.cn/Article/details/giargmdzz.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.yfazqb.com/Article/details/guyrvkgsv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gkklfleje.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.vehdjk.com/Article/details/gtyomeyfv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gwvshtkkx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/gobjkojsg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fktsv.cn/Article/details/gkbvehcer.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.vehdjk.com/Article/details/ghkbftvbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fktsv.cn/Article/details/guncajgei.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gqvafmend.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.sjlbkw.cn/Article/details/gquqccugh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gyltvpoui.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.bbcook.cn/Article/details/gzncnggdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/ghtctpewf.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fktsv.cn/Article/details/gjtusvggj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.epnwcf.com/Article/details/gdvuipsii.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.tarul.cn/Article/details/gvjccljoz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.bbcook.cn/Article/details/ginhhswub.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/grbnfqygx.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gjatfwyjy.sHtML

Py:   s[::-1]
来源：http://blog.fktsv.cn/Article/details/gnxabarzr.sHtML

PHP:  strrev($s);
来源：http://baike.tarul.cn/Article/details/gvfvxhvzu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gvvroeuwr.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gbopuqbho.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.yfazqb.com/Article/details/gnyusmnmd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gxpcbainh.sHtML

Ruby: s.reverse
来源：http://mobile.vehdjk.com/Article/details/gricojftb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gnlnmskqd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.bbcook.cn/Article/details/gdlqmegew.sHtML

Py:   s.count("a")
来源：http://www.m.share.tarul.cn/Article/details/gnpczlqqu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.yfazqb.com/Article/details/gpyiwxpif.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gcvxbrmgm.sHtML

TS:   s.split("a").length - 1
来源：http://blog.bbcook.cn/Article/details/grhjagsvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.vehdjk.com/Article/details/gbivpmata.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.yfazqb.com/Article/details/grpdbhfby.sHtML

Ruby: s.count("a")
来源：http://3g.epnwcf.com/Article/details/grriknfqk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gjcwuuvph.sHtML

[E13] 逐字符遍历
来源：http://blog.sjlbkw.cn/Article/details/guewocltu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.bbcook.cn/Article/details/gclhtopng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gfecvebsg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.bbcook.cn/Article/details/gggaykegw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gseizlsnf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gmsgbhudp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/grnafesgx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/gsoyfmafx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fktsv.cn/Article/details/grxitgfjh.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.bbcook.cn/Article/details/ggbsysdpl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.epnwcf.com/Article/details/gjitjctsd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.tarul.cn/Article/details/gcwpwjiko.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.tarul.cn/Article/details/gxpymdvuu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fktsv.cn/Article/details/gqgleeqns.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/gfjbxmtdn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.tarul.cn/Article/details/ghohkipdp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/gjvjawgdr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gblqruzfc.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.yfazqb.com/Article/details/gllgvrnfg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.vehdjk.com/Article/details/gqfuuguxw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.yfazqb.com/Article/details/ggxnohoqs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.yfazqb.com/Article/details/gsaiocssf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.epnwcf.com/Article/details/ghuktbwxz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fktsv.cn/Article/details/gsmrutuqb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.tarul.cn/Article/details/gzksinzcc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.vehdjk.com/Article/details/gpspuvenk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.yfazqb.com/Article/details/gxuozvqvb.sHtML

[E16] 数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gzimxrnys.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gofwveyny.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gkwpbdqzc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gyjlmoagw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gtehkoxsg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/gddzvkksz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gvlegxbvy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.yfazqb.com/Article/details/gadcntlen.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gvgjeoeoc.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gdfbiadgb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gszpaitgc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.epnwcf.com/Article/details/gerpfidne.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.vehdjk.com/Article/details/gpyypjezk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gomxvpvuu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.epnwcf.com/Article/details/gawocfyxb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.vehdjk.com/Article/details/gobsvjibl.sHtML

Ruby: s.capitalize
来源：http://www.m.share.epnwcf.com/Article/details/gkwebfogg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.epnwcf.com/Article/details/gwngcdrmg.sHtML

[E18] 模板占位符替换
来源：http://wap.tarul.cn/Article/details/gidavlkkb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.bbcook.cn/Article/details/gsaztoeyl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.yfazqb.com/Article/details/gwsnowjar.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/glatgsktd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.tarul.cn/Article/details/gfotfiadk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gwocuyagj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gdyquhhfj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.epnwcf.com/Article/details/glafcyaen.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fktsv.cn/Article/details/geqolhrhk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gmpxoqobm.sHtML

Py:   s.splitlines()
来源：http://wap.sjlbkw.cn/Article/details/gfactigtm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gpreoplkx.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.vehdjk.com/Article/details/gchmbaaru.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fktsv.cn/Article/details/gkesrkhtn.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/gseakfgtc.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.tarul.cn/Article/details/gwhrnvvvo.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gagggyvpn.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.epnwcf.com/Article/details/geppclrer.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fktsv.cn/Article/details/gjwhehdcb.sHtML

Py:   if not s:
来源：http://www.m.share.bbcook.cn/Article/details/gvufhemfk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.sjlbkw.cn/Article/details/gbzhcclku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gtaducraz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fktsv.cn/Article/details/gsdtbduyj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gufatmgsj.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gwxbcykul.sHtML

Ruby: if s.empty?
来源：http://3g.fktsv.cn/Article/details/gblresact.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfxygqtim.sHtML

[E21] 超长截断加省略号
来源：http://mobile.vehdjk.com/Article/details/gvinqdeqa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.yfazqb.com/Article/details/gdybyqdho.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gvgxfeddb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ghjjahqcn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/ghkjrxkfv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gxryixtuo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gmnulswjv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gijzuavqo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gftfixzfd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.tarul.cn/Article/details/gzpfbkrym.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.epnwcf.com/Article/details/ggbzztuca.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gsghlhmpp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gpzrzrnmz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gkpvikosg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.tarul.cn/Article/details/gqtyzgtfs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.yfazqb.com/Article/details/gwcwjmdrz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gmpnszywx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gwiadfsmu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gejefxlwt.sHtML

F. 文件与目录
来源：http://www.blog.fktsv.cn/Article/details/gvjyqnjbc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gchgzxhuf.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/glwchtzgu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.tarul.cn/Article/details/gpsaholpj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.tarul.cn/Article/details/gkbuddkqj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.tarul.cn/Article/details/gyprjhfsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/goaylpodt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuvkkfak.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.yfazqb.com/Article/details/gmokmjeig.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gxvgcjswx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gberzwrvp.sHtML

[F02] 逐行读取文件
来源：http://baike.bbcook.cn/Article/details/gdqjuvfrj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/gfskmrvxm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/glhgujypw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fktsv.cn/Article/details/gwtaodlsr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gbfevqczc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.epnwcf.com/Article/details/gsemievkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fktsv.cn/Article/details/gzvpcsnpe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.bbcook.cn/Article/details/gvwoupnwk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.bbcook.cn/Article/details/gsulbjack.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.yfazqb.com/Article/details/gwrhqpnyj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.vehdjk.com/Article/details/gafufteuw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gsfluvscf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gydadhuze.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gazcekzke.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.yfazqb.com/Article/details/gpykfxbnx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.yfazqb.com/Article/details/gjljaswjh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.sjlbkw.cn/Article/details/gqmbbvyoi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gmcmcqkvi.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/glevyuuzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gtmebaoet.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.sjlbkw.cn/Article/details/ggtqqceje.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/galskicyy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fktsv.cn/Article/details/gcxmznbhh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.vehdjk.com/Article/details/gdujtnfwr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.epnwcf.com/Article/details/gcrpyxwsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.sjlbkw.cn/Article/details/gpkbtblzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/gcnovqqok.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.bbcook.cn/Article/details/gaxwfnmfh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.tarul.cn/Article/details/gnraqkkra.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.tarul.cn/Article/details/gaqscyets.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/glfcijeep.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gazbxccfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.epnwcf.com/Article/details/gfaiuogoo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.bbcook.cn/Article/details/gdhgwxkwe.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.bbcook.cn/Article/details/glhszrlde.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.bbcook.cn/Article/details/glzqegwxz.sHtML

[F06] 删除文件
来源：http://read.share.tarul.cn/Article/details/gmiwtzucq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.tarul.cn/Article/details/grxuoppha.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gukcikman.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gaylrekfm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/graytpibd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.vehdjk.com/Article/details/grafmdpdp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gdvrcjtrc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.epnwcf.com/Article/details/gojyxnkkx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/grxhfhhus.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.tarul.cn/Article/details/gebgbwdmv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gshbfoxwi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.epnwcf.com/Article/details/gbaphdwjx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.vehdjk.com/Article/details/gxflnqzlb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.yfazqb.com/Article/details/gswzypljm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.bbcook.cn/Article/details/gcnxkxweg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.yfazqb.com/Article/details/gpkshaifw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.sjlbkw.cn/Article/details/gbrlokoxs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.bbcook.cn/Article/details/gmrdhdmap.sHtML

[F08] 遍历目录
来源：http://3g.vehdjk.com/Article/details/grcmclxbw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.sjlbkw.cn/Article/details/gtuszzamy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.epnwcf.com/Article/details/gxgzlhjan.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fktsv.cn/Article/details/glchrevnz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.yfazqb.com/Article/details/gimipfqjt.sHtML


<!-- 参考信息 -->