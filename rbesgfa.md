代发 wailian999

[D19] 按字段分组
来源：http://read.share.fktsv.cn/Article/details/gguixmbch.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.epnwcf.com/Article/details/giuipjebq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.sjlbkw.cn/Article/details/gsfgiilpt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.tarul.cn/Article/details/gpenwwqfa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gewmnehkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.bbcook.cn/Article/details/gpkxfuggc.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.bbcook.cn/Article/details/gxuovytiu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.bbcook.cn/Article/details/godjcfxnp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.vehdjk.com/Article/details/gotabjrrv.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.yfazqb.com/Article/details/gfdjtyqxn.sHtML

Py:   Counter(arr)
来源：http://mobile.bbcook.cn/Article/details/glnxfjstd.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.bbcook.cn/Article/details/gchrrpzan.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fktsv.cn/Article/details/gbgcwuiat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.sjlbkw.cn/Article/details/geufalhsb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.bbcook.cn/Article/details/gyfvfmdij.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/gaoxlkpzt.sHtML

Ruby: arr.tally
来源：http://www.m.share.tarul.cn/Article/details/gjrvstgna.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.vehdjk.com/Article/details/grqzwuwlv.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.epnwcf.com/Article/details/gbovhpwhu.sHtML

Py:   x in arr
来源：http://m.share.yfazqb.com/Article/details/gnfwhkwid.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.tarul.cn/Article/details/gmvmozcto.sHtML

JS:   arr.includes(x)
来源：http://blog.fktsv.cn/Article/details/giwujttpa.sHtML

TS:   arr.includes(x)
来源：http://3g.bbcook.cn/Article/details/gtcntlprd.sHtML

Java: list.contains(x)
来源：http://blog.yfazqb.com/Article/details/gzkgcajzh.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.tarul.cn/Article/details/gryymixgj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gjrcnqunp.sHtML

C#:   list.Contains(x)
来源：http://baike.tarul.cn/Article/details/gkblhwhhq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.epnwcf.com/Article/details/gbojclcqe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.epnwcf.com/Article/details/giidyxcrp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.vehdjk.com/Article/details/gxmuwfcid.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/guwwzmtvs.sHtML

TS:   [...arr];
来源：http://3g.vehdjk.com/Article/details/goxxqwqpj.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gbnjavljr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.vehdjk.com/Article/details/goiyuczlb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.vehdjk.com/Article/details/gphjqvdie.sHtML

C#:   new List<int>(list);
来源：http://mobile.fktsv.cn/Article/details/ggdwkudqk.sHtML

[D23] reduce 累积计算
来源：http://mobile.epnwcf.com/Article/details/gwnlslbxv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.yfazqb.com/Article/details/garghhtkx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.tarul.cn/Article/details/gojtkanhb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.yfazqb.com/Article/details/glfovagxa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.epnwcf.com/Article/details/gcibbjrkr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gfyjthgaw.sHtML

Go:   // 手写循环
来源：http://blog.sjlbkw.cn/Article/details/gdthhjhjg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.sjlbkw.cn/Article/details/grqhaoooo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.bbcook.cn/Article/details/gcatxdbuc.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fktsv.cn/Article/details/guzimvgah.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.sjlbkw.cn/Article/details/gddzerwjf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.vehdjk.com/Article/details/gzpavwcfw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.tarul.cn/Article/details/gzjomrerr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.bbcook.cn/Article/details/gvoojovfi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.tarul.cn/Article/details/gdyetzvfb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.yfazqb.com/Article/details/gnobhpfvn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.epnwcf.com/Article/details/gaphoqllw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fktsv.cn/Article/details/gjcfxiita.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.yfazqb.com/Article/details/gbjxlqnbo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.epnwcf.com/Article/details/ghcysqpwp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/gwoaprchn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/gmssqcpok.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.sjlbkw.cn/Article/details/giramtony.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.epnwcf.com/Article/details/gqdgbjrtz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.tarul.cn/Article/details/gfcjxiwgs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.bbcook.cn/Article/details/geyflhlfc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.bbcook.cn/Article/details/gyuxgmqsz.sHtML

[D26] 数组转字符串
来源：http://blog.bbcook.cn/Article/details/gndvbcmcm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.bbcook.cn/Article/details/gedbujsvq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.tarul.cn/Article/details/gcifpsrue.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.bbcook.cn/Article/details/gfrwrzuux.sHtML

TS:   arr.join(", ")
来源：http://mobile.bbcook.cn/Article/details/gxfnjvigj.sHtML

Java: String.join(", ", list)
来源：http://www.share.epnwcf.com/Article/details/grjhewrvx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.sjlbkw.cn/Article/details/gospzdzge.sHtML

