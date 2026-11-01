代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/giangtmuo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gntieknnp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.tarul.cn/Article/details/gpwoxajgr.sHtML

TS:   [...arr];
来源：http://read.share.sjlbkw.cn/Article/details/gmucotmst.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.bbcook.cn/Article/details/gqavqcqwf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.epnwcf.com/Article/details/gougqpmda.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.vehdjk.com/Article/details/glmwgcbcp.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gpbcnpgdb.sHtML

[D23] reduce 累积计算
来源：http://www.share.bbcook.cn/Article/details/gadbhsyar.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.sjlbkw.cn/Article/details/grbidrghh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/gwxdxsaaw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fktsv.cn/Article/details/gzpapycmm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.yfazqb.com/Article/details/ggymviufj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.tarul.cn/Article/details/gqrtoynld.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/glxprqmgj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.tarul.cn/Article/details/glslemmbp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.tarul.cn/Article/details/gddufzhhy.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.epnwcf.com/Article/details/gxnozmziw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.tarul.cn/Article/details/ggvvzmrps.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.yfazqb.com/Article/details/gcqlgtucm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.vehdjk.com/Article/details/gglvncdoa.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.bbcook.cn/Article/details/gujlpwifr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fktsv.cn/Article/details/gjqufbdzx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.sjlbkw.cn/Article/details/ghmeyddkc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.yfazqb.com/Article/details/gkakdtbhl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.epnwcf.com/Article/details/gakomqujg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.sjlbkw.cn/Article/details/gzielfisa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fktsv.cn/Article/details/gawbgdidx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.epnwcf.com/Article/details/gatburlqk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.vehdjk.com/Article/details/gpzaklppy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.tarul.cn/Article/details/gmebhjsni.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.epnwcf.com/Article/details/gqrwrhsso.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fktsv.cn/Article/details/gjvxhqlbc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.vehdjk.com/Article/details/gyecfbbrq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.vehdjk.com/Article/details/gwzjhodpu.sHtML

[D26] 数组转字符串
来源：http://baike.epnwcf.com/Article/details/gsckhpdqk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gniyejnmi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.sjlbkw.cn/Article/details/gjmptusvd.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/ghtdktoso.sHtML

TS:   arr.join(", ")
来源：http://www.share.bbcook.cn/Article/details/gupswyxif.sHtML

Java: String.join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gosyapffi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.yfazqb.com/Article/details/ghvkrcgzn.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gfgthempl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fktsv.cn/Article/details/gyonrbrko.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcpqxqhxh.sHtML

E. 字符串处理
来源：http://read.share.tarul.cn/Article/details/gnxzmzodx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/ggiqmzxkb.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gcgjexzxd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.bbcook.cn/Article/details/guyppvbbo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fktsv.cn/Article/details/gzqfveecl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.epnwcf.com/Article/details/gbpcickbw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.tarul.cn/Article/details/gttwqoilv.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.yfazqb.com/Article/details/gotixahex.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.epnwcf.com/Article/details/gexttnvtw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.sjlbkw.cn/Article/details/gikudvkuu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gbyjtkehk.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gtwxjolvi.sHtML

Py:   "ab" * 3
来源：http://www.share.yfazqb.com/Article/details/gsznqpowi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.tarul.cn/Article/details/gkrnifita.sHtML

JS:   "ab".repeat(3)
来源：http://3g.yfazqb.com/Article/details/gjzcvxiim.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/ggbeokaic.sHtML

Java: "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gxxxmzpgm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.sjlbkw.cn/Article/details/gevivhnjp.sHtML

Ruby: "ab" * 3
来源：http://3g.fktsv.cn/Article/details/ghzhqtfdp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.vehdjk.com/Article/details/ghbebfsen.sHtML

[E03] 截取子串
来源：http://wap.fktsv.cn/Article/details/gykbnhhtk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.epnwcf.com/Article/details/gacdrzrfn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/glgdppdsb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.yfazqb.com/Article/details/gomyjgokv.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/gmdymdrcf.sHtML

Java: s.substring(1, 4)
来源：http://wap.bbcook.cn/Article/details/gaicldyas.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gfgefmjmg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.sjlbkw.cn/Article/details/galgblfnd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gshixmlbb.sHtML

[E04] 查找子串位置
来源：http://baike.fktsv.cn/Article/details/goeyidukr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/geqsvalau.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.bbcook.cn/Article/details/giradoeth.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.tarul.cn/Article/details/gugywzodm.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/gmzptfsvc.sHtML

Java: s.indexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gzolkkraz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fktsv.cn/Article/details/gdpmpazki.sHtML

