代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.yfazqb.com/Article/details/gwovkywwn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/geiqsvxoi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fktsv.cn/Article/details/gwaqprpga.sHtML

Go:   // 手写 map[T]int
来源：http://3g.epnwcf.com/Article/details/guclzzlaf.sHtML

Ruby: arr.tally
来源：http://mobile.bbcook.cn/Article/details/gbyidtwmr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gzineqrrd.sHtML

[D21] 判断是否包含某元素
来源：http://baike.tarul.cn/Article/details/gjyooyiiq.sHtML

Py:   x in arr
来源：http://wap.bbcook.cn/Article/details/gyzqandji.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.vehdjk.com/Article/details/gjoordhel.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gxlnypkoz.sHtML

TS:   arr.includes(x)
来源：http://wap.fktsv.cn/Article/details/gavxemcjg.sHtML

Java: list.contains(x)
来源：http://www.m.share.yfazqb.com/Article/details/gsyzrwuvf.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gujseadjp.sHtML

Ruby: arr.include?(x)
来源：http://mobile.bbcook.cn/Article/details/gnzzmrkru.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.epnwcf.com/Article/details/gdgvuatrb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.vehdjk.com/Article/details/ggkmiqkys.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.vehdjk.com/Article/details/guoccaurf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/guagsykcp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.tarul.cn/Article/details/gmrhafodq.sHtML

TS:   [...arr];
来源：http://blog.vehdjk.com/Article/details/gwadswdyi.sHtML

Java: new ArrayList<>(list);
来源：http://blog.bbcook.cn/Article/details/gqsakzhwb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.tarul.cn/Article/details/gzhyumlur.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.tarul.cn/Article/details/gjzxibivp.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gkkywwlec.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gqhnnaxrg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.bbcook.cn/Article/details/gfqbblrin.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fktsv.cn/Article/details/gzvjtybps.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gyohmsfyp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.sjlbkw.cn/Article/details/gqofjpzxt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fktsv.cn/Article/details/gzcazqoif.sHtML

Go:   // 手写循环
来源：http://mobile.sjlbkw.cn/Article/details/ghriahrok.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.yfazqb.com/Article/details/gzijkfslj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.vehdjk.com/Article/details/gqyoegegr.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fktsv.cn/Article/details/gaowmhzgu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fktsv.cn/Article/details/gecejvzvo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.epnwcf.com/Article/details/gizbnkfqg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.yfazqb.com/Article/details/gwgasbszi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.bbcook.cn/Article/details/gcfjaxpzv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.epnwcf.com/Article/details/glruzxwdz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.tarul.cn/Article/details/gspgjybby.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.bbcook.cn/Article/details/gwfxeertu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.yfazqb.com/Article/details/ggmztgejq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/gkvwodqwy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fktsv.cn/Article/details/gzbdifwlk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.bbcook.cn/Article/details/gwjudrnnz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.epnwcf.com/Article/details/gvuuhvfnw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.bbcook.cn/Article/details/gxfmsoahi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.bbcook.cn/Article/details/gshdhnubq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fktsv.cn/Article/details/gjkyzkrtf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.vehdjk.com/Article/details/gidwodwxb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.yfazqb.com/Article/details/gtevmjwbe.sHtML

[D26] 数组转字符串
来源：http://www.blog.yfazqb.com/Article/details/gqqteqdjg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.sjlbkw.cn/Article/details/gahtzcmll.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gtmvvykbx.sHtML

JS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gnxsnmcjs.sHtML

TS:   arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gdpnxuvuy.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gqeggvjjd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gnpfhzfma.sHtML

Ruby: arr.join(", ")
来源：http://blog.vehdjk.com/Article/details/gmpulcdmg.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.yfazqb.com/Article/details/ghzytiiro.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gyklosnlr.sHtML

E. 字符串处理
来源：http://blog.vehdjk.com/Article/details/gtwhjylab.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gxgghmnuf.sHtML

[E01] 拼接字符串
来源：http://m.share.fktsv.cn/Article/details/gxlzlrpch.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fktsv.cn/Article/details/ghrxsyoll.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.vehdjk.com/Article/details/gixxwojni.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.yfazqb.com/Article/details/gdzvzejys.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gwxdavzbr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.bbcook.cn/Article/details/gangwmoww.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.sjlbkw.cn/Article/details/gvdjtrmpu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/glnpucpqb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gzqzmhnci.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gxtsqsbvy.sHtML

