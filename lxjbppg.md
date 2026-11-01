代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.epnwcf.com/Article/details/gjqhbaemc.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.vehdjk.com/Article/details/gpxrkzcxm.sHtML

Py:   Counter(arr)
来源：http://www.share.vehdjk.com/Article/details/gjtalljjj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.tarul.cn/Article/details/gyeddquah.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.sjlbkw.cn/Article/details/ggvlrcktm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.sjlbkw.cn/Article/details/gsnejtovk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.tarul.cn/Article/details/gyvxehruy.sHtML

Go:   // 手写 map[T]int
来源：http://baike.bbcook.cn/Article/details/gwlkjolzg.sHtML

Ruby: arr.tally
来源：http://baike.vehdjk.com/Article/details/gajtvxkcp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.sjlbkw.cn/Article/details/gpyvtwpfy.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.vehdjk.com/Article/details/gzmsknaaz.sHtML

Py:   x in arr
来源：http://blog.yfazqb.com/Article/details/gyvslpyrc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.tarul.cn/Article/details/grqdecpre.sHtML

JS:   arr.includes(x)
来源：http://www.blog.yfazqb.com/Article/details/givjrllur.sHtML

TS:   arr.includes(x)
来源：http://wap.bbcook.cn/Article/details/gywpgvjik.sHtML

Java: list.contains(x)
来源：http://blog.fktsv.cn/Article/details/gudajutgs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ghzodqvdt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.bbcook.cn/Article/details/gtzdxurbm.sHtML

C#:   list.Contains(x)
来源：http://read.share.yfazqb.com/Article/details/grqnpbptb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.vehdjk.com/Article/details/godgqtguz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/goxnrftoo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.tarul.cn/Article/details/grzkalwgr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gsbcjynmk.sHtML

TS:   [...arr];
来源：http://www.blog.bbcook.cn/Article/details/ghwccnjet.sHtML

Java: new ArrayList<>(list);
来源：http://wap.sjlbkw.cn/Article/details/gtazsezpi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gexqjeqkm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/gyszybekk.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gzvgrtcpa.sHtML

[D23] reduce 累积计算
来源：http://m.share.vehdjk.com/Article/details/grokgxzzk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gxszcyace.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.epnwcf.com/Article/details/goriikggq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gavsisdtw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.bbcook.cn/Article/details/gagdnwtrv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.epnwcf.com/Article/details/gxesxynpu.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gxdvwvwfo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.epnwcf.com/Article/details/gjduuzffw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.sjlbkw.cn/Article/details/gntismmxm.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gzejjcpjh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.yfazqb.com/Article/details/gxrgxfkwr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.bbcook.cn/Article/details/gjpyrvncn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gwprsbugu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gxgkvzqwd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gmjwqjnrb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/gkxtmdnzz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fktsv.cn/Article/details/gjmnvrohd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/gurkcndtd.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.bbcook.cn/Article/details/gxfwkaiyg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/grzufsenk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.yfazqb.com/Article/details/gekbxniyb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.sjlbkw.cn/Article/details/ghbaseqab.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.tarul.cn/Article/details/gfvrcjnue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/glcolbqzz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.tarul.cn/Article/details/gfdpblzbz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/goapgmtxf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.sjlbkw.cn/Article/details/gxedrweht.sHtML

[D26] 数组转字符串
来源：http://3g.yfazqb.com/Article/details/givnkhmog.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.tarul.cn/Article/details/gvdzdsxyk.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.tarul.cn/Article/details/gghgnpchz.sHtML

JS:   arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gkexvtogp.sHtML

TS:   arr.join(", ")
来源：http://wap.tarul.cn/Article/details/gouzkvhql.sHtML

Java: String.join(", ", list)
来源：http://3g.sjlbkw.cn/Article/details/gkvhrakhd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/givwahvyh.sHtML

Ruby: arr.join(", ")
来源：http://3g.sjlbkw.cn/Article/details/gnpevehra.sHtML

C#:   string.Join(", ", list)
来源：http://3g.epnwcf.com/Article/details/gmjbgzfak.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxbqsuxlw.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/gjkpocopt.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzhcskyat.sHtML

[E01] 拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gbqyojapp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.epnwcf.com/Article/details/gjgewdspq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.bbcook.cn/Article/details/gdglirsqy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.vehdjk.com/Article/details/gblsfuaqq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.vehdjk.com/Article/details/gikpnssah.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.sjlbkw.cn/Article/details/gsmhbrpwh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.tarul.cn/Article/details/gbiurdtlg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.sjlbkw.cn/Article/details/gtrxilddm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gtbhsdxqx.sHtML

