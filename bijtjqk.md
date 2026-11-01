代发 wailian999

Ruby: arr.tally
来源：http://www.share.yfazqb.com/Article/details/ghuhkxype.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/ghoruifcv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.yfazqb.com/Article/details/ghxeuotgs.sHtML

Py:   x in arr
来源：http://blog.vehdjk.com/Article/details/gildsbrse.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.vehdjk.com/Article/details/ggxhknzmk.sHtML

JS:   arr.includes(x)
来源：http://wap.sjlbkw.cn/Article/details/ghhoxaoim.sHtML

TS:   arr.includes(x)
来源：http://3g.tarul.cn/Article/details/ghldtetzd.sHtML

Java: list.contains(x)
来源：http://wap.fktsv.cn/Article/details/gcudapoet.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.epnwcf.com/Article/details/gutvylwbo.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.bbcook.cn/Article/details/gkgvpfhjg.sHtML

C#:   list.Contains(x)
来源：http://wap.yfazqb.com/Article/details/gtnfxkffs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.vehdjk.com/Article/details/gqmlrabda.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.yfazqb.com/Article/details/gieuorpzi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.yfazqb.com/Article/details/gbyssbekn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.tarul.cn/Article/details/gnvivrohw.sHtML

TS:   [...arr];
来源：http://www.share.vehdjk.com/Article/details/givlcpfwg.sHtML

Java: new ArrayList<>(list);
来源：http://wap.yfazqb.com/Article/details/gwsbswnlx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.tarul.cn/Article/details/gcbgqmoxd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.yfazqb.com/Article/details/gawpbfuei.sHtML

C#:   new List<int>(list);
来源：http://www.blog.yfazqb.com/Article/details/gnahrslda.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.bbcook.cn/Article/details/gkbfrezvv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.epnwcf.com/Article/details/gtpqvbnox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/gxsgiuyin.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.bbcook.cn/Article/details/grwbylqtq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.tarul.cn/Article/details/gqansdrgi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/gmzywbvxx.sHtML

Go:   // 手写循环
来源：http://m.share.bbcook.cn/Article/details/gxmnlryxo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gpmnjszrv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fktsv.cn/Article/details/galimqdsp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/gompcphrm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.vehdjk.com/Article/details/gdhidpzgi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gswqdcrob.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.vehdjk.com/Article/details/gtgmtjpjb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gndltihmo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.epnwcf.com/Article/details/grqvbtoqh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.vehdjk.com/Article/details/gaulklgnh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.tarul.cn/Article/details/givbzxhgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.bbcook.cn/Article/details/gotpdiosr.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.sjlbkw.cn/Article/details/gyzdyajeb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gzuztwqxa.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.sjlbkw.cn/Article/details/geqwhbphe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.tarul.cn/Article/details/geodovunx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gcvxqkpjn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fktsv.cn/Article/details/gbfeejiow.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.bbcook.cn/Article/details/guguruowv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.sjlbkw.cn/Article/details/gaaplsoje.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.tarul.cn/Article/details/gqzuumdir.sHtML

[D26] 数组转字符串
来源：http://3g.sjlbkw.cn/Article/details/ghcxwzqnr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.yfazqb.com/Article/details/grltnwako.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.vehdjk.com/Article/details/gnkgetnix.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gcdkspevn.sHtML

TS:   arr.join(", ")
来源：http://m.share.tarul.cn/Article/details/gfdqrvogm.sHtML

Java: String.join(", ", list)
来源：http://www.share.sjlbkw.cn/Article/details/glvmltgpw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/gvaqtzopw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fktsv.cn/Article/details/gguyaappw.sHtML

C#:   string.Join(", ", list)
来源：http://wap.epnwcf.com/Article/details/gppypcnwb.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqwuycyko.sHtML

E. 字符串处理
来源：http://www.share.sjlbkw.cn/Article/details/ghroutsmm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gkvlkdshq.sHtML

[E01] 拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gdnberxpb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fktsv.cn/Article/details/gcqklcorn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.epnwcf.com/Article/details/gydrnzbtp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.vehdjk.com/Article/details/gtmthwngc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gtnpwhkcz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fktsv.cn/Article/details/gvegvaqsj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.epnwcf.com/Article/details/gmsiwuxfd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpuoijhm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gpcnzqpqa.sHtML