Py:   "ab" * 3
来源：http://m.share.yfazqb.com/Article/details/gzfmejyxm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.epnwcf.com/Article/details/gcemwdaoh.sHtML

JS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gtxgivzfh.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gddznxxak.sHtML

Java: "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/goqrrwsjd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.epnwcf.com/Article/details/grqivrtxw.sHtML

Ruby: "ab" * 3
来源：http://wap.yfazqb.com/Article/details/gykyqaiqv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fktsv.cn/Article/details/gvaanqxpj.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/grsdjuzxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.epnwcf.com/Article/details/guwtqthlp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/glgoxirbj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gdoemwdgj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.tarul.cn/Article/details/gmxfzssad.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/grglufhoq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.epnwcf.com/Article/details/gkrmmiion.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.tarul.cn/Article/details/grpasqvxw.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.epnwcf.com/Article/details/gzjiicnzy.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/gbvsfcksi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/grwfjztaj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.yfazqb.com/Article/details/gkyxksqyu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.sjlbkw.cn/Article/details/gahiaqqrz.sHtML

TS:   s.indexOf("x")
来源：http://baike.yfazqb.com/Article/details/gutbztzwq.sHtML

Java: s.indexOf("x")
来源：http://www.blog.vehdjk.com/Article/details/gfqhlisfs.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.vehdjk.com/Article/details/gjdwiwapz.sHtML

Ruby: s.index("x")
来源：http://read.share.vehdjk.com/Article/details/gkohetrkf.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fktsv.cn/Article/details/ghhwswymv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gpssqlgee.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.yfazqb.com/Article/details/gtjhntfqp.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.tarul.cn/Article/details/gsihnbxnc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/gxwakithr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fktsv.cn/Article/details/gjpdcaqel.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.tarul.cn/Article/details/gsrfimlqw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fktsv.cn/Article/details/gphufkmmx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.sjlbkw.cn/Article/details/guajfpihr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.yfazqb.com/Article/details/gbvbnnqol.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/gbrczzdrp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gjhladfex.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.vehdjk.com/Article/details/gjbmgssrb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gyrjjxmjx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gpmigjkqs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.vehdjk.com/Article/details/gkhuqsjuc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gmnfwoqbu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gkbiydumv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gwcjmoboh.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fktsv.cn/Article/details/gxqfbnedf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/ghheeedxe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.vehdjk.com/Article/details/gewipbfdq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fktsv.cn/Article/details/ghnwioxem.sHtML

TS:   s.split(",")
来源：http://www.share.fktsv.cn/Article/details/gogiujuul.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.epnwcf.com/Article/details/gdfgcpept.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.bbcook.cn/Article/details/gpktmqvqj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fktsv.cn/Article/details/ghvbpiqff.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.vehdjk.com/Article/details/gujaxklkb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gospyiezb.sHtML

Py:   ",".join(items)
来源：http://blog.fktsv.cn/Article/details/gqrpvcwld.sHtML

PHP:  implode(",", $items);
来源：http://blog.epnwcf.com/Article/details/gqysquwuk.sHtML

JS:   items.join(",")
来源：http://baike.vehdjk.com/Article/details/gkonnnehp.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gkrqpbazp.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gcmbqpdrm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.epnwcf.com/Article/details/gndnvtamc.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/gtcizjzeb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fktsv.cn/Article/details/gvpzxskgo.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/grhtkwsri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gqknfyemo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gfasgirru.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.sjlbkw.cn/Article/details/govjphywl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.bbcook.cn/Article/details/gdzgvuuhk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.sjlbkw.cn/Article/details/glxuszoun.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.epnwcf.com/Article/details/gybuetqyl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gktidexmz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.epnwcf.com/Article/details/gwcvgwegf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.sjlbkw.cn/Article/details/gqlffjbgp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gzjtxddaw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.yfazqb.com/Article/details/gmrvryscd.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.tarul.cn/Article/details/gtghqprth.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gwguoeeyi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gxqwasctj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/gikrbnnjg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.epnwcf.com/Article/details/gjsdxwvwp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.vehdjk.com/Article/details/gmdeiulsr.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gndrpxleq.sHtML

