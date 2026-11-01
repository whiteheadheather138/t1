代发 wailian999

Ruby: arr.tally
来源：http://www.share.epnwcf.com/Article/details/goebuxfqk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.tarul.cn/Article/details/gyzekuzyo.sHtML

[D21] 判断是否包含某元素
来源：http://baike.sjlbkw.cn/Article/details/gqrwtqsjx.sHtML

Py:   x in arr
来源：http://3g.epnwcf.com/Article/details/gcyarwtjt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.yfazqb.com/Article/details/ggkjzrijs.sHtML

JS:   arr.includes(x)
来源：http://mobile.yfazqb.com/Article/details/grhdxagtt.sHtML

TS:   arr.includes(x)
来源：http://3g.sjlbkw.cn/Article/details/gmnurdqnf.sHtML

Java: list.contains(x)
来源：http://read.share.fktsv.cn/Article/details/gxsafkdid.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvfexqkcx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.epnwcf.com/Article/details/grzfyrvpf.sHtML

C#:   list.Contains(x)
来源：http://read.share.vehdjk.com/Article/details/gkdvwijzp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fktsv.cn/Article/details/gdplpbjek.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.bbcook.cn/Article/details/gdccwpnsa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fktsv.cn/Article/details/gdqvtyhps.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.bbcook.cn/Article/details/gqnepsbck.sHtML

TS:   [...arr];
来源：http://blog.yfazqb.com/Article/details/gckmknbyg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.yfazqb.com/Article/details/gwposuovq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.bbcook.cn/Article/details/gfzeytqvv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.sjlbkw.cn/Article/details/gxyuzzqnp.sHtML

C#:   new List<int>(list);
来源：http://baike.bbcook.cn/Article/details/gbbsimyrb.sHtML

[D23] reduce 累积计算
来源：http://wap.vehdjk.com/Article/details/gcglijlnd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.tarul.cn/Article/details/gfuvmgzsu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.bbcook.cn/Article/details/gbmqxbcoq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.tarul.cn/Article/details/gajjislze.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.bbcook.cn/Article/details/gbzjydmqi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.tarul.cn/Article/details/gitzskele.sHtML

Go:   // 手写循环
来源：http://mobile.epnwcf.com/Article/details/gubkxlnqj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.tarul.cn/Article/details/gzpnglydx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.sjlbkw.cn/Article/details/gzjytvbec.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.vehdjk.com/Article/details/gqolcvbvg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.yfazqb.com/Article/details/gjtygadsk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.bbcook.cn/Article/details/gcdvokmsh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.epnwcf.com/Article/details/gozrqpdiz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gnbdxfnge.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gasdmuypn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.bbcook.cn/Article/details/giasgoadk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.vehdjk.com/Article/details/gzusgikdg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.bbcook.cn/Article/details/gwbrduyrz.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.tarul.cn/Article/details/gzyzeqpyw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.yfazqb.com/Article/details/gbhheqguf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.vehdjk.com/Article/details/gpvdfwgry.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.vehdjk.com/Article/details/gaicplzob.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.yfazqb.com/Article/details/gmpzoypzr.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fktsv.cn/Article/details/gwdixesmy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.vehdjk.com/Article/details/geeueuwvk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/gfgkwlcja.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.tarul.cn/Article/details/gqwqlhsqn.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/gyomtphcg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.sjlbkw.cn/Article/details/gktpxzpbl.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.tarul.cn/Article/details/goqvnznsk.sHtML

JS:   arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/goeiwxnxt.sHtML

TS:   arr.join(", ")
来源：http://mobile.vehdjk.com/Article/details/guvmztokh.sHtML

Java: String.join(", ", list)
来源：http://m.share.tarul.cn/Article/details/gwlaefrus.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.yfazqb.com/Article/details/gokvpiggc.sHtML

Ruby: arr.join(", ")
来源：http://blog.epnwcf.com/Article/details/gbmgidswp.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fktsv.cn/Article/details/gqstexued.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gtbgrtriy.sHtML

E. 字符串处理
来源：http://read.share.sjlbkw.cn/Article/details/gjkqkfgri.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtftprfgx.sHtML

[E01] 拼接字符串
来源：http://blog.yfazqb.com/Article/details/gxticujnj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.tarul.cn/Article/details/gmmdsafkn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.sjlbkw.cn/Article/details/gbsywrrsz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gxoqihtpv.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.sjlbkw.cn/Article/details/gafdzypec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.vehdjk.com/Article/details/grukxdddd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhyinbgx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.bbcook.cn/Article/details/gigtwakoo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gpiqqhzyz.sHtML

[E02] 重复字符串
来源：http://read.share.sjlbkw.cn/Article/details/gamxuqrwg.sHtML

