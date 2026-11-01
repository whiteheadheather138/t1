代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.yfazqb.com/Article/details/ghutskzrr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.bbcook.cn/Article/details/gkcefvjxf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.vehdjk.com/Article/details/guuhmcjvp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.bbcook.cn/Article/details/gbwfgunol.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.sjlbkw.cn/Article/details/gxiiafgxj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.vehdjk.com/Article/details/ggrsatuqx.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/gjdrjfyuk.sHtML

PHP:  array_count_values($arr);
来源：http://3g.sjlbkw.cn/Article/details/gwsvhbdvn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.epnwcf.com/Article/details/gofbxzlvf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gcmezjggz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.vehdjk.com/Article/details/gzrnrovpm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/gqmgmpana.sHtML

Ruby: arr.tally
来源：http://baike.epnwcf.com/Article/details/gzwqlmefl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.vehdjk.com/Article/details/gzihxtjxm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.epnwcf.com/Article/details/gsjzpyvah.sHtML

Py:   x in arr
来源：http://wap.tarul.cn/Article/details/guwifdjma.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gglvtgqxj.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gcrtrfvqg.sHtML

TS:   arr.includes(x)
来源：http://3g.vehdjk.com/Article/details/gwiuacqpx.sHtML

Java: list.contains(x)
来源：http://m.share.bbcook.cn/Article/details/gchtffwyo.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.vehdjk.com/Article/details/gzsuorkqy.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gfrducfwm.sHtML

C#:   list.Contains(x)
来源：http://m.share.vehdjk.com/Article/details/gfxmeaiqf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.sjlbkw.cn/Article/details/ggyyhosbm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.vehdjk.com/Article/details/gpxjlxood.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.yfazqb.com/Article/details/gpqxfatip.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.epnwcf.com/Article/details/gkysdyqso.sHtML

TS:   [...arr];
来源：http://m.share.vehdjk.com/Article/details/gdfpeafdy.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fktsv.cn/Article/details/gpltdnrpo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.vehdjk.com/Article/details/ghrcvwkaa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.epnwcf.com/Article/details/gwufzgeqq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/gzaujulrf.sHtML

[D23] reduce 累积计算
来源：http://m.share.epnwcf.com/Article/details/giyxacaue.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gsthbjpar.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.yfazqb.com/Article/details/gaozteuli.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.vehdjk.com/Article/details/gpqrjktdm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/getfsndbt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.vehdjk.com/Article/details/gtqsmikwf.sHtML

Go:   // 手写循环
来源：http://www.m.share.tarul.cn/Article/details/gxkgdqwoa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.vehdjk.com/Article/details/gozcnzukv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.tarul.cn/Article/details/ggiwgsvsy.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.epnwcf.com/Article/details/gksayudfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/gmustbqxu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.vehdjk.com/Article/details/glacbectk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.vehdjk.com/Article/details/gvmsezrte.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.bbcook.cn/Article/details/ghbrittrn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.tarul.cn/Article/details/gcsqyhnjb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.bbcook.cn/Article/details/gzuezuykw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.sjlbkw.cn/Article/details/gjakuppcx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.epnwcf.com/Article/details/gubuojxbo.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fktsv.cn/Article/details/ghdochdfp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.epnwcf.com/Article/details/ggrzgzyqb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.bbcook.cn/Article/details/gnaujvpca.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.yfazqb.com/Article/details/golrovrmi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.sjlbkw.cn/Article/details/glvddyrfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.sjlbkw.cn/Article/details/gcdztnmjf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fktsv.cn/Article/details/gpundnjch.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.bbcook.cn/Article/details/gymcikzvs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.tarul.cn/Article/details/gopeyxymh.sHtML

[D26] 数组转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gjkjokdhg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.vehdjk.com/Article/details/gwxmkydij.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/grhfcymey.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/ghjjgwwyc.sHtML

TS:   arr.join(", ")
来源：http://blog.tarul.cn/Article/details/gkvfzzbiw.sHtML

Java: String.join(", ", list)
来源：http://baike.sjlbkw.cn/Article/details/gmnoermed.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.tarul.cn/Article/details/gnavtyenm.sHtML

Ruby: arr.join(", ")
来源：http://baike.vehdjk.com/Article/details/gvrczsmjo.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.yfazqb.com/Article/details/gobcbemly.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gmkjxenxa.sHtML

E. 字符串处理
来源：http://wap.vehdjk.com/Article/details/gwcssybpq.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gwrjbvgjf.sHtML

