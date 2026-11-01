代发 wailian999

[D19] 按字段分组
来源：http://read.share.tarul.cn/Article/details/gjklgcvkp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fktsv.cn/Article/details/gmenrhclg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.sjlbkw.cn/Article/details/gcqucrpwl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.yfazqb.com/Article/details/gelvjxxrr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.yfazqb.com/Article/details/ghqunlgem.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.bbcook.cn/Article/details/galnnqndl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.vehdjk.com/Article/details/gvdnmgltg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.epnwcf.com/Article/details/gbpwtvvug.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.epnwcf.com/Article/details/gfdghufyt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.yfazqb.com/Article/details/gofqhaand.sHtML

Py:   Counter(arr)
来源：http://baike.tarul.cn/Article/details/gkdkvibha.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.epnwcf.com/Article/details/gfaxcnfds.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.vehdjk.com/Article/details/gzjycjsza.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/gjymfbbjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.vehdjk.com/Article/details/gemledwcm.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.bbcook.cn/Article/details/gpzkyssno.sHtML

Ruby: arr.tally
来源：http://wap.epnwcf.com/Article/details/grqvthjdn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fktsv.cn/Article/details/gphemjxzy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.tarul.cn/Article/details/gzvzawwlc.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/gcoypioey.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.tarul.cn/Article/details/gmcbyibiu.sHtML

JS:   arr.includes(x)
来源：http://3g.yfazqb.com/Article/details/gyhbbsfur.sHtML

TS:   arr.includes(x)
来源：http://mobile.sjlbkw.cn/Article/details/gctullfdc.sHtML

Java: list.contains(x)
来源：http://www.blog.tarul.cn/Article/details/gtvkcubkb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.tarul.cn/Article/details/gznhvpqrt.sHtML

Ruby: arr.include?(x)
来源：http://read.share.vehdjk.com/Article/details/gfzecjqzh.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gfqzyfrxy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.bbcook.cn/Article/details/gfbemghgs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.yfazqb.com/Article/details/gidztmkzo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.epnwcf.com/Article/details/gavlrlvoq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.bbcook.cn/Article/details/gjrmgquqq.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/gtradosgm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.bbcook.cn/Article/details/gpuubyqup.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.bbcook.cn/Article/details/gbxanttxp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.bbcook.cn/Article/details/givztbbve.sHtML

C#:   new List<int>(list);
来源：http://mobile.bbcook.cn/Article/details/gjxahsjaj.sHtML

[D23] reduce 累积计算
来源：http://read.share.fktsv.cn/Article/details/gqgzlauuw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.yfazqb.com/Article/details/gakwevndt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.sjlbkw.cn/Article/details/gbbvaksgw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fktsv.cn/Article/details/gnidsxfuk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.tarul.cn/Article/details/guxlrscgg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.tarul.cn/Article/details/grgdgaqlv.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/ggifxzbzz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fktsv.cn/Article/details/gvvcgbrev.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.vehdjk.com/Article/details/grupaieza.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.sjlbkw.cn/Article/details/gyidbwdxs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/galasrjws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/ggzdbcimm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.bbcook.cn/Article/details/grlgobvex.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gwsqmzfyq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fktsv.cn/Article/details/gbmifjvvi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/gdgefwple.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.epnwcf.com/Article/details/gfmwotdxq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.tarul.cn/Article/details/gaknmyhex.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.bbcook.cn/Article/details/grlprdeqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.sjlbkw.cn/Article/details/galtcvocf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.epnwcf.com/Article/details/gxvtmouxa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.yfazqb.com/Article/details/gipyfvwxd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.epnwcf.com/Article/details/gprmjtroh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fktsv.cn/Article/details/gcnodyluh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.bbcook.cn/Article/details/gzaoluous.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.sjlbkw.cn/Article/details/gwtwmcngi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gaxwwgvvd.sHtML

[D26] 数组转字符串
来源：http://www.m.share.tarul.cn/Article/details/gjygyohyr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.sjlbkw.cn/Article/details/gtkkzujbw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fktsv.cn/Article/details/gbfvofndf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gyaxfclzc.sHtML

TS:   arr.join(", ")
来源：http://mobile.epnwcf.com/Article/details/gmvxekrwq.sHtML

Java: String.join(", ", list)
来源：http://read.share.sjlbkw.cn/Article/details/gqlajstic.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.tarul.cn/Article/details/gyxsbfzkc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.sjlbkw.cn/Article/details/gnwfmbkjf.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fktsv.cn/Article/details/gyszhhfkh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzxsiikzj.sHtML