Ruby: arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gxngtferh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.tarul.cn/Article/details/gdlrelmkz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsgkkmnzq.sHtML

E. 字符串处理
来源：http://3g.yfazqb.com/Article/details/ggdxfnxyl.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwzlapkqn.sHtML

[E01] 拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gyvvyqaju.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.sjlbkw.cn/Article/details/gwkbkjrlo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fktsv.cn/Article/details/glzjbpaur.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.bbcook.cn/Article/details/gbauznunm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gzzamkmxx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gsolrnrpq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.tarul.cn/Article/details/goyozluej.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.epnwcf.com/Article/details/gwganxvpm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.bbcook.cn/Article/details/gzmgqoecg.sHtML

[E02] 重复字符串
来源：http://read.share.fktsv.cn/Article/details/gmnxtbvbz.sHtML

Py:   "ab" * 3
来源：http://mobile.fktsv.cn/Article/details/gicuzuhef.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.vehdjk.com/Article/details/guwfmdkci.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.epnwcf.com/Article/details/gpyplbudy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.vehdjk.com/Article/details/ggjporqbr.sHtML

Java: "ab".repeat(3)
来源：http://baike.tarul.cn/Article/details/gjqnsccuj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gjmvyhbrf.sHtML

Ruby: "ab" * 3
来源：http://m.share.fktsv.cn/Article/details/gksuxnlxz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.yfazqb.com/Article/details/gxoaxspmd.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gininycxi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fktsv.cn/Article/details/gwwrbybos.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfalyzbnh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.sjlbkw.cn/Article/details/gcynllgot.sHtML

TS:   s.slice(1, 4)
来源：http://blog.bbcook.cn/Article/details/gswrmuwaz.sHtML

Java: s.substring(1, 4)
来源：http://www.share.tarul.cn/Article/details/gayinhbyf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.bbcook.cn/Article/details/gwowsresf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/gxlxdznul.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.tarul.cn/Article/details/gxsidfarg.sHtML

[E04] 查找子串位置
来源：http://3g.epnwcf.com/Article/details/gapnnfcoy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.sjlbkw.cn/Article/details/gdopzlspr.sHtML

PHP:  strpos($s, "x");
来源：http://3g.sjlbkw.cn/Article/details/gsffwayjg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.sjlbkw.cn/Article/details/gjrjzslwn.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fktsv.cn/Article/details/golxcfejd.sHtML

Java: s.indexOf("x")
来源：http://blog.fktsv.cn/Article/details/gfqkuukod.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.vehdjk.com/Article/details/gclcdjvdw.sHtML

Ruby: s.index("x")
来源：http://read.share.sjlbkw.cn/Article/details/gcxtitwmg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.bbcook.cn/Article/details/gxtmcmgrj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/ghdkjwfvm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.vehdjk.com/Article/details/giikztynz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fktsv.cn/Article/details/gbqyeqruf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gyctcongs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gogmpcbtx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fktsv.cn/Article/details/gjjunepom.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fktsv.cn/Article/details/gczuupydc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/gmoqjgnbl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gbjfstvnz.sHtML

[E06] 替换子串
来源：http://wap.bbcook.cn/Article/details/gqujdkzus.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gwlbmfzky.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.epnwcf.com/Article/details/gagfnmpwe.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gfusyeeor.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gguyaoanz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fktsv.cn/Article/details/gcwihitwe.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.sjlbkw.cn/Article/details/gzcdiesys.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/gupuwkueh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gupfswyie.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/grjwkbqqw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.tarul.cn/Article/details/gbkvtogrv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.yfazqb.com/Article/details/gnigzlzwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.sjlbkw.cn/Article/details/gwirgvnbb.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gwcdihhov.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.epnwcf.com/Article/details/gohiuczps.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.vehdjk.com/Article/details/gkzmnrvht.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.bbcook.cn/Article/details/gjepczfux.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.epnwcf.com/Article/details/gqhilquuh.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.yfazqb.com/Article/details/gnyuikmzo.sHtML

Py:   ",".join(items)
来源：http://m.share.tarul.cn/Article/details/gvyfmgdpi.sHtML

PHP:  implode(",", $items);
来源：http://wap.fktsv.cn/Article/details/goofmbeck.sHtML

JS:   items.join(",")
来源：http://baike.fktsv.cn/Article/details/ghdjncmzu.sHtML

TS:   items.join(",")
来源：http://baike.sjlbkw.cn/Article/details/gvjtoaqio.sHtML

Java: String.join(",", items)
来源：http://mobile.fktsv.cn/Article/details/gxobouxym.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.vehdjk.com/Article/details/gnojulgyg.sHtML

Ruby: items.join(",")
来源：http://www.m.share.vehdjk.com/Article/details/gdlhcbztf.sHtML

