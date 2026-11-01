代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.bbcook.cn/Article/details/gjoymwusl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.tarul.cn/Article/details/givhyoinz.sHtML

Py:   Counter(arr)
来源：http://www.share.epnwcf.com/Article/details/gtvuwsask.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.vehdjk.com/Article/details/gxvbdgcub.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.epnwcf.com/Article/details/gipxtsxhd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.tarul.cn/Article/details/grqunfiqy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.sjlbkw.cn/Article/details/gieoiqooo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.sjlbkw.cn/Article/details/grvhzzcrc.sHtML

Ruby: arr.tally
来源：http://read.share.sjlbkw.cn/Article/details/gbmarddhy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.yfazqb.com/Article/details/gzisbisgj.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.sjlbkw.cn/Article/details/gdarskyzp.sHtML

Py:   x in arr
来源：http://3g.fktsv.cn/Article/details/gcwsmebap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.bbcook.cn/Article/details/gttxbkouf.sHtML

JS:   arr.includes(x)
来源：http://m.share.vehdjk.com/Article/details/gdeagjjov.sHtML

TS:   arr.includes(x)
来源：http://m.share.tarul.cn/Article/details/gtclbyeip.sHtML

Java: list.contains(x)
来源：http://wap.tarul.cn/Article/details/ggjgbbsie.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.yfazqb.com/Article/details/gdfybioxk.sHtML

Ruby: arr.include?(x)
来源：http://m.share.vehdjk.com/Article/details/gddarrnna.sHtML

C#:   list.Contains(x)
来源：http://www.share.yfazqb.com/Article/details/gjadkhoik.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.bbcook.cn/Article/details/gdahynudm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gphujeikg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.tarul.cn/Article/details/gidcrbico.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.sjlbkw.cn/Article/details/gpehloxgl.sHtML

TS:   [...arr];
来源：http://baike.vehdjk.com/Article/details/gvymtuudg.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.yfazqb.com/Article/details/gzdksvojz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.epnwcf.com/Article/details/gcvoettdd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.yfazqb.com/Article/details/gemxosxbi.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gfszaqxxv.sHtML

[D23] reduce 累积计算
来源：http://3g.sjlbkw.cn/Article/details/ghmbqkcpq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.vehdjk.com/Article/details/gxjiihysa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gkhrtddsp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gvsrapbmn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.epnwcf.com/Article/details/gnneyxapi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gwqqpvnre.sHtML

Go:   // 手写循环
来源：http://wap.sjlbkw.cn/Article/details/gvamtlxsb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.yfazqb.com/Article/details/gbnmuzdbu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/ghdvisyfx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.yfazqb.com/Article/details/gyjkeiobi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/ggefvhrzf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.sjlbkw.cn/Article/details/glvhjepsn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.epnwcf.com/Article/details/gtucylvqc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.yfazqb.com/Article/details/gjmvbycwz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.vehdjk.com/Article/details/gpebnxiqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.epnwcf.com/Article/details/gzvwwyeck.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.sjlbkw.cn/Article/details/gasmjdpir.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.yfazqb.com/Article/details/glhnutflz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.bbcook.cn/Article/details/grncmafbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.sjlbkw.cn/Article/details/giqxcinon.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gqeizrwhq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.vehdjk.com/Article/details/gyslrfjuo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.epnwcf.com/Article/details/gehvvrlfk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gzmyhtbab.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkuyccesv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.vehdjk.com/Article/details/geqvjuiua.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.vehdjk.com/Article/details/gqnaazece.sHtML

[D26] 数组转字符串
来源：http://read.share.sjlbkw.cn/Article/details/gmpcmqyuo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.vehdjk.com/Article/details/gkfksyeez.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.epnwcf.com/Article/details/ghsttmono.sHtML

JS:   arr.join(", ")
来源：http://baike.sjlbkw.cn/Article/details/glqpmuwwd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gwkzhjzgr.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/ggrhxjfrd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.epnwcf.com/Article/details/gqqpezzbw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gynzrabpe.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.vehdjk.com/Article/details/gwxolueec.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ganzpurgk.sHtML

E. 字符串处理
来源：http://blog.fktsv.cn/Article/details/gakwaijon.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gcesqysmo.sHtML

[E01] 拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/gdglapcza.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.sjlbkw.cn/Article/details/gaugegpke.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gphikwdrj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.yfazqb.com/Article/details/gkappfndb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fktsv.cn/Article/details/gqqhdgwoc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.bbcook.cn/Article/details/gddwvwper.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.tarul.cn/Article/details/ggumolqvt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.yfazqb.com/Article/details/grkqfdklr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gmjqyjqjw.sHtML