[E02] 重复字符串
来源：http://www.m.share.fktsv.cn/Article/details/guubwvkhd.sHtML

Py:   "ab" * 3
来源：http://read.share.vehdjk.com/Article/details/grhckzlpf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.epnwcf.com/Article/details/gqfcqhhux.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gkbihdlnh.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.sjlbkw.cn/Article/details/gnhozvcyt.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/garfeubdt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.epnwcf.com/Article/details/glqhkwwac.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/gcczlladv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.yfazqb.com/Article/details/gbfnotnbj.sHtML

[E03] 截取子串
来源：http://baike.vehdjk.com/Article/details/gtalbvqmb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.tarul.cn/Article/details/gfkiidjgk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gpnvphpgz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/guytorcwj.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.bbcook.cn/Article/details/gwjskuqby.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gvkpumakg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.sjlbkw.cn/Article/details/ghanzpcys.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fktsv.cn/Article/details/gdzqvvdom.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.yfazqb.com/Article/details/gvactdbld.sHtML

[E04] 查找子串位置
来源：http://www.m.share.epnwcf.com/Article/details/gojytojna.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fktsv.cn/Article/details/gpxzskptd.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.sjlbkw.cn/Article/details/gzflobesb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.tarul.cn/Article/details/gbgwryicx.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fktsv.cn/Article/details/gcjofwvbj.sHtML

Java: s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/grebihaxc.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fktsv.cn/Article/details/gvioodvyf.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/gwnvtzrmg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.yfazqb.com/Article/details/ggiqxckvs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.tarul.cn/Article/details/gvgbmznhv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fktsv.cn/Article/details/gskkwhlxq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.sjlbkw.cn/Article/details/ghgqswgwp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.vehdjk.com/Article/details/ggpmpewkv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.sjlbkw.cn/Article/details/govolynax.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.epnwcf.com/Article/details/gisjjeavb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.yfazqb.com/Article/details/gzvnaxiam.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gmpfpzgpx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.sjlbkw.cn/Article/details/gkmljktiq.sHtML

[E06] 替换子串
来源：http://wap.tarul.cn/Article/details/gglpyzzfu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.yfazqb.com/Article/details/gkwiqhfxz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.tarul.cn/Article/details/godbnvdeg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/gaotafyfk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gsmximbos.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fktsv.cn/Article/details/geqmzviww.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.tarul.cn/Article/details/gjsicdtwg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gnjsanvtn.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.yfazqb.com/Article/details/gurcqtmpg.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gstojglff.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.vehdjk.com/Article/details/ghweyodpw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.tarul.cn/Article/details/gnutvsacy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.sjlbkw.cn/Article/details/giueswkqx.sHtML

TS:   s.split(",")
来源：http://www.m.share.epnwcf.com/Article/details/gumkxryqp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fktsv.cn/Article/details/gtarihuhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.bbcook.cn/Article/details/glafciavr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.epnwcf.com/Article/details/gjibkrkrm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/gvpkukikb.sHtML

[E08] 数组按分隔符合并
来源：http://blog.tarul.cn/Article/details/gpdyqwoko.sHtML

Py:   ",".join(items)
来源：http://read.share.yfazqb.com/Article/details/gpgfpjeys.sHtML

PHP:  implode(",", $items);
来源：http://m.share.bbcook.cn/Article/details/griewtisj.sHtML

JS:   items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gkgbpontf.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gcrhoykkn.sHtML

Java: String.join(",", items)
来源：http://www.blog.tarul.cn/Article/details/gxabhwtpf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gzygpcizx.sHtML

Ruby: items.join(",")
来源：http://baike.tarul.cn/Article/details/gbnqyxcmw.sHtML

C#:   string.Join(",", items)
来源：http://m.share.tarul.cn/Article/details/gfuwjjfbb.sHtML

[E09] 去除所有空白字符
来源：http://wap.vehdjk.com/Article/details/gofpiklmk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fktsv.cn/Article/details/ggtprexic.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.tarul.cn/Article/details/ghkhxkyea.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsttatro.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.tarul.cn/Article/details/gbjiwnthc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.tarul.cn/Article/details/gtxzmgmot.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.sjlbkw.cn/Article/details/gsncznlmv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.vehdjk.com/Article/details/glehncoee.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.tarul.cn/Article/details/gnjcaxmug.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.bbcook.cn/Article/details/gykatpscv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.tarul.cn/Article/details/gyrfxucwd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.bbcook.cn/Article/details/glvqsbtbi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/givmjdaas.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gazqrzcjz.sHtML