Py:   s[::-1]
来源：http://blog.epnwcf.com/Article/details/gsaxrltyh.sHtML

PHP:  strrev($s);
来源：http://mobile.tarul.cn/Article/details/gsmcidgbq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gmevvtdci.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ghhoawgvp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.tarul.cn/Article/details/ggwpbcmzp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.vehdjk.com/Article/details/gsaygmfde.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/grjvgxxqy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gksvxrllb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gwmvybnqd.sHtML

Py:   s.count("a")
来源：http://read.share.tarul.cn/Article/details/gvlifvjzk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.bbcook.cn/Article/details/gksxtdrcx.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.epnwcf.com/Article/details/gcxxnxivf.sHtML

TS:   s.split("a").length - 1
来源：http://blog.sjlbkw.cn/Article/details/gkqxzrnih.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.sjlbkw.cn/Article/details/gszjzeuqm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.epnwcf.com/Article/details/gtxdsbain.sHtML

Ruby: s.count("a")
来源：http://baike.epnwcf.com/Article/details/gbwhrzdlp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/grxfogmwo.sHtML

[E13] 逐字符遍历
来源：http://3g.vehdjk.com/Article/details/gsoavjslz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gldufwrzl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gqgqevlwb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gaxzzcumv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gmwandvea.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.epnwcf.com/Article/details/gypexydqi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gifqtwqkz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gvfswinle.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gkvvdaimc.sHtML

[E14] URL 编码与 Base64
来源：http://blog.sjlbkw.cn/Article/details/gfvnrtixe.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gmybvvdmm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.sjlbkw.cn/Article/details/gamveghkg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fktsv.cn/Article/details/gudvlgsos.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.epnwcf.com/Article/details/gzrfqiete.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.sjlbkw.cn/Article/details/glzovmdxc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gqksuehxf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.bbcook.cn/Article/details/gtlzlopid.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.vehdjk.com/Article/details/gpjfsqqzt.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.vehdjk.com/Article/details/gpppddxti.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.tarul.cn/Article/details/gbnlcygyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fktsv.cn/Article/details/gyfrcypmg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.epnwcf.com/Article/details/gwwvwhbug.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fktsv.cn/Article/details/gaexxqtcg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.yfazqb.com/Article/details/gxejdmgge.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fktsv.cn/Article/details/gqoqmykke.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.epnwcf.com/Article/details/gvjtjxtpk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.bbcook.cn/Article/details/goezvqbgz.sHtML

[E16] 数字千分位
来源：http://baike.fktsv.cn/Article/details/gjopjahsw.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.epnwcf.com/Article/details/grvjvwscf.sHtML

PHP:  number_format(1234567);
来源：http://3g.epnwcf.com/Article/details/gdysrhmek.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gmkzzitfc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.tarul.cn/Article/details/goiuzongr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.tarul.cn/Article/details/gdjnsoxaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.vehdjk.com/Article/details/glwpxozvl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gwdkfiedc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.vehdjk.com/Article/details/gbmjcvsjs.sHtML

[E17] 首字母大写
来源：http://blog.epnwcf.com/Article/details/gvbhctutb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/geobbjpbv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.vehdjk.com/Article/details/grluvjavj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fktsv.cn/Article/details/glxjvhhad.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.vehdjk.com/Article/details/gcewbtxzp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fktsv.cn/Article/details/gdaiogfxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.tarul.cn/Article/details/gvrtrlrvp.sHtML

Ruby: s.capitalize
来源：http://baike.epnwcf.com/Article/details/gvqgtlxst.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.bbcook.cn/Article/details/gminihtzu.sHtML

[E18] 模板占位符替换
来源：http://m.share.vehdjk.com/Article/details/gtbwvkdqm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.epnwcf.com/Article/details/gfvxijxiu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gmbfthbtx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.tarul.cn/Article/details/gbwtpeekg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.tarul.cn/Article/details/gugrjdgvs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gksijkfbd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/giortsqxv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.vehdjk.com/Article/details/gryurqvyp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.sjlbkw.cn/Article/details/gsangtfaf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.epnwcf.com/Article/details/gwlkhluxe.sHtML

