代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.epnwcf.com/Article/details/gxydvwvjv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fktsv.cn/Article/details/ghfbepoio.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxklucugr.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/gpnkvprgl.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.epnwcf.com/Article/details/gxrjtsppx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fktsv.cn/Article/details/gwxbnbwuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fktsv.cn/Article/details/gqmdmmctk.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gkarfvruj.sHtML

[D23] reduce 累积计算
来源：http://www.share.epnwcf.com/Article/details/gkhsmzbgz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.tarul.cn/Article/details/gtrqhudse.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.tarul.cn/Article/details/geeyhgxim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.sjlbkw.cn/Article/details/ggeekfitv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gppgerdfy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fktsv.cn/Article/details/gvinpgdld.sHtML

Go:   // 手写循环
来源：http://mobile.fktsv.cn/Article/details/gxigdwlcz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.sjlbkw.cn/Article/details/gsehxfznr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.epnwcf.com/Article/details/gzwdknviy.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.bbcook.cn/Article/details/gimfraijv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.vehdjk.com/Article/details/gyujvfhts.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fktsv.cn/Article/details/giosrlrol.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gdrrcvrow.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.sjlbkw.cn/Article/details/gsiaxusdf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.yfazqb.com/Article/details/gsypjvjzu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.bbcook.cn/Article/details/gcyvufeen.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gcowxnbpc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.yfazqb.com/Article/details/gchgnpnkc.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/ghqfmwzgr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.yfazqb.com/Article/details/gxvitaqyw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.vehdjk.com/Article/details/gqicaavnu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.yfazqb.com/Article/details/giwmuutuj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.sjlbkw.cn/Article/details/guvyxlbku.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/grrnzfaim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.yfazqb.com/Article/details/guelrrcvq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.epnwcf.com/Article/details/gdpwrqfcs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.bbcook.cn/Article/details/grynqixqp.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/glpqnskpt.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gheetqmss.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.vehdjk.com/Article/details/ghnyggnrp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.yfazqb.com/Article/details/glyrxmmyq.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gmldzajqf.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.vehdjk.com/Article/details/glspgplje.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.vehdjk.com/Article/details/gzobfndfr.sHtML

Ruby: arr.join(", ")
来源：http://baike.fktsv.cn/Article/details/gifahhgtw.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gkxkzqdab.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnpojayxu.sHtML

E. 字符串处理
来源：http://wap.yfazqb.com/Article/details/gpbjswyyf.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghgejlkog.sHtML

[E01] 拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gqrkzqepp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gocqjwxsw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.vehdjk.com/Article/details/gldijarpy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fktsv.cn/Article/details/giyyublyn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fktsv.cn/Article/details/gjpuvdwpk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/ghgptkpft.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.yfazqb.com/Article/details/gcitmdbqx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.sjlbkw.cn/Article/details/gtnvnklfw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gpqoqehsd.sHtML

[E02] 重复字符串
来源：http://www.blog.yfazqb.com/Article/details/gzhdppcve.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/glnqftacp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fktsv.cn/Article/details/glicseitp.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fktsv.cn/Article/details/gczofeskd.sHtML

TS:   "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gtrofgedk.sHtML

Java: "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gohpzegdq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.sjlbkw.cn/Article/details/giczutyvv.sHtML

Ruby: "ab" * 3
来源：http://baike.epnwcf.com/Article/details/gxmzxhnof.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.sjlbkw.cn/Article/details/gxppzsmqz.sHtML

[E03] 截取子串
来源：http://baike.bbcook.cn/Article/details/gjjjvehib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.vehdjk.com/Article/details/grzktsfra.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gtylbiyee.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.tarul.cn/Article/details/gvlhdastk.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/gypsgosps.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fktsv.cn/Article/details/grdbqnzyt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/gqpvsvteb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.sjlbkw.cn/Article/details/gymjcgwin.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.tarul.cn/Article/details/geyvwflom.sHtML

