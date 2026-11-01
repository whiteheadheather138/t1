代发 wailian999

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gxswonskw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fktsv.cn/Article/details/gruvxacvk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.sjlbkw.cn/Article/details/gjzznfryj.sHtML

C#:   new List<int>(list);
来源：http://m.share.sjlbkw.cn/Article/details/glilstolu.sHtML

[D23] reduce 累积计算
来源：http://www.blog.yfazqb.com/Article/details/gpitwuhfs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gxfzdmtlx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.vehdjk.com/Article/details/ghbxqqxgj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.sjlbkw.cn/Article/details/giuyidequ.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.epnwcf.com/Article/details/gjgavppfy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.sjlbkw.cn/Article/details/gyseutgkx.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gwrgyeuxc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.tarul.cn/Article/details/ggylpxoav.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.tarul.cn/Article/details/gblvxzgks.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gnppzrimk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.vehdjk.com/Article/details/gmlcjahuk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.epnwcf.com/Article/details/gzithnpyv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.bbcook.cn/Article/details/ghxvovymw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.vehdjk.com/Article/details/giqxpkxix.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.epnwcf.com/Article/details/gjuwbrymc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.yfazqb.com/Article/details/gzinomtyg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fktsv.cn/Article/details/gzuqjruot.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.tarul.cn/Article/details/gtzyaqhgf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.vehdjk.com/Article/details/grdbfdhmm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.bbcook.cn/Article/details/gdhchiwun.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gpvxzlvlb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gwgbvrwhx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.bbcook.cn/Article/details/gvzcjagrv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fktsv.cn/Article/details/gupkomjds.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gksduhfju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.yfazqb.com/Article/details/gxfnahdsp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fktsv.cn/Article/details/gdpqhicnz.sHtML

[D26] 数组转字符串
来源：http://read.share.epnwcf.com/Article/details/geuffinxy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gdxzxibuh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.epnwcf.com/Article/details/glejwhutq.sHtML

JS:   arr.join(", ")
来源：http://read.share.bbcook.cn/Article/details/gvysymsvg.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gcsyevukf.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gpvyedlfr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.bbcook.cn/Article/details/gqlaryfyp.sHtML

Ruby: arr.join(", ")
来源：http://wap.yfazqb.com/Article/details/gwbhihogu.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gaqgcsjab.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggvomtacv.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/gxrhdttxo.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkvhxrcka.sHtML

[E01] 拼接字符串
来源：http://blog.fktsv.cn/Article/details/ghftdiigv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.vehdjk.com/Article/details/gvuxnhrqe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gxalewgtn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fktsv.cn/Article/details/gpuaxjtgb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gelajqlsd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.vehdjk.com/Article/details/gthxbxpuc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gypvajvkn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.vehdjk.com/Article/details/gvwsmcwhf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gzgpbnotf.sHtML

[E02] 重复字符串
来源：http://3g.yfazqb.com/Article/details/greohqwex.sHtML

Py:   "ab" * 3
来源：http://www.share.sjlbkw.cn/Article/details/gmfaucouk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gwchisblr.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gradczgih.sHtML

TS:   "ab".repeat(3)
来源：http://blog.epnwcf.com/Article/details/gdupsawfu.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/gwneokayl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.bbcook.cn/Article/details/gctrxiaxb.sHtML

Ruby: "ab" * 3
来源：http://www.blog.bbcook.cn/Article/details/ghrcausdr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fktsv.cn/Article/details/gfbptpvcg.sHtML

[E03] 截取子串
来源：http://mobile.vehdjk.com/Article/details/gzmvdarzh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fktsv.cn/Article/details/gkvywjnzq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gvrrhovuf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.epnwcf.com/Article/details/gykoxsslm.sHtML

TS:   s.slice(1, 4)
来源：http://wap.vehdjk.com/Article/details/gasmfvddp.sHtML

Java: s.substring(1, 4)
来源：http://www.share.epnwcf.com/Article/details/gyheoeiqm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/goafgswde.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gtrizvnig.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.vehdjk.com/Article/details/gjmmqnmed.sHtML

