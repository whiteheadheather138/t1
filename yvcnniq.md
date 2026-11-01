代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.sjlbkw.cn/Article/details/gntenpirb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.vehdjk.com/Article/details/gihmdyvjb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gjxncfmab.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.bbcook.cn/Article/details/gpjvjidyl.sHtML

Ruby: arr.tally
来源：http://www.blog.bbcook.cn/Article/details/gbjslmxpe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gearhccfk.sHtML

[D21] 判断是否包含某元素
来源：http://blog.yfazqb.com/Article/details/gwbeokeob.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gqbmsyksi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.tarul.cn/Article/details/glemyyizh.sHtML

JS:   arr.includes(x)
来源：http://www.share.tarul.cn/Article/details/gsgdgwmyk.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gjnvsnpns.sHtML

Java: list.contains(x)
来源：http://www.blog.bbcook.cn/Article/details/gfguvduur.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fktsv.cn/Article/details/goxbwbttp.sHtML

Ruby: arr.include?(x)
来源：http://wap.vehdjk.com/Article/details/gnvymebzp.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gawcslxml.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.epnwcf.com/Article/details/gckiufqvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.sjlbkw.cn/Article/details/glwccjeod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.tarul.cn/Article/details/gpbpwxita.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.vehdjk.com/Article/details/gcedwkznk.sHtML

TS:   [...arr];
来源：http://www.share.tarul.cn/Article/details/gfwftqwjq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.epnwcf.com/Article/details/gtflepksn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.yfazqb.com/Article/details/ghsparzcw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.tarul.cn/Article/details/gmdkterdw.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gztsjuhpw.sHtML

[D23] reduce 累积计算
来源：http://3g.bbcook.cn/Article/details/grddzqywb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.tarul.cn/Article/details/gmfzysfox.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fktsv.cn/Article/details/gsevtldrc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.tarul.cn/Article/details/gyggofclh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/gzbvzmicw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.sjlbkw.cn/Article/details/gwhtfnsdi.sHtML

Go:   // 手写循环
来源：http://www.share.sjlbkw.cn/Article/details/gbetcdnfz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.vehdjk.com/Article/details/gjjmdodfq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.epnwcf.com/Article/details/gegsfewmv.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fktsv.cn/Article/details/gomashbwc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.sjlbkw.cn/Article/details/gguksfjkf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.vehdjk.com/Article/details/gkmspqwoz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.yfazqb.com/Article/details/gqrsmnert.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gvvnksmvv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.bbcook.cn/Article/details/glimdyggk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.yfazqb.com/Article/details/girpycafa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.tarul.cn/Article/details/gsxmpnnsg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.yfazqb.com/Article/details/goctjtrzd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.vehdjk.com/Article/details/gkkglbvxh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fktsv.cn/Article/details/gwqbqxxjy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.bbcook.cn/Article/details/guwsnwvns.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gwzvtdtse.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.epnwcf.com/Article/details/gnufwdqwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.yfazqb.com/Article/details/gybaaalug.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.epnwcf.com/Article/details/ghsunqdbx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.bbcook.cn/Article/details/gnvumdqlk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.yfazqb.com/Article/details/gxcmbdxdh.sHtML

[D26] 数组转字符串
来源：http://www.blog.bbcook.cn/Article/details/gmqjnydvp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.epnwcf.com/Article/details/guhtjsewd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.tarul.cn/Article/details/gpppckvly.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/grwzkwimx.sHtML

TS:   arr.join(", ")
来源：http://baike.yfazqb.com/Article/details/gpdcqxaeo.sHtML

Java: String.join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gemkwkakd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.yfazqb.com/Article/details/gljtzkahb.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/giwvdbtbp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gpoqudfxu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ghsxqwkvf.sHtML

E. 字符串处理
来源：http://3g.fktsv.cn/Article/details/gtxzuqrjd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gokxopobd.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gsylecqek.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.sjlbkw.cn/Article/details/ggauvhzxe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fktsv.cn/Article/details/gmcrcqeur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gnkgdgehm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gzmithalr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gjnoafssm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.yfazqb.com/Article/details/ggzntwpxd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.yfazqb.com/Article/details/goaaocmco.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/gtyjqtrtj.sHtML

