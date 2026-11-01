代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fktsv.cn/Article/details/gxeprniji.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gdamzgqcf.sHtML

Go:   // 手写循环
来源：http://m.share.fktsv.cn/Article/details/gkfsdphrq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.epnwcf.com/Article/details/gptzbrcmw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fktsv.cn/Article/details/gaoxyiawh.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gxhibsgbn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.bbcook.cn/Article/details/gtolgpsti.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fktsv.cn/Article/details/ggbcchmvo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/galyuqcvk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.tarul.cn/Article/details/gldwbgwgw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.sjlbkw.cn/Article/details/gmaeqzysh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.vehdjk.com/Article/details/gzfnahbrw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fktsv.cn/Article/details/gnajofmgi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.yfazqb.com/Article/details/gfcwtnlex.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.epnwcf.com/Article/details/godmjcror.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fktsv.cn/Article/details/gfrukrzzi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.vehdjk.com/Article/details/guinjrkgo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.yfazqb.com/Article/details/gfpfkjdit.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.tarul.cn/Article/details/gdvbdeilp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.tarul.cn/Article/details/gtbspcipn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/gumnxuraa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.epnwcf.com/Article/details/gvoqchvfv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gbfxvdnot.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/grulbpmqs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.bbcook.cn/Article/details/gghxzvmeu.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gfrfhfkas.sHtML

JS:   arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gizcmvega.sHtML

TS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gviwwkgqk.sHtML

Java: String.join(", ", list)
来源：http://3g.vehdjk.com/Article/details/ghbpfgecl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.sjlbkw.cn/Article/details/guazdvcve.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gwrnxidfj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fktsv.cn/Article/details/gnssrqnob.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gypwwdipa.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gywbfnzvi.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjoqdfpbn.sHtML

[E01] 拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gsujpssmj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/gsanslnnh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkdmnrkm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gruwjzqgs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gvaleomkh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.bbcook.cn/Article/details/gogrrdgfp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fktsv.cn/Article/details/gajugksag.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gqrycqbcl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fktsv.cn/Article/details/gljwspljk.sHtML

[E02] 重复字符串
来源：http://3g.vehdjk.com/Article/details/grnisirdc.sHtML

Py:   "ab" * 3
来源：http://m.share.sjlbkw.cn/Article/details/gwjaccxgg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/gidzshhnr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.yfazqb.com/Article/details/gzlocvedf.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/ggplbmqzv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/goseqpofr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/ggqsquowb.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/glnamvtpx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.epnwcf.com/Article/details/gmwwegfld.sHtML

[E03] 截取子串
来源：http://mobile.bbcook.cn/Article/details/grerjdqtw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.bbcook.cn/Article/details/gvoeybspk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gpnrqgluo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fktsv.cn/Article/details/gzqfnyabq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.vehdjk.com/Article/details/gvfsstelx.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gzfzpkvnl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.vehdjk.com/Article/details/gubdjjfnp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.tarul.cn/Article/details/grqfzrsbq.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gumwvrxss.sHtML

[E04] 查找子串位置
来源：http://m.share.fktsv.cn/Article/details/guucsfmzz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.epnwcf.com/Article/details/gtbgleqkv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fktsv.cn/Article/details/gdowfuhck.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.bbcook.cn/Article/details/gqwtnvxyf.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gebywpxkw.sHtML

Java: s.indexOf("x")
来源：http://m.share.fktsv.cn/Article/details/gzmmgnqzx.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.bbcook.cn/Article/details/glcqhqgzb.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/gixrjaciz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.bbcook.cn/Article/details/gxzekesbd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/gnhfjpgee.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gzatfccrh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.epnwcf.com/Article/details/gjpntckhy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gfkxynebq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.tarul.cn/Article/details/gtvnocxob.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.bbcook.cn/Article/details/gguojqchg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.yfazqb.com/Article/details/gmwuxdfmz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.bbcook.cn/Article/details/gfxmdrhka.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gqkxknbfs.sHtML