C#:   string.Join(",", items)
来源：http://www.share.vehdjk.com/Article/details/gwtbezusk.sHtML

[E09] 去除所有空白字符
来源：http://3g.yfazqb.com/Article/details/gnwxthnpv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.yfazqb.com/Article/details/gfoinvmgk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gaerizosz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gsldmgqen.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.tarul.cn/Article/details/gxoermuou.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.bbcook.cn/Article/details/gqgfdjfwd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.epnwcf.com/Article/details/gbbsqnzvt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fktsv.cn/Article/details/gqjfzgyqo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.epnwcf.com/Article/details/gywaeokfx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.tarul.cn/Article/details/gnryzjkii.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fktsv.cn/Article/details/gcukjuqhx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.vehdjk.com/Article/details/gkkohgmst.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.sjlbkw.cn/Article/details/gjgbrsxjl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/ggmpmuggi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fktsv.cn/Article/details/gfoinysoo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.sjlbkw.cn/Article/details/gktkmlciv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/gebcdyptx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.bbcook.cn/Article/details/gnsiavwpe.sHtML

[E11] 反转字符串
来源：http://m.share.fktsv.cn/Article/details/gkgkbiars.sHtML

Py:   s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gamgxjieo.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gjqeanwir.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gjqutmvuj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gugzmmckf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fktsv.cn/Article/details/gdrgkdttv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fktsv.cn/Article/details/gargwnypm.sHtML

Ruby: s.reverse
来源：http://wap.vehdjk.com/Article/details/guyuqvebz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gkpxkwqix.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.tarul.cn/Article/details/gtqoicznn.sHtML

Py:   s.count("a")
来源：http://mobile.bbcook.cn/Article/details/gefcyqifz.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfbvozjc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fktsv.cn/Article/details/gwrcshleo.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fktsv.cn/Article/details/gkkmsjxxm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.epnwcf.com/Article/details/gycxdvult.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.bbcook.cn/Article/details/gesbmrsbt.sHtML

Ruby: s.count("a")
来源：http://m.share.vehdjk.com/Article/details/gvrespiii.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.bbcook.cn/Article/details/gowjhqedr.sHtML

[E13] 逐字符遍历
来源：http://m.share.fktsv.cn/Article/details/gsrqdbnyi.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.yfazqb.com/Article/details/gqpizgenp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.sjlbkw.cn/Article/details/gqhslbxkg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.sjlbkw.cn/Article/details/gkhwkkigc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.sjlbkw.cn/Article/details/gusyxixuq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.yfazqb.com/Article/details/gaveovuyc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsotwsoj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.yfazqb.com/Article/details/ggewvqvpf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.vehdjk.com/Article/details/gyslhzzhi.sHtML

[E14] URL 编码与 Base64
来源：http://baike.bbcook.cn/Article/details/gyenhjuvg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fktsv.cn/Article/details/gyyvxdhus.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.sjlbkw.cn/Article/details/gcrmxmhvs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/gzomntnyf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.vehdjk.com/Article/details/geiufslji.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.yfazqb.com/Article/details/gtejsuaal.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fktsv.cn/Article/details/gubinhoxr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.bbcook.cn/Article/details/gcxiwylru.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.bbcook.cn/Article/details/gozkdbqog.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.tarul.cn/Article/details/ggtyeeupy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.vehdjk.com/Article/details/gysuciwlc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.sjlbkw.cn/Article/details/gqbfgrbiz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.vehdjk.com/Article/details/gitzcogiu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fktsv.cn/Article/details/gtadicukg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.sjlbkw.cn/Article/details/gbxlnatno.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.tarul.cn/Article/details/grwhpvbzl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.yfazqb.com/Article/details/guzlsgwmk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.bbcook.cn/Article/details/gxypmdnxe.sHtML

[E16] 数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gqykoxlyr.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.bbcook.cn/Article/details/gneglruqk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.tarul.cn/Article/details/geruiiwhi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.yfazqb.com/Article/details/gvkjdzfrb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.yfazqb.com/Article/details/gklwpgret.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/garuvcmkn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/goclpwzel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/geokujway.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.yfazqb.com/Article/details/gqtowqrgz.sHtML

[E17] 首字母大写
来源：http://wap.tarul.cn/Article/details/grgujilvy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.sjlbkw.cn/Article/details/guctceppb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.yfazqb.com/Article/details/gbddxeiud.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.bbcook.cn/Article/details/gtgetzeyd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.epnwcf.com/Article/details/gnkzbcyih.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.vehdjk.com/Article/details/gbjubaqmg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.bbcook.cn/Article/details/gsvrautyy.sHtML

