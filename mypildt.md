代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://mobile.tarul.cn/Article/details/gxccjiope.sHtML

Ruby: arr.include?(x)
来源：http://wap.sjlbkw.cn/Article/details/gjqlbkdfh.sHtML

C#:   list.Contains(x)
来源：http://baike.yfazqb.com/Article/details/gciswvudu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/grnswaqec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.epnwcf.com/Article/details/gpwirryce.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.tarul.cn/Article/details/guexqmroo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.vehdjk.com/Article/details/gnxctokcb.sHtML

TS:   [...arr];
来源：http://www.m.share.sjlbkw.cn/Article/details/gznpfshkz.sHtML

Java: new ArrayList<>(list);
来源：http://3g.tarul.cn/Article/details/gnfkjlabf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.yfazqb.com/Article/details/gzljlzsnu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.epnwcf.com/Article/details/grinolfun.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gbsboalol.sHtML

[D23] reduce 累积计算
来源：http://3g.fktsv.cn/Article/details/gdhifobsq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/gvzghdkhn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gyeksqapv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/grzmdfiop.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/ghfmeamsg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gneeupzye.sHtML

Go:   // 手写循环
来源：http://m.share.tarul.cn/Article/details/gedmabxmi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.sjlbkw.cn/Article/details/gaunetrey.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fktsv.cn/Article/details/gdubsdkdp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.yfazqb.com/Article/details/glnjllhvd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.vehdjk.com/Article/details/gntzozatb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.epnwcf.com/Article/details/gqvunmibd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fktsv.cn/Article/details/gfhmypwin.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/glvieaemp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.sjlbkw.cn/Article/details/gzijowcvl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gdjbpfuuu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.yfazqb.com/Article/details/grnqndiit.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.yfazqb.com/Article/details/gtuoanhsg.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.sjlbkw.cn/Article/details/gbcafntrx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.yfazqb.com/Article/details/gqrsrddjm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gxosjhdum.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gibziciug.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.bbcook.cn/Article/details/gahgwjitm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gqqenddoz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/gdohmcbkp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.bbcook.cn/Article/details/gfhxylkcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gynxzjzlc.sHtML

[D26] 数组转字符串
来源：http://blog.sjlbkw.cn/Article/details/gnwsxcmto.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gssblctdz.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.sjlbkw.cn/Article/details/gkqpxyzzw.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/glelkicgo.sHtML

TS:   arr.join(", ")
来源：http://www.blog.tarul.cn/Article/details/gfogfhkyc.sHtML

Java: String.join(", ", list)
来源：http://m.share.sjlbkw.cn/Article/details/gcepcmqna.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gpvpapfcq.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gmaajluou.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fktsv.cn/Article/details/gzymjtgnq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grtwlehbo.sHtML

E. 字符串处理
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzbvwyzq.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gsxhqglbm.sHtML

[E01] 拼接字符串
来源：http://mobile.fktsv.cn/Article/details/ggpkjcgzk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gorbtcykx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.epnwcf.com/Article/details/gzlcgtcsq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.epnwcf.com/Article/details/geptfixip.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.tarul.cn/Article/details/gvurtaqmi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.vehdjk.com/Article/details/gdknbonqr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.sjlbkw.cn/Article/details/gqhktywab.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/gizfepult.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gbsfhhhmn.sHtML

[E02] 重复字符串
来源：http://mobile.bbcook.cn/Article/details/gcihtyilq.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gzczugmsm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.vehdjk.com/Article/details/gxjoyodde.sHtML

JS:   "ab".repeat(3)
来源：http://3g.epnwcf.com/Article/details/gcpxqcpwr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gnkqcymgw.sHtML

Java: "ab".repeat(3)
来源：http://blog.vehdjk.com/Article/details/gzehfdxct.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/gjhmyflob.sHtML

Ruby: "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gbgowbbqb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gjdadtkzx.sHtML

[E03] 截取子串
来源：http://mobile.sjlbkw.cn/Article/details/gsioxskrz.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gocjsjcqg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gzvcmgjtc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/gczkgrqhd.sHtML