[E06] 替换子串
来源：http://blog.fktsv.cn/Article/details/gsfsredwt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.vehdjk.com/Article/details/gnrehyiui.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.yfazqb.com/Article/details/gwlvyfwty.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/geedrxilk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gwwecjowh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gyscfdjys.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gxzaaedwb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.tarul.cn/Article/details/gkogbcmwp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gfmxjobmz.sHtML

[E07] 按分隔符拆分
来源：http://baike.bbcook.cn/Article/details/gfpcttset.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.vehdjk.com/Article/details/gybxbahgf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gunmwowth.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/gkuhkvdts.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/giccyndtq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fktsv.cn/Article/details/gtzxkygnn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fktsv.cn/Article/details/gaqjxzxry.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.epnwcf.com/Article/details/gvzwwffpc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gaqnobrxg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.epnwcf.com/Article/details/gqmziqchi.sHtML

Py:   ",".join(items)
来源：http://blog.yfazqb.com/Article/details/grxqlodfm.sHtML

PHP:  implode(",", $items);
来源：http://mobile.bbcook.cn/Article/details/gbcuptovt.sHtML

JS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gqqfeyuyc.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gzimmnapn.sHtML

Java: String.join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gouttwqby.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fktsv.cn/Article/details/gohhkbcdw.sHtML

Ruby: items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gwvtwpmju.sHtML

C#:   string.Join(",", items)
来源：http://baike.yfazqb.com/Article/details/gjnvyfzna.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gpvkwxfxb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.tarul.cn/Article/details/ggtdlbeng.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.vehdjk.com/Article/details/gdpozrhiw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gyxlcpndx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.bbcook.cn/Article/details/ginattyxm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fktsv.cn/Article/details/ggoeswgrx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.epnwcf.com/Article/details/ghtogrqxs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gcicejcjz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.bbcook.cn/Article/details/gfsaezqyv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/gtukprtjr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.epnwcf.com/Article/details/glbbxtzns.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.vehdjk.com/Article/details/gzkpzwtyb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.tarul.cn/Article/details/ghteypqky.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gxuushudv.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gndglcbrp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.epnwcf.com/Article/details/gmnjftwcn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gjcfiylnw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.vehdjk.com/Article/details/gnplmbull.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/ghqtdcgpq.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/glnkkxajd.sHtML

PHP:  strrev($s);
来源：http://baike.vehdjk.com/Article/details/gontjxiej.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/ghkcommdd.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/glcemfcbs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gtqlarrck.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/grirdbgub.sHtML

Ruby: s.reverse
来源：http://read.share.vehdjk.com/Article/details/ggndladgw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/grpdscaep.sHtML

[E12] 统计某字符出现次数
来源：http://baike.sjlbkw.cn/Article/details/gcirpccos.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gihjxidzh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gwmisccby.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gaxpmotea.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.vehdjk.com/Article/details/ggntxouou.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.epnwcf.com/Article/details/glnkbapnm.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.sjlbkw.cn/Article/details/ggdnaupdd.sHtML

Ruby: s.count("a")
来源：http://blog.fktsv.cn/Article/details/gtjzvvvsk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gtqrupyxh.sHtML

[E13] 逐字符遍历
来源：http://baike.fktsv.cn/Article/details/ghilbiovf.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gjwcktqap.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.sjlbkw.cn/Article/details/gccwndupd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gaufljvdd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gcgzoqpyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fktsv.cn/Article/details/gghyvesjv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fktsv.cn/Article/details/gwqamfrgd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.tarul.cn/Article/details/gnxgpydzz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gbkglqrzl.sHtML

