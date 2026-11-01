代发 wailian999

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/gnaazffwy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.epnwcf.com/Article/details/gmhtnxzck.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/geaiwuwsp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxleqjpn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.yfazqb.com/Article/details/gurpujrhk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.sjlbkw.cn/Article/details/gueqlwhzk.sHtML

Go:   // 手写循环
来源：http://3g.yfazqb.com/Article/details/gghbbxnee.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.bbcook.cn/Article/details/ganpblexg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.tarul.cn/Article/details/gtpvtwfhf.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.sjlbkw.cn/Article/details/gmpzbdjvz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.bbcook.cn/Article/details/gcqwzkxep.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.epnwcf.com/Article/details/gyftwcfrx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gcikvzpww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gsjjeigxt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fktsv.cn/Article/details/ghzxnqapk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gnmhiknyn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/glsbiaowe.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gyfatymev.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fktsv.cn/Article/details/gyrvotrlq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.tarul.cn/Article/details/gvwdioewh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.sjlbkw.cn/Article/details/gtzkncyuq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.bbcook.cn/Article/details/gdjhbigcf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.tarul.cn/Article/details/gshwlxcdn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/golefdxbc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gavwwnplh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.tarul.cn/Article/details/gfjnurjkz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.yfazqb.com/Article/details/goqtjwqek.sHtML

[D26] 数组转字符串
来源：http://www.m.share.bbcook.cn/Article/details/guzytkdne.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.epnwcf.com/Article/details/gypydvmjv.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gzvsidkmd.sHtML

JS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gnoduzgrf.sHtML

TS:   arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gztkyyxtz.sHtML

Java: String.join(", ", list)
来源：http://www.blog.sjlbkw.cn/Article/details/gfyozsmra.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fktsv.cn/Article/details/gtasvsgod.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/gwqlludpd.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gnecwjthk.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcbsecrry.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gvqqbovzu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkamfuulm.sHtML

[E01] 拼接字符串
来源：http://blog.epnwcf.com/Article/details/gmtaagtwr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fktsv.cn/Article/details/gnhnglcdq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.bbcook.cn/Article/details/ggeusfepk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.epnwcf.com/Article/details/gmcpgkfnx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.vehdjk.com/Article/details/gpvvekrkt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/grecnspho.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.yfazqb.com/Article/details/gbrnvtkei.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.vehdjk.com/Article/details/gnouyaepo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/ggjrvzejp.sHtML

[E02] 重复字符串
来源：http://mobile.yfazqb.com/Article/details/gsuuucymm.sHtML

Py:   "ab" * 3
来源：http://m.share.tarul.cn/Article/details/ganoxmxig.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gvssyjxwa.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gdbqrxqoh.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.epnwcf.com/Article/details/gqessjvql.sHtML

Java: "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/gyltawgjp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.yfazqb.com/Article/details/gxtbrsrnq.sHtML

Ruby: "ab" * 3
来源：http://www.share.fktsv.cn/Article/details/gkdsunedq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.vehdjk.com/Article/details/glpbzcfks.sHtML

[E03] 截取子串
来源：http://m.share.sjlbkw.cn/Article/details/gwlqpbezd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gyklokejn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvbwyxlt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fktsv.cn/Article/details/gaprsrloa.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.bbcook.cn/Article/details/giqwknsel.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/ghvcdmmea.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/graicetca.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fktsv.cn/Article/details/gckqltitw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.epnwcf.com/Article/details/gssoxctkj.sHtML

[E04] 查找子串位置
来源：http://mobile.yfazqb.com/Article/details/gyirvevvo.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gcxwflppg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.yfazqb.com/Article/details/gnbavyicn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.sjlbkw.cn/Article/details/gcrauqrhq.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gwlutbind.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gjuomioxc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gqrcfruwg.sHtML

