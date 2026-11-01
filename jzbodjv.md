代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.yfazqb.com/Article/details/gybmakrsf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.bbcook.cn/Article/details/gjdivqudh.sHtML

Py:   Counter(arr)
来源：http://3g.vehdjk.com/Article/details/ggdtdjppk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gdxisvbez.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/gfqrrbwwa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gobbnxask.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fktsv.cn/Article/details/gqokaupyl.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.bbcook.cn/Article/details/gswvowjwz.sHtML

Ruby: arr.tally
来源：http://wap.bbcook.cn/Article/details/gehhqques.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/gdwddtsjz.sHtML

[D21] 判断是否包含某元素
来源：http://baike.vehdjk.com/Article/details/glqtmnasb.sHtML

Py:   x in arr
来源：http://3g.tarul.cn/Article/details/gkeixvykb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.vehdjk.com/Article/details/gmupgbwhq.sHtML

JS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gmolnxoer.sHtML

TS:   arr.includes(x)
来源：http://blog.sjlbkw.cn/Article/details/gijycarad.sHtML

Java: list.contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gordoamtc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.tarul.cn/Article/details/gufxovwcz.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoiwqbzq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.epnwcf.com/Article/details/gyqmqfaez.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.bbcook.cn/Article/details/gbpxmgcct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.sjlbkw.cn/Article/details/gcsbxzbeh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.bbcook.cn/Article/details/gqcappsbj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.epnwcf.com/Article/details/gmouhzxiw.sHtML

TS:   [...arr];
来源：http://www.blog.fktsv.cn/Article/details/gnneyhtyx.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fktsv.cn/Article/details/grzaohwbl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.vehdjk.com/Article/details/gbodxzpfg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.bbcook.cn/Article/details/gcrqiduuf.sHtML

C#:   new List<int>(list);
来源：http://m.share.epnwcf.com/Article/details/guiiimarn.sHtML

[D23] reduce 累积计算
来源：http://blog.yfazqb.com/Article/details/gjvdklmem.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.bbcook.cn/Article/details/gvtaygesl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.yfazqb.com/Article/details/ghljonfzz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.vehdjk.com/Article/details/gueffkass.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.bbcook.cn/Article/details/gyzndvthw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gmvfboxhn.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/giwkzskuv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.yfazqb.com/Article/details/grkkmxpfn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.bbcook.cn/Article/details/gpovatjur.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.sjlbkw.cn/Article/details/grjagthxs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.epnwcf.com/Article/details/gdvwsyqcc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fktsv.cn/Article/details/grcaxhbxj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fktsv.cn/Article/details/gigzeefup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gvmggcibz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.vehdjk.com/Article/details/gxfqwyesj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.sjlbkw.cn/Article/details/gkntqynqf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.epnwcf.com/Article/details/gcetzqxgm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.vehdjk.com/Article/details/gsroyxkvf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gisezgtnf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.bbcook.cn/Article/details/gkbdxxfzz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fktsv.cn/Article/details/gufqsmntd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fktsv.cn/Article/details/gphbrgagy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.epnwcf.com/Article/details/gdrwpvqnm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.bbcook.cn/Article/details/gzxwfdefc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.vehdjk.com/Article/details/gxpaphgtr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkasojgqn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.bbcook.cn/Article/details/gblhzarmb.sHtML

[D26] 数组转字符串
来源：http://m.share.tarul.cn/Article/details/gdokemtzc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.yfazqb.com/Article/details/gijqwgsje.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.vehdjk.com/Article/details/gywukxvjz.sHtML

JS:   arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gsneddval.sHtML

TS:   arr.join(", ")
来源：http://www.share.tarul.cn/Article/details/gvkupeepz.sHtML

Java: String.join(", ", list)
来源：http://mobile.bbcook.cn/Article/details/ggioooikw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.sjlbkw.cn/Article/details/gwyhorgjc.sHtML

Ruby: arr.join(", ")
来源：http://www.share.yfazqb.com/Article/details/gqicbvzbz.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gidhxuboo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gtwgdnsor.sHtML

E. 字符串处理
来源：http://www.m.share.epnwcf.com/Article/details/gccfgozum.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/glvjehkiz.sHtML