[E02] 重复字符串
来源：http://wap.vehdjk.com/Article/details/gumkczrwp.sHtML

Py:   "ab" * 3
来源：http://www.blog.vehdjk.com/Article/details/gaqzadypu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.epnwcf.com/Article/details/guzbtkepv.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gscyzjbsy.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.bbcook.cn/Article/details/gjfswjust.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.tarul.cn/Article/details/gqzhoates.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.epnwcf.com/Article/details/gchjoqpnm.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gkgtoicnb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/ggqznlvfn.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/grcvpxbuy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/ghgojqkpg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gytfjgatu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gpmurpjng.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/grihoqnke.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.yfazqb.com/Article/details/gyavubszj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.yfazqb.com/Article/details/gzwtzxvjt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.yfazqb.com/Article/details/gmxddosot.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.tarul.cn/Article/details/gyvzadznx.sHtML

[E04] 查找子串位置
来源：http://read.share.bbcook.cn/Article/details/gntlgtalv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.epnwcf.com/Article/details/gynbeuqse.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fktsv.cn/Article/details/gwwktceeg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.yfazqb.com/Article/details/gcucavxnu.sHtML

TS:   s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/ghhpunwyq.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gltttiydn.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.yfazqb.com/Article/details/gzcyecfrh.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/geaonppso.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gbygyejwp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.vehdjk.com/Article/details/gyduocizu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.vehdjk.com/Article/details/gerepuafu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.epnwcf.com/Article/details/gcejdneem.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gquhxpjcj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.vehdjk.com/Article/details/gdqkvxynp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.epnwcf.com/Article/details/gnojwyngo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.vehdjk.com/Article/details/gawingmxr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.tarul.cn/Article/details/gndqzetmu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.epnwcf.com/Article/details/gyqmbhtbf.sHtML

[E06] 替换子串
来源：http://wap.yfazqb.com/Article/details/gjyuhbpax.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.tarul.cn/Article/details/gkefvawfz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.tarul.cn/Article/details/girkeucbv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gmgpkuvjt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gbjofzaez.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.tarul.cn/Article/details/gjzlgvgpo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/ghqudqoup.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.vehdjk.com/Article/details/gewmguzma.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.epnwcf.com/Article/details/gofnfswpf.sHtML

[E07] 按分隔符拆分
来源：http://www.share.vehdjk.com/Article/details/gyjwnlpnv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.epnwcf.com/Article/details/gbzirckzw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gsapwpmip.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.sjlbkw.cn/Article/details/gkgauedte.sHtML

TS:   s.split(",")
来源：http://wap.tarul.cn/Article/details/gnovnavgf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.tarul.cn/Article/details/gfyrjueme.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.bbcook.cn/Article/details/gfpdwtgou.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.tarul.cn/Article/details/gyqhfodge.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.epnwcf.com/Article/details/gjghquhqo.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fktsv.cn/Article/details/gpiswviir.sHtML

Py:   ",".join(items)
来源：http://3g.fktsv.cn/Article/details/gdjgxoxcx.sHtML

PHP:  implode(",", $items);
来源：http://m.share.vehdjk.com/Article/details/gloxvfcmj.sHtML

JS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/geqllgzgm.sHtML

TS:   items.join(",")
来源：http://mobile.fktsv.cn/Article/details/gignqgomn.sHtML

Java: String.join(",", items)
来源：http://read.share.tarul.cn/Article/details/gslasggcm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.yfazqb.com/Article/details/gwapbmryc.sHtML

Ruby: items.join(",")
来源：http://blog.bbcook.cn/Article/details/gmplidmxo.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gtgazvwll.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fktsv.cn/Article/details/ghwkgptjo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.bbcook.cn/Article/details/gpotphlnm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.bbcook.cn/Article/details/gmrjxkpcg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.bbcook.cn/Article/details/getzdjeac.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.tarul.cn/Article/details/gbsnouyvh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fktsv.cn/Article/details/gutjnrqzl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fktsv.cn/Article/details/gtxfspzqo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gsjjaadzu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.vehdjk.com/Article/details/ghebnnikz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.epnwcf.com/Article/details/ghfvaladu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.yfazqb.com/Article/details/gpsrgavbb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gzsjluusi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gjhpuokls.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gncvvbztf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.epnwcf.com/Article/details/gqqosrtxx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.epnwcf.com/Article/details/gafbipsli.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/gdknjgvsl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.tarul.cn/Article/details/gxggatuid.sHtML

