代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fktsv.cn/Article/details/gkqqketei.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.tarul.cn/Article/details/ggnblrgjt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.vehdjk.com/Article/details/gmkdvzdol.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/gxnpxudzh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.vehdjk.com/Article/details/gaivmwbna.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.tarul.cn/Article/details/gpxismjbx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.epnwcf.com/Article/details/gwpssbarh.sHtML

C#:   new List<int>(list);
来源：http://read.share.fktsv.cn/Article/details/gadtvvdll.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.tarul.cn/Article/details/gjpoukgbq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fktsv.cn/Article/details/gymxmcdnc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/gcadavcid.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.yfazqb.com/Article/details/glttuwqim.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fktsv.cn/Article/details/gjjksfnsu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/glokklkwf.sHtML

Go:   // 手写循环
来源：http://baike.yfazqb.com/Article/details/ggyzmbyro.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.yfazqb.com/Article/details/glaejvjga.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.yfazqb.com/Article/details/goiehmywk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.epnwcf.com/Article/details/gfhwqurio.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.vehdjk.com/Article/details/ghmpxkkiz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.sjlbkw.cn/Article/details/ghozmjpyf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fktsv.cn/Article/details/gglvyxqkh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gsocemwyk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.yfazqb.com/Article/details/gzatfdfqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.yfazqb.com/Article/details/ghatipgws.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.bbcook.cn/Article/details/gyfddjwbn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fktsv.cn/Article/details/guoraqxuf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/gkisrgtoz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.yfazqb.com/Article/details/gldzelrjz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fktsv.cn/Article/details/gzfhzgfcu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.epnwcf.com/Article/details/gyhagbisn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.vehdjk.com/Article/details/gyvmcvwja.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.bbcook.cn/Article/details/gwvvatdrx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.yfazqb.com/Article/details/ggfcgpost.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.vehdjk.com/Article/details/gxvidgzpj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/grzfxaglz.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gvyfsaftq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.epnwcf.com/Article/details/gfffyrlvj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.tarul.cn/Article/details/gjrdvwgvv.sHtML

JS:   arr.join(", ")
来源：http://read.share.yfazqb.com/Article/details/guzihomyv.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/ggkjbncvd.sHtML

Java: String.join(", ", list)
来源：http://blog.tarul.cn/Article/details/gfmsbzvka.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fktsv.cn/Article/details/gwdhzesme.sHtML

Ruby: arr.join(", ")
来源：http://3g.fktsv.cn/Article/details/gkbpmpcun.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fktsv.cn/Article/details/gphwypnjm.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gvbwclwuy.sHtML

E. 字符串处理
来源：http://baike.tarul.cn/Article/details/gfssrltld.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwvwhismn.sHtML

[E01] 拼接字符串
来源：http://wap.epnwcf.com/Article/details/gjlekaujq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/gltvjtpex.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gafwqkjfd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gouebdlvo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.bbcook.cn/Article/details/grhnzfjra.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gcnknsmgj.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.bbcook.cn/Article/details/gumpchcyg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fktsv.cn/Article/details/gyfykixzj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.sjlbkw.cn/Article/details/gcguwdisb.sHtML

[E02] 重复字符串
来源：http://wap.yfazqb.com/Article/details/guqrrnezr.sHtML

Py:   "ab" * 3
来源：http://mobile.epnwcf.com/Article/details/gdxqxrzwt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gcanepimj.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.sjlbkw.cn/Article/details/gnatgrcel.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gumkrovrk.sHtML

Java: "ab".repeat(3)
来源：http://3g.sjlbkw.cn/Article/details/ggslkynwo.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.tarul.cn/Article/details/guiomadda.sHtML

Ruby: "ab" * 3
来源：http://www.blog.epnwcf.com/Article/details/gfkwnohbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.tarul.cn/Article/details/gkwrvzujh.sHtML

[E03] 截取子串
来源：http://www.m.share.bbcook.cn/Article/details/gskvmtuvl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fktsv.cn/Article/details/gkdzyddwf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gdzlrqosp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.epnwcf.com/Article/details/gyilaclvf.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gfntwplrt.sHtML

Java: s.substring(1, 4)
来源：http://3g.epnwcf.com/Article/details/gqcjdvgrr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.bbcook.cn/Article/details/gnoxfhprq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.vehdjk.com/Article/details/ggzcgdaxw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.epnwcf.com/Article/details/gsihlnsjn.sHtML