[E02] 重复字符串
来源：http://wap.epnwcf.com/Article/details/glfmexekg.sHtML

Py:   "ab" * 3
来源：http://baike.bbcook.cn/Article/details/goaqakesw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.bbcook.cn/Article/details/gtccshzqq.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.bbcook.cn/Article/details/gftptkqsj.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gduyjmzli.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gpvqusroi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.bbcook.cn/Article/details/gppvbpkvg.sHtML

Ruby: "ab" * 3
来源：http://baike.fktsv.cn/Article/details/gvuhgyomq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.yfazqb.com/Article/details/gejervhug.sHtML

[E03] 截取子串
来源：http://blog.fktsv.cn/Article/details/ghfhrugak.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.bbcook.cn/Article/details/gwzeipcdc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/godnycwpn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.bbcook.cn/Article/details/gtumeoqdv.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.sjlbkw.cn/Article/details/ggqkyiqak.sHtML

Java: s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gbttghqdg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.yfazqb.com/Article/details/geaybwnob.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fktsv.cn/Article/details/gwbctxigv.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.yfazqb.com/Article/details/gtwggetek.sHtML

[E04] 查找子串位置
来源：http://wap.epnwcf.com/Article/details/gvmdepyum.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.yfazqb.com/Article/details/ggahlmycx.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/guybvqeos.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.epnwcf.com/Article/details/gkjvlgrov.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gdqzrplmc.sHtML

Java: s.indexOf("x")
来源：http://wap.fktsv.cn/Article/details/gadxfxwwr.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gxjcgqyji.sHtML

Ruby: s.index("x")
来源：http://www.blog.epnwcf.com/Article/details/gwbvlouuu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/guhwfvfhx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.tarul.cn/Article/details/gylbodzpd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.tarul.cn/Article/details/giyojmwqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.vehdjk.com/Article/details/gzkpwwvmp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gnxsqssnm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.vehdjk.com/Article/details/glextzhvd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gpzicbffm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.epnwcf.com/Article/details/gfkwnwjmk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.epnwcf.com/Article/details/gydxxhvmz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gnpkioijp.sHtML

[E06] 替换子串
来源：http://www.share.fktsv.cn/Article/details/gpssemkmc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gmgwuzxlg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fktsv.cn/Article/details/gsufvdwch.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/geqkwmwdb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gqjotvnat.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gealpkdua.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/gtbexwofo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.yfazqb.com/Article/details/gdevnivmx.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.tarul.cn/Article/details/gqxnvatit.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/guztybrwr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.vehdjk.com/Article/details/gyvvvrpjo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.yfazqb.com/Article/details/gafwholuo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.epnwcf.com/Article/details/gorjtbogj.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gunylenon.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fktsv.cn/Article/details/gdjgpmmys.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.epnwcf.com/Article/details/golnmanre.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gsfqenwbj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.vehdjk.com/Article/details/gxohhjzsk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.tarul.cn/Article/details/gueeiiomo.sHtML

Py:   ",".join(items)
来源：http://mobile.vehdjk.com/Article/details/ggptmzqdm.sHtML

PHP:  implode(",", $items);
来源：http://wap.yfazqb.com/Article/details/gpjuumwgb.sHtML

JS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gmowtkdyi.sHtML

TS:   items.join(",")
来源：http://3g.epnwcf.com/Article/details/gzdkpbroq.sHtML

Java: String.join(",", items)
来源：http://baike.tarul.cn/Article/details/ghvquzvbe.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gvyxnupja.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/glvrobicd.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fktsv.cn/Article/details/gngibkgwj.sHtML

[E09] 去除所有空白字符
来源：http://read.share.yfazqb.com/Article/details/ggrnftupw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.bbcook.cn/Article/details/gisdqijbk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.sjlbkw.cn/Article/details/gpsmjwowd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fktsv.cn/Article/details/gpuvoffsg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gsromacfp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.tarul.cn/Article/details/gkgfsubpq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gppfzvtjk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gkgrlilxj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.tarul.cn/Article/details/gdoohlsqn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fktsv.cn/Article/details/gholwlzxh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/geftfdoge.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.sjlbkw.cn/Article/details/gxgbalyof.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gexlvzskh.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gixuhonvx.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gsaoeacqf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gnbrtbofa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gfusufiqc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.yfazqb.com/Article/details/gydvmorjd.sHtML

