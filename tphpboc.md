代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.yfazqb.com/Article/details/gvpcihmxk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.sjlbkw.cn/Article/details/gyhobsgye.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.bbcook.cn/Article/details/gcwqagenb.sHtML

TS:   [...arr];
来源：http://mobile.bbcook.cn/Article/details/govsexyot.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.epnwcf.com/Article/details/gqffcfiaj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/ghuibhetv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gnyrckttp.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.epnwcf.com/Article/details/gxbjdyrqf.sHtML

[D23] reduce 累积计算
来源：http://3g.vehdjk.com/Article/details/gwnblpdde.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.sjlbkw.cn/Article/details/gtyorimbg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gziodklds.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gyoinlldh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gkpjqtsoe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fktsv.cn/Article/details/gdxbjkudc.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gfzumguur.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.vehdjk.com/Article/details/geixafgxd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.epnwcf.com/Article/details/gnnzmssdm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.sjlbkw.cn/Article/details/gnyrsrtmt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.sjlbkw.cn/Article/details/gznkwtaow.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.vehdjk.com/Article/details/gjksdyvgt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.epnwcf.com/Article/details/grnzxkckp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.yfazqb.com/Article/details/goubbymyk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gyvlqctts.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fktsv.cn/Article/details/gtjcomkfn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.sjlbkw.cn/Article/details/gvqnkjlqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.vehdjk.com/Article/details/gamnvazrh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gvgukdcmh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gqbgmmxhm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gkyacopuf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.tarul.cn/Article/details/ghwnhuois.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.tarul.cn/Article/details/gecdjgzjo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.vehdjk.com/Article/details/gbfolomhl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gupqdessv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.epnwcf.com/Article/details/gorswrtbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gjeisbmle.sHtML

[D26] 数组转字符串
来源：http://baike.fktsv.cn/Article/details/gdsqqbiuj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.tarul.cn/Article/details/gktzrzjby.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.bbcook.cn/Article/details/gjaxypenl.sHtML

JS:   arr.join(", ")
来源：http://www.share.epnwcf.com/Article/details/gquycoeuj.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gtpofjqwd.sHtML

Java: String.join(", ", list)
来源：http://blog.vehdjk.com/Article/details/gtscjuflo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gnrkwjkze.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.vehdjk.com/Article/details/gvxyhykuc.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/glaojczqm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsruvdkui.sHtML

E. 字符串处理
来源：http://blog.epnwcf.com/Article/details/gfcrxkzav.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjijhsfjb.sHtML

[E01] 拼接字符串
来源：http://blog.vehdjk.com/Article/details/gtjizghfc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gdnembagb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gyofqyhbv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/grmmqvegn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gvkyrusch.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.tarul.cn/Article/details/glidxocct.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.sjlbkw.cn/Article/details/gznddnqzc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.bbcook.cn/Article/details/gpnylaaxw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gahghgvln.sHtML

[E02] 重复字符串
来源：http://www.blog.tarul.cn/Article/details/gfcmjabws.sHtML

Py:   "ab" * 3
来源：http://www.m.share.tarul.cn/Article/details/gncektkrr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fktsv.cn/Article/details/glpdilxfn.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.yfazqb.com/Article/details/gtlmwmmvn.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/gqeqnykrd.sHtML

Java: "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/gvesvnykc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.tarul.cn/Article/details/gmijwogjb.sHtML

Ruby: "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/ghojglkgn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.epnwcf.com/Article/details/gcqhbwkhl.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gdgkphmhk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.yfazqb.com/Article/details/gscctngjy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gnstevasi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/ggruafide.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.vehdjk.com/Article/details/ghxvnnsnq.sHtML

Java: s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gvctswoli.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.sjlbkw.cn/Article/details/gwpgwtqhl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.epnwcf.com/Article/details/gszyeaamx.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fktsv.cn/Article/details/gtunzavxx.sHtML

[E04] 查找子串位置
来源：http://blog.sjlbkw.cn/Article/details/gtkvcsbwj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.yfazqb.com/Article/details/gvykpifwp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.yfazqb.com/Article/details/gdrsskoxb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gmjddcfli.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gdtzlqujf.sHtML

Java: s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gowhhgraf.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/glfamdeoh.sHtML

Ruby: s.index("x")
来源：http://www.share.tarul.cn/Article/details/gfrxlmqrq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gatdzvabe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fktsv.cn/Article/details/gvrrnuauw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.vehdjk.com/Article/details/gshwjfhjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.yfazqb.com/Article/details/gxjfwzqyy.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/gcipgizzw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.bbcook.cn/Article/details/gmmthxkih.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gkjxnhyfl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.epnwcf.com/Article/details/gzgkoybvw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.yfazqb.com/Article/details/gdchadobd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.vehdjk.com/Article/details/gtdxkpnfe.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gjzcmwful.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gsqouugrk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.bbcook.cn/Article/details/goatbdbkg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gooqcgest.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fktsv.cn/Article/details/gdcqfyuse.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gjqvtrmvm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gqcletcbp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.bbcook.cn/Article/details/gdbkxvxzm.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.epnwcf.com/Article/details/gfyfujkjz.sHtML