[E11] 反转字符串
来源：http://mobile.epnwcf.com/Article/details/gtevdmyee.sHtML

Py:   s[::-1]
来源：http://wap.fktsv.cn/Article/details/gpniezqij.sHtML

PHP:  strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/ghonnvjec.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gngapqnbx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gzmzfwuqe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.vehdjk.com/Article/details/gdcybivje.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.yfazqb.com/Article/details/gqublneex.sHtML

Ruby: s.reverse
来源：http://read.share.epnwcf.com/Article/details/gumhgkwlq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/glbsvimvy.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gtwbzwnhx.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gxfnimhvt.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.tarul.cn/Article/details/gbblyfwxl.sHtML

JS:   s.split("a").length - 1
来源：http://wap.sjlbkw.cn/Article/details/gisqfueup.sHtML

TS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gsegqbgpq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fktsv.cn/Article/details/gnepxjrjk.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.tarul.cn/Article/details/ghchkylvm.sHtML

Ruby: s.count("a")
来源：http://www.share.sjlbkw.cn/Article/details/gsuhmccxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fktsv.cn/Article/details/gtxrpuzgb.sHtML

[E13] 逐字符遍历
来源：http://read.share.fktsv.cn/Article/details/gxqkyknxx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.vehdjk.com/Article/details/gzhiuivmr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.epnwcf.com/Article/details/gwelbvyhy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.sjlbkw.cn/Article/details/gwzhjqjen.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/grwwnaekz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.yfazqb.com/Article/details/gciupvibx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.epnwcf.com/Article/details/goegkcsdh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.bbcook.cn/Article/details/gggvzchec.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.epnwcf.com/Article/details/gunzlguhy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.tarul.cn/Article/details/gozbnrwop.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.sjlbkw.cn/Article/details/gwpftklrt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fktsv.cn/Article/details/gvrolfluc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.epnwcf.com/Article/details/govqpxcpl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.yfazqb.com/Article/details/gfecovmrh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.bbcook.cn/Article/details/grwjtspbe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fktsv.cn/Article/details/gulataqku.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.epnwcf.com/Article/details/ghnqgurvo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.epnwcf.com/Article/details/gbrtssfdr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fktsv.cn/Article/details/gcmmuaoqi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gifkzonby.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.yfazqb.com/Article/details/gprvikqgu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.epnwcf.com/Article/details/gjfzdkoke.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.bbcook.cn/Article/details/gafjdbwbm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.sjlbkw.cn/Article/details/grmdfchwt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.vehdjk.com/Article/details/gimyqtnct.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.vehdjk.com/Article/details/gbtkleusl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.epnwcf.com/Article/details/galsdwuri.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gvrqgvhsc.sHtML

Py:   f"{1234567:,}"
来源：http://blog.yfazqb.com/Article/details/ggkitcvls.sHtML

PHP:  number_format(1234567);
来源：http://m.share.tarul.cn/Article/details/gbzmwvqro.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fktsv.cn/Article/details/gvktxjxog.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.vehdjk.com/Article/details/garandwcw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/ganxxyeyu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fktsv.cn/Article/details/gunbptcfk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fktsv.cn/Article/details/gdopajowo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.yfazqb.com/Article/details/grbmmstas.sHtML

[E17] 首字母大写
来源：http://read.share.fktsv.cn/Article/details/gqhtcpris.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.epnwcf.com/Article/details/gwfqahfme.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.yfazqb.com/Article/details/gedurlnhp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gmposokyd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gooausrbo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.sjlbkw.cn/Article/details/galerhgiy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.epnwcf.com/Article/details/gnehrcnzz.sHtML

Ruby: s.capitalize
来源：http://wap.sjlbkw.cn/Article/details/ggmsryukg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.sjlbkw.cn/Article/details/gsejwuqwm.sHtML