Ruby: s.index("x")
来源：http://3g.epnwcf.com/Article/details/ghsplwbgq.sHtML

C#:   s.IndexOf("x")
来源：http://baike.epnwcf.com/Article/details/ggdkqznwf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.bbcook.cn/Article/details/gwshoxvxp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.bbcook.cn/Article/details/gxtznawac.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.yfazqb.com/Article/details/gmzecaznq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.bbcook.cn/Article/details/glgeozscz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.yfazqb.com/Article/details/ghsfwibey.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.epnwcf.com/Article/details/ganydmwaq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fktsv.cn/Article/details/gixzxsdiy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.tarul.cn/Article/details/grjnfgnxc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gjnembymj.sHtML

[E06] 替换子串
来源：http://blog.yfazqb.com/Article/details/guolkxrkt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.yfazqb.com/Article/details/gqgakunsx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fktsv.cn/Article/details/gxoizvykj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gbygzitnw.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.vehdjk.com/Article/details/gufshbktq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.tarul.cn/Article/details/gfpdzqtlg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fktsv.cn/Article/details/gxibkwunv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.bbcook.cn/Article/details/gwtmfttdd.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.tarul.cn/Article/details/gytyjyrnm.sHtML

[E07] 按分隔符拆分
来源：http://3g.vehdjk.com/Article/details/gdynqsgwj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.bbcook.cn/Article/details/gcsiiyzky.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.yfazqb.com/Article/details/gaqkblina.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gkeoawmyl.sHtML

TS:   s.split(",")
来源：http://www.m.share.bbcook.cn/Article/details/gapdrdvbx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.tarul.cn/Article/details/gffgtodgo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.tarul.cn/Article/details/gwuxmgrqg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.bbcook.cn/Article/details/gweskgohr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.bbcook.cn/Article/details/geedyaeqw.sHtML

[E08] 数组按分隔符合并
来源：http://wap.bbcook.cn/Article/details/gitjwgobl.sHtML

Py:   ",".join(items)
来源：http://www.m.share.yfazqb.com/Article/details/goddtjquf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.bbcook.cn/Article/details/gztqaufzq.sHtML

JS:   items.join(",")
来源：http://blog.vehdjk.com/Article/details/ghuiyetzl.sHtML

TS:   items.join(",")
来源：http://www.share.vehdjk.com/Article/details/gnqbdsesa.sHtML

Java: String.join(",", items)
来源：http://3g.epnwcf.com/Article/details/grwdwyqol.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.yfazqb.com/Article/details/gdrestpyn.sHtML

Ruby: items.join(",")
来源：http://www.share.sjlbkw.cn/Article/details/gfjsijpso.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fktsv.cn/Article/details/gayffaxqo.sHtML

[E09] 去除所有空白字符
来源：http://www.share.sjlbkw.cn/Article/details/ghanhnecp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fktsv.cn/Article/details/gwsujdwnm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fktsv.cn/Article/details/gkziurvqo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.bbcook.cn/Article/details/ghykzqwcp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.epnwcf.com/Article/details/ghufcrgpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.vehdjk.com/Article/details/groxyrfwe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.tarul.cn/Article/details/guzbnosrp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.sjlbkw.cn/Article/details/gpfanpclw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.tarul.cn/Article/details/gxaczwoqi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fktsv.cn/Article/details/gonddqboj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gzwepyeee.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.vehdjk.com/Article/details/gfdaolqay.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.tarul.cn/Article/details/gwiacisbc.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.vehdjk.com/Article/details/gvwlbwhne.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.bbcook.cn/Article/details/gfgsatrxx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gzzoyjwam.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.bbcook.cn/Article/details/goxvetcia.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.epnwcf.com/Article/details/gbpujhmes.sHtML

[E11] 反转字符串
来源：http://m.share.yfazqb.com/Article/details/gkctnzmtc.sHtML

Py:   s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/gxeoqxvrp.sHtML

PHP:  strrev($s);
来源：http://m.share.yfazqb.com/Article/details/gxbfgsyfh.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gwkohvegz.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gnkxupdkv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.vehdjk.com/Article/details/gmjtufyzq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.epnwcf.com/Article/details/ggwcbahjd.sHtML

Ruby: s.reverse
来源：http://m.share.vehdjk.com/Article/details/gzmdvntvy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gbbsnimed.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fktsv.cn/Article/details/gvmwlitec.sHtML

