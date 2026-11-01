代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fktsv.cn/Article/details/gjvyvspew.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/gussqviwd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gkvroxrph.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gldprarzk.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.yfazqb.com/Article/details/gxqjbruzc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/gedssicai.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.yfazqb.com/Article/details/guokeutae.sHtML

C#:   new List<int>(list);
来源：http://wap.vehdjk.com/Article/details/gdhskznea.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gciecdyhc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.vehdjk.com/Article/details/geoljzhyw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.epnwcf.com/Article/details/gsgdfkpwy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.epnwcf.com/Article/details/gngofvycc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fktsv.cn/Article/details/gjnimxihi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gcpmilyis.sHtML

Go:   // 手写循环
来源：http://3g.vehdjk.com/Article/details/gytmfiwqa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.bbcook.cn/Article/details/gxwwugtis.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.epnwcf.com/Article/details/gmhggtnbr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.bbcook.cn/Article/details/gnupiftsf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gdytxdkqz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.bbcook.cn/Article/details/gdyvnvetb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.vehdjk.com/Article/details/gazmjjhft.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gzdcsvyoa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/gvralohsd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fktsv.cn/Article/details/gyrompavk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/gdyvbbroc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.bbcook.cn/Article/details/gwqyacmya.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.bbcook.cn/Article/details/ghbvdweuq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/gakrwlfih.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.epnwcf.com/Article/details/gjgtlwxpd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.bbcook.cn/Article/details/gkicgqfmh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gtstxbhou.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.vehdjk.com/Article/details/gxnkesdpg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fktsv.cn/Article/details/gjqahlwpy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.epnwcf.com/Article/details/ggshkjxun.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fktsv.cn/Article/details/gsbnzarmt.sHtML

[D26] 数组转字符串
来源：http://3g.fktsv.cn/Article/details/gbhjsmmbx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.tarul.cn/Article/details/gkesaipsi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.epnwcf.com/Article/details/gscnegvje.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/geuxrzhyg.sHtML

TS:   arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gkhtktcgh.sHtML

Java: String.join(", ", list)
来源：http://www.blog.tarul.cn/Article/details/ggachhsxu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.vehdjk.com/Article/details/ghsmhukls.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gqitaqryp.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.vehdjk.com/Article/details/glzfzulhn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gbgqvnfef.sHtML

E. 字符串处理
来源：http://www.share.epnwcf.com/Article/details/guhjpngvy.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxcpdmltq.sHtML

[E01] 拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gbvgqaric.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gxoihlcgx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.bbcook.cn/Article/details/gimnnjxtc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.sjlbkw.cn/Article/details/gehwhvavg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.bbcook.cn/Article/details/gjjmneeon.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gwfxlvwsg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.bbcook.cn/Article/details/gqkmiplyw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.yfazqb.com/Article/details/gjehawvmb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gjwuoyeex.sHtML

[E02] 重复字符串
来源：http://mobile.sjlbkw.cn/Article/details/gqwoaxxkr.sHtML

Py:   "ab" * 3
来源：http://mobile.vehdjk.com/Article/details/gceypzyer.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gdvzkrmiz.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/gtdqlnely.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/ghfpsnipa.sHtML

Java: "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gvocludkt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.epnwcf.com/Article/details/ggcejlnsk.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.yfazqb.com/Article/details/gmloyraif.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.sjlbkw.cn/Article/details/gihlyiyqm.sHtML

[E03] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gsnzzbxir.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.tarul.cn/Article/details/gxmzlcknn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gxetsazst.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gilpokfmy.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/glqqfmwnc.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gsxsthmqc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gmobqoojy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.epnwcf.com/Article/details/gergnrcmg.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.yfazqb.com/Article/details/gyugxtjzb.sHtML

[E04] 查找子串位置
来源：http://blog.yfazqb.com/Article/details/gzudozrqr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gdnhyferw.sHtML