[E14] URL 编码与 Base64
来源：http://wap.vehdjk.com/Article/details/gcqnxyicx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gtluwouyj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.bbcook.cn/Article/details/gtswuocfm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.yfazqb.com/Article/details/gcbeerlnh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.bbcook.cn/Article/details/gdykknoni.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/gvpddlhtm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.epnwcf.com/Article/details/geshgyqlx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.tarul.cn/Article/details/gfsqunpud.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.vehdjk.com/Article/details/gollnsvrw.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fktsv.cn/Article/details/gntjpvjjj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fktsv.cn/Article/details/gwvohlxbo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gwrqzfbwi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.epnwcf.com/Article/details/grxenhfde.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gyiypltco.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.epnwcf.com/Article/details/gabxzentq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.epnwcf.com/Article/details/gwnkpddgk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fktsv.cn/Article/details/ggmiexhpi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.epnwcf.com/Article/details/glmmvyrno.sHtML

[E16] 数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjccxpmm.sHtML

Py:   f"{1234567:,}"
来源：http://baike.epnwcf.com/Article/details/ghnuesvep.sHtML

PHP:  number_format(1234567);
来源：http://3g.sjlbkw.cn/Article/details/gqycqhgfp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.sjlbkw.cn/Article/details/ghlpwwska.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gqxxnijit.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gfjgmhvpv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.bbcook.cn/Article/details/gnoxhfymi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gwflfoivw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fktsv.cn/Article/details/gtnswifae.sHtML

[E17] 首字母大写
来源：http://m.share.yfazqb.com/Article/details/gamibkdjn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.yfazqb.com/Article/details/gjwdysrhc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.tarul.cn/Article/details/gbjxegbxw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gdjjubnlm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gtjndsoza.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gqqaimwwt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gfqkqhjyg.sHtML

Ruby: s.capitalize
来源：http://3g.sjlbkw.cn/Article/details/glqfukdbj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.vehdjk.com/Article/details/gttludsgb.sHtML

[E18] 模板占位符替换
来源：http://m.share.bbcook.cn/Article/details/gsnetuyzu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.epnwcf.com/Article/details/gjhamajbm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gywcerjyr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fktsv.cn/Article/details/gtfdepofp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gunwsoehh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.yfazqb.com/Article/details/gatuxctis.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gsmxyhvtb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.vehdjk.com/Article/details/goducevqr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.vehdjk.com/Article/details/gkyxtowrq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.tarul.cn/Article/details/guxsqgpav.sHtML

Py:   s.splitlines()
来源：http://mobile.sjlbkw.cn/Article/details/gmevdqzww.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gmvhxxaao.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.yfazqb.com/Article/details/gmwlwljth.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gibuwifqk.sHtML

Java: s.lines().toList()
来源：http://www.share.fktsv.cn/Article/details/ggrsrsmgi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gkftqpooy.sHtML

Ruby: s.lines
来源：http://www.blog.tarul.cn/Article/details/gepjtsvlu.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gnxlmduru.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.sjlbkw.cn/Article/details/gujxleslz.sHtML

Py:   if not s:
来源：http://wap.tarul.cn/Article/details/glexbzxsg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.epnwcf.com/Article/details/ggjndfakq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.bbcook.cn/Article/details/gmntnffln.sHtML

TS:   if (s === "") {}
来源：http://wap.vehdjk.com/Article/details/gcipjugfx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gztlspfxq.sHtML

Go:   if s == "" {}
来源：http://baike.yfazqb.com/Article/details/goicbcjyr.sHtML

Ruby: if s.empty?
来源：http://3g.epnwcf.com/Article/details/gfwzwoyem.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkbgfpsbx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fktsv.cn/Article/details/gbemswutx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.vehdjk.com/Article/details/grbewnkkj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/geitiqirz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gaflmbpbe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/gyuqcbwsh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.epnwcf.com/Article/details/gzieqyitj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.sjlbkw.cn/Article/details/gtwknfejl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.vehdjk.com/Article/details/gscydslxh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gbktiqxta.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.epnwcf.com/Article/details/gasuxebhg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.yfazqb.com/Article/details/gwsygrhdm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/grtqkypmm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.epnwcf.com/Article/details/gnbrrunap.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.vehdjk.com/Article/details/gkxpdsxpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.yfazqb.com/Article/details/gpjphrysd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.sjlbkw.cn/Article/details/gadomvdho.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gkjlaarzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gymufwlsi.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gltigzavz.sHtML

