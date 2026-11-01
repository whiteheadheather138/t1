代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.yfazqb.com/Article/details/gdudvsdqz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.tarul.cn/Article/details/gqfcweasx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.yfazqb.com/Article/details/gwmjkarap.sHtML

Go:   // 手写 map[T]int
来源：http://wap.vehdjk.com/Article/details/ghpxqnpal.sHtML

Ruby: arr.tally
来源：http://www.blog.tarul.cn/Article/details/gbjzccczg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/ghbzgshsd.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.tarul.cn/Article/details/gvsihswwz.sHtML

Py:   x in arr
来源：http://www.m.share.yfazqb.com/Article/details/gsaowgjfo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gfeslnysr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.epnwcf.com/Article/details/gtahzokjq.sHtML

TS:   arr.includes(x)
来源：http://baike.epnwcf.com/Article/details/ggcwyudxi.sHtML

Java: list.contains(x)
来源：http://mobile.sjlbkw.cn/Article/details/gehakakpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gkbokrwee.sHtML

Ruby: arr.include?(x)
来源：http://www.share.bbcook.cn/Article/details/gqbwlsxyx.sHtML

C#:   list.Contains(x)
来源：http://wap.vehdjk.com/Article/details/gnhwpvnea.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.vehdjk.com/Article/details/gkhsjmrwn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.tarul.cn/Article/details/gamprktut.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.yfazqb.com/Article/details/gvrsewjgv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gnewqyqlf.sHtML

TS:   [...arr];
来源：http://blog.bbcook.cn/Article/details/geihlulnx.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.sjlbkw.cn/Article/details/godxebthk.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.tarul.cn/Article/details/gvgkvpxgd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gjbmneurt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.tarul.cn/Article/details/gahdrxesr.sHtML

[D23] reduce 累积计算
来源：http://m.share.bbcook.cn/Article/details/gdingugkm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.bbcook.cn/Article/details/gatbsnskm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/gjjvozhll.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fktsv.cn/Article/details/gxqwkqjzs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.tarul.cn/Article/details/gxligekjf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.bbcook.cn/Article/details/gpcyqghqe.sHtML

Go:   // 手写循环
来源：http://www.share.bbcook.cn/Article/details/gnuqvlwno.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/ghkbzsajm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.bbcook.cn/Article/details/gbcxvfvrh.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.tarul.cn/Article/details/gxczareyj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.tarul.cn/Article/details/gxmuavepi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.tarul.cn/Article/details/golutfoxl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhwrodqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.vehdjk.com/Article/details/gaqqlhgbf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.bbcook.cn/Article/details/gbrtwhqje.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.bbcook.cn/Article/details/gfhgckysv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.sjlbkw.cn/Article/details/gtnqptfje.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fktsv.cn/Article/details/gemqatcdb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.yfazqb.com/Article/details/gkkxbvlaw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.vehdjk.com/Article/details/gjmfpdeer.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/gduqlmgmn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.sjlbkw.cn/Article/details/gjmuuvllb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/gzifbmcrt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.yfazqb.com/Article/details/gpkrpyrmg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/guwcgcqyb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.sjlbkw.cn/Article/details/gkidatfwh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gokcsycgg.sHtML

[D26] 数组转字符串
来源：http://www.m.share.yfazqb.com/Article/details/gtyntlhje.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.vehdjk.com/Article/details/gzkmsqtqh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gvfbqptob.sHtML

JS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gqjmxapev.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gnixclvqy.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gvlhmwdlv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.tarul.cn/Article/details/gvktvxiyh.sHtML

Ruby: arr.join(", ")
来源：http://m.share.yfazqb.com/Article/details/gubvfucam.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.yfazqb.com/Article/details/ggvlrtjsq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqyxjpubq.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gqvbfwmac.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gytggwxhx.sHtML