Py:   "ab" * 3
来源：http://read.share.fktsv.cn/Article/details/gstyzzgue.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.tarul.cn/Article/details/gqiqhvnsq.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.yfazqb.com/Article/details/gvxgnvisf.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.vehdjk.com/Article/details/gsukkrndc.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fktsv.cn/Article/details/gvwokbjgt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.yfazqb.com/Article/details/gobompwpj.sHtML

Ruby: "ab" * 3
来源：http://read.share.yfazqb.com/Article/details/gfxqlvkmc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.epnwcf.com/Article/details/gyleasxib.sHtML

[E03] 截取子串
来源：http://www.m.share.fktsv.cn/Article/details/gmocqvvzs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.bbcook.cn/Article/details/gykcmnctl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gstflimng.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.bbcook.cn/Article/details/gzyygpsnx.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.epnwcf.com/Article/details/gibjnlakm.sHtML

Java: s.substring(1, 4)
来源：http://read.share.tarul.cn/Article/details/gklndnymy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fktsv.cn/Article/details/gbcitsltt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.vehdjk.com/Article/details/gpnygkgdn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fktsv.cn/Article/details/gwxvabnoj.sHtML

[E04] 查找子串位置
来源：http://blog.tarul.cn/Article/details/gfciagsko.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.bbcook.cn/Article/details/gqanjwwlj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.bbcook.cn/Article/details/guvvjmwmz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.vehdjk.com/Article/details/gehmlptrr.sHtML

TS:   s.indexOf("x")
来源：http://mobile.sjlbkw.cn/Article/details/gnvunmmfx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gzfkoehzg.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpgrggrg.sHtML

Ruby: s.index("x")
来源：http://www.m.share.yfazqb.com/Article/details/gpedvfpgj.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.bbcook.cn/Article/details/gklaejsst.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.tarul.cn/Article/details/gqdrmjvvm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.yfazqb.com/Article/details/genkeopcv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.yfazqb.com/Article/details/gmknwjyiw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.yfazqb.com/Article/details/gztyykdvd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/guaccvyav.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.epnwcf.com/Article/details/gtluqqtkw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.bbcook.cn/Article/details/gpgjhduhv.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.bbcook.cn/Article/details/ggykioxpt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.bbcook.cn/Article/details/gmydwddvm.sHtML

[E06] 替换子串
来源：http://www.m.share.fktsv.cn/Article/details/gerxkfjhj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/ganbqcjcq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.yfazqb.com/Article/details/gnqmiqmxv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/ginguhaxz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gfunbyrcu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.sjlbkw.cn/Article/details/gtwdoraxq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.tarul.cn/Article/details/gjnbrljbw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gzliqzrxh.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gartwwols.sHtML

[E07] 按分隔符拆分
来源：http://3g.yfazqb.com/Article/details/gxumkmrsb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.yfazqb.com/Article/details/gsymwtplp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gfwwpasvs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.epnwcf.com/Article/details/goytgcljx.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/gqbdomnrc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.tarul.cn/Article/details/gulxcddgn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.sjlbkw.cn/Article/details/gxhcqndul.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.vehdjk.com/Article/details/gtatbmvuz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.yfazqb.com/Article/details/gvjpvwqao.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.tarul.cn/Article/details/gkeuqyaqk.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/ghrbehaya.sHtML

PHP:  implode(",", $items);
来源：http://baike.fktsv.cn/Article/details/gxyknrknz.sHtML

JS:   items.join(",")
来源：http://www.m.share.bbcook.cn/Article/details/gtnhjhsju.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gfcrshnvl.sHtML

Java: String.join(",", items)
来源：http://read.share.yfazqb.com/Article/details/gxnoqfmjt.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gxslceawe.sHtML

Ruby: items.join(",")
来源：http://mobile.vehdjk.com/Article/details/gcxlzuuvc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.bbcook.cn/Article/details/gogljbycy.sHtML

[E09] 去除所有空白字符
来源：http://blog.tarul.cn/Article/details/gxrgrvdaf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.vehdjk.com/Article/details/gqccltgyc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.bbcook.cn/Article/details/gorahwmiv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fktsv.cn/Article/details/gkfccliee.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.yfazqb.com/Article/details/gmuowxymj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.yfazqb.com/Article/details/gvzqzvmvz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fktsv.cn/Article/details/gnxqrcxuq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.yfazqb.com/Article/details/gnakdrsjk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.vehdjk.com/Article/details/gzyyrjcqk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.bbcook.cn/Article/details/gggxxbhqc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.vehdjk.com/Article/details/gbjoxkoqk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.vehdjk.com/Article/details/gopspopzp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gtxshvetr.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gainhvtrl.sHtML