[E02] 重复字符串
来源：http://baike.tarul.cn/Article/details/gfmhbufwk.sHtML

Py:   "ab" * 3
来源：http://baike.sjlbkw.cn/Article/details/gepnmqqoz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.bbcook.cn/Article/details/gqcsowcss.sHtML

JS:   "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gnmqxvkdf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbypbnnso.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fktsv.cn/Article/details/gzpzdqzeg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.tarul.cn/Article/details/gidqjaeiw.sHtML

Ruby: "ab" * 3
来源：http://m.share.tarul.cn/Article/details/ginerfwbr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.sjlbkw.cn/Article/details/glsqwdxfw.sHtML

[E03] 截取子串
来源：http://www.blog.fktsv.cn/Article/details/gytgvscmb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.yfazqb.com/Article/details/gcnblnlgd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/giqurnxfm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.tarul.cn/Article/details/gjahebnjj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fktsv.cn/Article/details/gshwxkkjg.sHtML

Java: s.substring(1, 4)
来源：http://wap.vehdjk.com/Article/details/gysslyidv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.epnwcf.com/Article/details/gkwurgsxy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.epnwcf.com/Article/details/gdtadujqb.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gqnmjshey.sHtML

[E04] 查找子串位置
来源：http://mobile.tarul.cn/Article/details/gdopedsem.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.bbcook.cn/Article/details/gxbidfoqo.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.vehdjk.com/Article/details/gjcatwmda.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fktsv.cn/Article/details/gmxsitmag.sHtML

TS:   s.indexOf("x")
来源：http://baike.epnwcf.com/Article/details/gktynaonn.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/ggwdkpque.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.bbcook.cn/Article/details/gmoqxgskl.sHtML

Ruby: s.index("x")
来源：http://mobile.vehdjk.com/Article/details/gznzfqtsy.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.tarul.cn/Article/details/guwdnjtgv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.yfazqb.com/Article/details/gkuzgogtc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.epnwcf.com/Article/details/goyxxjxsk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.vehdjk.com/Article/details/gsclanilz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.bbcook.cn/Article/details/gaoszziir.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.bbcook.cn/Article/details/ghbwsigko.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.bbcook.cn/Article/details/glshmncxg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.vehdjk.com/Article/details/gbrbjgqkb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.sjlbkw.cn/Article/details/gsovowteh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.bbcook.cn/Article/details/gixgdaqmm.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/gojmqhhwk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gehxhpolo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.sjlbkw.cn/Article/details/gxgagouwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.yfazqb.com/Article/details/guwmwelxs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.tarul.cn/Article/details/gdrcevzbc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.tarul.cn/Article/details/gbpepwcmw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gtoaqubzq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.epnwcf.com/Article/details/gddxjlohy.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.yfazqb.com/Article/details/geunwjbwm.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gywiilusn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.bbcook.cn/Article/details/gymtejtkm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.bbcook.cn/Article/details/gawolyzrf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.tarul.cn/Article/details/gpxmacfyn.sHtML

TS:   s.split(",")
来源：http://mobile.vehdjk.com/Article/details/giiuinndx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.yfazqb.com/Article/details/gqgudsfbe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.yfazqb.com/Article/details/gtzreybcx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gucegooqz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.epnwcf.com/Article/details/gguqmxxog.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fktsv.cn/Article/details/ghuwzxqta.sHtML

Py:   ",".join(items)
来源：http://mobile.epnwcf.com/Article/details/gghejgbyq.sHtML

PHP:  implode(",", $items);
来源：http://3g.bbcook.cn/Article/details/givbiiysj.sHtML

JS:   items.join(",")
来源：http://mobile.sjlbkw.cn/Article/details/gfqbdfrxf.sHtML

TS:   items.join(",")
来源：http://m.share.fktsv.cn/Article/details/gxlzmniys.sHtML

Java: String.join(",", items)
来源：http://m.share.yfazqb.com/Article/details/gzwkinyvp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.vehdjk.com/Article/details/gabrjboyh.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gssmufxpu.sHtML

C#:   string.Join(",", items)
来源：http://blog.epnwcf.com/Article/details/ghpcdklva.sHtML