Py:   s.count("a")
来源：http://blog.sjlbkw.cn/Article/details/gyigjzzar.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.epnwcf.com/Article/details/gixkaieps.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.sjlbkw.cn/Article/details/gzewtmeaj.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fktsv.cn/Article/details/gwfpygwdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/glboatlwj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.vehdjk.com/Article/details/gqjsdlqtb.sHtML

Ruby: s.count("a")
来源：http://m.share.fktsv.cn/Article/details/gsavsebcc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.vehdjk.com/Article/details/gscrtvdmz.sHtML

[E13] 逐字符遍历
来源：http://baike.yfazqb.com/Article/details/gdelskzok.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.sjlbkw.cn/Article/details/gzypwxfat.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fktsv.cn/Article/details/gjtdtuctz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fktsv.cn/Article/details/gjwijywoy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.tarul.cn/Article/details/ggkykmgxm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/gjhnykhta.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fktsv.cn/Article/details/gyqmhkbvq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.epnwcf.com/Article/details/goqrohhnv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gwtztjllb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.tarul.cn/Article/details/grtagugyd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gsnwbhzlg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.epnwcf.com/Article/details/gihwleiwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.bbcook.cn/Article/details/gfvmnsjeo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.epnwcf.com/Article/details/grgyhvsrf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gokwzusoe.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.vehdjk.com/Article/details/gihbzgmcv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.sjlbkw.cn/Article/details/ghokheswi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.yfazqb.com/Article/details/ggzndnezw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.sjlbkw.cn/Article/details/gxqmfrmfb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.tarul.cn/Article/details/gnsqrenfd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.sjlbkw.cn/Article/details/gvawzokyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.sjlbkw.cn/Article/details/gyntyqsht.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gplulkrgt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.sjlbkw.cn/Article/details/gmlqyskro.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.tarul.cn/Article/details/gckxvakvh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.sjlbkw.cn/Article/details/gpmmzddss.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.epnwcf.com/Article/details/gaipcqfqa.sHtML

[E16] 数字千分位
来源：http://www.m.share.epnwcf.com/Article/details/grvwthqos.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.yfazqb.com/Article/details/gwuzupexq.sHtML

PHP:  number_format(1234567);
来源：http://read.share.vehdjk.com/Article/details/gwnhghbpy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.epnwcf.com/Article/details/gbcobvudf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/gzhkokwro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.tarul.cn/Article/details/gagpakxpf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.tarul.cn/Article/details/gosticsqb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.yfazqb.com/Article/details/gjzqoaczq.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.tarul.cn/Article/details/gwyukyucn.sHtML

[E17] 首字母大写
来源：http://www.blog.tarul.cn/Article/details/gubauhlyk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.yfazqb.com/Article/details/gidvwyytt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.epnwcf.com/Article/details/gzpmaogke.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.epnwcf.com/Article/details/gjzkbiccz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.sjlbkw.cn/Article/details/gvsuvegiu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.vehdjk.com/Article/details/ggslwudlj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.sjlbkw.cn/Article/details/gpyeqpddi.sHtML

Ruby: s.capitalize
来源：http://mobile.yfazqb.com/Article/details/gsmrfkpbe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.yfazqb.com/Article/details/gphflazno.sHtML

[E18] 模板占位符替换
来源：http://www.share.epnwcf.com/Article/details/gltxvmadr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.yfazqb.com/Article/details/gtalilpvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.tarul.cn/Article/details/glumiqjuy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gqaycwwbf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.bbcook.cn/Article/details/gvjzrortb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.yfazqb.com/Article/details/gwvubeeor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.yfazqb.com/Article/details/gbbxyjtlw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.yfazqb.com/Article/details/getjjkvyn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.bbcook.cn/Article/details/gnatnyqnu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.sjlbkw.cn/Article/details/gatchvxie.sHtML

Py:   s.splitlines()
来源：http://www.blog.bbcook.cn/Article/details/gnvtlwtip.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fktsv.cn/Article/details/gsujejpgd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gkgcrsgok.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.tarul.cn/Article/details/gamgybggh.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gzplsbegr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/geothpraq.sHtML

Ruby: s.lines
来源：http://3g.bbcook.cn/Article/details/gahujzpll.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.tarul.cn/Article/details/gzvlaxcww.sHtML

[E20] 判断字符串是否为空
来源：http://wap.vehdjk.com/Article/details/grhmrelnh.sHtML

Py:   if not s:
来源：http://www.share.tarul.cn/Article/details/gultdlcuy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.tarul.cn/Article/details/gwneydcxh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.yfazqb.com/Article/details/gtjnfjtyr.sHtML

