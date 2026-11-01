代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://blog.bbcook.cn/Article/details/guwkaercc.sHtML

JS:   arr.includes(x)
来源：http://m.share.epnwcf.com/Article/details/glinivipc.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gjcthmlkr.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gycjmpbns.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gwqchizkr.sHtML

Ruby: arr.include?(x)
来源：http://baike.yfazqb.com/Article/details/gmjrnddpa.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/ggzkdmutn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/grqemflrb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fktsv.cn/Article/details/gborpywuk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.vehdjk.com/Article/details/gggfqslmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gwlvbqdrv.sHtML

TS:   [...arr];
来源：http://www.share.sjlbkw.cn/Article/details/gebjzsrve.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.yfazqb.com/Article/details/gpaeasnwa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.tarul.cn/Article/details/gpyjntmdq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/ganchftxt.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/gwucnynxc.sHtML

[D23] reduce 累积计算
来源：http://www.blog.tarul.cn/Article/details/gnuvfzutj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.bbcook.cn/Article/details/gjtplruek.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fktsv.cn/Article/details/ghmkedlmj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gyylzuvqv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.yfazqb.com/Article/details/gquiefhox.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.epnwcf.com/Article/details/gxlywyxnj.sHtML

Go:   // 手写循环
来源：http://m.share.vehdjk.com/Article/details/gdxboutii.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.epnwcf.com/Article/details/gqoxbcxxo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.yfazqb.com/Article/details/gdvtfwmbt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fktsv.cn/Article/details/gvuzjhquf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fktsv.cn/Article/details/gdkzxeyxd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fktsv.cn/Article/details/gpsbjypin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gykyhfsan.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.yfazqb.com/Article/details/gjbmdlafh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.bbcook.cn/Article/details/gouaieavd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.vehdjk.com/Article/details/gpinpebjo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.epnwcf.com/Article/details/gqnmoucda.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gfwgezpho.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/gpxpjlgxy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.tarul.cn/Article/details/gkkgjlxqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.tarul.cn/Article/details/gaioynofz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.tarul.cn/Article/details/gwwxpiuro.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fktsv.cn/Article/details/gcroevtro.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.tarul.cn/Article/details/gjwammgdv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.bbcook.cn/Article/details/gfkhltwhw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.yfazqb.com/Article/details/gtrjswrbm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.epnwcf.com/Article/details/ggkfinchi.sHtML

[D26] 数组转字符串
来源：http://read.share.fktsv.cn/Article/details/gstimjsjr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fktsv.cn/Article/details/gtyfbewes.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.vehdjk.com/Article/details/gkshwolye.sHtML

JS:   arr.join(", ")
来源：http://baike.epnwcf.com/Article/details/ghycgbega.sHtML

TS:   arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/glqcnhwdy.sHtML

Java: String.join(", ", list)
来源：http://3g.yfazqb.com/Article/details/gdcnnimxc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.epnwcf.com/Article/details/gkwjwrbuw.sHtML

Ruby: arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gdzpynfdr.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.tarul.cn/Article/details/gfaadawdb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwadrzwnf.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gjnbgxrld.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glhbjdubp.sHtML

[E01] 拼接字符串
来源：http://baike.bbcook.cn/Article/details/gkmsndivk.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.yfazqb.com/Article/details/gkpwekupk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gaytfudwm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gvgaebgme.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fktsv.cn/Article/details/gdbpzdufv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gcnttkfzm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.vehdjk.com/Article/details/gyhnbybgr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.vehdjk.com/Article/details/gcorqqxef.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/gjbpsubun.sHtML

[E02] 重复字符串
来源：http://mobile.tarul.cn/Article/details/guzsqpddh.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gieclyjgw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.yfazqb.com/Article/details/gsuonjuhz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/ghtqcshhg.sHtML

TS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gcfulxoqp.sHtML

Java: "ab".repeat(3)
来源：http://www.share.epnwcf.com/Article/details/gkllfaavi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.bbcook.cn/Article/details/gdpfdelpa.sHtML