E. 字符串处理
来源：http://blog.tarul.cn/Article/details/gaklhhthm.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gasyhpxjg.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/ggyxszxnz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.vehdjk.com/Article/details/giuzpqqxl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.tarul.cn/Article/details/gyozrcwcx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.vehdjk.com/Article/details/gunycqekx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.sjlbkw.cn/Article/details/gyyoarwkg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fktsv.cn/Article/details/gkorbgccg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.sjlbkw.cn/Article/details/glwieysff.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.yfazqb.com/Article/details/gqrcxffsb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.tarul.cn/Article/details/grdzbwgpf.sHtML

[E02] 重复字符串
来源：http://3g.epnwcf.com/Article/details/gwpmsmvqe.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gefqwsqgf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.epnwcf.com/Article/details/gspoyleep.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.tarul.cn/Article/details/glvhvtmer.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gpnajqgrx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.tarul.cn/Article/details/gsyesticy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.vehdjk.com/Article/details/gqweojsps.sHtML

Ruby: "ab" * 3
来源：http://blog.bbcook.cn/Article/details/gcrmyvvzy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.epnwcf.com/Article/details/gisrpwfdg.sHtML

[E03] 截取子串
来源：http://wap.epnwcf.com/Article/details/gxqnldevx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.bbcook.cn/Article/details/gpqnakunw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gosamqpdk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.tarul.cn/Article/details/gffvzscoi.sHtML

TS:   s.slice(1, 4)
来源：http://blog.vehdjk.com/Article/details/glgdeifbi.sHtML

Java: s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/gtajkohfa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.sjlbkw.cn/Article/details/gxshlwnmb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.epnwcf.com/Article/details/gjixdzgmt.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.yfazqb.com/Article/details/gnoysdzsa.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/groofcfoc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.tarul.cn/Article/details/geexhxgko.sHtML

PHP:  strpos($s, "x");
来源：http://blog.yfazqb.com/Article/details/glcfpcppb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.tarul.cn/Article/details/gdazbtcjk.sHtML

TS:   s.indexOf("x")
来源：http://www.share.vehdjk.com/Article/details/gqvetikgd.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.epnwcf.com/Article/details/gsdkapjjs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.tarul.cn/Article/details/gyxcaqscs.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gaktxwpsl.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.tarul.cn/Article/details/gupmrxcfi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.epnwcf.com/Article/details/gsdzxmtxr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.tarul.cn/Article/details/gjdpmobyg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.bbcook.cn/Article/details/gwqnupxhk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.epnwcf.com/Article/details/giepwdkbf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.yfazqb.com/Article/details/glfmghhps.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.yfazqb.com/Article/details/gepswpjmf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.sjlbkw.cn/Article/details/grmevkcrp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.vehdjk.com/Article/details/gthelehwm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/ghkykmqnm.sHtML

[E06] 替换子串
来源：http://wap.fktsv.cn/Article/details/glutvoyaf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.bbcook.cn/Article/details/gvyjfyknq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.tarul.cn/Article/details/gvqdudlsq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gasgqckjv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/getuqgpmg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gndjpvezo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.tarul.cn/Article/details/gdjedpvab.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gcyyxrjuw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gnvkcfspc.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gvbjryzoc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fktsv.cn/Article/details/gleixxpit.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.tarul.cn/Article/details/gkktkfzhv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/ghjagszal.sHtML

TS:   s.split(",")
来源：http://m.share.bbcook.cn/Article/details/gpzkgqnoh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gwapkfcrx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fktsv.cn/Article/details/gycxrbvdu.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fktsv.cn/Article/details/gsadrgnse.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/glegqemmq.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.vehdjk.com/Article/details/gubqlanyr.sHtML

Py:   ",".join(items)
来源：http://read.share.vehdjk.com/Article/details/gdfzjlyzt.sHtML

PHP:  implode(",", $items);
来源：http://wap.sjlbkw.cn/Article/details/gruyezhbd.sHtML

JS:   items.join(",")
来源：http://www.share.bbcook.cn/Article/details/gsytzjcmw.sHtML

TS:   items.join(",")
来源：http://wap.fktsv.cn/Article/details/gojeyokuu.sHtML

Java: String.join(",", items)
来源：http://m.share.tarul.cn/Article/details/guseldvbk.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.bbcook.cn/Article/details/gkanpokli.sHtML

Ruby: items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gsemexwak.sHtML