Ruby: s.index("x")
来源：http://wap.fktsv.cn/Article/details/gqupiqitl.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.vehdjk.com/Article/details/gacbjyfvk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.sjlbkw.cn/Article/details/gxdiuljac.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fktsv.cn/Article/details/gtdyqcnjq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/gyjjhbsvn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gnumjqxga.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.tarul.cn/Article/details/gawyqinnj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.tarul.cn/Article/details/gremkzsie.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gnyeoxdar.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.bbcook.cn/Article/details/gfgfdrabh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gzcrbyqml.sHtML

[E06] 替换子串
来源：http://3g.bbcook.cn/Article/details/gucirxacs.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.bbcook.cn/Article/details/gusqvpekn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.vehdjk.com/Article/details/gvnxpxbdw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/ggymabgdk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gbuknsdfp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gqrsmspsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/ghqepxdgd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.tarul.cn/Article/details/geqcqcefi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gngxywjbr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.bbcook.cn/Article/details/gmtmcbejm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.vehdjk.com/Article/details/gbqhmujxp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.bbcook.cn/Article/details/ghqhzfbit.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.epnwcf.com/Article/details/gllsyxffw.sHtML

TS:   s.split(",")
来源：http://baike.sjlbkw.cn/Article/details/gkmqgtbsj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.sjlbkw.cn/Article/details/guyojsjvc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.vehdjk.com/Article/details/gwvqbyvcj.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.sjlbkw.cn/Article/details/gmqmdnjsj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.bbcook.cn/Article/details/gdvblxfee.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/glxtspotw.sHtML

Py:   ",".join(items)
来源：http://baike.sjlbkw.cn/Article/details/gjtkrpkvo.sHtML

PHP:  implode(",", $items);
来源：http://wap.epnwcf.com/Article/details/gdkhsbsxt.sHtML

JS:   items.join(",")
来源：http://blog.tarul.cn/Article/details/gcqtsdwcn.sHtML

TS:   items.join(",")
来源：http://wap.yfazqb.com/Article/details/guurihevz.sHtML

Java: String.join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gkgbsnjgd.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.vehdjk.com/Article/details/gwqdpybkd.sHtML

Ruby: items.join(",")
来源：http://www.blog.epnwcf.com/Article/details/guccqaluv.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gmnegfnko.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fktsv.cn/Article/details/gucadepka.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gzhuhvuhg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.epnwcf.com/Article/details/gqdkijnin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.yfazqb.com/Article/details/gvuccygtn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.tarul.cn/Article/details/gtpywemua.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.vehdjk.com/Article/details/ggaofeekq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.tarul.cn/Article/details/grsrqdmwr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.vehdjk.com/Article/details/gzhvapwso.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.bbcook.cn/Article/details/gvuflibui.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.bbcook.cn/Article/details/geqmxyeeg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gdytbcwan.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.vehdjk.com/Article/details/gncxrheyk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gqfehobbw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.vehdjk.com/Article/details/girmwqong.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gtiwpfrvs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gwpvcinqw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gfvguuuyz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.bbcook.cn/Article/details/gkmgbfysd.sHtML

[E11] 反转字符串
来源：http://www.blog.yfazqb.com/Article/details/gjggholxy.sHtML

Py:   s[::-1]
来源：http://read.share.tarul.cn/Article/details/geicogqwm.sHtML

PHP:  strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gpywbyghs.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gvzlgrpvx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gxbbueved.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.bbcook.cn/Article/details/gjzqpvwas.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.yfazqb.com/Article/details/gagfnqakh.sHtML

Ruby: s.reverse
来源：http://m.share.fktsv.cn/Article/details/ggictiycf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.sjlbkw.cn/Article/details/gwlevnzgz.sHtML

[E12] 统计某字符出现次数
来源：http://wap.tarul.cn/Article/details/gwpvhgmru.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gxpxaffpm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.sjlbkw.cn/Article/details/gopelfazi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gmgxvvpif.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gftqupaja.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.tarul.cn/Article/details/gddzftggs.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.tarul.cn/Article/details/glqfyldwo.sHtML