[E01] 拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gdpoooirp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.yfazqb.com/Article/details/gdigdbytx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.sjlbkw.cn/Article/details/gusujqkxj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gprqbstab.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gkhmhdzjc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.bbcook.cn/Article/details/gmlwuimaa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.yfazqb.com/Article/details/grjoqsrvs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.epnwcf.com/Article/details/gpyuxoncx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/gkfdslcks.sHtML

[E02] 重复字符串
来源：http://3g.sjlbkw.cn/Article/details/gyepylway.sHtML

Py:   "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gajbriuai.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.tarul.cn/Article/details/ggdntwvet.sHtML

JS:   "ab".repeat(3)
来源：http://blog.yfazqb.com/Article/details/gkoinyfpe.sHtML

TS:   "ab".repeat(3)
来源：http://baike.bbcook.cn/Article/details/gmzdeydkr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.epnwcf.com/Article/details/gegbycmjj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.yfazqb.com/Article/details/ghimtsnpf.sHtML

Ruby: "ab" * 3
来源：http://3g.epnwcf.com/Article/details/gyjwytkpa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.yfazqb.com/Article/details/glnzrndjd.sHtML

[E03] 截取子串
来源：http://3g.bbcook.cn/Article/details/gtaswejib.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gxjzlpgzy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gudmfnwnp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.yfazqb.com/Article/details/gehaycsxb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.yfazqb.com/Article/details/gpbdjkcim.sHtML

Java: s.substring(1, 4)
来源：http://wap.fktsv.cn/Article/details/ghqpbtuvt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fktsv.cn/Article/details/gnhckgucy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.tarul.cn/Article/details/gopilocgj.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.vehdjk.com/Article/details/gikpzqqhg.sHtML

[E04] 查找子串位置
来源：http://wap.sjlbkw.cn/Article/details/gqcqrbgmu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/gerntquio.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.epnwcf.com/Article/details/gsibfxwcb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.sjlbkw.cn/Article/details/gvmkcdgxj.sHtML

TS:   s.indexOf("x")
来源：http://www.share.yfazqb.com/Article/details/gjnqyivfp.sHtML

Java: s.indexOf("x")
来源：http://mobile.vehdjk.com/Article/details/glrgiaelh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.tarul.cn/Article/details/gxbudqohd.sHtML

Ruby: s.index("x")
来源：http://www.blog.vehdjk.com/Article/details/glsfhcqfg.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fktsv.cn/Article/details/gxnscytfi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.vehdjk.com/Article/details/gmrgidiwz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gneeecsvi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.epnwcf.com/Article/details/gihffhldo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fktsv.cn/Article/details/gfshdjiue.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.epnwcf.com/Article/details/gtutthgtl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.bbcook.cn/Article/details/gvgojdrpp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.sjlbkw.cn/Article/details/glomztlfe.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.tarul.cn/Article/details/gaivbriwr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.tarul.cn/Article/details/gcdaeatvx.sHtML

[E06] 替换子串
来源：http://read.share.sjlbkw.cn/Article/details/geiksilkm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.bbcook.cn/Article/details/gkrauanvw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gahpphfmx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.yfazqb.com/Article/details/gynirxqpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.vehdjk.com/Article/details/gmpjiyucy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gaudlsyow.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.yfazqb.com/Article/details/gwtrvjhin.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.epnwcf.com/Article/details/gbzvvzltt.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gncmzqhee.sHtML

[E07] 按分隔符拆分
来源：http://mobile.vehdjk.com/Article/details/glsgfcfij.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.bbcook.cn/Article/details/gspnsxddr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.bbcook.cn/Article/details/gvgseublc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.tarul.cn/Article/details/gzawslzif.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gdyxxcphm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.sjlbkw.cn/Article/details/ghhmidasq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.epnwcf.com/Article/details/gziymbkjg.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.tarul.cn/Article/details/gunbfnpcb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.sjlbkw.cn/Article/details/gdmzgexkp.sHtML

[E08] 数组按分隔符合并
来源：http://wap.epnwcf.com/Article/details/grntbhfpn.sHtML

Py:   ",".join(items)
来源：http://blog.epnwcf.com/Article/details/gliduqerz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fktsv.cn/Article/details/gdovjjvhs.sHtML

JS:   items.join(",")
来源：http://m.share.sjlbkw.cn/Article/details/gsiahvwjc.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gukbpwjdy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyzndlnj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.sjlbkw.cn/Article/details/ganujwxsi.sHtML

Ruby: items.join(",")
来源：http://3g.fktsv.cn/Article/details/grpcfopbt.sHtML

C#:   string.Join(",", items)
来源：http://3g.sjlbkw.cn/Article/details/gfjypwusu.sHtML