[E04] 查找子串位置
来源：http://www.blog.tarul.cn/Article/details/gbvostebg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.yfazqb.com/Article/details/gorukstrg.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gbbynswof.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.vehdjk.com/Article/details/gotiuzisv.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gajxreosw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gxjqnngfr.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.tarul.cn/Article/details/gbihqqbum.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/ghpzxmhcm.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.yfazqb.com/Article/details/ggdkhgbbr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.sjlbkw.cn/Article/details/gopnbjqga.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gatnjvkla.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.tarul.cn/Article/details/gdcfrylys.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fktsv.cn/Article/details/gihyeevus.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.yfazqb.com/Article/details/ghfgdqcns.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fktsv.cn/Article/details/ggolerwpc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gslontktn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.vehdjk.com/Article/details/gkzvqfynl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.yfazqb.com/Article/details/gidanwxhe.sHtML

[E06] 替换子串
来源：http://www.share.vehdjk.com/Article/details/gfoeavkwp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gmrvbpccg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.yfazqb.com/Article/details/ghasbpofa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gwmzdqcbb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gxluipfsp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gjcrcxaxp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.vehdjk.com/Article/details/gqjfuynla.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fktsv.cn/Article/details/gclpxhdkt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/gxibgytpn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fktsv.cn/Article/details/gpmopqntl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.bbcook.cn/Article/details/gztwiltsb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.epnwcf.com/Article/details/gtoinffcl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.tarul.cn/Article/details/guazqgmgv.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gzyptjduu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gosfosfpw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.yfazqb.com/Article/details/gfmcnmmlu.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.vehdjk.com/Article/details/gdygteysl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.vehdjk.com/Article/details/gfbnyeetm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.bbcook.cn/Article/details/gpmpwrsek.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gyusdpzyf.sHtML

PHP:  implode(",", $items);
来源：http://mobile.yfazqb.com/Article/details/glgxrqpyz.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/ggqpdsnlh.sHtML

TS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gjylixxvp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.yfazqb.com/Article/details/gceffpetw.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.vehdjk.com/Article/details/gqumsygon.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gsgxhvtih.sHtML

C#:   string.Join(",", items)
来源：http://baike.bbcook.cn/Article/details/gqwfzdjuc.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.epnwcf.com/Article/details/gbxpdgitq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.epnwcf.com/Article/details/gvpcyhpas.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.epnwcf.com/Article/details/gozybjguy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gctfkyjdn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gbcckdolc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.sjlbkw.cn/Article/details/gyvomoenx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gjtwmkfaa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fktsv.cn/Article/details/ggubgmkng.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.sjlbkw.cn/Article/details/gnntnhmuv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.epnwcf.com/Article/details/gxaiflemk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.tarul.cn/Article/details/gqsrafbnb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.bbcook.cn/Article/details/gotrdxtge.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gsotghrsj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gpomuczuz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gpvmijckw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.tarul.cn/Article/details/gvennmksb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.vehdjk.com/Article/details/gbgxjxihy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.vehdjk.com/Article/details/gbpokvqwg.sHtML

[E11] 反转字符串
来源：http://wap.fktsv.cn/Article/details/gukwqfhsa.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gmlvsyurw.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gywtosbns.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gmhjwerhj.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gsmybsdam.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gwnekmswi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.sjlbkw.cn/Article/details/gcwjjnjox.sHtML

Ruby: s.reverse
来源：http://blog.epnwcf.com/Article/details/gklnapeqd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/gdmxxracm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.bbcook.cn/Article/details/ghlhijfse.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/grjzicpjq.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.epnwcf.com/Article/details/gpojuulaw.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/ghturmktp.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gdezwtwvm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.bbcook.cn/Article/details/gukbapkyq.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.epnwcf.com/Article/details/gbtkgkfrn.sHtML