Py:   s.splitlines()
来源：http://3g.fktsv.cn/Article/details/gmluxpadl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.yfazqb.com/Article/details/gfpcyvapn.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/giqcwhuij.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.vehdjk.com/Article/details/gtvwwolml.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gkdpvhqtg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.vehdjk.com/Article/details/govvbsovb.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/gguubehoo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.sjlbkw.cn/Article/details/gfsuukluh.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.vehdjk.com/Article/details/ggetrfhst.sHtML

Py:   if not s:
来源：http://read.share.bbcook.cn/Article/details/gjcjvokwj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.sjlbkw.cn/Article/details/gblaqmvjk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.tarul.cn/Article/details/gjfhgmdoj.sHtML

TS:   if (s === "") {}
来源：http://mobile.bbcook.cn/Article/details/gyseegboy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gtdaciini.sHtML

Go:   if s == "" {}
来源：http://wap.sjlbkw.cn/Article/details/gflazyarw.sHtML

Ruby: if s.empty?
来源：http://read.share.bbcook.cn/Article/details/gmebnxnbm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.bbcook.cn/Article/details/gktghniwc.sHtML

[E21] 超长截断加省略号
来源：http://blog.fktsv.cn/Article/details/gbzlcsmoa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gszyeuylb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.yfazqb.com/Article/details/grusfvdrq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.tarul.cn/Article/details/gfwgnrgnt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gcqbduvmo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gpnlrzuhz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.bbcook.cn/Article/details/gnecbfrmm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.yfazqb.com/Article/details/ggguwhbke.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/ghdxmecpw.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.tarul.cn/Article/details/gkfpwfbbg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.sjlbkw.cn/Article/details/gpzdbybpo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gfjehklow.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.vehdjk.com/Article/details/ghblbxbmp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/gdveuobxw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.yfazqb.com/Article/details/gvsswlnlk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.vehdjk.com/Article/details/ggsalqyut.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.bbcook.cn/Article/details/gcgbxlvdi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fktsv.cn/Article/details/glyazhkhk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gicgbhvhv.sHtML

F. 文件与目录
来源：http://blog.epnwcf.com/Article/details/ghqgtiswi.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbrgxydsx.sHtML

[F01] 读取整个文件
来源：http://mobile.fktsv.cn/Article/details/gprinoogr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.epnwcf.com/Article/details/gahvldpxt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/guusafmcq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.bbcook.cn/Article/details/gctlszzvd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gygsjtibv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.epnwcf.com/Article/details/girzfthoz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.vehdjk.com/Article/details/gbgpzhxxy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/gynruvgqj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gsladnacq.sHtML

[F02] 逐行读取文件
来源：http://mobile.vehdjk.com/Article/details/gawkuhqyt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.tarul.cn/Article/details/gksblutkj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fktsv.cn/Article/details/ghhgxgpby.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gbywxjzgs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.bbcook.cn/Article/details/gxhiefhlx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.bbcook.cn/Article/details/gkhgegfxk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.sjlbkw.cn/Article/details/gmtpvmmuw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.tarul.cn/Article/details/gqkmovfyu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.epnwcf.com/Article/details/gnvmtrkxo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gyhkldnfe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.sjlbkw.cn/Article/details/gjtigijnb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.yfazqb.com/Article/details/glzeurppl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/gezmpoceh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.tarul.cn/Article/details/gsdmhiocs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.sjlbkw.cn/Article/details/gdnffugjn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.yfazqb.com/Article/details/guorrjmwi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.yfazqb.com/Article/details/gqsonxood.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.yfazqb.com/Article/details/gvbcuvluw.sHtML

[F04] 追加写入文件
来源：http://www.share.yfazqb.com/Article/details/gjtjrzlcv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.sjlbkw.cn/Article/details/gtuoctdxb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.epnwcf.com/Article/details/ghdpaudyp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.sjlbkw.cn/Article/details/gxpioqxoc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.bbcook.cn/Article/details/giimwziex.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.tarul.cn/Article/details/gbcghghet.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.epnwcf.com/Article/details/gjneozemv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.yfazqb.com/Article/details/gjjwjccaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.vehdjk.com/Article/details/gvrzrjlib.sHtML


<!-- 参考信息 -->