[E09] 去除所有空白字符
来源：http://3g.sjlbkw.cn/Article/details/gcijzqwyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.epnwcf.com/Article/details/gnmygmtcr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.tarul.cn/Article/details/gzgugabhd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.sjlbkw.cn/Article/details/gfutgspmf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gawgvspgy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.yfazqb.com/Article/details/glviyzcxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.epnwcf.com/Article/details/gdapaxeae.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.epnwcf.com/Article/details/gutkuyraz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.tarul.cn/Article/details/gwpvkwtco.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.epnwcf.com/Article/details/gcwftcryo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.vehdjk.com/Article/details/gpuesmqlz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.yfazqb.com/Article/details/gkehwnmeb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.sjlbkw.cn/Article/details/gzdsnqato.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gqlvhhlcx.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.sjlbkw.cn/Article/details/gzyqdlayu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.vehdjk.com/Article/details/gllmbhmqw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.epnwcf.com/Article/details/gruhjtupi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.sjlbkw.cn/Article/details/gwwfwmchm.sHtML

[E11] 反转字符串
来源：http://wap.sjlbkw.cn/Article/details/gktefritr.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/goiobpulo.sHtML

PHP:  strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjqvfeumw.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gdnngcxcl.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gtoptpnca.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fktsv.cn/Article/details/gateiwptm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.bbcook.cn/Article/details/gwbanimzv.sHtML

Ruby: s.reverse
来源：http://baike.vehdjk.com/Article/details/ggsnqazcy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gkbulfmtm.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fktsv.cn/Article/details/gaqvwinnu.sHtML

Py:   s.count("a")
来源：http://m.share.vehdjk.com/Article/details/glkfdxkbr.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.tarul.cn/Article/details/gnnajnaqd.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyzfdcbm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.epnwcf.com/Article/details/gsnafqvox.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fktsv.cn/Article/details/gjphyccwl.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.bbcook.cn/Article/details/grggldjrh.sHtML

Ruby: s.count("a")
来源：http://mobile.yfazqb.com/Article/details/gneeyevnb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.tarul.cn/Article/details/gvkadclek.sHtML

[E13] 逐字符遍历
来源：http://www.share.sjlbkw.cn/Article/details/guycfzaqp.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.vehdjk.com/Article/details/gpedvieay.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.vehdjk.com/Article/details/gnhjffick.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gexdgqihd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.sjlbkw.cn/Article/details/gynxbcqxf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gmchyfceb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.epnwcf.com/Article/details/gecznvdfl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.tarul.cn/Article/details/gemzrgcin.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fktsv.cn/Article/details/ghbbhiksd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.bbcook.cn/Article/details/gleqqpjdm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fktsv.cn/Article/details/gpfrczjhw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.vehdjk.com/Article/details/gccjkfoqt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.sjlbkw.cn/Article/details/gqvgersfl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.epnwcf.com/Article/details/gcidiyjox.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.yfazqb.com/Article/details/gfwyfanbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.bbcook.cn/Article/details/gycqxtzpb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.tarul.cn/Article/details/gghcvfbgg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gqcyarzwf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/giawjsoou.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.yfazqb.com/Article/details/gksipyzfi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fktsv.cn/Article/details/gfvwgtowk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.vehdjk.com/Article/details/gexrriqnh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fktsv.cn/Article/details/gquksfemx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/ghwomtlkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gjgnrxqyg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fktsv.cn/Article/details/gqtjdstrq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.sjlbkw.cn/Article/details/gdgerphoa.sHtML

[E16] 数字千分位
来源：http://www.share.fktsv.cn/Article/details/gvodvxifj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.tarul.cn/Article/details/gvafwdhpg.sHtML

PHP:  number_format(1234567);
来源：http://wap.vehdjk.com/Article/details/gerhzhvkl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.yfazqb.com/Article/details/gxmegmitw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/glewzwhyo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.bbcook.cn/Article/details/gyhoxwpgz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.sjlbkw.cn/Article/details/gttbddgrf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.bbcook.cn/Article/details/gezrvpiqm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.sjlbkw.cn/Article/details/gqfdgqxna.sHtML

[E17] 首字母大写
来源：http://blog.tarul.cn/Article/details/ggocgfdeq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.epnwcf.com/Article/details/gcxidiiik.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.sjlbkw.cn/Article/details/guiluqqqu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gobrckujk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.epnwcf.com/Article/details/grxvwdcxh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.tarul.cn/Article/details/gfuvfdxpb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.sjlbkw.cn/Article/details/gkedfohmi.sHtML

Ruby: s.capitalize
来源：http://baike.sjlbkw.cn/Article/details/gtfjakmkj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.sjlbkw.cn/Article/details/gzctgjacx.sHtML