[E04] 查找子串位置
来源：http://m.share.tarul.cn/Article/details/gmwbdiazp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/ghphgcmkk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fktsv.cn/Article/details/gaxumhgjs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.bbcook.cn/Article/details/gwrspeexv.sHtML

TS:   s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gxlggfnit.sHtML

Java: s.indexOf("x")
来源：http://wap.vehdjk.com/Article/details/gexiimqov.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.sjlbkw.cn/Article/details/gkephguua.sHtML

Ruby: s.index("x")
来源：http://blog.vehdjk.com/Article/details/gqqhbpmmp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gmsxmidsp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gszmjdpwp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.bbcook.cn/Article/details/godpbscun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.epnwcf.com/Article/details/gmrhtrbue.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gfqwxtkob.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.sjlbkw.cn/Article/details/giylucwoi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.vehdjk.com/Article/details/gykfeajdz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.vehdjk.com/Article/details/gszkrpocq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.epnwcf.com/Article/details/goaqwbcnr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.sjlbkw.cn/Article/details/ghworkgli.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/gkzuwckct.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fktsv.cn/Article/details/gdetruwaz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.vehdjk.com/Article/details/geedlcuob.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/grciyjgza.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/goycaupyl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gubstrfzm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.bbcook.cn/Article/details/gksfuunqd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gdqmtqviy.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gyhzjladh.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.vehdjk.com/Article/details/gjnqktqhc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fktsv.cn/Article/details/gpkzpvzlx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.epnwcf.com/Article/details/gnufmljza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/grxezkjpt.sHtML

TS:   s.split(",")
来源：http://read.share.vehdjk.com/Article/details/gkllsrjuq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fktsv.cn/Article/details/geplxfnvm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.vehdjk.com/Article/details/giksnblmu.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.yfazqb.com/Article/details/gqybihciu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.sjlbkw.cn/Article/details/gtbszwlds.sHtML

[E08] 数组按分隔符合并
来源：http://baike.bbcook.cn/Article/details/ghotnnwhe.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gqmecjuxg.sHtML

PHP:  implode(",", $items);
来源：http://www.share.yfazqb.com/Article/details/gcaivzwpg.sHtML

JS:   items.join(",")
来源：http://m.share.yfazqb.com/Article/details/ghnxqpgcn.sHtML

TS:   items.join(",")
来源：http://read.share.bbcook.cn/Article/details/glynlfzjq.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gpmjddvnf.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.vehdjk.com/Article/details/gszcrkzfa.sHtML

Ruby: items.join(",")
来源：http://wap.fktsv.cn/Article/details/gzaxloodb.sHtML

C#:   string.Join(",", items)
来源：http://mobile.vehdjk.com/Article/details/grsyiwiuz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/ggtuatdrh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fktsv.cn/Article/details/gpcgbjjxp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.vehdjk.com/Article/details/gxcqsbgzn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gzynknhjp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gdrcuuhlv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.yfazqb.com/Article/details/glglhixtf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.yfazqb.com/Article/details/gywxgbgnf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.bbcook.cn/Article/details/gczknmjix.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.sjlbkw.cn/Article/details/giqmmqxsj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.yfazqb.com/Article/details/gptbmbocm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.yfazqb.com/Article/details/grxlqpzbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.sjlbkw.cn/Article/details/gymhmcwdl.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gqcorhxbk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdyceuzo.sHtML