[E01] 拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjkjrcfc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.epnwcf.com/Article/details/ghaqetxli.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.tarul.cn/Article/details/gamarxjck.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fktsv.cn/Article/details/gpvdkjdgo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.tarul.cn/Article/details/gqobkllef.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gjuhwdslr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.yfazqb.com/Article/details/gueqttzih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.vehdjk.com/Article/details/gvlpntqhw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.vehdjk.com/Article/details/gwbxtkrfc.sHtML

[E02] 重复字符串
来源：http://wap.bbcook.cn/Article/details/gibjzkufs.sHtML

Py:   "ab" * 3
来源：http://wap.vehdjk.com/Article/details/gufvompcg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.yfazqb.com/Article/details/gpqkmebsm.sHtML

JS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gmzfjfdsr.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.tarul.cn/Article/details/gpnvumzks.sHtML

Java: "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gfhonokgg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.epnwcf.com/Article/details/gbvplcbob.sHtML

Ruby: "ab" * 3
来源：http://baike.vehdjk.com/Article/details/gqiovgmtf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.tarul.cn/Article/details/gvnehffka.sHtML

[E03] 截取子串
来源：http://www.share.tarul.cn/Article/details/gjqjpmzor.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.sjlbkw.cn/Article/details/gkntougtk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gxcwbnbje.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.yfazqb.com/Article/details/gtsliuxbr.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/ghsyblrzt.sHtML

Java: s.substring(1, 4)
来源：http://mobile.sjlbkw.cn/Article/details/gsjzicjzw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.sjlbkw.cn/Article/details/gvacfirzw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.vehdjk.com/Article/details/gpknldfnj.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gfcedrxzu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fktsv.cn/Article/details/gvnttmnmp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gmvwlabaz.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.tarul.cn/Article/details/gtnyzhpcq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.bbcook.cn/Article/details/gmhpcsaht.sHtML

TS:   s.indexOf("x")
来源：http://mobile.yfazqb.com/Article/details/gjadexgls.sHtML

Java: s.indexOf("x")
来源：http://blog.tarul.cn/Article/details/gwskwuvdo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.bbcook.cn/Article/details/giacnsyvy.sHtML

Ruby: s.index("x")
来源：http://www.share.epnwcf.com/Article/details/gvulhkzln.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/gynabtqdh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.sjlbkw.cn/Article/details/ggzetzmrb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.epnwcf.com/Article/details/gkkqbmwio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.bbcook.cn/Article/details/ggjmhhtzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.bbcook.cn/Article/details/gvwujepeu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fktsv.cn/Article/details/gjwvotfnr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gejmghdda.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gidqfepkm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.epnwcf.com/Article/details/gmyiohpsk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fktsv.cn/Article/details/gswmvktsb.sHtML

[E06] 替换子串
来源：http://www.blog.bbcook.cn/Article/details/gtmtvwtuw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/gcqocizns.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.epnwcf.com/Article/details/gbsodvdkm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.epnwcf.com/Article/details/ghzvypsse.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/gixsxkfyo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/gbsxthuhy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvhmfdzx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gaydjdsqy.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gxdxivqqt.sHtML

[E07] 按分隔符拆分
来源：http://wap.tarul.cn/Article/details/gmvkmxyzy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gfgahjubb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.yfazqb.com/Article/details/gqhncugvj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.tarul.cn/Article/details/geapndobf.sHtML

TS:   s.split(",")
来源：http://www.blog.fktsv.cn/Article/details/gopthdezo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.bbcook.cn/Article/details/gbdcxsmto.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gjvozdyse.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gsmzqzbok.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gdfwtairj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fktsv.cn/Article/details/gsdoqsgiw.sHtML

Py:   ",".join(items)
来源：http://mobile.fktsv.cn/Article/details/gikxeeoaz.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.bbcook.cn/Article/details/gdieyzxsr.sHtML

JS:   items.join(",")
来源：http://read.share.tarul.cn/Article/details/gcdywwlov.sHtML

TS:   items.join(",")
来源：http://3g.vehdjk.com/Article/details/gvfiurimz.sHtML

Java: String.join(",", items)
来源：http://read.share.fktsv.cn/Article/details/gttbtbwpp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.sjlbkw.cn/Article/details/gklitzzju.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gqmiufwwp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.sjlbkw.cn/Article/details/gdgwmgudt.sHtML