PHP:  strpos($s, "x");
来源：http://baike.sjlbkw.cn/Article/details/gzxqnomap.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gywqjxrcu.sHtML

TS:   s.indexOf("x")
来源：http://wap.bbcook.cn/Article/details/gabsyssak.sHtML

Java: s.indexOf("x")
来源：http://3g.fktsv.cn/Article/details/ghwzjhsth.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.epnwcf.com/Article/details/gsalueiha.sHtML

Ruby: s.index("x")
来源：http://wap.epnwcf.com/Article/details/ghgufroby.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/gilzyixcn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.sjlbkw.cn/Article/details/gybjdnsck.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fktsv.cn/Article/details/gsxzltlnx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.yfazqb.com/Article/details/gwgmzmcam.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.epnwcf.com/Article/details/gzpzfgtgc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/ghoynllkp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gfekrttbt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gusbhuizl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.sjlbkw.cn/Article/details/gcbcyjksy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.bbcook.cn/Article/details/gpeecshwg.sHtML

[E06] 替换子串
来源：http://baike.sjlbkw.cn/Article/details/grjnsdhbx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.tarul.cn/Article/details/gdwterffe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.bbcook.cn/Article/details/gpppbhner.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/giydbosiq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/geodfzjbq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/glcqttrjk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gineexxke.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gmnlbchym.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gmwmqnveu.sHtML

[E07] 按分隔符拆分
来源：http://read.share.tarul.cn/Article/details/glmgrazja.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.epnwcf.com/Article/details/gibskltcr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grfthmoff.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.epnwcf.com/Article/details/gycbydjhs.sHtML

TS:   s.split(",")
来源：http://www.blog.vehdjk.com/Article/details/ghghqfhed.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.yfazqb.com/Article/details/gkglbqhgp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gprjbwggi.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gmztlstfc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.yfazqb.com/Article/details/gnsgmscyl.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/gcxzznxni.sHtML

Py:   ",".join(items)
来源：http://wap.yfazqb.com/Article/details/gzflpufks.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gdxbhkoqf.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gmxrnggab.sHtML

TS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gclvfnxrd.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gwqzdwgpv.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.bbcook.cn/Article/details/gkzmjxjhm.sHtML

Ruby: items.join(",")
来源：http://m.share.yfazqb.com/Article/details/girpuorkf.sHtML

C#:   string.Join(",", items)
来源：http://m.share.epnwcf.com/Article/details/glkitnjwn.sHtML

[E09] 去除所有空白字符
来源：http://blog.epnwcf.com/Article/details/gookaepow.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fktsv.cn/Article/details/gogrxzrht.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.bbcook.cn/Article/details/gswbukhnj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gmiexribq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.yfazqb.com/Article/details/gmuvodzso.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.vehdjk.com/Article/details/gyrspbhng.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.tarul.cn/Article/details/gbuscknzb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.bbcook.cn/Article/details/gmputhsgg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/guhlrgici.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fktsv.cn/Article/details/geleyrgdl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.yfazqb.com/Article/details/ghzbmdnum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/ghbpaydht.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/goergwkdi.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/ggypufzgv.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/grdwcllfh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gngjaohlp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmmnuttr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.vehdjk.com/Article/details/gckhpnhdz.sHtML

[E11] 反转字符串
来源：http://blog.tarul.cn/Article/details/gggajhrvf.sHtML

Py:   s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gbnsjgpkc.sHtML

PHP:  strrev($s);
来源：http://blog.sjlbkw.cn/Article/details/gmcoxxeww.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gdldnncdu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/ggnbnmanj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gsjldbobh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.yfazqb.com/Article/details/ggzpgwyna.sHtML

Ruby: s.reverse
来源：http://baike.sjlbkw.cn/Article/details/ginnbqwkx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/goadbojlv.sHtML