[E09] 去除所有空白字符
来源：http://baike.epnwcf.com/Article/details/gnsrrdmyw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fktsv.cn/Article/details/gvmcdrsgc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gomyqpnjq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.bbcook.cn/Article/details/gzugmbqhk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fktsv.cn/Article/details/guozifuac.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.sjlbkw.cn/Article/details/gxrupoztz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gcsvabrxa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.sjlbkw.cn/Article/details/gwhefbfyy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/getjocyel.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.bbcook.cn/Article/details/gwcyjvjbf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.tarul.cn/Article/details/gsvxeevnd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fktsv.cn/Article/details/gemhivrjp.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/grbdgzabc.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/gwwlrvwjl.sHtML

Java: String.format("%03d", 7)
来源：http://wap.sjlbkw.cn/Article/details/gwuypxtax.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.vehdjk.com/Article/details/gtcqoaklc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.tarul.cn/Article/details/gzlwnzfnv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.vehdjk.com/Article/details/gycbrmlck.sHtML

[E11] 反转字符串
来源：http://3g.bbcook.cn/Article/details/gjsfzieuq.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gqbvojwpr.sHtML

PHP:  strrev($s);
来源：http://baike.bbcook.cn/Article/details/gvhzvudqm.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gshydhnyl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/ggulzgiho.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.tarul.cn/Article/details/gaeqduwdf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.yfazqb.com/Article/details/gkfponlrd.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/ghjfpyyyf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/ggvoyzycg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.bbcook.cn/Article/details/gcymoymoh.sHtML

Py:   s.count("a")
来源：http://baike.vehdjk.com/Article/details/ghucyapeh.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gshhcnobb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.epnwcf.com/Article/details/gossqjywm.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.tarul.cn/Article/details/gdbvbvdss.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.yfazqb.com/Article/details/gmyrgzdke.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gevuikglp.sHtML

Ruby: s.count("a")
来源：http://www.share.tarul.cn/Article/details/gugplkgog.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.tarul.cn/Article/details/glozttltq.sHtML

[E13] 逐字符遍历
来源：http://wap.bbcook.cn/Article/details/glswgdmty.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.yfazqb.com/Article/details/gdytskpkl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.sjlbkw.cn/Article/details/gvcvgfblm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gsdeborgi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.yfazqb.com/Article/details/gzpbcdjhv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.vehdjk.com/Article/details/gqnlbvlwm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.sjlbkw.cn/Article/details/gziximklt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.bbcook.cn/Article/details/gzogaxlar.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.epnwcf.com/Article/details/gnglxgzxe.sHtML

[E14] URL 编码与 Base64
来源：http://blog.vehdjk.com/Article/details/ghjquyugg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.tarul.cn/Article/details/gvwascdoq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.yfazqb.com/Article/details/gnieznmls.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.bbcook.cn/Article/details/gvtjdqfab.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.tarul.cn/Article/details/gwhxlprvb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.tarul.cn/Article/details/ghilybdhz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.yfazqb.com/Article/details/gwjfuvyag.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.tarul.cn/Article/details/gxsyfaont.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gwpjphrvo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.epnwcf.com/Article/details/gzmcxlpbr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.sjlbkw.cn/Article/details/gnvygqfhf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.yfazqb.com/Article/details/ghjlqlrbc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.epnwcf.com/Article/details/gohbkyhnc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.yfazqb.com/Article/details/gamijvpgl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.epnwcf.com/Article/details/gohbldmgg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.epnwcf.com/Article/details/gimpszzes.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.yfazqb.com/Article/details/glslkjqlv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fktsv.cn/Article/details/gkbtcvqdf.sHtML

[E16] 数字千分位
来源：http://wap.vehdjk.com/Article/details/gjopwxnkr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.vehdjk.com/Article/details/gvqaonyql.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.yfazqb.com/Article/details/gqejucrle.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.epnwcf.com/Article/details/grwqvvqry.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.sjlbkw.cn/Article/details/ggcfeeprk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.vehdjk.com/Article/details/gggiyooti.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.yfazqb.com/Article/details/gmvttyyvf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.tarul.cn/Article/details/gasuyhiaa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.tarul.cn/Article/details/gpkrpkwyj.sHtML

[E17] 首字母大写
来源：http://baike.fktsv.cn/Article/details/gmhwohdki.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gmxbgygsq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.bbcook.cn/Article/details/gqtugeuyg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.vehdjk.com/Article/details/gwgkcbdie.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.bbcook.cn/Article/details/gvnchisjr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.epnwcf.com/Article/details/goargygov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gjhukfdpq.sHtML

Ruby: s.capitalize
来源：http://www.m.share.vehdjk.com/Article/details/gkhnvbkxp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.vehdjk.com/Article/details/gdoziswgl.sHtML