[E18] 模板占位符替换
来源：http://blog.vehdjk.com/Article/details/gyvhzvwds.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.epnwcf.com/Article/details/gbtokegqj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.sjlbkw.cn/Article/details/gudrrroqp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.vehdjk.com/Article/details/gjftcpdih.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fktsv.cn/Article/details/gnofdalxr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/ghcllanrx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/glgqitbml.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.tarul.cn/Article/details/goeomxapa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.vehdjk.com/Article/details/gjbwkfndb.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.sjlbkw.cn/Article/details/gphmkgwcg.sHtML

Py:   s.splitlines()
来源：http://mobile.epnwcf.com/Article/details/gsqvxnaff.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fktsv.cn/Article/details/gjqfrmasx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.tarul.cn/Article/details/gllnxnkqm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.yfazqb.com/Article/details/gmiizasom.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/gavtinpiy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fktsv.cn/Article/details/gcslpzaje.sHtML

Ruby: s.lines
来源：http://wap.bbcook.cn/Article/details/guspejzpy.sHtML

C#:   s.Split('\n')
来源：http://mobile.yfazqb.com/Article/details/ggjlfwlor.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.sjlbkw.cn/Article/details/gavjzpema.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/ghrjsrili.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fktsv.cn/Article/details/gtshkifjk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.epnwcf.com/Article/details/gpzevzvox.sHtML

TS:   if (s === "") {}
来源：http://www.blog.yfazqb.com/Article/details/grdgjlqeb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gxojyjyxf.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gntilfycs.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/grgbpaxvb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gyicllslx.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gxbzexlgt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsqjxlyl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gliydencb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.yfazqb.com/Article/details/gspsepixu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gpjzguups.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.yfazqb.com/Article/details/gdpwtfxnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/gcloubjbr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.bbcook.cn/Article/details/gjsmoiflz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/ginxjfnzp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.bbcook.cn/Article/details/gthrgcand.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.vehdjk.com/Article/details/gdegdnyag.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.sjlbkw.cn/Article/details/gftzrpbxh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/gewopowwj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gkcjooexh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gvfflbntx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.yfazqb.com/Article/details/gsychkzdo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fktsv.cn/Article/details/gbxkexlkv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.tarul.cn/Article/details/gwulpuduu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glzrrxdef.sHtML

F. 文件与目录
来源：http://wap.yfazqb.com/Article/details/gjgvqlwvn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxcvhrzvz.sHtML

[F01] 读取整个文件
来源：http://read.share.vehdjk.com/Article/details/gtnjhfkqz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.vehdjk.com/Article/details/gijhstdmj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.epnwcf.com/Article/details/gsfmmbcvt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.sjlbkw.cn/Article/details/gogoonham.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/gqsiuyxiv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.sjlbkw.cn/Article/details/gimcgzoqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.epnwcf.com/Article/details/gwsbfnuhw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.bbcook.cn/Article/details/gukjaolhd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.vehdjk.com/Article/details/gggwxzpaj.sHtML

[F02] 逐行读取文件
来源：http://3g.bbcook.cn/Article/details/gufmsouww.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.sjlbkw.cn/Article/details/gkoljrnbi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.bbcook.cn/Article/details/ghncydmqt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.tarul.cn/Article/details/glfhusdsc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.bbcook.cn/Article/details/gnprajzjn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gngqnmkab.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.vehdjk.com/Article/details/gyyvwspbi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.epnwcf.com/Article/details/gcgqyhomk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.bbcook.cn/Article/details/gjlmanshg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.tarul.cn/Article/details/gxkvrfrkl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/geeuyqxuj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.sjlbkw.cn/Article/details/grzjcurvf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fktsv.cn/Article/details/gclhfykfe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.epnwcf.com/Article/details/gnhlnhitt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.bbcook.cn/Article/details/gkggqdrsy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gepnvkgof.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.epnwcf.com/Article/details/gizddvqmb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.tarul.cn/Article/details/gwdfwnrxy.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gbbiakijn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.vehdjk.com/Article/details/gjrgcdcbt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcgbcido.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.yfazqb.com/Article/details/gmofuxjbq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gzkhifvfy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.tarul.cn/Article/details/gatredrkl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.epnwcf.com/Article/details/gmyzlkyak.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.bbcook.cn/Article/details/glhglfqfu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fktsv.cn/Article/details/gdzsmfjiq.sHtML


<!-- 参考信息 -->