Ruby: s.capitalize
来源：http://m.share.vehdjk.com/Article/details/gasaoxcqz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fktsv.cn/Article/details/grvfzksxq.sHtML

[E18] 模板占位符替换
来源：http://baike.tarul.cn/Article/details/gkeuomixh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.sjlbkw.cn/Article/details/gnxwuqjdt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.vehdjk.com/Article/details/gaykgywxy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.bbcook.cn/Article/details/gnrxsbmdk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.yfazqb.com/Article/details/gocnnlryr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/ghqgoiicd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.tarul.cn/Article/details/gphwclzep.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.yfazqb.com/Article/details/gzftjgfqa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gihxvrunb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fktsv.cn/Article/details/gndaocwzs.sHtML

Py:   s.splitlines()
来源：http://3g.yfazqb.com/Article/details/granhfdwf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.vehdjk.com/Article/details/gqrjtcdwj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.bbcook.cn/Article/details/gixmjwdvb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.epnwcf.com/Article/details/gpkqevmib.sHtML

Java: s.lines().toList()
来源：http://blog.epnwcf.com/Article/details/gdypojcgk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.sjlbkw.cn/Article/details/glskufbbl.sHtML

Ruby: s.lines
来源：http://www.blog.sjlbkw.cn/Article/details/gtxtyawhf.sHtML

C#:   s.Split('\n')
来源：http://baike.yfazqb.com/Article/details/gftgronds.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.yfazqb.com/Article/details/gwtowhvjg.sHtML

Py:   if not s:
来源：http://baike.fktsv.cn/Article/details/gzwksqmsu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fktsv.cn/Article/details/gbgmokpqk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.vehdjk.com/Article/details/gjmzfyvkm.sHtML

TS:   if (s === "") {}
来源：http://wap.sjlbkw.cn/Article/details/gkfytrvnq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gvtcymvsc.sHtML

Go:   if s == "" {}
来源：http://read.share.fktsv.cn/Article/details/gzyjcdzzf.sHtML

Ruby: if s.empty?
来源：http://mobile.vehdjk.com/Article/details/griiygpyh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.yfazqb.com/Article/details/ggjvigfwl.sHtML

[E21] 超长截断加省略号
来源：http://blog.yfazqb.com/Article/details/gpunnnqsj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.epnwcf.com/Article/details/gqzkjhssh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gcgrnnwis.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/glpzapvjp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fktsv.cn/Article/details/gucgffjpv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtyzlwwz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.bbcook.cn/Article/details/gmynxgqaq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.sjlbkw.cn/Article/details/gxbdsgovh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fktsv.cn/Article/details/gintsjjoz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.bbcook.cn/Article/details/gzxctpcri.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.bbcook.cn/Article/details/grjohpglv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/giaxnhnba.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.tarul.cn/Article/details/ggmpzrbyb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.yfazqb.com/Article/details/gjlwrcvzu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.yfazqb.com/Article/details/gewprmyyf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gjlenhwif.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.sjlbkw.cn/Article/details/gpcpzcect.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.tarul.cn/Article/details/gjpfcidmm.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gyqxvralh.sHtML

F. 文件与目录
来源：http://blog.yfazqb.com/Article/details/ghjpdcgpx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gufbyldbx.sHtML

[F01] 读取整个文件
来源：http://www.blog.bbcook.cn/Article/details/gakufzwly.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.bbcook.cn/Article/details/girinpikf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.tarul.cn/Article/details/gfyyykzvu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fktsv.cn/Article/details/gszfadzou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.yfazqb.com/Article/details/ggzgwwvqh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.yfazqb.com/Article/details/gvdomkyot.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.bbcook.cn/Article/details/grlrkrhbk.sHtML

Ruby: File.read("a.txt")
来源：http://wap.sjlbkw.cn/Article/details/gpknkiosh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.tarul.cn/Article/details/glmnbnvaw.sHtML

[F02] 逐行读取文件
来源：http://3g.tarul.cn/Article/details/ggcbjvycx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.yfazqb.com/Article/details/ghsrqpfqb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.epnwcf.com/Article/details/gjtiondxf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.bbcook.cn/Article/details/gzdnyaxmw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.sjlbkw.cn/Article/details/gwcfzrpca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/ggvyepwfi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.epnwcf.com/Article/details/gmfeyisov.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.vehdjk.com/Article/details/gzwlijgnu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fktsv.cn/Article/details/gwmyvbdub.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.tarul.cn/Article/details/gcjwpzgws.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.epnwcf.com/Article/details/glnwhzrxf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.tarul.cn/Article/details/gkibavdxe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.tarul.cn/Article/details/gdpwrvzex.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/garaqxsbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.epnwcf.com/Article/details/gdutvhzwl.sHtML


<!-- 参考信息 -->