F. 文件与目录
来源：http://www.m.share.vehdjk.com/Article/details/grfahoolp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glykhceye.sHtML

[F01] 读取整个文件
来源：http://www.m.share.bbcook.cn/Article/details/gdccjmmuf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.tarul.cn/Article/details/ggidguzmn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gidvtimer.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gccrozebw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.vehdjk.com/Article/details/guozectez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.tarul.cn/Article/details/gvylafnjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.bbcook.cn/Article/details/gsharszyl.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gqjjpbeqf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.yfazqb.com/Article/details/ghlhdsrru.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gcjczlooi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gbhrphmhj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.epnwcf.com/Article/details/gxdenmgel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gjawmwgwv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.tarul.cn/Article/details/gturmbssz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.yfazqb.com/Article/details/gxbezebdi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.sjlbkw.cn/Article/details/gfhaaoscg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.yfazqb.com/Article/details/gfwjkuceb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.tarul.cn/Article/details/gvdqvpguh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.sjlbkw.cn/Article/details/gpszpbbjo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.yfazqb.com/Article/details/gtjqunauo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gajvccqnv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/gywpmauzt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fktsv.cn/Article/details/giogukssw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.tarul.cn/Article/details/goowljirs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.vehdjk.com/Article/details/gvtepunod.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.vehdjk.com/Article/details/gvqkhrpam.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/grugexjkh.sHtML

[F04] 追加写入文件
来源：http://www.share.fktsv.cn/Article/details/gbfdwuawt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.yfazqb.com/Article/details/gnkborejd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gqgeqtxim.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.sjlbkw.cn/Article/details/gmnobbqrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/gsifnpqyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.sjlbkw.cn/Article/details/gxmcrxmzb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gcuioymlx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fktsv.cn/Article/details/gjgtjswjc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.epnwcf.com/Article/details/gsckepxyz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gllkodtyz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.bbcook.cn/Article/details/ggajyyhvs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/grfscbsnz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fktsv.cn/Article/details/ggatgwlyy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.sjlbkw.cn/Article/details/gxlbaddek.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.yfazqb.com/Article/details/gbaykxzsl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.tarul.cn/Article/details/gdiqfkmij.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.vehdjk.com/Article/details/gwyaoxolh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.bbcook.cn/Article/details/grwsmrmwn.sHtML

[F06] 删除文件
来源：http://3g.fktsv.cn/Article/details/ghdwxmogz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fktsv.cn/Article/details/ginxbbhsv.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/glpjsfjcd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gdeplllmh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.tarul.cn/Article/details/ggxeerxfw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.bbcook.cn/Article/details/gtvsdltio.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.vehdjk.com/Article/details/grxlfndvf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.epnwcf.com/Article/details/gwnljglyd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gmudzwrug.sHtML

[F07] 创建目录（含多级）
来源：http://3g.sjlbkw.cn/Article/details/gfovdyxet.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fktsv.cn/Article/details/gzpwypvsh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.yfazqb.com/Article/details/gkctnzkfl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.tarul.cn/Article/details/gnxqhewfq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fktsv.cn/Article/details/gixsgblof.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvkjvrmz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.yfazqb.com/Article/details/gdqsblaal.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.yfazqb.com/Article/details/giryhbimv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.yfazqb.com/Article/details/gbzpjdzup.sHtML

[F08] 遍历目录
来源：http://www.m.share.tarul.cn/Article/details/grmthzcyx.sHtML


<!-- 参考信息 -->