TS:   s.slice(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gxnwejjml.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gfqtvpwvo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.vehdjk.com/Article/details/guvtceynk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.sjlbkw.cn/Article/details/ghyvkgwzt.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.epnwcf.com/Article/details/gyfanmjqu.sHtML

[E04] 查找子串位置
来源：http://www.share.yfazqb.com/Article/details/gxaaaodxc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.vehdjk.com/Article/details/gmpozjrdw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.sjlbkw.cn/Article/details/gbxyqjwrt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.tarul.cn/Article/details/gqazwatqi.sHtML

TS:   s.indexOf("x")
来源：http://baike.bbcook.cn/Article/details/gogbiekyq.sHtML

Java: s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gzokbogux.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.yfazqb.com/Article/details/gcglrameq.sHtML

Ruby: s.index("x")
来源：http://blog.fktsv.cn/Article/details/gkejmqzgx.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gxkhqtrfc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.yfazqb.com/Article/details/gdvxchvbr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.epnwcf.com/Article/details/gufjpnnkf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.tarul.cn/Article/details/ghkpmtesm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.vehdjk.com/Article/details/gxcaxophb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.yfazqb.com/Article/details/gvguoxkeu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvlulbxz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.epnwcf.com/Article/details/gkizhfnec.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fktsv.cn/Article/details/gvsbnncpx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.vehdjk.com/Article/details/glrycbbfz.sHtML

[E06] 替换子串
来源：http://www.m.share.yfazqb.com/Article/details/gaqfcufmw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.epnwcf.com/Article/details/gpmnnhgrv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.sjlbkw.cn/Article/details/gnjnoghcs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gmpkpxynl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gskrcamxk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gybictzvu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gebtndrph.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gmsbkogeu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.epnwcf.com/Article/details/gpbphrait.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gdcoujcfk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.sjlbkw.cn/Article/details/gehdtywvx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gdlwurjjr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.bbcook.cn/Article/details/gsuvbwxzk.sHtML

TS:   s.split(",")
来源：http://www.blog.yfazqb.com/Article/details/gyttclkcs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.tarul.cn/Article/details/gqcxvounw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fktsv.cn/Article/details/gyweehmmz.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.tarul.cn/Article/details/gbkjtzlcb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.sjlbkw.cn/Article/details/gsteppxlq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.bbcook.cn/Article/details/gtiqmcsgy.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/ggtbxbwak.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fktsv.cn/Article/details/geniicxdl.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gsvchjmru.sHtML

TS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gxotcxszs.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gicvogzfa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.yfazqb.com/Article/details/gynxcplrb.sHtML

Ruby: items.join(",")
来源：http://mobile.yfazqb.com/Article/details/gqwgkkual.sHtML

C#:   string.Join(",", items)
来源：http://3g.yfazqb.com/Article/details/gctxpehyf.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/geiezmsrd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.epnwcf.com/Article/details/guieihqhn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaozmtbqs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.vehdjk.com/Article/details/gvymgnyph.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.epnwcf.com/Article/details/gaayqvrlw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.bbcook.cn/Article/details/ghgdxfkse.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.bbcook.cn/Article/details/ggnwryskj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.epnwcf.com/Article/details/gwyczrwvg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.yfazqb.com/Article/details/gprkzvcgw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.tarul.cn/Article/details/gqdladqkr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gwevlwqkl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.epnwcf.com/Article/details/gcoordpiv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gaimlxhsv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gpcmjpmxb.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gvttpdwaa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.epnwcf.com/Article/details/gvbtizifb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gxdqyqnux.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/goqdvizcn.sHtML

[E11] 反转字符串
来源：http://www.blog.epnwcf.com/Article/details/gfwrwrlyu.sHtML

Py:   s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gyadnrtjo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gxnrhoysl.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gfthwzltw.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gufkyuqni.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fktsv.cn/Article/details/geagsvxlj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.sjlbkw.cn/Article/details/gzbnvxoyi.sHtML

Ruby: s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gypaocdmz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/grgfcuiwi.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gsxrhpytc.sHtML

Py:   s.count("a")
来源：http://www.blog.yfazqb.com/Article/details/gdponijnm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/ghpfmtexi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.vehdjk.com/Article/details/gzgbkxsgz.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.bbcook.cn/Article/details/gjlodwluh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.epnwcf.com/Article/details/gzzrgzuvz.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.epnwcf.com/Article/details/ghczhlwco.sHtML

Ruby: s.count("a")
来源：http://3g.bbcook.cn/Article/details/gamsqqjlt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.yfazqb.com/Article/details/gegpsbelf.sHtML

[E13] 逐字符遍历
来源：http://mobile.vehdjk.com/Article/details/gdrvarorg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.vehdjk.com/Article/details/gognrwwzg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.yfazqb.com/Article/details/gowhebxeu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gxotwwzzo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.bbcook.cn/Article/details/gzqqadlxh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.bbcook.cn/Article/details/gyxpfbcsg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.tarul.cn/Article/details/gdfvyqniy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.tarul.cn/Article/details/gsvzwyqfr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.vehdjk.com/Article/details/ghtmzgewz.sHtML

[E14] URL 编码与 Base64
来源：http://wap.bbcook.cn/Article/details/grphycihi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.sjlbkw.cn/Article/details/gxqlhshfk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gfvgkopka.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.sjlbkw.cn/Article/details/gzmtgufno.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.epnwcf.com/Article/details/getejizbn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.tarul.cn/Article/details/grsuiiuau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fktsv.cn/Article/details/gzbxfzxil.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gxvifmjte.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.yfazqb.com/Article/details/gmphcblik.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.bbcook.cn/Article/details/gouqnvrth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/gotduitor.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.vehdjk.com/Article/details/gznyzdwlx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/ghsurfcfg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.epnwcf.com/Article/details/ghogfphqz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.bbcook.cn/Article/details/gdpopyrru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.yfazqb.com/Article/details/gunroqwwo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.tarul.cn/Article/details/gjgtuosrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.yfazqb.com/Article/details/gdmqhzjnd.sHtML

[E16] 数字千分位
来源：http://blog.tarul.cn/Article/details/ggsvphdrk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/goctxlhuc.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.epnwcf.com/Article/details/ghwvdlxoz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gigfoxtqi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/glfoyibtu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.vehdjk.com/Article/details/gkrsgcvon.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvqfjzjj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gxtktfqqa.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.yfazqb.com/Article/details/ganmfbxfv.sHtML

[E17] 首字母大写
来源：http://read.share.tarul.cn/Article/details/gmkgosrsz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.tarul.cn/Article/details/gmxmitpgb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fktsv.cn/Article/details/gjenbtoob.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fktsv.cn/Article/details/gihrfxaxl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.yfazqb.com/Article/details/giwahcfti.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.epnwcf.com/Article/details/gypebvyen.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fktsv.cn/Article/details/ghcqcsjrj.sHtML

Ruby: s.capitalize
来源：http://www.share.yfazqb.com/Article/details/gbbqmafps.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.vehdjk.com/Article/details/ghbjzzlei.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.sjlbkw.cn/Article/details/geeieofid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gkzosvrkj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gmcfzjsgh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.vehdjk.com/Article/details/gymqsgthw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gutczazzg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gpcainqwo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.sjlbkw.cn/Article/details/ghbgixyei.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.epnwcf.com/Article/details/ggckbujrc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/ghcuwjpeu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.tarul.cn/Article/details/gsvsnnzjq.sHtML

Py:   s.splitlines()
来源：http://wap.epnwcf.com/Article/details/gndhwrflc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.bbcook.cn/Article/details/gscjijbfg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/gkuxnugep.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.sjlbkw.cn/Article/details/gormhbzzc.sHtML

Java: s.lines().toList()
来源：http://read.share.yfazqb.com/Article/details/gccmumicn.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.vehdjk.com/Article/details/gdgggwwpn.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gpjgzvduc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gcqyaclui.sHtML

[E20] 判断字符串是否为空
来源：http://blog.tarul.cn/Article/details/gwuwjtfvb.sHtML

Py:   if not s:
来源：http://www.share.epnwcf.com/Article/details/gycqrqxzr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gxykqgaoc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gmqzlzfsv.sHtML

TS:   if (s === "") {}
来源：http://3g.sjlbkw.cn/Article/details/ggefwbevc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/govwecewm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.bbcook.cn/Article/details/gxfiyvbna.sHtML

Ruby: if s.empty?
来源：http://baike.bbcook.cn/Article/details/gjtbjvvnp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.sjlbkw.cn/Article/details/gypesagko.sHtML

[E21] 超长截断加省略号
来源：http://wap.tarul.cn/Article/details/gysdfijrl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.vehdjk.com/Article/details/gbwrtauqw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gzafbeted.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/ggxtfxnhe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gwoaydlsq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.tarul.cn/Article/details/glmbyipsm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.epnwcf.com/Article/details/gqzfehhht.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.sjlbkw.cn/Article/details/gxtdnhtcv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fktsv.cn/Article/details/gyfcfzegg.sHtML

[E22] 字节长度与字符长度
来源：http://wap.bbcook.cn/Article/details/gqidwwurf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.sjlbkw.cn/Article/details/gfzgyfwzb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gvlhnpomg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.tarul.cn/Article/details/gruacvvfp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gzuohukyj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.yfazqb.com/Article/details/gyualzphr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.tarul.cn/Article/details/gmorkqxhp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.tarul.cn/Article/details/ggbnqrunp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.yfazqb.com/Article/details/gfohervob.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdoflxcxo.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gxiabkyug.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjiwcynnh.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gbxmwamhe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.vehdjk.com/Article/details/gvijborvd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fktsv.cn/Article/details/gblqfytbu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/gpricvjzb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.tarul.cn/Article/details/gsfrbmdhb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.epnwcf.com/Article/details/gvbuyllhp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.sjlbkw.cn/Article/details/gofnnxghc.sHtML

Ruby: File.read("a.txt")
来源：http://baike.sjlbkw.cn/Article/details/guiosxtxg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gflvpssfi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.epnwcf.com/Article/details/gdztqxxok.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.vehdjk.com/Article/details/gvwrtozab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.tarul.cn/Article/details/ghzrdgvbu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gmlkodvdb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.vehdjk.com/Article/details/gdmwpyumf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.bbcook.cn/Article/details/gdstkcepm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.yfazqb.com/Article/details/gbpouagim.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gkeyxocpx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.vehdjk.com/Article/details/gcbnucvko.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.yfazqb.com/Article/details/gzbgnduon.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.vehdjk.com/Article/details/gruhuguzh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/gwaoqkutr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.sjlbkw.cn/Article/details/gyqduunnr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.bbcook.cn/Article/details/gczeavrqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gizuflzlm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.tarul.cn/Article/details/gyumjkynn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.bbcook.cn/Article/details/gcjuiphrg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.yfazqb.com/Article/details/gkronoqmr.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gsmrmirgk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.epnwcf.com/Article/details/ggccrgbtp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/ghajbgmwb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fktsv.cn/Article/details/giztxmbyi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.tarul.cn/Article/details/gfkamdtrt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fktsv.cn/Article/details/ghstweggd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.sjlbkw.cn/Article/details/gcfdmtytv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.sjlbkw.cn/Article/details/gfqmbrnze.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fktsv.cn/Article/details/gwoejxxwt.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.vehdjk.com/Article/details/ggehffoem.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.sjlbkw.cn/Article/details/gkitynkzn.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.vehdjk.com/Article/details/giucbmkgu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.tarul.cn/Article/details/gefozcezy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.epnwcf.com/Article/details/ghqkdciyd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/ggoeyeljs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.yfazqb.com/Article/details/gsybaenkb.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.vehdjk.com/Article/details/gpbjlpbkl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.tarul.cn/Article/details/ggmgsbibq.sHtML

[F06] 删除文件
来源：http://blog.yfazqb.com/Article/details/gpkpyfznc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.bbcook.cn/Article/details/gwrvqeohf.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gopumzugj.sHtML


<!-- 参考信息 -->