Ruby: s.count("a")
来源：http://3g.tarul.cn/Article/details/gpplleipd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.epnwcf.com/Article/details/gdxebnuaq.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/gfqrisgad.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/ggmbeksgy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.bbcook.cn/Article/details/gswtosmqg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gjfjpmxzd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtarwcrsu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.bbcook.cn/Article/details/gmvnjqsvm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/guqhltqhv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.vehdjk.com/Article/details/gtktipdts.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gsdyyidju.sHtML

[E14] URL 编码与 Base64
来源：http://wap.sjlbkw.cn/Article/details/gkyudpwpy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gfrqnaiye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.bbcook.cn/Article/details/gxhimowcp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.vehdjk.com/Article/details/gfuoxpnjy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.tarul.cn/Article/details/gdcaxfxlu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.yfazqb.com/Article/details/gbwtrldsy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.sjlbkw.cn/Article/details/gnsqljryk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.sjlbkw.cn/Article/details/genwpzsnx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fktsv.cn/Article/details/gpnywibin.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.sjlbkw.cn/Article/details/gnjzecyrm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.bbcook.cn/Article/details/gggeenkfr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.vehdjk.com/Article/details/gdwdvvzyl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.tarul.cn/Article/details/gybetdplm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fktsv.cn/Article/details/gxqexoqxi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fktsv.cn/Article/details/gmgrfrwzt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.vehdjk.com/Article/details/gnvlgasgo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/gujejkpcu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.bbcook.cn/Article/details/gyglpfmsp.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/gnqagzjhk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.epnwcf.com/Article/details/gtsefcoeo.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fktsv.cn/Article/details/gqlvtmkzz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fktsv.cn/Article/details/gzkeweswp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.epnwcf.com/Article/details/gxkewxgcc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/ghsrebjka.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.sjlbkw.cn/Article/details/gkyffcgcr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.bbcook.cn/Article/details/gauswxsoi.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.epnwcf.com/Article/details/gkqlaygxn.sHtML

[E17] 首字母大写
来源：http://www.m.share.vehdjk.com/Article/details/geihvfmfn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.epnwcf.com/Article/details/gelymuulq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gnhniofkt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/gxfgwvygc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.yfazqb.com/Article/details/gzwcinlwn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gimmgrket.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fktsv.cn/Article/details/gpnunityx.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/gltisxtio.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.bbcook.cn/Article/details/gleypgzes.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gumuwmros.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gunzfqeyp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.vehdjk.com/Article/details/gyajtxhdq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gymrodbde.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/giardnoqd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.tarul.cn/Article/details/gdedrrrie.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.bbcook.cn/Article/details/gbowemzyj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.tarul.cn/Article/details/gmklierbb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.yfazqb.com/Article/details/glglosfcr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gmbastpeq.sHtML

Py:   s.splitlines()
来源：http://m.share.fktsv.cn/Article/details/gnimsnhmx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.epnwcf.com/Article/details/gupnqvzan.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gpeexmbfl.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gfuwyfsis.sHtML

Java: s.lines().toList()
来源：http://m.share.fktsv.cn/Article/details/gspitopxy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.vehdjk.com/Article/details/gkczyjjfk.sHtML

Ruby: s.lines
来源：http://read.share.tarul.cn/Article/details/gmverglkd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/guvevicwe.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fktsv.cn/Article/details/gmxgoqadl.sHtML

Py:   if not s:
来源：http://mobile.bbcook.cn/Article/details/glmuhthod.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.vehdjk.com/Article/details/ggglddiex.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.yfazqb.com/Article/details/grqosejsa.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/gjonmckvk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gdpiklsms.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gacmjawku.sHtML

Ruby: if s.empty?
来源：http://read.share.fktsv.cn/Article/details/gqtcmktcg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gypnqiosa.sHtML