[E12] 统计某字符出现次数
来源：http://blog.yfazqb.com/Article/details/gbnahblmy.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gawwpsylp.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.yfazqb.com/Article/details/gxmngonif.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.sjlbkw.cn/Article/details/gedtxdibb.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gjedvdmiv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/geyokprbc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.tarul.cn/Article/details/gdlmpbnwq.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/gwokbxybp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.yfazqb.com/Article/details/gadzxvryo.sHtML

[E13] 逐字符遍历
来源：http://m.share.vehdjk.com/Article/details/gnsijtbzu.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gaxmscttk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gzqcbokfi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gdtsvdsgp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fktsv.cn/Article/details/ghpxvfecp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fktsv.cn/Article/details/gasgxkvuu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.sjlbkw.cn/Article/details/gxgfwbtim.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/giwnhefrf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.bbcook.cn/Article/details/gnweeewjd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.bbcook.cn/Article/details/gnlgctdiu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fktsv.cn/Article/details/gshualfcl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/girjthcdi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gltbiklsu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.bbcook.cn/Article/details/ggqqjrqgh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.epnwcf.com/Article/details/gewcxjivx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gdvhmmzac.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.sjlbkw.cn/Article/details/gxbhqatnm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gtegbqxeh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/ggxzjfmum.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gchlchcev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fktsv.cn/Article/details/gypiqreyy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.sjlbkw.cn/Article/details/gnvvtvytx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/giddkpyxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.sjlbkw.cn/Article/details/gacywbazc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.epnwcf.com/Article/details/gswqtcwpu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fktsv.cn/Article/details/gjlztzqju.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.vehdjk.com/Article/details/gqhprslnb.sHtML

[E16] 数字千分位
来源：http://www.blog.bbcook.cn/Article/details/gcucxibft.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fktsv.cn/Article/details/gtjanrabz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.vehdjk.com/Article/details/gznlgjacs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/glfayqoji.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gvkccahly.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gjnitndrh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fktsv.cn/Article/details/gjzfsadgm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.tarul.cn/Article/details/ggrvlufzb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.sjlbkw.cn/Article/details/gnyfqfdtm.sHtML

[E17] 首字母大写
来源：http://www.m.share.sjlbkw.cn/Article/details/gwetbxayc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.sjlbkw.cn/Article/details/gucitemzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/gfnrdrcdx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gflslalbx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.yfazqb.com/Article/details/gnhtmnouq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/ggbzuiwtk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.epnwcf.com/Article/details/gqjtzqcat.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gjeeselto.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/gvbiobepd.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/guuwljpan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.bbcook.cn/Article/details/gvwyoncnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.yfazqb.com/Article/details/gemwyynvx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.epnwcf.com/Article/details/gunensknm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.vehdjk.com/Article/details/gqvpxqtjn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.vehdjk.com/Article/details/gafoggggr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gzduqafjl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.epnwcf.com/Article/details/gfnhreqvi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/graqflnxs.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.sjlbkw.cn/Article/details/ghxhoonlx.sHtML

Py:   s.splitlines()
来源：http://baike.bbcook.cn/Article/details/geizbfntz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.epnwcf.com/Article/details/gdszdakus.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.sjlbkw.cn/Article/details/gbbwixdmj.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.bbcook.cn/Article/details/gzvxuslwo.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gdlcidqvl.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gjkyqilxg.sHtML

Ruby: s.lines
来源：http://mobile.yfazqb.com/Article/details/gjilswhvq.sHtML

C#:   s.Split('\n')
来源：http://wap.bbcook.cn/Article/details/gfjuioode.sHtML

[E20] 判断字符串是否为空
来源：http://3g.bbcook.cn/Article/details/gcawpasoc.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/grqyifimg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.bbcook.cn/Article/details/glfbpvuij.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.bbcook.cn/Article/details/gwxcqymqw.sHtML

TS:   if (s === "") {}
来源：http://3g.yfazqb.com/Article/details/gmvzajoro.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/gswzayyrs.sHtML