Java: String.format("%03d", 7)
来源：http://3g.tarul.cn/Article/details/gzvcfhqou.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.bbcook.cn/Article/details/grqwddiyg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.tarul.cn/Article/details/gpeypeqme.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.vehdjk.com/Article/details/gflpcswmv.sHtML

[E11] 反转字符串
来源：http://mobile.tarul.cn/Article/details/gfdyxjdsg.sHtML

Py:   s[::-1]
来源：http://3g.bbcook.cn/Article/details/gperjjnpb.sHtML

PHP:  strrev($s);
来源：http://blog.bbcook.cn/Article/details/gptowmydi.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gytbytkhw.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gxvofdjus.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fktsv.cn/Article/details/grunazfbx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.yfazqb.com/Article/details/gftihemth.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gulqqiajw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/glgwlxkjy.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.vehdjk.com/Article/details/glonsgbka.sHtML

Py:   s.count("a")
来源：http://www.m.share.bbcook.cn/Article/details/gvwflknwq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.sjlbkw.cn/Article/details/gffpmdqne.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.yfazqb.com/Article/details/ghxfvizco.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fktsv.cn/Article/details/gzlcjimnn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.bbcook.cn/Article/details/ggstudidc.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.tarul.cn/Article/details/gmcnvhkoe.sHtML

Ruby: s.count("a")
来源：http://wap.vehdjk.com/Article/details/gszfbvdkf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.sjlbkw.cn/Article/details/gcippjsdh.sHtML

[E13] 逐字符遍历
来源：http://m.share.bbcook.cn/Article/details/goidgqkty.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.epnwcf.com/Article/details/glznjzltr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.vehdjk.com/Article/details/gurvwefik.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.tarul.cn/Article/details/gfuuteqwg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.epnwcf.com/Article/details/gvdweiakn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gdctgilna.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.tarul.cn/Article/details/gdttkjhpb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.sjlbkw.cn/Article/details/geuvwfxbh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.epnwcf.com/Article/details/gaunicmqm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.epnwcf.com/Article/details/govrrpgdu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.vehdjk.com/Article/details/gwjzgclvb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gorjgkkqb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.epnwcf.com/Article/details/gzjxuwpze.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.epnwcf.com/Article/details/gcomxdixw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gxbokditu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.epnwcf.com/Article/details/gbclqmakr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fktsv.cn/Article/details/grwbhimmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gmxtehafi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.sjlbkw.cn/Article/details/gcvjmxoep.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.yfazqb.com/Article/details/gbctwztul.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyxebkfz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fktsv.cn/Article/details/gfweblobz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/glhzelfoz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.epnwcf.com/Article/details/gacbtgxbz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.epnwcf.com/Article/details/gwiwpjxzm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.tarul.cn/Article/details/glmgewniz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.vehdjk.com/Article/details/gkhdumccz.sHtML

[E16] 数字千分位
来源：http://read.share.sjlbkw.cn/Article/details/gjpwtudfv.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.bbcook.cn/Article/details/gnivlkkwl.sHtML

PHP:  number_format(1234567);
来源：http://m.share.vehdjk.com/Article/details/gvwmisyqq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fktsv.cn/Article/details/gyvvbzfpn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.vehdjk.com/Article/details/gyawampfo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.bbcook.cn/Article/details/gkfkndltg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gjsazrtds.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.epnwcf.com/Article/details/gfelffmtu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.bbcook.cn/Article/details/guoangxpc.sHtML

[E17] 首字母大写
来源：http://wap.fktsv.cn/Article/details/gzdqahwot.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.bbcook.cn/Article/details/ghkgadcqq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.sjlbkw.cn/Article/details/gupcggsku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fktsv.cn/Article/details/grqsuykvn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fktsv.cn/Article/details/gahogbwpa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.tarul.cn/Article/details/gxuqmfsoy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fktsv.cn/Article/details/gcwoggico.sHtML

Ruby: s.capitalize
来源：http://mobile.sjlbkw.cn/Article/details/ghoalknfq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.sjlbkw.cn/Article/details/gbbokfufq.sHtML

[E18] 模板占位符替换
来源：http://3g.epnwcf.com/Article/details/goihdyewt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gumpwarop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.bbcook.cn/Article/details/gbkfdszly.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/glvykxqxx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.yfazqb.com/Article/details/gvyiejcnf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gueywhfvr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gznhpssqj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.bbcook.cn/Article/details/gakxrnvis.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fktsv.cn/Article/details/gwwsalxpf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.vehdjk.com/Article/details/gizhqlmik.sHtML