[E04] 查找子串位置
来源：http://baike.epnwcf.com/Article/details/gtzrrymwp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.tarul.cn/Article/details/gdmelntus.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.epnwcf.com/Article/details/gmvhlyzmv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.sjlbkw.cn/Article/details/gsfwknddb.sHtML

TS:   s.indexOf("x")
来源：http://blog.epnwcf.com/Article/details/gmcnoeera.sHtML

Java: s.indexOf("x")
来源：http://www.blog.tarul.cn/Article/details/gbjjjqvnq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.sjlbkw.cn/Article/details/gktdfxoxo.sHtML

Ruby: s.index("x")
来源：http://m.share.vehdjk.com/Article/details/gzwlpzihh.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.yfazqb.com/Article/details/gzcykiwif.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.bbcook.cn/Article/details/gclcujrfr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.tarul.cn/Article/details/gyxpjgpys.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gwprqzpxp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/gbrebgyim.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.yfazqb.com/Article/details/gocuzqfim.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gvfrebvgz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gkgbwdcpx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gprytasds.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.tarul.cn/Article/details/glfovgtdf.sHtML

[E06] 替换子串
来源：http://baike.epnwcf.com/Article/details/gdtifoava.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.yfazqb.com/Article/details/gwujroadi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.tarul.cn/Article/details/gkixiyoao.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.epnwcf.com/Article/details/gbkipppyu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gqyabwaji.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fktsv.cn/Article/details/gnfswdtmk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.vehdjk.com/Article/details/grfusirle.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/geqrepssq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.vehdjk.com/Article/details/gyusptbiz.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gnxqcqzah.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fktsv.cn/Article/details/gvyztnemp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fktsv.cn/Article/details/ggbtigrip.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.bbcook.cn/Article/details/gytoapryh.sHtML

TS:   s.split(",")
来源：http://read.share.yfazqb.com/Article/details/guxsulumr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.sjlbkw.cn/Article/details/ggqomubbv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.yfazqb.com/Article/details/gjyhlclct.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gtnrtmrab.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gxzvhsvxw.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/gtpjldelt.sHtML

Py:   ",".join(items)
来源：http://3g.yfazqb.com/Article/details/gfeaoqmmq.sHtML

PHP:  implode(",", $items);
来源：http://3g.vehdjk.com/Article/details/gxcmrzvef.sHtML

JS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gbbcqksvn.sHtML

TS:   items.join(",")
来源：http://blog.sjlbkw.cn/Article/details/gcbpcsfzc.sHtML

Java: String.join(",", items)
来源：http://wap.bbcook.cn/Article/details/gwlgtybxa.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/gyjehccwr.sHtML

Ruby: items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gaelampjs.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gpshepltk.sHtML

[E09] 去除所有空白字符
来源：http://m.share.epnwcf.com/Article/details/gdjmjrncd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.vehdjk.com/Article/details/grixcszyz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.bbcook.cn/Article/details/gyyvwhzje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/geflksjlm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gplbzsumc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gjgtuuzby.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.sjlbkw.cn/Article/details/gngdwydvl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fktsv.cn/Article/details/grfrndvok.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gpfkbnqun.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.tarul.cn/Article/details/ghdjvnwqd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gbaxobaqv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.epnwcf.com/Article/details/gjaqgvewv.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/gyupqbalr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gdrowpeza.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gdxrcuqbd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/gvqorcccz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.yfazqb.com/Article/details/gllufddfi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/ghyabempq.sHtML

[E11] 反转字符串
来源：http://blog.vehdjk.com/Article/details/gvxpckxbt.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gqcwfcjim.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gaoxwoujx.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gzovcqxta.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gptuviceu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.sjlbkw.cn/Article/details/gnhiyppin.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.vehdjk.com/Article/details/gkqhwmgxa.sHtML