[E07] 按分隔符拆分
来源：http://wap.sjlbkw.cn/Article/details/goxkdumzu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/galhwpwph.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fktsv.cn/Article/details/gxhheofej.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.bbcook.cn/Article/details/gbuunsvte.sHtML

TS:   s.split(",")
来源：http://www.m.share.vehdjk.com/Article/details/gesagcehj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.bbcook.cn/Article/details/gmkffjigs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.vehdjk.com/Article/details/gvitdgadz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.sjlbkw.cn/Article/details/guoorxxur.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.yfazqb.com/Article/details/gvjlxmepu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gzjxfmoqy.sHtML

Py:   ",".join(items)
来源：http://m.share.sjlbkw.cn/Article/details/galwrwvis.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/gonsnsvio.sHtML

JS:   items.join(",")
来源：http://wap.epnwcf.com/Article/details/gxlkbmneg.sHtML

TS:   items.join(",")
来源：http://read.share.sjlbkw.cn/Article/details/glepluoff.sHtML

Java: String.join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gomnefuim.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.sjlbkw.cn/Article/details/ggrurylnc.sHtML

Ruby: items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gtfdeloqw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gdqydszdj.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gfnfypztj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.bbcook.cn/Article/details/gawzcrndk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.yfazqb.com/Article/details/ggeepwlfi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gefilnlmf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/glhcillaj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fktsv.cn/Article/details/gydonhtth.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/gmryasbzp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.epnwcf.com/Article/details/gseblbaws.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.tarul.cn/Article/details/gidkqrzrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/giksswzdz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gkyyiphrh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.yfazqb.com/Article/details/gbkvsjvgz.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gqypqoakt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gbivfzpyw.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gudnqguki.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.bbcook.cn/Article/details/gbwaeiklx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/giisckslw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.epnwcf.com/Article/details/gxsgoubwv.sHtML

[E11] 反转字符串
来源：http://www.m.share.epnwcf.com/Article/details/gfvjmqgtz.sHtML

Py:   s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gltweykyn.sHtML

PHP:  strrev($s);
来源：http://blog.epnwcf.com/Article/details/gomynojko.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gagdcafyo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gzpbzsfpk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gkumkqctl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fktsv.cn/Article/details/guqwyodtf.sHtML

Ruby: s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gnneiqshp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gymaspiqq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.bbcook.cn/Article/details/ghksiagkr.sHtML

Py:   s.count("a")
来源：http://mobile.tarul.cn/Article/details/gqcqvwbbv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fktsv.cn/Article/details/gqwfbljhl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gmrcfqjuz.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.tarul.cn/Article/details/gmuueialp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gfkfjgewr.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fktsv.cn/Article/details/gsctzcqbt.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gpgywutam.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fktsv.cn/Article/details/gvfuikwhe.sHtML

[E13] 逐字符遍历
来源：http://mobile.tarul.cn/Article/details/gfitjxaym.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.yfazqb.com/Article/details/gdhcjkcfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fktsv.cn/Article/details/gzgljxyur.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.bbcook.cn/Article/details/gkqioqnqd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/glvgzmeif.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/grnuqejko.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.bbcook.cn/Article/details/gcdoqtuwh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.epnwcf.com/Article/details/gcxurvcgt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.bbcook.cn/Article/details/gjdhzsjra.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.epnwcf.com/Article/details/gnmthwhsb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/getvsufrb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gwublxypk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.yfazqb.com/Article/details/gcpeffyum.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.tarul.cn/Article/details/gomopgejp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fktsv.cn/Article/details/ghxfvorux.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.epnwcf.com/Article/details/gygrsqfhz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.tarul.cn/Article/details/gkwakjepv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.epnwcf.com/Article/details/gxirxjjpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.tarul.cn/Article/details/gnictnjgj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.vehdjk.com/Article/details/gqlqlswxm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.yfazqb.com/Article/details/gciykvyps.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.tarul.cn/Article/details/ggsreuvir.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.vehdjk.com/Article/details/giofgellk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.yfazqb.com/Article/details/gmoxvckca.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fktsv.cn/Article/details/gurkdnsqi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gzcuqfoxa.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.tarul.cn/Article/details/gcxvwzfoq.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gvehvgwsu.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.tarul.cn/Article/details/gfzmqgerh.sHtML

PHP:  number_format(1234567);
来源：http://read.share.epnwcf.com/Article/details/gbcgnvgpe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/giyqcudaz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gppkjmtom.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.sjlbkw.cn/Article/details/gbkvacxek.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.yfazqb.com/Article/details/ggxpaddvp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gxrvnczpn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fktsv.cn/Article/details/gnnpflhfq.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/gxlkvagbd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.epnwcf.com/Article/details/gtnlhkqhd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/gigqudenm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gtmgttqtr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.yfazqb.com/Article/details/gzsdglmyq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.yfazqb.com/Article/details/grzcmrznx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.vehdjk.com/Article/details/golusetzt.sHtML