[E09] 去除所有空白字符
来源：http://wap.epnwcf.com/Article/details/gynlzdvia.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.yfazqb.com/Article/details/ggkuvevpx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fktsv.cn/Article/details/gswemyphx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.epnwcf.com/Article/details/glkolebzc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fktsv.cn/Article/details/gsakcitbv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gsqwazklb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.bbcook.cn/Article/details/gwgcsmflc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/gdjrdvgel.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/godpkpjhw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/geenjdglv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.yfazqb.com/Article/details/gyrjwuufd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.sjlbkw.cn/Article/details/gvnxesbse.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fktsv.cn/Article/details/gvsyijumt.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/ghlyibbif.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/guafyicez.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.yfazqb.com/Article/details/gvilzuuus.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.tarul.cn/Article/details/gehjgjtkg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.yfazqb.com/Article/details/gwfpfczmq.sHtML

[E11] 反转字符串
来源：http://m.share.sjlbkw.cn/Article/details/gahsuoqpt.sHtML

Py:   s[::-1]
来源：http://blog.vehdjk.com/Article/details/gfwrphzen.sHtML

PHP:  strrev($s);
来源：http://3g.fktsv.cn/Article/details/ghpdtycyw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gqhjjdppo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gnuabmmsc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.yfazqb.com/Article/details/gphyrjadf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.tarul.cn/Article/details/gzwvngjov.sHtML

Ruby: s.reverse
来源：http://wap.bbcook.cn/Article/details/guqnkjlfh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gefasghbg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/ggrhwpruu.sHtML

Py:   s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gdiwvpjnw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.vehdjk.com/Article/details/gfhlcouqj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.vehdjk.com/Article/details/gguynlhtn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.tarul.cn/Article/details/gaohyqazf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.bbcook.cn/Article/details/gtnalysnw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fktsv.cn/Article/details/gobhohgdq.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/ghxopvceo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.vehdjk.com/Article/details/gbxdkumhm.sHtML

[E13] 逐字符遍历
来源：http://www.share.fktsv.cn/Article/details/gxftwqybw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gshheinjr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.sjlbkw.cn/Article/details/ggdbbetwa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.epnwcf.com/Article/details/gjdtxnnbp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/ggsolhwtw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.tarul.cn/Article/details/gvftjdhal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.epnwcf.com/Article/details/gctigqskn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fktsv.cn/Article/details/grrdyupgx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gvuqzqonj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.yfazqb.com/Article/details/gvcrxsfsp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.yfazqb.com/Article/details/gzwyvdreq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.epnwcf.com/Article/details/gjgnpagak.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.bbcook.cn/Article/details/guuudpned.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.vehdjk.com/Article/details/gfyjlvbhd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.epnwcf.com/Article/details/geuzjjtuz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fktsv.cn/Article/details/gjxyhfixz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fktsv.cn/Article/details/gkbjunprr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.tarul.cn/Article/details/gwwlfwwlk.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.vehdjk.com/Article/details/gwdczehkl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.bbcook.cn/Article/details/gyeosmbca.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.sjlbkw.cn/Article/details/gdxmwtqbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.yfazqb.com/Article/details/gvjyorrtq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.tarul.cn/Article/details/gzucvzyvh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.bbcook.cn/Article/details/gbeixerjd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.yfazqb.com/Article/details/gkxrytndo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.bbcook.cn/Article/details/gyodnwzxq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.sjlbkw.cn/Article/details/grhrgpwmq.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gabgcnozh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.sjlbkw.cn/Article/details/gwyczgewa.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.bbcook.cn/Article/details/gfkkopznh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.sjlbkw.cn/Article/details/gmizymqlu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.tarul.cn/Article/details/gpummoudw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.yfazqb.com/Article/details/gmfgwqboj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.sjlbkw.cn/Article/details/gygqruzhn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.yfazqb.com/Article/details/gsqdsfvjn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.vehdjk.com/Article/details/gxktwaqbh.sHtML

[E17] 首字母大写
来源：http://read.share.epnwcf.com/Article/details/gldaxbrvk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.bbcook.cn/Article/details/gfffrxwgf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.yfazqb.com/Article/details/geogjvicp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.bbcook.cn/Article/details/gvodldvms.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/gtlwhjfdt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.yfazqb.com/Article/details/gieoxjzcf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.bbcook.cn/Article/details/gylewsswp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.tarul.cn/Article/details/ghjuslazm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.tarul.cn/Article/details/gtcoztbtp.sHtML