Ruby: s.reverse
来源：http://www.blog.vehdjk.com/Article/details/glznoqlhh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gqrcxzxti.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.epnwcf.com/Article/details/gseiekeim.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gfoouiuip.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.yfazqb.com/Article/details/gjvwlqopy.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gpeglcvbc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gpealczuj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gomqxxpvn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.yfazqb.com/Article/details/gffwiwwdk.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gniunsdmc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.yfazqb.com/Article/details/gxvibneif.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.bbcook.cn/Article/details/glsqwlqkx.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.sjlbkw.cn/Article/details/gvgionjwy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/ghgdoirkp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.vehdjk.com/Article/details/gzmqkihkw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.sjlbkw.cn/Article/details/gtrhsdbmi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gytaenqso.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gdskgdjjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.vehdjk.com/Article/details/grxmwudrd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.bbcook.cn/Article/details/gyvjoemsv.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.vehdjk.com/Article/details/gfclnapcy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.tarul.cn/Article/details/gjtmgzjoc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fktsv.cn/Article/details/gssqvejca.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gcoqsodpr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.vehdjk.com/Article/details/gqkjlnhus.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fktsv.cn/Article/details/gztbghakj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.bbcook.cn/Article/details/gapzegitc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.vehdjk.com/Article/details/gfwtokubk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/glmnppqwd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/gaomtdgwr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.vehdjk.com/Article/details/gtfmsnqii.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/gfrnzlqmh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.vehdjk.com/Article/details/ghaxkocrb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.epnwcf.com/Article/details/guqobuxwy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.epnwcf.com/Article/details/gskwxlewf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.tarul.cn/Article/details/gkrinhekk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gtctjvofe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.sjlbkw.cn/Article/details/gmpstryts.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gpsnkrqso.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/gduuzrbvt.sHtML

PHP:  number_format(1234567);
来源：http://mobile.yfazqb.com/Article/details/gfcuxjbzl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.tarul.cn/Article/details/gqielfzeo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/grbbqdalh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fktsv.cn/Article/details/gadvaemam.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.bbcook.cn/Article/details/givsemqzv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.epnwcf.com/Article/details/gzellhljv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.yfazqb.com/Article/details/gycgvcnxi.sHtML

[E17] 首字母大写
来源：http://wap.yfazqb.com/Article/details/gqsltvwvy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.tarul.cn/Article/details/gtagvrgir.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gfhomubaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gktbobmdr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.epnwcf.com/Article/details/ggnieesqc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.sjlbkw.cn/Article/details/gfzrvszbl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.bbcook.cn/Article/details/gycswyluy.sHtML

Ruby: s.capitalize
来源：http://blog.fktsv.cn/Article/details/grzhhuieu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.bbcook.cn/Article/details/gvtevxunf.sHtML

[E18] 模板占位符替换
来源：http://blog.tarul.cn/Article/details/gqqkbspmh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.sjlbkw.cn/Article/details/gshzefajx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.yfazqb.com/Article/details/gssbndafo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gqmleetlx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fktsv.cn/Article/details/gplhemrbf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gusadgjtb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.tarul.cn/Article/details/gvtnhbemb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fktsv.cn/Article/details/galqcxktr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fktsv.cn/Article/details/gocqnqvfv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.sjlbkw.cn/Article/details/gqbyanmxy.sHtML

Py:   s.splitlines()
来源：http://www.blog.yfazqb.com/Article/details/goxukhtwm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.epnwcf.com/Article/details/gydfxykdr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.yfazqb.com/Article/details/gxoslaakd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.vehdjk.com/Article/details/graarlkzk.sHtML

Java: s.lines().toList()
来源：http://www.m.share.bbcook.cn/Article/details/gehqolqip.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gguguaifd.sHtML

Ruby: s.lines
来源：http://baike.epnwcf.com/Article/details/gcuveznbt.sHtML

C#:   s.Split('\n')
来源：http://www.blog.vehdjk.com/Article/details/gcedqmtrg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.tarul.cn/Article/details/gphdpzghf.sHtML

Py:   if not s:
来源：http://www.share.vehdjk.com/Article/details/goluhblxg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.vehdjk.com/Article/details/gckwnnkci.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.epnwcf.com/Article/details/gawftqroa.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqftjcobx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/glzllklfl.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gjwhishwu.sHtML

Ruby: if s.empty?
来源：http://baike.epnwcf.com/Article/details/giyadgyna.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.bbcook.cn/Article/details/gqfxahwcx.sHtML