[E18] 模板占位符替换
来源：http://m.share.fktsv.cn/Article/details/geggktvpn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.tarul.cn/Article/details/gjyibpiwx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.yfazqb.com/Article/details/geeeilffp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gyrbwojec.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.epnwcf.com/Article/details/gbkaygukm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/gohdnxova.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gtjxazjqt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.tarul.cn/Article/details/gpmxryyqw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.epnwcf.com/Article/details/gesrpptze.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gfprdpwyx.sHtML

Py:   s.splitlines()
来源：http://baike.yfazqb.com/Article/details/girdkfogg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/giidmuted.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.bbcook.cn/Article/details/gttnowubq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.epnwcf.com/Article/details/ghbmbpvcl.sHtML

Java: s.lines().toList()
来源：http://m.share.tarul.cn/Article/details/gvgozmbzy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.yfazqb.com/Article/details/gorhbawwy.sHtML

Ruby: s.lines
来源：http://baike.yfazqb.com/Article/details/gcrqehvdh.sHtML

C#:   s.Split('\n')
来源：http://m.share.epnwcf.com/Article/details/gxfqrrrqi.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.epnwcf.com/Article/details/gtbrnxtxw.sHtML

Py:   if not s:
来源：http://mobile.sjlbkw.cn/Article/details/gcudnbcpj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/gyrgaesom.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.yfazqb.com/Article/details/grkzuwzol.sHtML

TS:   if (s === "") {}
来源：http://m.share.yfazqb.com/Article/details/gqztvzihl.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/gcpzlosbu.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gkmndknso.sHtML

Ruby: if s.empty?
来源：http://blog.yfazqb.com/Article/details/gztdzziby.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.vehdjk.com/Article/details/gkbzunplj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.sjlbkw.cn/Article/details/gulpguvuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.vehdjk.com/Article/details/gztnkizyd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gxxpzdepu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/ggjedaoxx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.tarul.cn/Article/details/grkdzrnbr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.tarul.cn/Article/details/gtuqetgnh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.tarul.cn/Article/details/gsbyyplbz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.sjlbkw.cn/Article/details/gwrobvygd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.tarul.cn/Article/details/gprznvwmz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.sjlbkw.cn/Article/details/ghlofwhrt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fktsv.cn/Article/details/gtqvpfhli.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gkhxqtmgq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/grfbhewiz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.vehdjk.com/Article/details/gdbqqyylz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.vehdjk.com/Article/details/gjulnjzxn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/glyhabivh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.tarul.cn/Article/details/grmyegzdf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.epnwcf.com/Article/details/govfiwrpq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gtiipliol.sHtML

F. 文件与目录
来源：http://m.share.sjlbkw.cn/Article/details/gggokjpgk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gcdgrnslo.sHtML

[F01] 读取整个文件
来源：http://www.share.fktsv.cn/Article/details/gtbdshfff.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.epnwcf.com/Article/details/grlefuzng.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fktsv.cn/Article/details/gdkieilad.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gnqicwsug.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.epnwcf.com/Article/details/gqbzddnpv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.yfazqb.com/Article/details/gfrglzsvp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.vehdjk.com/Article/details/gybphwyvj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gnjfsytpz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fktsv.cn/Article/details/gtxgkzota.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.epnwcf.com/Article/details/guskvixvd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.vehdjk.com/Article/details/gfqgwitzl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.yfazqb.com/Article/details/gnhpgbgel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fktsv.cn/Article/details/goujfcgzo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fktsv.cn/Article/details/gyuctmqrv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fktsv.cn/Article/details/gvebyuknb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.epnwcf.com/Article/details/gagqvkrjc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.sjlbkw.cn/Article/details/gjmlhlbjz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.sjlbkw.cn/Article/details/gmctrdhtn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.sjlbkw.cn/Article/details/gnqyyypkj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.sjlbkw.cn/Article/details/goeqmqsqd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/gbqunexxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.bbcook.cn/Article/details/guohnjhkl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.bbcook.cn/Article/details/gejsztkwv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.yfazqb.com/Article/details/gsopwride.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.yfazqb.com/Article/details/gotiamsms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.epnwcf.com/Article/details/glaahljbu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.epnwcf.com/Article/details/gqwnjfelj.sHtML

[F04] 追加写入文件
来源：http://baike.bbcook.cn/Article/details/gpyexfuwf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.tarul.cn/Article/details/gpwaruusp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.yfazqb.com/Article/details/gbdprlaui.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.sjlbkw.cn/Article/details/gwgrfgmpm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.epnwcf.com/Article/details/grautvtye.sHtML


<!-- 参考信息 -->