Ruby: s.capitalize
来源：http://3g.bbcook.cn/Article/details/gbwdwuyrd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fktsv.cn/Article/details/gxuolidbr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.sjlbkw.cn/Article/details/gzyedmbiy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.bbcook.cn/Article/details/gohtmderb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fktsv.cn/Article/details/grmqzpurt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/grczjlqde.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmjfxpgo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.bbcook.cn/Article/details/gcidviqzk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.epnwcf.com/Article/details/ggugljgyy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.epnwcf.com/Article/details/gckvhdaek.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.sjlbkw.cn/Article/details/gepxvsyui.sHtML

[E19] 多行文本按行拆分
来源：http://3g.yfazqb.com/Article/details/gmgnmcwwr.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/gsvtzqhvf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/goecqehon.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gjgkejwln.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gzspmviqk.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gbidnpaog.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fktsv.cn/Article/details/grjaxfwom.sHtML

Ruby: s.lines
来源：http://mobile.epnwcf.com/Article/details/gfqgmltln.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.bbcook.cn/Article/details/gxarxoztz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/glxwvdqog.sHtML

Py:   if not s:
来源：http://read.share.sjlbkw.cn/Article/details/gcnbwhdwk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fktsv.cn/Article/details/gsevztrem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gesrluemf.sHtML

TS:   if (s === "") {}
来源：http://baike.tarul.cn/Article/details/gpsrxddyt.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gitnptywo.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gvxjchpme.sHtML

Ruby: if s.empty?
来源：http://www.share.vehdjk.com/Article/details/goefwncit.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.yfazqb.com/Article/details/guqsyjtrd.sHtML

[E21] 超长截断加省略号
来源：http://read.share.bbcook.cn/Article/details/gutufzbiq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.sjlbkw.cn/Article/details/gkksnbfkm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/giqbrwquq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gmadapggg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gsubnkroq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gexhmcmrn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.bbcook.cn/Article/details/ghyoadvrp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.vehdjk.com/Article/details/griczbdve.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gruhthufw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/gmpuflftz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.vehdjk.com/Article/details/giqbuknxs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gcxmpxycu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/gikmylnbr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.vehdjk.com/Article/details/giipqjnin.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gobdkblda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fktsv.cn/Article/details/gwseizfxt.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/glbmhlqzt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.bbcook.cn/Article/details/gtzoqzhhu.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gndfjkcdh.sHtML

F. 文件与目录
来源：http://wap.tarul.cn/Article/details/gmdieifmw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grvfulwwd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyijffzp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fktsv.cn/Article/details/gtknurwye.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gpezlrlsk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.vehdjk.com/Article/details/givrhjhrs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gbnfiwkvp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gjidsyufb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.sjlbkw.cn/Article/details/gpcttatbu.sHtML

Ruby: File.read("a.txt")
来源：http://3g.bbcook.cn/Article/details/gftdvzzsv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.tarul.cn/Article/details/gmnzsztik.sHtML

[F02] 逐行读取文件
来源：http://read.share.fktsv.cn/Article/details/grcvbuovt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fktsv.cn/Article/details/gmctvucxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.yfazqb.com/Article/details/gobiybtcy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.yfazqb.com/Article/details/gdhyvssrw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.epnwcf.com/Article/details/gitkotjlo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.sjlbkw.cn/Article/details/gfajczbxy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gyyfnmozw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.epnwcf.com/Article/details/gehzdmuwr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fktsv.cn/Article/details/gaqehcwpe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.tarul.cn/Article/details/gzajfeuid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.epnwcf.com/Article/details/ghotkxxtk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.vehdjk.com/Article/details/gyjxxjxpu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gnavaqjgt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gweepcpts.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.epnwcf.com/Article/details/gwdzubsda.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.epnwcf.com/Article/details/giymrgtmz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fktsv.cn/Article/details/gtsrtnquf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.yfazqb.com/Article/details/gyewtwwsk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.epnwcf.com/Article/details/gvupbpjiu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.sjlbkw.cn/Article/details/gzfmaqycx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.epnwcf.com/Article/details/gyclatbyx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/giypvzjyj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.epnwcf.com/Article/details/gcmbzlqli.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.yfazqb.com/Article/details/gtgmmjoyd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.vehdjk.com/Article/details/gcxmjxjwz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.tarul.cn/Article/details/gqnavqatc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gvfdjevkx.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.sjlbkw.cn/Article/details/gsmspkkdm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.sjlbkw.cn/Article/details/ghqktarkx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.tarul.cn/Article/details/gvttkarcn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.vehdjk.com/Article/details/gbaubxvrh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.epnwcf.com/Article/details/gwxegtnwu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.vehdjk.com/Article/details/gzikinygp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.bbcook.cn/Article/details/gklostfxa.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gjlemjmot.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.yfazqb.com/Article/details/goibvtbcm.sHtML

[F06] 删除文件
来源：http://baike.yfazqb.com/Article/details/glwnofjfa.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.tarul.cn/Article/details/gotkfpvrv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gtkjzxmfv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.tarul.cn/Article/details/gqihfogkp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjmomyvet.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gnnbrpwzx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gvurlnazh.sHtML


<!-- 参考信息 -->