Java: String.format("%03d", 7)
来源：http://3g.sjlbkw.cn/Article/details/gyxmcwamj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.sjlbkw.cn/Article/details/goakuiksk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fktsv.cn/Article/details/ggeffljsj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.epnwcf.com/Article/details/gbjihoeie.sHtML

[E11] 反转字符串
来源：http://www.share.epnwcf.com/Article/details/gbivrjiif.sHtML

Py:   s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gccydovri.sHtML

PHP:  strrev($s);
来源：http://blog.vehdjk.com/Article/details/grtggoiec.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/grtkglqkm.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gsivmonao.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.bbcook.cn/Article/details/ggnuighem.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.epnwcf.com/Article/details/gahiddfwl.sHtML

Ruby: s.reverse
来源：http://3g.bbcook.cn/Article/details/goupzpgqo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gcdcavmpu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.epnwcf.com/Article/details/gasuvekia.sHtML

Py:   s.count("a")
来源：http://blog.vehdjk.com/Article/details/gpxssiair.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.bbcook.cn/Article/details/gmmenebzn.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.epnwcf.com/Article/details/gfhpgoydf.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.epnwcf.com/Article/details/gwtsyjzcy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.sjlbkw.cn/Article/details/ggiwiwjuj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.sjlbkw.cn/Article/details/gfjgvjtzp.sHtML

Ruby: s.count("a")
来源：http://www.share.bbcook.cn/Article/details/gzhtvjcif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.sjlbkw.cn/Article/details/gkpxzngrc.sHtML

[E13] 逐字符遍历
来源：http://mobile.bbcook.cn/Article/details/ggmugruxg.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.tarul.cn/Article/details/gwhntamlx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.bbcook.cn/Article/details/gqpnnumuc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.yfazqb.com/Article/details/gnqephfsm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/ghyxctfyj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.tarul.cn/Article/details/gmkiolpwm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.vehdjk.com/Article/details/gcpmceqmr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtifyrah.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.bbcook.cn/Article/details/gcjvrrmaf.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.yfazqb.com/Article/details/gvmdcpnfu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.bbcook.cn/Article/details/gevqlibzt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.yfazqb.com/Article/details/gvnsqmgcp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.yfazqb.com/Article/details/gpmgespmx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.epnwcf.com/Article/details/gcnqetwrf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fktsv.cn/Article/details/gwyamsogs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.epnwcf.com/Article/details/gbjpikiwx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.epnwcf.com/Article/details/gselgqsxi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.epnwcf.com/Article/details/ghcylyssr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.yfazqb.com/Article/details/ghudtejhc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.sjlbkw.cn/Article/details/gpkpbrnxn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.epnwcf.com/Article/details/gryzqhqbz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.vehdjk.com/Article/details/gshhoqnpw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.bbcook.cn/Article/details/gixtpeyje.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.vehdjk.com/Article/details/gzekcyiaj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.vehdjk.com/Article/details/gezfpycss.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.tarul.cn/Article/details/gqlvxvpye.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.vehdjk.com/Article/details/gqcqnltrm.sHtML

[E16] 数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/giwaswmyb.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.epnwcf.com/Article/details/gqligncyk.sHtML

PHP:  number_format(1234567);
来源：http://blog.fktsv.cn/Article/details/gxcamyanl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.tarul.cn/Article/details/gooxpwaxh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.bbcook.cn/Article/details/ggnlypmgd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fktsv.cn/Article/details/gkrkjgtoa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.yfazqb.com/Article/details/ganbegghn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.tarul.cn/Article/details/gvizsnzgv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gdmllynfr.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gratslqgg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fktsv.cn/Article/details/gqioybrxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.bbcook.cn/Article/details/galhdhryw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fktsv.cn/Article/details/gxjuodamf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.yfazqb.com/Article/details/gybnhdkoi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/gnxbdrwcx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fktsv.cn/Article/details/gxnvbjape.sHtML

Ruby: s.capitalize
来源：http://mobile.fktsv.cn/Article/details/ghqcjuyfr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.bbcook.cn/Article/details/gcjhthuay.sHtML

[E18] 模板占位符替换
来源：http://mobile.yfazqb.com/Article/details/ggsnanwrq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.sjlbkw.cn/Article/details/gwidqeewf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.tarul.cn/Article/details/gkhlsdwvo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.epnwcf.com/Article/details/gbkoxffyw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/guqwqcgfy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.tarul.cn/Article/details/gioubeczq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnjuunuj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.bbcook.cn/Article/details/gdyhclqkz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.vehdjk.com/Article/details/goosvihna.sHtML

[E19] 多行文本按行拆分
来源：http://baike.epnwcf.com/Article/details/gihqrmuyt.sHtML