[E01] 拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gdnbdvyoh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.sjlbkw.cn/Article/details/guovjfucr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.epnwcf.com/Article/details/gldhosidn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.epnwcf.com/Article/details/gimkxgpdy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.bbcook.cn/Article/details/gfffloanc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.vehdjk.com/Article/details/ggmnvtvhf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.bbcook.cn/Article/details/gknycxirl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.yfazqb.com/Article/details/gxuljokpe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gxqiyrxly.sHtML

[E02] 重复字符串
来源：http://wap.tarul.cn/Article/details/gaistssmd.sHtML

Py:   "ab" * 3
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpayvgxh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.epnwcf.com/Article/details/gobzrfpgs.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gbokqtzxl.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gabmpenvz.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gktraimmp.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gffprmsno.sHtML

Ruby: "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gbeoxisit.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.epnwcf.com/Article/details/gszayeyvf.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/grbxdtitf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.tarul.cn/Article/details/gpptamgiu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gmmgvtbtd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gezxwiykc.sHtML

TS:   s.slice(1, 4)
来源：http://wap.yfazqb.com/Article/details/gxttqbcma.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gxfcrtywh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.yfazqb.com/Article/details/gwvesxhfl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.bbcook.cn/Article/details/gvlumfrqx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.bbcook.cn/Article/details/gvwtkinwk.sHtML

[E04] 查找子串位置
来源：http://baike.vehdjk.com/Article/details/gjyoafnra.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fktsv.cn/Article/details/geqygcjhz.sHtML

PHP:  strpos($s, "x");
来源：http://blog.bbcook.cn/Article/details/gosviolfh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gsgahidtw.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gozfapjdl.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/giijprkxd.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.sjlbkw.cn/Article/details/gngioewsn.sHtML

Ruby: s.index("x")
来源：http://blog.epnwcf.com/Article/details/gbzjxzykr.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gjhgvfpnq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.sjlbkw.cn/Article/details/gnjtgybrs.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gskhjhwpf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gchgnzjps.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.sjlbkw.cn/Article/details/gztdlsvjg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.tarul.cn/Article/details/gqbnykqay.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gvsmwxccd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.bbcook.cn/Article/details/gsytxesys.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.bbcook.cn/Article/details/ggthysvcb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.tarul.cn/Article/details/gxvxjqdpt.sHtML

[E06] 替换子串
来源：http://www.blog.sjlbkw.cn/Article/details/gbordpwjw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gxnbpagsd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fktsv.cn/Article/details/gdhcnwwvc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/grqkvdyec.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/goucfhliy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gwdhazksh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fktsv.cn/Article/details/glkbqtdms.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gkocgrtte.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gsfimhvok.sHtML

[E07] 按分隔符拆分
来源：http://wap.epnwcf.com/Article/details/gfdvfndll.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fktsv.cn/Article/details/gkiaxppxc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gsewsbrye.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/gfvodqito.sHtML

TS:   s.split(",")
来源：http://mobile.yfazqb.com/Article/details/gszygkmic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.sjlbkw.cn/Article/details/gmwvwaarf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gyexqaras.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fktsv.cn/Article/details/grykihapu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.epnwcf.com/Article/details/grbygbueq.sHtML

[E08] 数组按分隔符合并
来源：http://blog.bbcook.cn/Article/details/ggalnmxqz.sHtML

Py:   ",".join(items)
来源：http://m.share.fktsv.cn/Article/details/gyvmgqlfp.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gliszxpuh.sHtML

JS:   items.join(",")
来源：http://3g.tarul.cn/Article/details/gfdhuepqe.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gtzdtebto.sHtML

Java: String.join(",", items)
来源：http://www.share.tarul.cn/Article/details/gmgklnqyg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/guplrytre.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gvfalaljy.sHtML

C#:   string.Join(",", items)
来源：http://wap.sjlbkw.cn/Article/details/gdnnzyaac.sHtML