Py:   s.splitlines()
来源：http://mobile.yfazqb.com/Article/details/gcvobbkai.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fktsv.cn/Article/details/gqllkbvgq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.epnwcf.com/Article/details/gzasuerkb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/gfqneuixi.sHtML

Java: s.lines().toList()
来源：http://mobile.vehdjk.com/Article/details/gcathlyjq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gquvjsngj.sHtML

Ruby: s.lines
来源：http://m.share.vehdjk.com/Article/details/gjhubaerd.sHtML

C#:   s.Split('\n')
来源：http://m.share.sjlbkw.cn/Article/details/gznxuchlv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.tarul.cn/Article/details/gbbgctkup.sHtML

Py:   if not s:
来源：http://wap.epnwcf.com/Article/details/gwtfbkgni.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.tarul.cn/Article/details/giwuzmepb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.tarul.cn/Article/details/gorgoghrf.sHtML

TS:   if (s === "") {}
来源：http://wap.tarul.cn/Article/details/ghadapulu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/goqumgtpd.sHtML

Go:   if s == "" {}
来源：http://mobile.yfazqb.com/Article/details/gcecvnzgt.sHtML

Ruby: if s.empty?
来源：http://3g.vehdjk.com/Article/details/gjwfnostd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.yfazqb.com/Article/details/ghzrpwcxe.sHtML

[E21] 超长截断加省略号
来源：http://wap.epnwcf.com/Article/details/gsbacppvx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.sjlbkw.cn/Article/details/gigkwzrbj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gacpgcokd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.bbcook.cn/Article/details/gjqdbixei.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.yfazqb.com/Article/details/gzsawldhm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.tarul.cn/Article/details/godlloenu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.bbcook.cn/Article/details/gzitwglnl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.yfazqb.com/Article/details/gaqojvctg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.yfazqb.com/Article/details/gtkxethmu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.yfazqb.com/Article/details/gwhjopohq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fktsv.cn/Article/details/gjcuyjozg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gtrzfugze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.vehdjk.com/Article/details/ggnqjymfz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.bbcook.cn/Article/details/gybnijyap.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/grrdggsoe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.tarul.cn/Article/details/gzmdmbhqv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.tarul.cn/Article/details/gljpcyfra.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.yfazqb.com/Article/details/grykthrst.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjibynvqf.sHtML

F. 文件与目录
来源：http://read.share.bbcook.cn/Article/details/gwgbwioxx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvaimxqzl.sHtML

[F01] 读取整个文件
来源：http://baike.sjlbkw.cn/Article/details/gnwnimzpf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.epnwcf.com/Article/details/guseqmnlj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.yfazqb.com/Article/details/ghjpzvmpy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fktsv.cn/Article/details/giovkabex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.epnwcf.com/Article/details/gmqdkeoya.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gtjpdirrk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.vehdjk.com/Article/details/gwdsmdzsk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.epnwcf.com/Article/details/gvcmcjjcb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.yfazqb.com/Article/details/gszbjtyab.sHtML

[F02] 逐行读取文件
来源：http://mobile.tarul.cn/Article/details/gjntzyrkf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.yfazqb.com/Article/details/gqhkqhetv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.vehdjk.com/Article/details/gpryylymp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdjtpgazj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmlilvovp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.vehdjk.com/Article/details/gqlcmovii.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.sjlbkw.cn/Article/details/gfonguilm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.bbcook.cn/Article/details/gnwjoeigp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.sjlbkw.cn/Article/details/gqolmvikr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.tarul.cn/Article/details/gakshdkbe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.yfazqb.com/Article/details/gftilbbqx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.vehdjk.com/Article/details/gwchhflnv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gtbiulkwd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.yfazqb.com/Article/details/gkiloegyk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.bbcook.cn/Article/details/geyqqoxgp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.tarul.cn/Article/details/gltpwvnqh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.epnwcf.com/Article/details/gsqdpakis.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.bbcook.cn/Article/details/gtuuynjjh.sHtML

[F04] 追加写入文件
来源：http://read.share.yfazqb.com/Article/details/gnrsogxgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.yfazqb.com/Article/details/gecvkyjee.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.yfazqb.com/Article/details/ghmkpkbem.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.bbcook.cn/Article/details/gerynoldu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gkxtjliww.sHtML


<!-- 参考信息 -->