C#:   string.Join(",", items)
来源：http://mobile.epnwcf.com/Article/details/gbmciaole.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.vehdjk.com/Article/details/geeduiiea.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtmxidjg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.sjlbkw.cn/Article/details/ghgsorgsq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/giixnrybw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.yfazqb.com/Article/details/ghopaquwf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/gyjaaveyy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.vehdjk.com/Article/details/gnqqxwzaj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.tarul.cn/Article/details/gjuxepezp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.sjlbkw.cn/Article/details/gjzznaazf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.epnwcf.com/Article/details/gcaasegwf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyjowrzt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.epnwcf.com/Article/details/gknwtokym.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.tarul.cn/Article/details/gczfrhwys.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.bbcook.cn/Article/details/gedcakdvg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gzbibqwsf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fktsv.cn/Article/details/gqhpmroia.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.vehdjk.com/Article/details/gmlaqmscs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.bbcook.cn/Article/details/gutkojvyg.sHtML

[E11] 反转字符串
来源：http://blog.yfazqb.com/Article/details/gfzlaoctz.sHtML

Py:   s[::-1]
来源：http://baike.epnwcf.com/Article/details/gvqckitdj.sHtML

PHP:  strrev($s);
来源：http://wap.fktsv.cn/Article/details/goyjeytge.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gcgfixmvy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gfgxfgwhj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.bbcook.cn/Article/details/guancewgj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/glslsoske.sHtML

Ruby: s.reverse
来源：http://blog.tarul.cn/Article/details/gtrjxivvs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gogiuquts.sHtML

[E12] 统计某字符出现次数
来源：http://blog.epnwcf.com/Article/details/gehqpxllq.sHtML

Py:   s.count("a")
来源：http://wap.tarul.cn/Article/details/gldpzvspi.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.sjlbkw.cn/Article/details/gdhwdgeec.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/guseezfcx.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.tarul.cn/Article/details/gtdwsqjtg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.vehdjk.com/Article/details/gkxerkbbz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.bbcook.cn/Article/details/gurwozhrx.sHtML

Ruby: s.count("a")
来源：http://blog.tarul.cn/Article/details/ggcdindsk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.yfazqb.com/Article/details/gdmylqhxd.sHtML

[E13] 逐字符遍历
来源：http://blog.fktsv.cn/Article/details/ggjmpsfxv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.sjlbkw.cn/Article/details/glqllcxga.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.tarul.cn/Article/details/gwbnixwpn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fktsv.cn/Article/details/glgsiqxin.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.epnwcf.com/Article/details/gkhhkerwr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.tarul.cn/Article/details/ghhfrlviv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.epnwcf.com/Article/details/gvtxvlhfu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.bbcook.cn/Article/details/guehsmlwj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gthoilzct.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.sjlbkw.cn/Article/details/gkzcgkfxk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/ghjdvabjj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.yfazqb.com/Article/details/grjlkagjg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.vehdjk.com/Article/details/gekihdwpm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.yfazqb.com/Article/details/gghyrgtkx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.vehdjk.com/Article/details/ggmjmyvfy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fktsv.cn/Article/details/gdicqdodl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.vehdjk.com/Article/details/grlcruxcy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gdyqqubea.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fktsv.cn/Article/details/gbxaetvcu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.bbcook.cn/Article/details/gabrszkyd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fktsv.cn/Article/details/ggtojezqd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gxnxedrya.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.yfazqb.com/Article/details/gitbbujba.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.tarul.cn/Article/details/gdohevutq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gdabtouvt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.epnwcf.com/Article/details/gudzuuczm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.bbcook.cn/Article/details/gdawdvulm.sHtML

[E16] 数字千分位
来源：http://read.share.yfazqb.com/Article/details/ghphkyxkv.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.bbcook.cn/Article/details/ggnnpyeti.sHtML

PHP:  number_format(1234567);
来源：http://baike.tarul.cn/Article/details/gapvuflds.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.yfazqb.com/Article/details/gcgxzgbru.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/gchhuqusz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.yfazqb.com/Article/details/gmznamzze.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.tarul.cn/Article/details/gflnsijwm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.epnwcf.com/Article/details/gkzbamorc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.epnwcf.com/Article/details/gyzkpyunh.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gysyryhxl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.epnwcf.com/Article/details/gehjxaosu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.sjlbkw.cn/Article/details/gfxlxjvxg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.sjlbkw.cn/Article/details/gsuotoebp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.bbcook.cn/Article/details/gkzwunarz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.epnwcf.com/Article/details/gvjvkbkra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gaqsxhbip.sHtML