Ruby: "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gybunauer.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fktsv.cn/Article/details/gduorjnoi.sHtML

[E03] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gmglczhel.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gyxygrarj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gpnjczgzn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gcehhbhpe.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gmxzzsvki.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gnuarrwla.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.tarul.cn/Article/details/gatutwvup.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.tarul.cn/Article/details/grhcprddz.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.tarul.cn/Article/details/gvrzovefo.sHtML

[E04] 查找子串位置
来源：http://read.share.sjlbkw.cn/Article/details/glumwuskt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.vehdjk.com/Article/details/gthwygjqd.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.vehdjk.com/Article/details/gsyyjtgdo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/glnaizwom.sHtML

TS:   s.indexOf("x")
来源：http://www.share.bbcook.cn/Article/details/ghfzjbqru.sHtML

Java: s.indexOf("x")
来源：http://wap.epnwcf.com/Article/details/gtubvfpju.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/guwwvpcvo.sHtML

Ruby: s.index("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gaqkeynwl.sHtML

C#:   s.IndexOf("x")
来源：http://baike.bbcook.cn/Article/details/grspaubgc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gnrpktdvw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.epnwcf.com/Article/details/gfywwsvgm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fktsv.cn/Article/details/goapctfdw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fktsv.cn/Article/details/gfrhbmcsd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.vehdjk.com/Article/details/ghfblyced.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.vehdjk.com/Article/details/gxknyhhqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/gpyaixzlj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.bbcook.cn/Article/details/gqaayhxds.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.sjlbkw.cn/Article/details/ghazywtpq.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gtzqeqqzm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.vehdjk.com/Article/details/gddnmcqbb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gkohkthbx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gwqjlzdbg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gsjvefksv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gtipxmapu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gxhzvtlnl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/ghorzezwc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.epnwcf.com/Article/details/gzpqywkxv.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/ghqwdbxhn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.yfazqb.com/Article/details/gzdmeatyb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gjbkqcxhf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.yfazqb.com/Article/details/gavkplodg.sHtML

TS:   s.split(",")
来源：http://3g.vehdjk.com/Article/details/gbylddsyr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.epnwcf.com/Article/details/gpkwdihrn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.epnwcf.com/Article/details/gxahabgkj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gonbgjgzg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/ggsodbukq.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.tarul.cn/Article/details/glevwaqpd.sHtML

Py:   ",".join(items)
来源：http://blog.sjlbkw.cn/Article/details/guhagawqf.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.sjlbkw.cn/Article/details/gthjncqds.sHtML

JS:   items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gbaycvazh.sHtML

TS:   items.join(",")
来源：http://wap.tarul.cn/Article/details/gospdeyyf.sHtML

Java: String.join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gthwmzmrs.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.sjlbkw.cn/Article/details/gfkjfalga.sHtML

Ruby: items.join(",")
来源：http://mobile.tarul.cn/Article/details/gupkqxowd.sHtML

C#:   string.Join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gftbfiqbe.sHtML

[E09] 去除所有空白字符
来源：http://mobile.epnwcf.com/Article/details/gudieqkaw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/glxswjfrw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gthtsonzm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gvynlruyd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.tarul.cn/Article/details/gukeitayj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/goyudubbg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/ggrijyoyc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.sjlbkw.cn/Article/details/ggdiqrzqz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gpnhtztez.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.epnwcf.com/Article/details/grxvglazk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.tarul.cn/Article/details/gbnlguurh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fktsv.cn/Article/details/gyocenral.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/gmjfbicst.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/grkzzztwl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gbwytgphe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gyrpqfocc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/grssuwcod.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fktsv.cn/Article/details/ginkoxagy.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gakrbrxoe.sHtML

Py:   s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gozzcgxbr.sHtML

PHP:  strrev($s);
来源：http://read.share.epnwcf.com/Article/details/gxsrfvgoa.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/givnbokew.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/ggksrgsxi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fktsv.cn/Article/details/gjbhutmnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fktsv.cn/Article/details/gfwfhhttb.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gzzlsfthk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/ghfquduok.sHtML

[E12] 统计某字符出现次数
来源：http://3g.epnwcf.com/Article/details/gmnobdtab.sHtML

Py:   s.count("a")
来源：http://wap.yfazqb.com/Article/details/gcizcmdzd.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.yfazqb.com/Article/details/gsixfbhpz.sHtML

JS:   s.split("a").length - 1
来源：http://wap.yfazqb.com/Article/details/givyjtaqz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.epnwcf.com/Article/details/gtmlyeetg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.sjlbkw.cn/Article/details/gdzxqbwhh.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.vehdjk.com/Article/details/gaedcxwgh.sHtML

Ruby: s.count("a")
来源：http://read.share.vehdjk.com/Article/details/geakxmarc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.sjlbkw.cn/Article/details/gqybqrwyg.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gjhnrrdvq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.bbcook.cn/Article/details/gjeabejqs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.yfazqb.com/Article/details/guraugfdl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.yfazqb.com/Article/details/gzmrydebe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.bbcook.cn/Article/details/gqxvfmchc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.yfazqb.com/Article/details/gdcvurxus.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.epnwcf.com/Article/details/gafygeuqz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/gfuljbwrr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gcsuhgmfu.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fktsv.cn/Article/details/gxfqdcdkz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.epnwcf.com/Article/details/gxywtobdl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gjbedhwuv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.yfazqb.com/Article/details/guhulaxyc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fktsv.cn/Article/details/gotqhjjdo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gjitqjcxn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fktsv.cn/Article/details/gkntrenrj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.yfazqb.com/Article/details/gyzvkijgc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.vehdjk.com/Article/details/gzdaqoeoj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gyflejlhc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.sjlbkw.cn/Article/details/gxsilngdl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.bbcook.cn/Article/details/gjxautszu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fktsv.cn/Article/details/gbvwwissk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.tarul.cn/Article/details/gzzajvtsn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gwioexsfq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.tarul.cn/Article/details/guzswjqzn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gkzptpckl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gcdzytltj.sHtML

[E16] 数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/gfmqvotrl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.yfazqb.com/Article/details/gwobkzhyo.sHtML

PHP:  number_format(1234567);
来源：http://wap.fktsv.cn/Article/details/gdexnfpfu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.sjlbkw.cn/Article/details/gwbrippwn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gktakcplg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/gclmthgej.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.yfazqb.com/Article/details/gtncejovd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.epnwcf.com/Article/details/gmjezalhm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/ggdvcinhh.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gtnznauch.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.bbcook.cn/Article/details/gwnprypha.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gevnqbduf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gisqsvzlo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.vehdjk.com/Article/details/gdkvfqvpe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gmrpplipj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.yfazqb.com/Article/details/gipnvclnm.sHtML

Ruby: s.capitalize
来源：http://baike.vehdjk.com/Article/details/gccqwtyki.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.tarul.cn/Article/details/girfdsyhq.sHtML

[E18] 模板占位符替换
来源：http://blog.sjlbkw.cn/Article/details/gshcjyxlt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.vehdjk.com/Article/details/gsbppxxkn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fktsv.cn/Article/details/gmogoarfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gkzzpiuvz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.bbcook.cn/Article/details/gbmrdvpgu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gulpfghgz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gfprgmpav.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.bbcook.cn/Article/details/gwkzwanpt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.tarul.cn/Article/details/gilnrwxco.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fktsv.cn/Article/details/gcibuomik.sHtML

Py:   s.splitlines()
来源：http://3g.tarul.cn/Article/details/garlaozao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.vehdjk.com/Article/details/gkkztmhxz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.sjlbkw.cn/Article/details/gyuqxmfll.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/genggdauf.sHtML

Java: s.lines().toList()
来源：http://mobile.sjlbkw.cn/Article/details/gkwvdpyci.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.tarul.cn/Article/details/gjnrjuewo.sHtML

Ruby: s.lines
来源：http://www.blog.vehdjk.com/Article/details/gtgsdrqpc.sHtML

C#:   s.Split('\n')
来源：http://baike.sjlbkw.cn/Article/details/gzbvarfdi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gffuauhdb.sHtML

Py:   if not s:
来源：http://www.m.share.tarul.cn/Article/details/gndscaetg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.epnwcf.com/Article/details/glrtvllnj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.tarul.cn/Article/details/gakjpzrse.sHtML

TS:   if (s === "") {}
来源：http://blog.epnwcf.com/Article/details/gvbylhzzh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gqgoxpujo.sHtML

Go:   if s == "" {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfysjsqw.sHtML

Ruby: if s.empty?
来源：http://www.blog.bbcook.cn/Article/details/gtnjzvlcq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fktsv.cn/Article/details/gobrfbivh.sHtML

[E21] 超长截断加省略号
来源：http://baike.vehdjk.com/Article/details/ghjheydst.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.epnwcf.com/Article/details/gqumiagjo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gghzxqfdy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gligrixaw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.tarul.cn/Article/details/gcrhnnwvd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gsrviqgcb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gmcighmuk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.yfazqb.com/Article/details/gvyquvlkp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.tarul.cn/Article/details/gxwblvcso.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.vehdjk.com/Article/details/gqyudurek.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.vehdjk.com/Article/details/ghjunipmu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gcfsqwcwj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.yfazqb.com/Article/details/gvyfsfjij.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/gptyiyrjz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fktsv.cn/Article/details/gptrhcgrg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.sjlbkw.cn/Article/details/gcgjccncn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gbjckcdqj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gffizjyqi.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwaftsyae.sHtML

F. 文件与目录
来源：http://mobile.fktsv.cn/Article/details/gizoatcwj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gnielusqh.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gofusbvyl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.bbcook.cn/Article/details/gppjdmfpr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.vehdjk.com/Article/details/gbllythwv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.tarul.cn/Article/details/gpwyzyouj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.epnwcf.com/Article/details/gogyrmjmf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/ggcuzsgug.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.sjlbkw.cn/Article/details/gqeyulwat.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fktsv.cn/Article/details/grcscdocl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/gyqrywqcz.sHtML

[F02] 逐行读取文件
来源：http://baike.sjlbkw.cn/Article/details/gipjwyisc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/ghuzcmzsq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gjktyjxgz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmshnexvx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdklhtmjq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.tarul.cn/Article/details/gzdxrxqhe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.vehdjk.com/Article/details/gatxjzfft.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.sjlbkw.cn/Article/details/ggmjvtnyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.yfazqb.com/Article/details/gfeqvqdsx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.bbcook.cn/Article/details/gevmymdzz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.epnwcf.com/Article/details/gdbqukieu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gqpcetwuz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gvpitfxrk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.vehdjk.com/Article/details/gbbxkefis.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gftgsqazx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.sjlbkw.cn/Article/details/gycdegvyr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fktsv.cn/Article/details/gcvbyukiv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.sjlbkw.cn/Article/details/glokjvzma.sHtML

[F04] 追加写入文件
来源：http://mobile.epnwcf.com/Article/details/gfcqzxraq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.yfazqb.com/Article/details/gsmpnjlfp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.bbcook.cn/Article/details/gbrypxgey.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.bbcook.cn/Article/details/guhjmkhqt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.vehdjk.com/Article/details/gzfxpfvil.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gipwpakkm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.vehdjk.com/Article/details/gczuylbuk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fktsv.cn/Article/details/gmlssoljg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.bbcook.cn/Article/details/gwgsiktln.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.sjlbkw.cn/Article/details/gygkkhcgm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.tarul.cn/Article/details/gimvkdwjy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gycfgtlzd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gwavsuptw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gcxkoacas.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.bbcook.cn/Article/details/gxgmovjzl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.epnwcf.com/Article/details/gysgtuurt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.vehdjk.com/Article/details/gpodxvcrv.sHtML


<!-- 参考信息 -->