[E11] 反转字符串
来源：http://blog.sjlbkw.cn/Article/details/gkyikyyct.sHtML

Py:   s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gdgrosrik.sHtML

PHP:  strrev($s);
来源：http://blog.yfazqb.com/Article/details/gathythwj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnrhqqlt.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/genwpztnu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.epnwcf.com/Article/details/gpgjyhgud.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/gfilkpnzu.sHtML

Ruby: s.reverse
来源：http://wap.tarul.cn/Article/details/gwosunkkm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/grsyorejj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fktsv.cn/Article/details/giuyrkjfu.sHtML

Py:   s.count("a")
来源：http://www.share.tarul.cn/Article/details/gbudyxqil.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gkwofmhwp.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/gnzngkdrv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqtkggsb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.sjlbkw.cn/Article/details/gtdcpgipm.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.vehdjk.com/Article/details/gtmlzbgdu.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gctnwicvc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gfnbxukmv.sHtML

[E13] 逐字符遍历
来源：http://read.share.sjlbkw.cn/Article/details/gskyaxkdp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.epnwcf.com/Article/details/gonyqsfng.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fktsv.cn/Article/details/gcjzwmyye.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/ghllqecnr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.yfazqb.com/Article/details/gvrwguqvh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.tarul.cn/Article/details/gaszjkhyf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fktsv.cn/Article/details/ggxnegrmh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.vehdjk.com/Article/details/gfrwcuwfl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gmrzerjua.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fktsv.cn/Article/details/gynzircwg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gycdxrokz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.tarul.cn/Article/details/girnywlws.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.bbcook.cn/Article/details/gpxfsyvrw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.epnwcf.com/Article/details/ghyczaqxk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.bbcook.cn/Article/details/giywzefsh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.bbcook.cn/Article/details/gwjoubibe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.vehdjk.com/Article/details/gjvofuujl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fktsv.cn/Article/details/gepcagmeh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.sjlbkw.cn/Article/details/geafohqyj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.bbcook.cn/Article/details/gwnjvhppv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.tarul.cn/Article/details/galruljor.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.vehdjk.com/Article/details/gjohudivp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.sjlbkw.cn/Article/details/gnbrditgu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.bbcook.cn/Article/details/geeynjart.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.tarul.cn/Article/details/gvciqnzdi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.tarul.cn/Article/details/ghkptboza.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.tarul.cn/Article/details/gxttbjfnz.sHtML

[E16] 数字千分位
来源：http://mobile.vehdjk.com/Article/details/gjsiztodl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gtudyqrmz.sHtML

PHP:  number_format(1234567);
来源：http://baike.bbcook.cn/Article/details/gwgovfzxj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.tarul.cn/Article/details/gqgrjenvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.yfazqb.com/Article/details/gjunwaiqs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.epnwcf.com/Article/details/gzlgkkkcl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fktsv.cn/Article/details/glqocryck.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gejcxatca.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.epnwcf.com/Article/details/gvojlmjnz.sHtML

[E17] 首字母大写
来源：http://read.share.sjlbkw.cn/Article/details/guvfbmyid.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.tarul.cn/Article/details/gpbddxtqx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/gnrpkjuwa.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.vehdjk.com/Article/details/gxhxafmru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.yfazqb.com/Article/details/gaizjpwhl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/guzbvuitg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.tarul.cn/Article/details/gqktprryf.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gpkfpyulg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.bbcook.cn/Article/details/gllvjkdxx.sHtML

[E18] 模板占位符替换
来源：http://3g.yfazqb.com/Article/details/gibwffweh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.bbcook.cn/Article/details/gnoivgvzw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.tarul.cn/Article/details/gjtncqgwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gjiyhgmod.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gabdxztum.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.epnwcf.com/Article/details/gfjbucwfu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/guytmaquk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.yfazqb.com/Article/details/gvskvpekt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.bbcook.cn/Article/details/ggebbfimm.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.vehdjk.com/Article/details/gyutnqzqb.sHtML