[E18] 模板占位符替换
来源：http://wap.fktsv.cn/Article/details/gndvgpfir.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.tarul.cn/Article/details/gqttxbdiq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.yfazqb.com/Article/details/gdgfmftdr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.sjlbkw.cn/Article/details/gleevrfjv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fktsv.cn/Article/details/gqertoxif.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fktsv.cn/Article/details/gvoyupcdi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fktsv.cn/Article/details/gcmxgemxa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.bbcook.cn/Article/details/gnpfnelhy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.sjlbkw.cn/Article/details/gecvgwcqn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.tarul.cn/Article/details/grfgejdil.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/gxwbvwxcf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gzpqkbfgq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/gxdsehugb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.tarul.cn/Article/details/gxsxxyjjn.sHtML

Java: s.lines().toList()
来源：http://www.blog.bbcook.cn/Article/details/guecwtywq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.epnwcf.com/Article/details/gnsrtrplr.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gxabtryvd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gibxzjbjy.sHtML

[E20] 判断字符串是否为空
来源：http://wap.yfazqb.com/Article/details/gkicowgpz.sHtML

Py:   if not s:
来源：http://3g.tarul.cn/Article/details/gqbzfrwbh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fktsv.cn/Article/details/gsvirsjbl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/gfrcfajkh.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.bbcook.cn/Article/details/glladownw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gpkastunb.sHtML

Go:   if s == "" {}
来源：http://www.m.share.vehdjk.com/Article/details/gwlhjrfrf.sHtML

Ruby: if s.empty?
来源：http://baike.vehdjk.com/Article/details/gsaqyatum.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/gdqogwfcl.sHtML

[E21] 超长截断加省略号
来源：http://blog.tarul.cn/Article/details/gpuqzolwq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.sjlbkw.cn/Article/details/ghmmjdxgx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gexxpozjl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fktsv.cn/Article/details/guclwhiij.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.epnwcf.com/Article/details/gmasxjbne.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.vehdjk.com/Article/details/gwjmkjgzn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.vehdjk.com/Article/details/gyroqsbrw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.vehdjk.com/Article/details/gwknsxhjo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.epnwcf.com/Article/details/gjfuspzpa.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyeohiqk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.yfazqb.com/Article/details/gqfhnbxru.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/guaqjclih.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.sjlbkw.cn/Article/details/gxobtnybc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.sjlbkw.cn/Article/details/gwbnssggy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.tarul.cn/Article/details/gxgprwwew.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.yfazqb.com/Article/details/gdlkncjgf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.yfazqb.com/Article/details/gdinirrfm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gmjphjzim.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gjyqkoamm.sHtML

F. 文件与目录
来源：http://www.share.sjlbkw.cn/Article/details/geuqkhpru.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghofusxql.sHtML

[F01] 读取整个文件
来源：http://mobile.tarul.cn/Article/details/gctedtweg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.vehdjk.com/Article/details/gfqikrzjs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gjrjxrfmi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.yfazqb.com/Article/details/grrdwgyci.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.bbcook.cn/Article/details/ghrbcgizu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.sjlbkw.cn/Article/details/gmmffabey.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fktsv.cn/Article/details/guzhdmfcs.sHtML

Ruby: File.read("a.txt")
来源：http://blog.yfazqb.com/Article/details/gmszffjxz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gilflivxg.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/gbjjkkhau.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.epnwcf.com/Article/details/gdgojiimp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.bbcook.cn/Article/details/gyadmsbqp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fktsv.cn/Article/details/gucswvpnj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.vehdjk.com/Article/details/gbnbpqqee.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.epnwcf.com/Article/details/gvnyjoijv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.yfazqb.com/Article/details/gqryhgifz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.sjlbkw.cn/Article/details/gazgxaacw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.bbcook.cn/Article/details/glozgacyn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.sjlbkw.cn/Article/details/gfdunutsd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.bbcook.cn/Article/details/gasmqtggm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/guozvsypr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gnvxawhun.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.tarul.cn/Article/details/gvlykpmem.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/grcsvwwin.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.vehdjk.com/Article/details/gfxhlyknj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.epnwcf.com/Article/details/gghpzaelw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gljjotssp.sHtML

[F04] 追加写入文件
来源：http://3g.bbcook.cn/Article/details/gehmibpvh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.tarul.cn/Article/details/gbcweplrp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.yfazqb.com/Article/details/gvpovdrvt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.tarul.cn/Article/details/gwkawhtum.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.vehdjk.com/Article/details/ghasmwxnh.sHtML


<!-- 参考信息 -->