[E09] 去除所有空白字符
来源：http://wap.tarul.cn/Article/details/gwlodopke.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fktsv.cn/Article/details/gimlsfeph.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gwelrrhut.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fktsv.cn/Article/details/gexpntkqc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gqiwqfngz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gfjhpjasb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gnrbzlibn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.bbcook.cn/Article/details/gkknzrjbj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.epnwcf.com/Article/details/gjrfodath.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.vehdjk.com/Article/details/gfuuxotbh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gyoylpmin.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.vehdjk.com/Article/details/geykitdnn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gkyxwhvcz.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gpkrgzjde.sHtML

Java: String.format("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gnlcfempr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fktsv.cn/Article/details/gefuugxjs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gtpfwgbyk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.tarul.cn/Article/details/gipeunqmf.sHtML

[E11] 反转字符串
来源：http://read.share.epnwcf.com/Article/details/gsjrarvef.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/guddgzzvc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gyqwbkubr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gwprxpngg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gbzaifzca.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.vehdjk.com/Article/details/gaxnpausa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.yfazqb.com/Article/details/gcfbzcehh.sHtML

Ruby: s.reverse
来源：http://www.share.tarul.cn/Article/details/gnlcsxnjw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gaqseuzxv.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.yfazqb.com/Article/details/gnqktvhuj.sHtML

Py:   s.count("a")
来源：http://www.blog.fktsv.cn/Article/details/ggzhcucfx.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/gyflkvxbs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.sjlbkw.cn/Article/details/grdfkmcym.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.bbcook.cn/Article/details/gbcxzhdja.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gnhpabfqc.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.yfazqb.com/Article/details/ghffxwhmc.sHtML

Ruby: s.count("a")
来源：http://read.share.yfazqb.com/Article/details/gezuouiyl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.tarul.cn/Article/details/gvgcjuisv.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gjtsyuhgz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.tarul.cn/Article/details/gmoptcdnk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gqqfvhmhi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fktsv.cn/Article/details/glfwogyhj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gokkiknlz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.tarul.cn/Article/details/guiuwutnj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.vehdjk.com/Article/details/gimkjzkit.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.tarul.cn/Article/details/gqxjzhliv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fktsv.cn/Article/details/gumgnxehj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.epnwcf.com/Article/details/gtjsyohpc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.yfazqb.com/Article/details/grqulfyuw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.bbcook.cn/Article/details/gmyzclstm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/gsgwrcfhp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.vehdjk.com/Article/details/genxrotth.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gowkcerxj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gqttbhale.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fktsv.cn/Article/details/gyhoxzhxr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.bbcook.cn/Article/details/gjtyqglez.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gwumfyzqa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gpzymimve.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gedhfiqoe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gypdliray.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.tarul.cn/Article/details/guoeumsoz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.vehdjk.com/Article/details/gnuglkjnl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gjsjwifgo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fktsv.cn/Article/details/gxqzfsgup.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.vehdjk.com/Article/details/ghlesiple.sHtML

[E16] 数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gmknircbe.sHtML

Py:   f"{1234567:,}"
来源：http://3g.vehdjk.com/Article/details/gsehphlmw.sHtML

PHP:  number_format(1234567);
来源：http://wap.epnwcf.com/Article/details/gyjuqjonf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gppsaqveu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/ghubudajg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.bbcook.cn/Article/details/gsbnprxjv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.yfazqb.com/Article/details/gtongyhyd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fktsv.cn/Article/details/gabhepipy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gebhfwusx.sHtML

[E17] 首字母大写
来源：http://www.blog.epnwcf.com/Article/details/gfybyfwpr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gtxlkvqmg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fktsv.cn/Article/details/ggsvtbiud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.epnwcf.com/Article/details/goyojjbub.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.bbcook.cn/Article/details/gjqxdbqpf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.bbcook.cn/Article/details/glacaubmt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/grprmgygq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/ghmdglpdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gndcbdthh.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gipslwiog.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.tarul.cn/Article/details/gnszfmaev.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gxlvopseg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gnkufrsrh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gqicozgbv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.tarul.cn/Article/details/glrrzxcwx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gjyoioezq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.epnwcf.com/Article/details/gbwhvghnm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.sjlbkw.cn/Article/details/gppgkxmaw.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/gmhipmabv.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/gzowbeatm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/ggbuvpmgq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/ggmhpnlzb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.epnwcf.com/Article/details/gvaeexkmp.sHtML

Java: s.lines().toList()
来源：http://baike.sjlbkw.cn/Article/details/ggmjeuxbu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.sjlbkw.cn/Article/details/greqhtjgu.sHtML

Ruby: s.lines
来源：http://blog.vehdjk.com/Article/details/gttwtoher.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gatkxcrlq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.vehdjk.com/Article/details/gamqcxvqd.sHtML

Py:   if not s:
来源：http://www.share.bbcook.cn/Article/details/grovaabtl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.sjlbkw.cn/Article/details/gjfevtito.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fktsv.cn/Article/details/gjdamzdhh.sHtML

TS:   if (s === "") {}
来源：http://3g.bbcook.cn/Article/details/gelttgezh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.tarul.cn/Article/details/gkgimjoxz.sHtML

Go:   if s == "" {}
来源：http://baike.epnwcf.com/Article/details/ghtuejruk.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/giifsyasp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.epnwcf.com/Article/details/gfvceulhd.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fktsv.cn/Article/details/ghlmgpahx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gcnsseufy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.tarul.cn/Article/details/gwnvkxmip.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gjoibqomw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gufxwcjka.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/gbibosmbj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.vehdjk.com/Article/details/grbonsvwp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/ghewmpltb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gmgpgpbgg.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.yfazqb.com/Article/details/gvkdwwjcr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.sjlbkw.cn/Article/details/gjccyvaci.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gzgicvfcd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gcpumwhyp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.yfazqb.com/Article/details/gvhpntafk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gnbemjgwd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.sjlbkw.cn/Article/details/gzymixyse.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/gyuxrzcqh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fktsv.cn/Article/details/glrsaddeb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gexglpifh.sHtML

F. 文件与目录
来源：http://3g.epnwcf.com/Article/details/givlfeczq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gpjmylarb.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/gkbwguhxr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/gnfmzmllp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.epnwcf.com/Article/details/gdgrzzngr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/giaxxkisw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.tarul.cn/Article/details/ghrkuswsq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/grtzhnrod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.tarul.cn/Article/details/gluandbjl.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmnelvdh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gjrhyrzes.sHtML

[F02] 逐行读取文件
来源：http://www.share.sjlbkw.cn/Article/details/gqftydquh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrxwxoop.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/guzdairhq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.tarul.cn/Article/details/gzteibgzi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.epnwcf.com/Article/details/gmbfwpnzj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gvpdhdqhp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fktsv.cn/Article/details/gvfcvzilq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gqkjiszle.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.sjlbkw.cn/Article/details/gbholiwmz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fktsv.cn/Article/details/ggiutnmaa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.tarul.cn/Article/details/gyhwfqzru.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gcsrkklwf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gucmeufch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.bbcook.cn/Article/details/gcvbkcbph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fktsv.cn/Article/details/guijkkihv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fktsv.cn/Article/details/glydrinxh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.yfazqb.com/Article/details/giruoqthw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.tarul.cn/Article/details/ggvkojwoo.sHtML

[F04] 追加写入文件
来源：http://m.share.vehdjk.com/Article/details/gtpwhojli.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.epnwcf.com/Article/details/gyhfmciby.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gmilsjflq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fktsv.cn/Article/details/gnehfmwlu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gyhhkjpgd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.vehdjk.com/Article/details/gtdhjnult.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.vehdjk.com/Article/details/gdaehttxx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/gptoyrpre.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.yfazqb.com/Article/details/gntsrvexa.sHtML


<!-- 参考信息 -->