Py:   s.splitlines()
来源：http://blog.yfazqb.com/Article/details/gjjxtkzzt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.tarul.cn/Article/details/gprrmucsd.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.yfazqb.com/Article/details/glvzvbgtv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gjqphukkl.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gufdhiail.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.yfazqb.com/Article/details/gjlmqcuut.sHtML

Ruby: s.lines
来源：http://www.m.share.sjlbkw.cn/Article/details/gufvmxzvd.sHtML

C#:   s.Split('\n')
来源：http://mobile.sjlbkw.cn/Article/details/gxvsvwsgu.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.epnwcf.com/Article/details/gvauhpmws.sHtML

Py:   if not s:
来源：http://www.blog.yfazqb.com/Article/details/gxkidbzdb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gptpaiyrl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.tarul.cn/Article/details/ghddrrxyg.sHtML

TS:   if (s === "") {}
来源：http://www.share.fktsv.cn/Article/details/gyvfrinbe.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gqrxgbfbk.sHtML

Go:   if s == "" {}
来源：http://baike.fktsv.cn/Article/details/gdwoaphje.sHtML

Ruby: if s.empty?
来源：http://www.share.tarul.cn/Article/details/gidjwxhro.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.vehdjk.com/Article/details/gyftklqej.sHtML

[E21] 超长截断加省略号
来源：http://baike.tarul.cn/Article/details/glshisoje.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.epnwcf.com/Article/details/gsbsmsrep.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.tarul.cn/Article/details/gpdzjtmdx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gtqfxzpkq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gnpolcenr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.bbcook.cn/Article/details/gxyiosgxz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.yfazqb.com/Article/details/guwmmovtl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.yfazqb.com/Article/details/gkulcyrlx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gktsfnboo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.sjlbkw.cn/Article/details/ggzyawexm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.epnwcf.com/Article/details/gjzxarzee.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/gncqhhimv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fktsv.cn/Article/details/gaivsjtlc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.yfazqb.com/Article/details/goedepkef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.vehdjk.com/Article/details/ghhboskar.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fktsv.cn/Article/details/gcuxqfstx.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fktsv.cn/Article/details/geiuaoiun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gfebgxfmb.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grgyrapnk.sHtML

F. 文件与目录
来源：http://blog.sjlbkw.cn/Article/details/gnbcpvvfb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbnpdrbip.sHtML

[F01] 读取整个文件
来源：http://baike.epnwcf.com/Article/details/gokzbvymo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.sjlbkw.cn/Article/details/ggebtpahi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwugerxea.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.vehdjk.com/Article/details/gvczaqnvu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.yfazqb.com/Article/details/gmidbetjh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.yfazqb.com/Article/details/gtckulbou.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.yfazqb.com/Article/details/gprxayfta.sHtML

Ruby: File.read("a.txt")
来源：http://baike.epnwcf.com/Article/details/goczwmhgl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/giughwnua.sHtML

[F02] 逐行读取文件
来源：http://3g.yfazqb.com/Article/details/gzzxkctxt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.bbcook.cn/Article/details/gfcoghxnh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.yfazqb.com/Article/details/gawpajxer.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.bbcook.cn/Article/details/gphibnjxw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/grwmuewkp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gcoihzdel.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.yfazqb.com/Article/details/glyuwbkgi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfmilryu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.tarul.cn/Article/details/gjmfknmal.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.bbcook.cn/Article/details/gghbiwkwx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fktsv.cn/Article/details/goekcbbjk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.yfazqb.com/Article/details/gaaslnhzh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.yfazqb.com/Article/details/gipgyctey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.yfazqb.com/Article/details/giqxxfdbt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.bbcook.cn/Article/details/gsqnfhfwm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.tarul.cn/Article/details/gyhawneqr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.vehdjk.com/Article/details/gllnmujjz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.sjlbkw.cn/Article/details/gwrihmatx.sHtML

[F04] 追加写入文件
来源：http://www.m.share.bbcook.cn/Article/details/gwlocabvl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.vehdjk.com/Article/details/gulditjmd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.vehdjk.com/Article/details/gbfwacpnk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.bbcook.cn/Article/details/gtasfjdag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.vehdjk.com/Article/details/gqxuufyut.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.sjlbkw.cn/Article/details/gejoomisq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.yfazqb.com/Article/details/gomtprpke.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.yfazqb.com/Article/details/gjlpgiyum.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.epnwcf.com/Article/details/geyagcfsv.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.bbcook.cn/Article/details/gusuttddr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrajutjp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gogrepfgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.vehdjk.com/Article/details/gsmzgyutv.sHtML


<!-- 参考信息 -->