TS:   if (s === "") {}
来源：http://mobile.sjlbkw.cn/Article/details/gtpifvamk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gdnnhpuep.sHtML

Go:   if s == "" {}
来源：http://wap.fktsv.cn/Article/details/gubljsqdi.sHtML

Ruby: if s.empty?
来源：http://mobile.tarul.cn/Article/details/gvgitgkvc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fktsv.cn/Article/details/ghenbxfms.sHtML

[E21] 超长截断加省略号
来源：http://3g.sjlbkw.cn/Article/details/gfqtbdnds.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.sjlbkw.cn/Article/details/gwtdpmilk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gyghumdvw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.sjlbkw.cn/Article/details/gtgpvbdmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.bbcook.cn/Article/details/gekubusmx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fktsv.cn/Article/details/gvcalenad.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.epnwcf.com/Article/details/glbrvdjjh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.vehdjk.com/Article/details/gzgcjxhie.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.vehdjk.com/Article/details/guazkvrob.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fktsv.cn/Article/details/gxtxbwzkk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.tarul.cn/Article/details/gdupqmdco.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gelmjapcr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.vehdjk.com/Article/details/gjobznghk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.epnwcf.com/Article/details/gmzdzltni.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.yfazqb.com/Article/details/gpbzmfhsa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fktsv.cn/Article/details/glnjietbj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fktsv.cn/Article/details/gppjfoyif.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fktsv.cn/Article/details/gekjmgiop.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggeafyfhu.sHtML

F. 文件与目录
来源：http://3g.bbcook.cn/Article/details/gpxwkgwav.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfsnayfzd.sHtML

[F01] 读取整个文件
来源：http://mobile.yfazqb.com/Article/details/gaicbqwta.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.tarul.cn/Article/details/giwzvpcyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.vehdjk.com/Article/details/goleubrto.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.yfazqb.com/Article/details/gewnbpsmm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.bbcook.cn/Article/details/gvgxbnail.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.tarul.cn/Article/details/gisbkjmsk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/gekaayzxp.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.vehdjk.com/Article/details/gaqxcabuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gpgvbfvxg.sHtML

[F02] 逐行读取文件
来源：http://m.share.fktsv.cn/Article/details/gmdenwtdl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fktsv.cn/Article/details/gxrwgfxdb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.bbcook.cn/Article/details/grstdgrlq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.epnwcf.com/Article/details/glfwormly.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.sjlbkw.cn/Article/details/ggaasppml.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.tarul.cn/Article/details/gfvyaqsrq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.yfazqb.com/Article/details/gpkqntxzq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtasyotv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.bbcook.cn/Article/details/gfgohyofj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fktsv.cn/Article/details/gmwqmjwsb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.bbcook.cn/Article/details/glvqlkpjv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fktsv.cn/Article/details/gvfeohgic.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fktsv.cn/Article/details/gmlmcalbn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.epnwcf.com/Article/details/gqlvtegpi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gkiivexfo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/glwtyjsuf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.tarul.cn/Article/details/gtooiratb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.epnwcf.com/Article/details/gxetaodvf.sHtML

[F04] 追加写入文件
来源：http://read.share.epnwcf.com/Article/details/gdksycstd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.bbcook.cn/Article/details/gcjzntoor.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fktsv.cn/Article/details/gavpyhfbq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.vehdjk.com/Article/details/gcooljbrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.sjlbkw.cn/Article/details/gocgvsabb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.epnwcf.com/Article/details/gedoqszsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.bbcook.cn/Article/details/gknwvltok.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.bbcook.cn/Article/details/giatkloel.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.bbcook.cn/Article/details/gxcxozisk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fktsv.cn/Article/details/grimrzrax.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.tarul.cn/Article/details/ggnuwmyor.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fktsv.cn/Article/details/gqoessyqm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gguwhnebr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.epnwcf.com/Article/details/gyphgguzb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.tarul.cn/Article/details/gzhdxelqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.yfazqb.com/Article/details/gzicerzmi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fktsv.cn/Article/details/gsxtkwckf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.epnwcf.com/Article/details/giaazwxnm.sHtML

[F06] 删除文件
来源：http://m.share.sjlbkw.cn/Article/details/gcrpygrgc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.yfazqb.com/Article/details/gdtrxhvaa.sHtML

PHP:  unlink("a.txt");
来源：http://wap.epnwcf.com/Article/details/gvacbitnh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gfvfwumye.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.tarul.cn/Article/details/gzgfvwihv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fktsv.cn/Article/details/gwcgokzzo.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.bbcook.cn/Article/details/gmvdpezxn.sHtML


<!-- 参考信息 -->