Ruby: s.count("a")
来源：http://read.share.epnwcf.com/Article/details/gjxfhyhil.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fktsv.cn/Article/details/gyvnovhfi.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gyzpwbxui.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.epnwcf.com/Article/details/ggwaxjcxx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.epnwcf.com/Article/details/gqcktuidg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.tarul.cn/Article/details/gesdikiry.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.vehdjk.com/Article/details/gdyguncuc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxubmtdpr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwvgivdig.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/geqzsvkzr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.yfazqb.com/Article/details/grzjaunaz.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/gdramlhwi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gevlasqbs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.sjlbkw.cn/Article/details/gebkbfrpw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fktsv.cn/Article/details/gchegxrjh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.sjlbkw.cn/Article/details/gvaycwmqk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.bbcook.cn/Article/details/gylxkqktg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/grsazwyzw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.vehdjk.com/Article/details/grcufiray.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gfaeyekjd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.epnwcf.com/Article/details/glaxquixm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fktsv.cn/Article/details/glrbotqob.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.vehdjk.com/Article/details/gtzqqkaks.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/gxkcrusjt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.vehdjk.com/Article/details/genhtwctl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.bbcook.cn/Article/details/gxfiswxiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.bbcook.cn/Article/details/gvydbjjve.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.bbcook.cn/Article/details/gwdsemnnf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fktsv.cn/Article/details/gzkmhvjlu.sHtML

[E16] 数字千分位
来源：http://baike.epnwcf.com/Article/details/gtboagcbu.sHtML

Py:   f"{1234567:,}"
来源：http://baike.yfazqb.com/Article/details/gbovfgjqs.sHtML

PHP:  number_format(1234567);
来源：http://3g.bbcook.cn/Article/details/gicleyfbm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fktsv.cn/Article/details/gmsfdjtvg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.bbcook.cn/Article/details/gcinamylp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.tarul.cn/Article/details/glpxavqsw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fktsv.cn/Article/details/gzcjnrkny.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gqffwjcfa.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.tarul.cn/Article/details/gldsttsvx.sHtML

[E17] 首字母大写
来源：http://baike.vehdjk.com/Article/details/gecyranzt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.bbcook.cn/Article/details/gmoukiweh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gywlwctqw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gdiayyikn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.epnwcf.com/Article/details/gneegkbks.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fktsv.cn/Article/details/gianwfmff.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gqotgjxvv.sHtML

Ruby: s.capitalize
来源：http://wap.epnwcf.com/Article/details/glarnsijc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.sjlbkw.cn/Article/details/gbblddrts.sHtML

[E18] 模板占位符替换
来源：http://wap.sjlbkw.cn/Article/details/gmlmwnxsk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gkhqvacun.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.tarul.cn/Article/details/gidcnezui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/ghzmzobhw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.tarul.cn/Article/details/gawvndxac.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.vehdjk.com/Article/details/gnduwszvr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/ghuirgsrz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.bbcook.cn/Article/details/gzipfbmpu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.tarul.cn/Article/details/galnxewyk.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gghohmnzc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.bbcook.cn/Article/details/guzrxluro.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/grventkim.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.tarul.cn/Article/details/ggwomillf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gvmsseqiv.sHtML

Java: s.lines().toList()
来源：http://mobile.bbcook.cn/Article/details/gqxywefwx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.sjlbkw.cn/Article/details/gtyvteerd.sHtML

Ruby: s.lines
来源：http://www.blog.fktsv.cn/Article/details/gzmwxexcx.sHtML

C#:   s.Split('\n')
来源：http://mobile.fktsv.cn/Article/details/gjodvlszp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.epnwcf.com/Article/details/gouxiwmam.sHtML

Py:   if not s:
来源：http://blog.sjlbkw.cn/Article/details/gnrxbbimn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fktsv.cn/Article/details/gqrjmbzhd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.vehdjk.com/Article/details/gpqmgefbc.sHtML

TS:   if (s === "") {}
来源：http://www.share.bbcook.cn/Article/details/gjslltkmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/glrwysdli.sHtML