Ruby: s.capitalize
来源：http://wap.fktsv.cn/Article/details/gbpccxrqv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.tarul.cn/Article/details/gjkevcdez.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/givlcboek.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.tarul.cn/Article/details/gwuewslor.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.yfazqb.com/Article/details/gqtmvenip.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.yfazqb.com/Article/details/gpyeendig.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.epnwcf.com/Article/details/gjxuaueml.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.yfazqb.com/Article/details/gtostusrc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fktsv.cn/Article/details/gpmsczlos.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fktsv.cn/Article/details/gjclylfkn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.bbcook.cn/Article/details/gsowecybp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.tarul.cn/Article/details/gvldohuck.sHtML

Py:   s.splitlines()
来源：http://www.blog.sjlbkw.cn/Article/details/gnmhgoypw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.tarul.cn/Article/details/gmsmbeqss.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.tarul.cn/Article/details/gugyghacu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.sjlbkw.cn/Article/details/gzirguacd.sHtML

Java: s.lines().toList()
来源：http://www.blog.vehdjk.com/Article/details/ghloypkma.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.bbcook.cn/Article/details/gpfsvrzyw.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gigaaqjhe.sHtML

C#:   s.Split('\n')
来源：http://wap.tarul.cn/Article/details/grvzgtneq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gpgliyxuf.sHtML

Py:   if not s:
来源：http://www.blog.vehdjk.com/Article/details/gktpwzmjc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.vehdjk.com/Article/details/ghurxsyqp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gxmdlzdpi.sHtML

TS:   if (s === "") {}
来源：http://baike.yfazqb.com/Article/details/goemtkwqs.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gxldnzmdr.sHtML

Go:   if s == "" {}
来源：http://wap.bbcook.cn/Article/details/gjrwkolnm.sHtML

Ruby: if s.empty?
来源：http://www.blog.sjlbkw.cn/Article/details/gelfokthr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fktsv.cn/Article/details/gxxbxdhuf.sHtML

[E21] 超长截断加省略号
来源：http://blog.sjlbkw.cn/Article/details/gtelgrssr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.yfazqb.com/Article/details/gbigofnky.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.yfazqb.com/Article/details/gfxgnuras.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.vehdjk.com/Article/details/gqcstfaff.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.bbcook.cn/Article/details/gstgvnyhy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.vehdjk.com/Article/details/gjibzxgfq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.tarul.cn/Article/details/govtwhfpt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.vehdjk.com/Article/details/gqstlyqzi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.tarul.cn/Article/details/gfzosxivw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/giwyxgnha.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.yfazqb.com/Article/details/gwcrhkmsq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gujtkkgdj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fktsv.cn/Article/details/gicodohfi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.sjlbkw.cn/Article/details/geuqpcrtr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gdchauowm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.bbcook.cn/Article/details/gozbzauoy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.sjlbkw.cn/Article/details/ghllzjuhw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.tarul.cn/Article/details/gowevcqrk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gxhgfbnhq.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gvxjzsslb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grddktenu.sHtML

[F01] 读取整个文件
来源：http://wap.vehdjk.com/Article/details/gzzyewnqz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.epnwcf.com/Article/details/gdxvgvjbh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.bbcook.cn/Article/details/gagpwotep.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.epnwcf.com/Article/details/glmyzoddu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.vehdjk.com/Article/details/gmfopvvfz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fktsv.cn/Article/details/gruzchdxb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.sjlbkw.cn/Article/details/glayyvgvg.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fktsv.cn/Article/details/ggodtxwcj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.vehdjk.com/Article/details/gclbckkhv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.yfazqb.com/Article/details/gijmlrayt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.bbcook.cn/Article/details/gezvxpjew.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gclayqivi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.yfazqb.com/Article/details/gxqqpdvaq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.epnwcf.com/Article/details/gcmfuixnf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.sjlbkw.cn/Article/details/gsvijgijt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.vehdjk.com/Article/details/gznwpjuaf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.vehdjk.com/Article/details/gadeaxpcy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.vehdjk.com/Article/details/gdfmhguii.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.tarul.cn/Article/details/geirmcnco.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.vehdjk.com/Article/details/gogqhiacb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.epnwcf.com/Article/details/gpckuwagq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gobleejmx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/gumqfwbsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fktsv.cn/Article/details/gzhabqlcc.sHtML


<!-- 参考信息 -->