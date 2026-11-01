代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.epnwcf.com/Article/details/gsevkelxx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.vehdjk.com/Article/details/gfgymimac.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.sjlbkw.cn/Article/details/gukuaqazt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.yfazqb.com/Article/details/gmsfkcubp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpreoevh.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.yfazqb.com/Article/details/gjrmukxnh.sHtML

Py:   Counter(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gkwnkziwd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.bbcook.cn/Article/details/gbxhslyts.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.vehdjk.com/Article/details/ggpgzescf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.bbcook.cn/Article/details/gcqbbvepi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.yfazqb.com/Article/details/gcfwaekut.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.vehdjk.com/Article/details/gnpbxldzk.sHtML

Ruby: arr.tally
来源：http://www.m.share.sjlbkw.cn/Article/details/guexplmwk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.epnwcf.com/Article/details/gxuvaojac.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.vehdjk.com/Article/details/gsfhbqipb.sHtML

Py:   x in arr
来源：http://mobile.fktsv.cn/Article/details/ghailomfm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.yfazqb.com/Article/details/gyxqtrrps.sHtML

JS:   arr.includes(x)
来源：http://www.blog.tarul.cn/Article/details/gaszeiuem.sHtML

TS:   arr.includes(x)
来源：http://read.share.bbcook.cn/Article/details/ggarhmiig.sHtML

Java: list.contains(x)
来源：http://m.share.yfazqb.com/Article/details/gjacyalie.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gkclyijhq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.tarul.cn/Article/details/gjcuyybam.sHtML

C#:   list.Contains(x)
来源：http://3g.bbcook.cn/Article/details/gluytxkzm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.sjlbkw.cn/Article/details/glfcmbekh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fktsv.cn/Article/details/gjxaexwdu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.sjlbkw.cn/Article/details/gupdxhdjw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.vehdjk.com/Article/details/gnkeklnyq.sHtML

TS:   [...arr];
来源：http://baike.yfazqb.com/Article/details/gvnaltmol.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fktsv.cn/Article/details/gsbvriwdf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.sjlbkw.cn/Article/details/gtdtsntrl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.sjlbkw.cn/Article/details/gkaorcekk.sHtML

C#:   new List<int>(list);
来源：http://read.share.tarul.cn/Article/details/gjdbfkwhe.sHtML

[D23] reduce 累积计算
来源：http://www.blog.vehdjk.com/Article/details/gxwdxczmx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.vehdjk.com/Article/details/gmucelugu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.epnwcf.com/Article/details/gdenmakme.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.epnwcf.com/Article/details/gfumsmjcs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/gqxlbfijf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.bbcook.cn/Article/details/gtioqlyvm.sHtML

Go:   // 手写循环
来源：http://blog.epnwcf.com/Article/details/gmpncwjqw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gxfhvehfi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/gogyuahlr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.tarul.cn/Article/details/gjmwfaqyn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.epnwcf.com/Article/details/gxkrlmcbw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.yfazqb.com/Article/details/gxwerafdz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.tarul.cn/Article/details/gkgohercs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gnnhuyhhi.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.yfazqb.com/Article/details/gmxlczteg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.tarul.cn/Article/details/gquoampbm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.tarul.cn/Article/details/gbobngzev.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.yfazqb.com/Article/details/goqsbxevq.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fktsv.cn/Article/details/gthphnqxv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.yfazqb.com/Article/details/gbowctqrt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.epnwcf.com/Article/details/gbdruevrr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.tarul.cn/Article/details/guidxbfcm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.vehdjk.com/Article/details/glzuxjctx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.yfazqb.com/Article/details/garhybbvy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fktsv.cn/Article/details/gwwemczbm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.bbcook.cn/Article/details/grvbsfceo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.yfazqb.com/Article/details/gyxdyhvxd.sHtML

[D26] 数组转字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gdmapdboz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.bbcook.cn/Article/details/grlegnsss.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.sjlbkw.cn/Article/details/guyrkdhtl.sHtML

JS:   arr.join(", ")
来源：http://3g.vehdjk.com/Article/details/gzovlhpub.sHtML

TS:   arr.join(", ")
来源：http://3g.bbcook.cn/Article/details/gjhrlzfja.sHtML

Java: String.join(", ", list)
来源：http://blog.bbcook.cn/Article/details/gzlmyaiuy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.sjlbkw.cn/Article/details/gesdkimip.sHtML

Ruby: arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/gbjugdaht.sHtML

C#:   string.Join(", ", list)
来源：http://baike.bbcook.cn/Article/details/gndjgneqi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvcgiopjr.sHtML

E. 字符串处理
来源：http://mobile.yfazqb.com/Article/details/grhclcrhl.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkuctanmm.sHtML

[E01] 拼接字符串
来源：http://www.share.yfazqb.com/Article/details/ggwxletfq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.vehdjk.com/Article/details/grfjadgmo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.vehdjk.com/Article/details/gxvpnksix.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.tarul.cn/Article/details/gjjhfqtpx.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.vehdjk.com/Article/details/gzpxpagmt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.bbcook.cn/Article/details/gwuyxnmde.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.vehdjk.com/Article/details/gxqmfohef.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.epnwcf.com/Article/details/gswvaroea.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.bbcook.cn/Article/details/gypghslgd.sHtML

[E02] 重复字符串
来源：http://mobile.epnwcf.com/Article/details/gmsqkvlmw.sHtML

Py:   "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gjfhxkxfv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.yfazqb.com/Article/details/gufhaacnz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.epnwcf.com/Article/details/gutspoapw.sHtML

TS:   "ab".repeat(3)
来源：http://blog.sjlbkw.cn/Article/details/gqeoopltd.sHtML

Java: "ab".repeat(3)
来源：http://read.share.sjlbkw.cn/Article/details/gmwanrhjq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.epnwcf.com/Article/details/gfrlvcmry.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fktsv.cn/Article/details/ghgljuufd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/godceasae.sHtML

[E03] 截取子串
来源：http://read.share.bbcook.cn/Article/details/gslxgfwth.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.vehdjk.com/Article/details/gqgtklzfx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gzsbzavyj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.sjlbkw.cn/Article/details/gzbdsacix.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fktsv.cn/Article/details/gekhelggq.sHtML

Java: s.substring(1, 4)
来源：http://blog.sjlbkw.cn/Article/details/gazgiavqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/ggbjvwohk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.sjlbkw.cn/Article/details/gbrtcqmsx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gyqcllkhs.sHtML

[E04] 查找子串位置
来源：http://m.share.vehdjk.com/Article/details/gaelzguds.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.bbcook.cn/Article/details/ghvknmzva.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gigvdhvjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.bbcook.cn/Article/details/gxpcblmcx.sHtML

TS:   s.indexOf("x")
来源：http://m.share.vehdjk.com/Article/details/gausirmtc.sHtML

Java: s.indexOf("x")
来源：http://www.share.tarul.cn/Article/details/givkxbigl.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.vehdjk.com/Article/details/gvzyanapq.sHtML

Ruby: s.index("x")
来源：http://wap.tarul.cn/Article/details/gtqblpigf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.epnwcf.com/Article/details/gxesdqnzl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.bbcook.cn/Article/details/geztvfszy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.sjlbkw.cn/Article/details/gmyybtnqm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.epnwcf.com/Article/details/gwwcrrdmq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.yfazqb.com/Article/details/gvxxcdazu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.bbcook.cn/Article/details/gtnwkhdly.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.tarul.cn/Article/details/geayuhvtk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.yfazqb.com/Article/details/gypbhbpxk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.tarul.cn/Article/details/grobgcvro.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.sjlbkw.cn/Article/details/ghknamcmr.sHtML

[E06] 替换子串
来源：http://3g.fktsv.cn/Article/details/gvhxjckhf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.sjlbkw.cn/Article/details/gyhlomzjn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.epnwcf.com/Article/details/gddaknntq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fktsv.cn/Article/details/geqghfpzt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.yfazqb.com/Article/details/gqtxoqkag.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.tarul.cn/Article/details/gazurvmfu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.epnwcf.com/Article/details/gdrpvudmy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.epnwcf.com/Article/details/gegrorytw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gkvmvajat.sHtML

[E07] 按分隔符拆分
来源：http://3g.tarul.cn/Article/details/gpfeyjslm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.sjlbkw.cn/Article/details/grrijjjwz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.sjlbkw.cn/Article/details/gjzmwypyo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.vehdjk.com/Article/details/gezsbjxdh.sHtML

TS:   s.split(",")
来源：http://read.share.sjlbkw.cn/Article/details/gkvrnakhg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.yfazqb.com/Article/details/gorcdmwom.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fktsv.cn/Article/details/gbhaguzah.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.epnwcf.com/Article/details/grfvpkifa.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.yfazqb.com/Article/details/gveukckqc.sHtML

[E08] 数组按分隔符合并
来源：http://3g.yfazqb.com/Article/details/gpmlpequk.sHtML

Py:   ",".join(items)
来源：http://www.blog.yfazqb.com/Article/details/gzooklhms.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gblkpougl.sHtML

JS:   items.join(",")
来源：http://baike.epnwcf.com/Article/details/gipixuwzj.sHtML

TS:   items.join(",")
来源：http://read.share.epnwcf.com/Article/details/gwyadiwir.sHtML

Java: String.join(",", items)
来源：http://www.blog.epnwcf.com/Article/details/grnrcrxcf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fktsv.cn/Article/details/gzeugsxej.sHtML

Ruby: items.join(",")
来源：http://blog.yfazqb.com/Article/details/gxuhdljqg.sHtML

C#:   string.Join(",", items)
来源：http://read.share.sjlbkw.cn/Article/details/gyikboxsk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.sjlbkw.cn/Article/details/gwaiodrgf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.epnwcf.com/Article/details/gpfdxydtl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.yfazqb.com/Article/details/gknwnnfng.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.yfazqb.com/Article/details/gsiguxhjz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fktsv.cn/Article/details/gflcaztbg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.vehdjk.com/Article/details/goywwcnyp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.tarul.cn/Article/details/grdjyzxlt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.sjlbkw.cn/Article/details/gishrtzrw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.vehdjk.com/Article/details/guiubnxkk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.sjlbkw.cn/Article/details/gsciyxozu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fktsv.cn/Article/details/glsrzwhot.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.epnwcf.com/Article/details/gnkmacork.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.sjlbkw.cn/Article/details/gyqjrnumi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.bbcook.cn/Article/details/gukyamgdr.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.bbcook.cn/Article/details/gwdpuyips.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.tarul.cn/Article/details/gazdulhak.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.yfazqb.com/Article/details/gyjvktbzm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.yfazqb.com/Article/details/grrzarczp.sHtML

[E11] 反转字符串
来源：http://www.share.tarul.cn/Article/details/gegyqnowy.sHtML

Py:   s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gzlncurdi.sHtML

PHP:  strrev($s);
来源：http://wap.epnwcf.com/Article/details/gddaonzeh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/grsrjitnm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gbgmaebvl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.vehdjk.com/Article/details/gdfjnoskf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.bbcook.cn/Article/details/gepzwwyss.sHtML

Ruby: s.reverse
来源：http://blog.bbcook.cn/Article/details/gtzfiqunm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gsbcseviq.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.bbcook.cn/Article/details/gpewsaamw.sHtML

Py:   s.count("a")
来源：http://baike.bbcook.cn/Article/details/gbhzrtvjk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.vehdjk.com/Article/details/gghcjjwpr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.bbcook.cn/Article/details/gnsnyxthe.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.tarul.cn/Article/details/gtygxcqra.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/geqdopzts.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.bbcook.cn/Article/details/gxqkrqjtz.sHtML

Ruby: s.count("a")
来源：http://3g.yfazqb.com/Article/details/gfwbsvmiz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.epnwcf.com/Article/details/gzdrouhfr.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fktsv.cn/Article/details/ghxptbwhc.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fktsv.cn/Article/details/gsrzyjlkz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.bbcook.cn/Article/details/gisuddyyd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.yfazqb.com/Article/details/ggsxcakeh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gzjvplged.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.epnwcf.com/Article/details/gqfbcypfg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.yfazqb.com/Article/details/gzfljzays.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.sjlbkw.cn/Article/details/gdvnhmjgc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.bbcook.cn/Article/details/gaztoinij.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fktsv.cn/Article/details/gnqwfotao.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fktsv.cn/Article/details/ggujyefqn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gtszrzejq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.tarul.cn/Article/details/gjwumkavp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.vehdjk.com/Article/details/gsyqaypsv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.yfazqb.com/Article/details/gcwqkcwpa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.yfazqb.com/Article/details/gmqqjaeev.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.sjlbkw.cn/Article/details/gvphsgssk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.bbcook.cn/Article/details/ggrewnnal.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.sjlbkw.cn/Article/details/gjsmginyc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.epnwcf.com/Article/details/geyposmri.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.vehdjk.com/Article/details/gqezwyhcr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fktsv.cn/Article/details/gaqudpubo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.yfazqb.com/Article/details/gbdiygplr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.vehdjk.com/Article/details/ghuonjxuh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.yfazqb.com/Article/details/gfppatrkz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.yfazqb.com/Article/details/geyiamies.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.yfazqb.com/Article/details/glkdkrjov.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/gcytfrlnq.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkepkvpd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.sjlbkw.cn/Article/details/ghbmqkrvu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.bbcook.cn/Article/details/gugxzaawo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fktsv.cn/Article/details/gkpktneyi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fktsv.cn/Article/details/gzaapjtga.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.vehdjk.com/Article/details/gqrxtpumy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.sjlbkw.cn/Article/details/gfznokgwi.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fktsv.cn/Article/details/gffailalc.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gdgzkafku.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.bbcook.cn/Article/details/gpthljxhh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.tarul.cn/Article/details/gdrvtsyor.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gmkjnmtju.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.tarul.cn/Article/details/gevhtkcub.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fktsv.cn/Article/details/gdupesntn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.yfazqb.com/Article/details/ghzdxmigz.sHtML

Ruby: s.capitalize
来源：http://3g.fktsv.cn/Article/details/glinfitbu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.bbcook.cn/Article/details/gkwckeexh.sHtML

[E18] 模板占位符替换
来源：http://www.share.tarul.cn/Article/details/gdlmovewf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.yfazqb.com/Article/details/gutlhdgat.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.vehdjk.com/Article/details/gcumtpdhh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.epnwcf.com/Article/details/gamwdchjc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.tarul.cn/Article/details/gbevmnnwb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.sjlbkw.cn/Article/details/grdtpabbt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.epnwcf.com/Article/details/glevexbxk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.yfazqb.com/Article/details/gheircxbc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.epnwcf.com/Article/details/gdiejtabm.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.yfazqb.com/Article/details/gluxbdqln.sHtML

Py:   s.splitlines()
来源：http://m.share.epnwcf.com/Article/details/giqybsotx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.vehdjk.com/Article/details/gdjpvjido.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.vehdjk.com/Article/details/gxnqgobgs.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.bbcook.cn/Article/details/grqciggaq.sHtML

Java: s.lines().toList()
来源：http://3g.yfazqb.com/Article/details/gbpyqpeyr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.epnwcf.com/Article/details/gjufvzqsw.sHtML

Ruby: s.lines
来源：http://www.share.vehdjk.com/Article/details/gxkufvvmi.sHtML

C#:   s.Split('\n')
来源：http://baike.epnwcf.com/Article/details/gvseoxarc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.vehdjk.com/Article/details/gmbkivbzp.sHtML

Py:   if not s:
来源：http://www.blog.epnwcf.com/Article/details/guehuqzlp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fktsv.cn/Article/details/gbxemjseb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.vehdjk.com/Article/details/gbnopfuwj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fktsv.cn/Article/details/gqcprlhfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gzbhjjxub.sHtML

Go:   if s == "" {}
来源：http://3g.yfazqb.com/Article/details/grdfxpjgd.sHtML

Ruby: if s.empty?
来源：http://www.share.sjlbkw.cn/Article/details/gbmwvvqfh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.bbcook.cn/Article/details/gcjvyemzt.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fktsv.cn/Article/details/gsadrgaaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.vehdjk.com/Article/details/gsxsnszks.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gqpkuobwv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.bbcook.cn/Article/details/ggbcmofck.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.sjlbkw.cn/Article/details/gjnxsmhwo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.bbcook.cn/Article/details/ggnidowvk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.sjlbkw.cn/Article/details/gzmlbyhww.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.bbcook.cn/Article/details/gubjembsu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fktsv.cn/Article/details/ggoxucnmw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fktsv.cn/Article/details/ghtbsdojk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fktsv.cn/Article/details/grkkxoalb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gghfbcwst.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.tarul.cn/Article/details/ggpzcayxh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.bbcook.cn/Article/details/gkxddtdsl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.bbcook.cn/Article/details/gdofjljey.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.bbcook.cn/Article/details/gpqlmdhjc.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.bbcook.cn/Article/details/gwyovbkyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.epnwcf.com/Article/details/gvozcikef.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfwohumuo.sHtML

F. 文件与目录
来源：http://wap.epnwcf.com/Article/details/gvprqldyx.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gixutootq.sHtML

[F01] 读取整个文件
来源：http://wap.tarul.cn/Article/details/grzdgigmr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.sjlbkw.cn/Article/details/gwlokpfmu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.sjlbkw.cn/Article/details/ggkpxjpvi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.epnwcf.com/Article/details/gtkrksvkl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.yfazqb.com/Article/details/gaqfltfko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.yfazqb.com/Article/details/grgcbqckd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.bbcook.cn/Article/details/gdkofocun.sHtML

Ruby: File.read("a.txt")
来源：http://wap.epnwcf.com/Article/details/gnjtjclqh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.epnwcf.com/Article/details/gezgjnhfr.sHtML

[F02] 逐行读取文件
来源：http://read.share.sjlbkw.cn/Article/details/ghmlabpsu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.bbcook.cn/Article/details/gjgfzeviw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fktsv.cn/Article/details/gqsolosdq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.yfazqb.com/Article/details/gmktrtusf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.yfazqb.com/Article/details/gxcqjyqdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fktsv.cn/Article/details/gqrhserea.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.bbcook.cn/Article/details/geantpwyz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.bbcook.cn/Article/details/grbkmvrfy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.tarul.cn/Article/details/gajmombhj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.bbcook.cn/Article/details/gbvyvqbge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.tarul.cn/Article/details/gbaofqpaq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fktsv.cn/Article/details/gosaecwqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fktsv.cn/Article/details/ghihnybie.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.bbcook.cn/Article/details/glbraqfqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.bbcook.cn/Article/details/gqzjujtvj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.bbcook.cn/Article/details/gaguvnfmk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.epnwcf.com/Article/details/gqporaeej.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.tarul.cn/Article/details/gkoyzshqd.sHtML

[F04] 追加写入文件
来源：http://baike.yfazqb.com/Article/details/gabsqvwqr.sHtML


<!-- 参考信息 -->