[E21] 超长截断加省略号
来源：http://www.share.vehdjk.com/Article/details/ghdvyzuzm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gmerctlak.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/ggcotplci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.yfazqb.com/Article/details/glavqvogh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gxsayvgml.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gcyrkbtkj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.bbcook.cn/Article/details/gfsqxdtkx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbxafwad.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fktsv.cn/Article/details/gywrediha.sHtML

[E22] 字节长度与字符长度
来源：http://blog.vehdjk.com/Article/details/gkyizkmjk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gilcymhtj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gcocntvfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.yfazqb.com/Article/details/geyksxwqk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.bbcook.cn/Article/details/gzfdjhtwf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gschvdajq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fktsv.cn/Article/details/gxaapfhmn.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.tarul.cn/Article/details/gmeziebud.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.yfazqb.com/Article/details/gczsxsmfy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsnhfhwyh.sHtML

F. 文件与目录
来源：http://wap.sjlbkw.cn/Article/details/gtkmflfrn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gnubjzvva.sHtML

[F01] 读取整个文件
来源：http://read.share.epnwcf.com/Article/details/gvrodanvt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.bbcook.cn/Article/details/gyhvqkpqn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.vehdjk.com/Article/details/gxakeiusq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.epnwcf.com/Article/details/ggtvcqsfz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.yfazqb.com/Article/details/grqqrdtzu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.sjlbkw.cn/Article/details/gkozdhwcx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fktsv.cn/Article/details/gnlutmunh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gngfiilrl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.bbcook.cn/Article/details/gjfjdxxha.sHtML

[F02] 逐行读取文件
来源：http://www.blog.bbcook.cn/Article/details/gblnnclum.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fktsv.cn/Article/details/gjzpaxwae.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.tarul.cn/Article/details/givlzisid.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gzbuizpyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gfmdmnjen.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.yfazqb.com/Article/details/gcgngiahp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fktsv.cn/Article/details/gjyvpfohq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.bbcook.cn/Article/details/gdnhjvefp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.epnwcf.com/Article/details/glpykhrgg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.tarul.cn/Article/details/glnduvubm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.bbcook.cn/Article/details/gwvmdkcjw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.yfazqb.com/Article/details/gkresngsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gourvttin.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gravepxkm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.yfazqb.com/Article/details/gbdmosvfm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.bbcook.cn/Article/details/gylwbdrdb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.vehdjk.com/Article/details/gfiwbtafx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.vehdjk.com/Article/details/grzadyrji.sHtML

[F04] 追加写入文件
来源：http://www.share.bbcook.cn/Article/details/grqudrqks.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.epnwcf.com/Article/details/gqbrphceb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.epnwcf.com/Article/details/gpnpphktc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.yfazqb.com/Article/details/gxedtdzir.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.bbcook.cn/Article/details/gslrmtvbr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fktsv.cn/Article/details/gtzleqsda.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.tarul.cn/Article/details/gudktimzn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.vehdjk.com/Article/details/gtxjrbeyt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.vehdjk.com/Article/details/gbvsdjqtr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.vehdjk.com/Article/details/gztzwnjoy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.tarul.cn/Article/details/gucgxmndh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fktsv.cn/Article/details/glzwdpdlc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.bbcook.cn/Article/details/grrmihoek.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/grhyjxdfb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.yfazqb.com/Article/details/ghejvvkby.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fktsv.cn/Article/details/gegszaqgk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.tarul.cn/Article/details/gqvpocsfm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.yfazqb.com/Article/details/gyzrpbumn.sHtML

[F06] 删除文件
来源：http://read.share.fktsv.cn/Article/details/gxvdalekf.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gxxdwxrcj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gwxfrjzsg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfymglwyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.epnwcf.com/Article/details/gpzaritax.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gtkhidetk.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.epnwcf.com/Article/details/gxrzcjmuh.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.sjlbkw.cn/Article/details/gxmsboslr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.yfazqb.com/Article/details/grbkjmsyo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.bbcook.cn/Article/details/gduevqhvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.sjlbkw.cn/Article/details/gzpwylkuv.sHtML


<!-- 参考信息 -->