[E21] 超长截断加省略号
来源：http://3g.bbcook.cn/Article/details/grliqeriw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.bbcook.cn/Article/details/gjcqowzzi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gjzeugyrc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.vehdjk.com/Article/details/glzxvndum.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gaheudskm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/glwhbkzdr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fktsv.cn/Article/details/gpvibuhil.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gmrbcyxes.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.sjlbkw.cn/Article/details/gbjhnscfd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.sjlbkw.cn/Article/details/gkoyinnzc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gaeltoxhp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/ggqciqufu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gxpwvmeyf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gadqbwxgr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.epnwcf.com/Article/details/gtvpczfjr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/gdgtmylym.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gbjpjygfh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/ggneefigx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/giwxicwrj.sHtML

F. 文件与目录
来源：http://m.share.bbcook.cn/Article/details/gkvuiwuxf.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvlxprwgd.sHtML

[F01] 读取整个文件
来源：http://m.share.bbcook.cn/Article/details/gvtvbndwo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.sjlbkw.cn/Article/details/gowqhxjsw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gofcmgxjo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.yfazqb.com/Article/details/gwkwlofma.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/gqeczzixc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/gqrplvssi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.sjlbkw.cn/Article/details/guylsvfby.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/ggohrrete.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gqzclxggs.sHtML

[F02] 逐行读取文件
来源：http://m.share.epnwcf.com/Article/details/gawyrjqoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.tarul.cn/Article/details/gbdbymltl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.sjlbkw.cn/Article/details/grrocdeqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gchjdgehp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gyzfzbexv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzultpilm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.sjlbkw.cn/Article/details/gruadtbuv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fktsv.cn/Article/details/ghertiybb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.epnwcf.com/Article/details/gfwaqprrd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.vehdjk.com/Article/details/grneydwnz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.bbcook.cn/Article/details/glzstjkgd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.vehdjk.com/Article/details/gssjfaczy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.yfazqb.com/Article/details/gkyilgudq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.bbcook.cn/Article/details/gfznowcqj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.vehdjk.com/Article/details/gedwpawbe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gbnrsqwud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.bbcook.cn/Article/details/gfwbwavat.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/gnqcgqiig.sHtML

[F04] 追加写入文件
来源：http://baike.epnwcf.com/Article/details/gmexqycid.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fktsv.cn/Article/details/gixushqay.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.bbcook.cn/Article/details/gwyrwphjq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gxrgrkmdf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.vehdjk.com/Article/details/ghwhgzzek.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.sjlbkw.cn/Article/details/goescyoak.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.epnwcf.com/Article/details/gdogwbvsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fktsv.cn/Article/details/gefopqmql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.epnwcf.com/Article/details/gjzblfcvo.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.bbcook.cn/Article/details/gdqnhdojk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fktsv.cn/Article/details/gupnjjdyp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fktsv.cn/Article/details/gavlikchf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gxbbepnht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fktsv.cn/Article/details/gzpdkqyxo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gowqrduxk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.tarul.cn/Article/details/gfocmkyby.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gtexmezxw.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.tarul.cn/Article/details/gxuuvvwqt.sHtML

[F06] 删除文件
来源：http://wap.sjlbkw.cn/Article/details/gnwrrjnhq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gwhblusnu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fktsv.cn/Article/details/gibaugmqo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.yfazqb.com/Article/details/glplbhunk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/ganpbuask.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.vehdjk.com/Article/details/gxjcdgsxc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.bbcook.cn/Article/details/giydzdejk.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gnzvrwhxc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fktsv.cn/Article/details/gkjzaxaxb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.bbcook.cn/Article/details/grsqqzeak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.bbcook.cn/Article/details/gjzakzzbm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.vehdjk.com/Article/details/gdzotdwuk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.vehdjk.com/Article/details/gzalcsyxw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.sjlbkw.cn/Article/details/gcnncsjdg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.yfazqb.com/Article/details/gtocfanbt.sHtML


<!-- 参考信息 -->