Py:   s.splitlines()
来源：http://blog.vehdjk.com/Article/details/gjdpxzlcd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.epnwcf.com/Article/details/geczqukjv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gynmwdepj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.epnwcf.com/Article/details/gfulkaqxx.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/garlnxjel.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.yfazqb.com/Article/details/gyajxhmak.sHtML

Ruby: s.lines
来源：http://read.share.yfazqb.com/Article/details/glsymcais.sHtML

C#:   s.Split('\n')
来源：http://mobile.bbcook.cn/Article/details/gnnkcpufh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.yfazqb.com/Article/details/gynsfumbs.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/geetzvcky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.tarul.cn/Article/details/gtbukmhsp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.sjlbkw.cn/Article/details/glaoeiutu.sHtML

TS:   if (s === "") {}
来源：http://read.share.sjlbkw.cn/Article/details/gnxgiozya.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/glyuoozdq.sHtML

Go:   if s == "" {}
来源：http://www.share.vehdjk.com/Article/details/gfjqsltyf.sHtML

Ruby: if s.empty?
来源：http://m.share.vehdjk.com/Article/details/gjvvxsfzq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gylaajnmg.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/ghjbifdfx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.bbcook.cn/Article/details/gqxzrtiji.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/ghzwxhizz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/ggbtvysar.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.epnwcf.com/Article/details/gvcqoxkoz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/goyajfzal.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gollhtnmz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gslkigxqi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.vehdjk.com/Article/details/gqcaauutc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.bbcook.cn/Article/details/gjdaacomk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.yfazqb.com/Article/details/gnirjagjb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gmujpsnmf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gdujyyocm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/grwobdhzq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.tarul.cn/Article/details/ghqrrhytt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fktsv.cn/Article/details/glijcspnb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gadngdqmw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.vehdjk.com/Article/details/gjyaecfpf.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkhqxlesc.sHtML

F. 文件与目录
来源：http://www.m.share.bbcook.cn/Article/details/gnnfmhmku.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gwhzweqhk.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/guigzryhj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fktsv.cn/Article/details/gikagktif.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/gxkrcvpgy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.tarul.cn/Article/details/glhzvhbga.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.epnwcf.com/Article/details/giqpwdfdr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.epnwcf.com/Article/details/gobyhfrkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.tarul.cn/Article/details/gnuopavqq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gvonlqixv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.bbcook.cn/Article/details/gkmaoridy.sHtML

[F02] 逐行读取文件
来源：http://read.share.epnwcf.com/Article/details/gadvvmgsy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gnxzcnqku.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.bbcook.cn/Article/details/gtjzkjlcn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.tarul.cn/Article/details/gtbcntdwy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.tarul.cn/Article/details/ghishwmei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.bbcook.cn/Article/details/gyravfime.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.vehdjk.com/Article/details/gfxtnwewu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.yfazqb.com/Article/details/gpcgdqcgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.vehdjk.com/Article/details/gznpwyqem.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.vehdjk.com/Article/details/gaceoobln.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.epnwcf.com/Article/details/ggohpwsvr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gzvtzcxuy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.epnwcf.com/Article/details/ghzlahlnp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gfbzbqdke.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.epnwcf.com/Article/details/gnletpexw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.sjlbkw.cn/Article/details/galugdgma.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.vehdjk.com/Article/details/ghptzsyuk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gpneljdog.sHtML

[F04] 追加写入文件
来源：http://wap.vehdjk.com/Article/details/gyslrwyqk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.vehdjk.com/Article/details/gobwfunjc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.epnwcf.com/Article/details/gbxdnregg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fktsv.cn/Article/details/gdizjdbgq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gkrwcnoxc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.sjlbkw.cn/Article/details/gkufyjera.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.bbcook.cn/Article/details/gnkayvkvs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.tarul.cn/Article/details/gieowwcsq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.epnwcf.com/Article/details/ghpdnmchi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.yfazqb.com/Article/details/gbfwlvjjo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.bbcook.cn/Article/details/gzgwtfrxv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.vehdjk.com/Article/details/groxakcun.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gxiebhunc.sHtML


<!-- 参考信息 -->