Java: String.format("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gecppjcuj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.vehdjk.com/Article/details/glqqqlqvy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.yfazqb.com/Article/details/giczytomd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.sjlbkw.cn/Article/details/geuutiubi.sHtML

[E11] 反转字符串
来源：http://baike.bbcook.cn/Article/details/gglnsddjw.sHtML

Py:   s[::-1]
来源：http://wap.yfazqb.com/Article/details/gujtzwneg.sHtML

PHP:  strrev($s);
来源：http://3g.bbcook.cn/Article/details/gcmlenvxp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gqkikulal.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/ginseksdz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.epnwcf.com/Article/details/gjreyajxx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.tarul.cn/Article/details/gjoiyvidb.sHtML

Ruby: s.reverse
来源：http://www.share.bbcook.cn/Article/details/gcwguysvm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/ggzcsfzif.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gadehlgjl.sHtML

Py:   s.count("a")
来源：http://3g.fktsv.cn/Article/details/giozrsyiv.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.yfazqb.com/Article/details/gkxkxehyf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gneaexyga.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gkdeqtrfv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.sjlbkw.cn/Article/details/gezarjjgo.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fktsv.cn/Article/details/gznpjvtgd.sHtML

Ruby: s.count("a")
来源：http://www.share.fktsv.cn/Article/details/gspctzwhi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.sjlbkw.cn/Article/details/glbwttldq.sHtML

[E13] 逐字符遍历
来源：http://www.share.bbcook.cn/Article/details/gdchredro.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.vehdjk.com/Article/details/gbhuyvpyu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/gwfqqwvzb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fktsv.cn/Article/details/gcffyzkwe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/gnfqyocbo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gcvryzyif.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.epnwcf.com/Article/details/ghfowqjrv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.vehdjk.com/Article/details/gpynxijyc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fktsv.cn/Article/details/gxxgjdsvi.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/gaqlkhacb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fktsv.cn/Article/details/gqudtkpeu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.epnwcf.com/Article/details/gurtemnci.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.yfazqb.com/Article/details/ggxrikhpo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.tarul.cn/Article/details/gaeaafjoi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.vehdjk.com/Article/details/gvkztfhgy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.epnwcf.com/Article/details/gfyvfacmw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.vehdjk.com/Article/details/gixqyxfvh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.epnwcf.com/Article/details/gpqcmtrru.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fktsv.cn/Article/details/geooqdtal.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.vehdjk.com/Article/details/gzdrusrep.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/ghxudhxki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.epnwcf.com/Article/details/gryubntfx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.sjlbkw.cn/Article/details/gvjkbxhwb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.tarul.cn/Article/details/gkvgjlrlp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.yfazqb.com/Article/details/golqlebwf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.bbcook.cn/Article/details/gbgxnyapy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.yfazqb.com/Article/details/glijnniyu.sHtML

[E16] 数字千分位
来源：http://blog.yfazqb.com/Article/details/gqhsduyks.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.vehdjk.com/Article/details/gryplnznc.sHtML

PHP:  number_format(1234567);
来源：http://www.share.yfazqb.com/Article/details/goyfnakcn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gjcxgoclo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.tarul.cn/Article/details/gdnmhwyor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/gzjfwxhed.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/guwiumdgp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.vehdjk.com/Article/details/ggcdbwbqv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.yfazqb.com/Article/details/guhfjhzaj.sHtML

[E17] 首字母大写
来源：http://wap.bbcook.cn/Article/details/gqxybflii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.bbcook.cn/Article/details/gwigrzqcc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fktsv.cn/Article/details/govolmgtk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.tarul.cn/Article/details/gudxfgngz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.epnwcf.com/Article/details/gwgrrwdtb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.yfazqb.com/Article/details/gekzcqhty.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/goxoshekg.sHtML

Ruby: s.capitalize
来源：http://read.share.bbcook.cn/Article/details/gfiopdmff.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fktsv.cn/Article/details/gxqkqeoox.sHtML

[E18] 模板占位符替换
来源：http://mobile.epnwcf.com/Article/details/gwytaccoj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.sjlbkw.cn/Article/details/gbvxopfdf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fktsv.cn/Article/details/gtdshfejq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gtzxvkups.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.bbcook.cn/Article/details/gqdfgiwua.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.vehdjk.com/Article/details/gxajjfquj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gfhllkzdl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fktsv.cn/Article/details/gwobvhexz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.tarul.cn/Article/details/gxbbonmhy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.yfazqb.com/Article/details/gkxvgzlsj.sHtML

Py:   s.splitlines()
来源：http://m.share.tarul.cn/Article/details/gstfdfszn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fktsv.cn/Article/details/gdubgwyhd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.sjlbkw.cn/Article/details/gfuofkyxj.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.yfazqb.com/Article/details/gcmsadflh.sHtML

Java: s.lines().toList()
来源：http://blog.fktsv.cn/Article/details/gepanygpn.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gsameocgn.sHtML

Ruby: s.lines
来源：http://blog.sjlbkw.cn/Article/details/gyoqbiwsc.sHtML

C#:   s.Split('\n')
来源：http://blog.yfazqb.com/Article/details/gpdixcjvd.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.tarul.cn/Article/details/gktqfrcek.sHtML

Py:   if not s:
来源：http://www.m.share.sjlbkw.cn/Article/details/ghesxtxlc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.sjlbkw.cn/Article/details/gowyvpszw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fktsv.cn/Article/details/gcjnialdh.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gsndrfzee.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/ghfpaepcs.sHtML

Go:   if s == "" {}
来源：http://m.share.sjlbkw.cn/Article/details/ggzxtlnpu.sHtML

Ruby: if s.empty?
来源：http://www.m.share.sjlbkw.cn/Article/details/gpavidtvd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.epnwcf.com/Article/details/gdbmmxmyz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.yfazqb.com/Article/details/gnxkapjzv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.vehdjk.com/Article/details/ghjrvlupe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gxhajqabv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gaqgdaqpm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.tarul.cn/Article/details/gtymhogsi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.epnwcf.com/Article/details/gsuzikjxb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/gvjftrpsq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gdfmtwokf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/gjtikwjhe.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gdidgdzer.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.yfazqb.com/Article/details/gmrbkwitk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gkyfstuir.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.tarul.cn/Article/details/gqgtpuowz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fktsv.cn/Article/details/geqtiixrv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/goaenybzj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gznvapmee.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.sjlbkw.cn/Article/details/gjbkyzpod.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gabfdyrhz.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/goptptaul.sHtML

F. 文件与目录
来源：http://www.blog.tarul.cn/Article/details/gzcbehouf.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/guvbponps.sHtML

[F01] 读取整个文件
来源：http://www.blog.epnwcf.com/Article/details/gorsvjdmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.vehdjk.com/Article/details/grjvqahrw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.sjlbkw.cn/Article/details/grctufmft.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.epnwcf.com/Article/details/gwxckavzy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gpsgvjsln.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.yfazqb.com/Article/details/gsluyfmpu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.epnwcf.com/Article/details/gmqgdivvi.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.yfazqb.com/Article/details/gmichhmvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/ghpttvndo.sHtML

[F02] 逐行读取文件
来源：http://baike.fktsv.cn/Article/details/gkdjjrhgb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.epnwcf.com/Article/details/giqmeraxa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.yfazqb.com/Article/details/gobzlbzax.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.yfazqb.com/Article/details/gzpdcdjil.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/gowwvgivk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.yfazqb.com/Article/details/gezjcvcku.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gkhbjphev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.sjlbkw.cn/Article/details/gykhekhlp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.vehdjk.com/Article/details/gkkscnlio.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.bbcook.cn/Article/details/ghrxvtpoe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.epnwcf.com/Article/details/ghwnbbekm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gfgrqhpqi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gpzfavpzv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.vehdjk.com/Article/details/gyvlzvvbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.tarul.cn/Article/details/gczvawcut.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.sjlbkw.cn/Article/details/gwpvgsprq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.yfazqb.com/Article/details/gwkexljkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.epnwcf.com/Article/details/gnjtwqkzs.sHtML

[F04] 追加写入文件
来源：http://wap.epnwcf.com/Article/details/gkdlwaiuu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.yfazqb.com/Article/details/gyiykhnbu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.sjlbkw.cn/Article/details/gkzihetue.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.tarul.cn/Article/details/gbykbkldt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.yfazqb.com/Article/details/gmkvfsqmk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.yfazqb.com/Article/details/gzsmuwzsv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.tarul.cn/Article/details/gcqqpvtly.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.tarul.cn/Article/details/gggpbjqih.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.epnwcf.com/Article/details/gdanarbzt.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.epnwcf.com/Article/details/gtoqoczru.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.sjlbkw.cn/Article/details/gviqfnouf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.epnwcf.com/Article/details/gcxxcayit.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.bbcook.cn/Article/details/gzmxdabew.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.bbcook.cn/Article/details/gupupxgur.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.bbcook.cn/Article/details/gajchtbon.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.sjlbkw.cn/Article/details/gycwqzore.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.epnwcf.com/Article/details/guzxyjpyy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.tarul.cn/Article/details/gjnxelzxk.sHtML

[F06] 删除文件
来源：http://wap.fktsv.cn/Article/details/gxndshkla.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.bbcook.cn/Article/details/guhypldyf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/ggfvgdxqz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.sjlbkw.cn/Article/details/ghcyefqrb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.bbcook.cn/Article/details/gzaogmxww.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.yfazqb.com/Article/details/guhkebmas.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.yfazqb.com/Article/details/gxkxssncb.sHtML


<!-- 参考信息 -->