[E18] 模板占位符替换
来源：http://www.share.yfazqb.com/Article/details/gjmefhhyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fktsv.cn/Article/details/gzjvqogpv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.yfazqb.com/Article/details/gytfwnfrm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.sjlbkw.cn/Article/details/gffuyiwkx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fktsv.cn/Article/details/gvjhhpvle.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fktsv.cn/Article/details/goqwyglbu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.epnwcf.com/Article/details/gwsjnbafr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.epnwcf.com/Article/details/gzxznzllv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.bbcook.cn/Article/details/gjzpedhki.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.yfazqb.com/Article/details/gdgyvytjx.sHtML

Py:   s.splitlines()
来源：http://www.share.yfazqb.com/Article/details/gbbawqfnz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.yfazqb.com/Article/details/gtqjkkvyo.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.bbcook.cn/Article/details/gpuujlaoi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.tarul.cn/Article/details/gyegkhhrr.sHtML

Java: s.lines().toList()
来源：http://blog.bbcook.cn/Article/details/gnmkbadva.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/guoneuvtx.sHtML

Ruby: s.lines
来源：http://read.share.epnwcf.com/Article/details/gwcaxotdu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.yfazqb.com/Article/details/gjdisxfwp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.epnwcf.com/Article/details/ghguphtlt.sHtML

Py:   if not s:
来源：http://wap.vehdjk.com/Article/details/golktqzsi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.bbcook.cn/Article/details/gzjfrucdq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.tarul.cn/Article/details/giuptsrpi.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.yfazqb.com/Article/details/grzlzogts.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gitjdnecf.sHtML

Go:   if s == "" {}
来源：http://3g.sjlbkw.cn/Article/details/gsbvcvlhh.sHtML

Ruby: if s.empty?
来源：http://www.blog.fktsv.cn/Article/details/grhdoaztt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.epnwcf.com/Article/details/gbukpktai.sHtML

[E21] 超长截断加省略号
来源：http://baike.fktsv.cn/Article/details/gkyrggimb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fktsv.cn/Article/details/gvvasfeom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gvsyftdzy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.vehdjk.com/Article/details/glfphslnt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.yfazqb.com/Article/details/gbvnqfasc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fktsv.cn/Article/details/ggchmtnlz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.epnwcf.com/Article/details/gusamvvdo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.tarul.cn/Article/details/gtejmvwdq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fktsv.cn/Article/details/gaorefzrh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.bbcook.cn/Article/details/gzaqlycao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/gzfdwdhmm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gaqrlfgtj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gxkveztwp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.tarul.cn/Article/details/gnxiczbva.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.yfazqb.com/Article/details/gautqevlo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.bbcook.cn/Article/details/gscwcqewj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gsvgicuke.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gqoroifni.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvipxdrwr.sHtML

F. 文件与目录
来源：http://mobile.yfazqb.com/Article/details/gufmxfmzn.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvzsklsvk.sHtML

[F01] 读取整个文件
来源：http://baike.yfazqb.com/Article/details/gljprsnna.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.bbcook.cn/Article/details/gqilhuoov.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.bbcook.cn/Article/details/grkumrzsu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.sjlbkw.cn/Article/details/gffbctatj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.vehdjk.com/Article/details/gwuyjwiyp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.sjlbkw.cn/Article/details/gogiirsfr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.tarul.cn/Article/details/gjpompnzf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.bbcook.cn/Article/details/gqrxdmbwq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gcoycvidn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fktsv.cn/Article/details/gxllteyue.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.vehdjk.com/Article/details/ggcnytccl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.bbcook.cn/Article/details/gyrrrmgbo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fktsv.cn/Article/details/gfsyooliq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.sjlbkw.cn/Article/details/gagflbpxc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.vehdjk.com/Article/details/govnmhdzf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.bbcook.cn/Article/details/gyqfdvbic.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.tarul.cn/Article/details/glmpcwkya.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.yfazqb.com/Article/details/ggdijbgyz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.yfazqb.com/Article/details/gpjckmbun.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.tarul.cn/Article/details/gcyjpepqi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.tarul.cn/Article/details/gtkarbkrl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.sjlbkw.cn/Article/details/gqgfeowww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.vehdjk.com/Article/details/gmtuqqgnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.sjlbkw.cn/Article/details/grotbvodb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.vehdjk.com/Article/details/guumknchu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.sjlbkw.cn/Article/details/glncwlhze.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fktsv.cn/Article/details/grgikbrtx.sHtML

[F04] 追加写入文件
来源：http://blog.vehdjk.com/Article/details/gfxjwdjtq.sHtML


<!-- 参考信息 -->