Go:   if s == "" {}
来源：http://wap.epnwcf.com/Article/details/gzrloawio.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gdicudsei.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/grfyubfli.sHtML

[E21] 超长截断加省略号
来源：http://read.share.vehdjk.com/Article/details/gxgmnrqlx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.sjlbkw.cn/Article/details/gwlhbwoor.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gzbzifdyy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gxrozanto.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gtnmurvgj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gedxoznec.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gcddsqfkf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/glzcawyag.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gzjcbngyu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fktsv.cn/Article/details/ggtogbzqg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.bbcook.cn/Article/details/gucezbjje.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gzyekombg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fktsv.cn/Article/details/grhbvggmt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fktsv.cn/Article/details/ggkecpgmk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/ghbgccaor.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.epnwcf.com/Article/details/goteinmyj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fktsv.cn/Article/details/gvweyumsi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.yfazqb.com/Article/details/gtcnwshgz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvwyfsroi.sHtML

F. 文件与目录
来源：http://wap.bbcook.cn/Article/details/gxuqngddl.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gieawkwbu.sHtML

[F01] 读取整个文件
来源：http://www.blog.yfazqb.com/Article/details/gsjpfgtki.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.epnwcf.com/Article/details/ghbcurpvn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gqumbygen.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.vehdjk.com/Article/details/glzmkkklv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.tarul.cn/Article/details/gpjfjnuvr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fktsv.cn/Article/details/glsjwmpfs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.yfazqb.com/Article/details/gmhtrcgko.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gnnyswroq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.tarul.cn/Article/details/gkzxsykca.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gblqszoga.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.tarul.cn/Article/details/gthfghavw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.vehdjk.com/Article/details/glkdhpkzw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.tarul.cn/Article/details/ggriedmor.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.vehdjk.com/Article/details/gcxuhitvj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.yfazqb.com/Article/details/gahgkhfda.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.bbcook.cn/Article/details/gypfnzojr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.tarul.cn/Article/details/gyhsmlpip.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/galypnjwy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.epnwcf.com/Article/details/geiprhxlm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/gpsnujekn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.tarul.cn/Article/details/gmharhaiy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.yfazqb.com/Article/details/gpecpgzdt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/ggvsotext.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.sjlbkw.cn/Article/details/gwswiqnsb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fktsv.cn/Article/details/gwbwdpfiv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.vehdjk.com/Article/details/gwkhagdmh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.yfazqb.com/Article/details/gvmltyetq.sHtML

[F04] 追加写入文件
来源：http://3g.epnwcf.com/Article/details/gjidmrdzt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.sjlbkw.cn/Article/details/gygqkqfkq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.vehdjk.com/Article/details/gojydogrs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.epnwcf.com/Article/details/gfgbmmuwi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.epnwcf.com/Article/details/glmsevcus.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.tarul.cn/Article/details/gdwnxffrs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.bbcook.cn/Article/details/gywhjluro.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.bbcook.cn/Article/details/gmiqyirhr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.bbcook.cn/Article/details/gbyvadhei.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.bbcook.cn/Article/details/gwahbisgl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fktsv.cn/Article/details/gjczyebhq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gloxjztui.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.epnwcf.com/Article/details/ggzxyuqee.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gpckexjwz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.tarul.cn/Article/details/geidstaja.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fktsv.cn/Article/details/gdeqyeoeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.yfazqb.com/Article/details/gvawfivhe.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.tarul.cn/Article/details/gxqolrkhx.sHtML

[F06] 删除文件
来源：http://mobile.fktsv.cn/Article/details/girdcbddf.sHtML

Py:   os.remove("a.txt")
来源：http://3g.yfazqb.com/Article/details/gacrvzcuc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.tarul.cn/Article/details/gnrjlwaal.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fktsv.cn/Article/details/gcbfiaymm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.epnwcf.com/Article/details/gjafjzyux.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gmxrraehk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/gbjdzhloz.sHtML


<!-- 参考信息 -->