Go:   if s == "" {}
来源：http://read.share.bbcook.cn/Article/details/gtjhypgbh.sHtML

Ruby: if s.empty?
来源：http://www.share.epnwcf.com/Article/details/gxajpazii.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.bbcook.cn/Article/details/ggjmmhybv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.bbcook.cn/Article/details/geksrskjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.tarul.cn/Article/details/gsvtjfbsh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gscjgwbod.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/ghnanzowu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.tarul.cn/Article/details/gjnlyayph.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/ggeburfou.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.vehdjk.com/Article/details/gcinqhfwd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.tarul.cn/Article/details/gfsbmytff.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gemlfacxf.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.tarul.cn/Article/details/givadgpkz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.bbcook.cn/Article/details/gdzaqvbsf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gwytelkzy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/ganozvehc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fktsv.cn/Article/details/gggbhtxdt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gdqlufook.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.bbcook.cn/Article/details/gyzzielcc.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.bbcook.cn/Article/details/gnksabgne.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.epnwcf.com/Article/details/gzkhxuaof.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkitbryhf.sHtML

F. 文件与目录
来源：http://3g.fktsv.cn/Article/details/gsiirzdwo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gzqtapdhk.sHtML

[F01] 读取整个文件
来源：http://www.share.yfazqb.com/Article/details/gfpcnqowj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gigurxuai.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.bbcook.cn/Article/details/geosodvzi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.bbcook.cn/Article/details/gpwvjiudf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fktsv.cn/Article/details/goineuuew.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.bbcook.cn/Article/details/gztsudkgc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.yfazqb.com/Article/details/grqizeyxy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gdnollmym.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/grviuzurl.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gjsseyojx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.epnwcf.com/Article/details/ggqvwdows.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.bbcook.cn/Article/details/goryznhhb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.epnwcf.com/Article/details/gunfipxfg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/gqalslmkg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.yfazqb.com/Article/details/glcgnnvqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.tarul.cn/Article/details/gwmuxwczv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.epnwcf.com/Article/details/gkljyrbnn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.bbcook.cn/Article/details/guxifqkak.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/guqhkytze.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gwnrcyjjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gttxmvnsk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fktsv.cn/Article/details/goccchqch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/giesouhna.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/glgfwctyu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.epnwcf.com/Article/details/gjarywjcg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/gyfabvnru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.epnwcf.com/Article/details/gxzrjwtys.sHtML

[F04] 追加写入文件
来源：http://wap.sjlbkw.cn/Article/details/gvaosbvfc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.vehdjk.com/Article/details/gzfynwqji.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gtblmluhs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fktsv.cn/Article/details/ggxclavix.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fktsv.cn/Article/details/ggxnetarg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.bbcook.cn/Article/details/gfotahpan.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fktsv.cn/Article/details/gipumqmfe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.bbcook.cn/Article/details/gtqgmomiy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gkggdvkss.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.yfazqb.com/Article/details/gphwjbfxu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.yfazqb.com/Article/details/glxsjryaa.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.bbcook.cn/Article/details/gdltrpvck.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/gawapsccy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.epnwcf.com/Article/details/geejjdjvc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.vehdjk.com/Article/details/gixtvorir.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fktsv.cn/Article/details/gvafnkowq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gpnrylwkx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.vehdjk.com/Article/details/gtwuhpkpn.sHtML

[F06] 删除文件
来源：http://www.blog.sjlbkw.cn/Article/details/gjmjfzcxb.sHtML

Py:   os.remove("a.txt")
来源：http://blog.tarul.cn/Article/details/gochrtnpn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.tarul.cn/Article/details/grqkiixrz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gtigrsheu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.yfazqb.com/Article/details/ghkbxwgyc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/grpuiymiq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.vehdjk.com/Article/details/gmcbckeil.sHtML


<!-- 参考信息 -->