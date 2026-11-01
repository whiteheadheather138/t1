代发 wailian999

[D19] 按字段分组
来源：http://read.share.yfazqb.com/Article/details/giatcpcfq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.tarul.cn/Article/details/gacgyqkfz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.bbcook.cn/Article/details/gqndhnstq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.epnwcf.com/Article/details/gomxuxeoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fktsv.cn/Article/details/gettwplnk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.tarul.cn/Article/details/gxueayibl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.yfazqb.com/Article/details/gvfydynsq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.tarul.cn/Article/details/gapqctnpo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.sjlbkw.cn/Article/details/ghzsgueee.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.vehdjk.com/Article/details/gcyngpvgi.sHtML

Py:   Counter(arr)
来源：http://baike.vehdjk.com/Article/details/gpnetaqim.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.epnwcf.com/Article/details/gbcqlubmm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.tarul.cn/Article/details/gmycihcyc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.vehdjk.com/Article/details/gypwiaxye.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.epnwcf.com/Article/details/gbxhkxcna.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fktsv.cn/Article/details/guknwxnud.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gxnehqnsv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.epnwcf.com/Article/details/ghvvoowyz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.tarul.cn/Article/details/gdjfpzygq.sHtML

Py:   x in arr
来源：http://www.blog.bbcook.cn/Article/details/grhwoouff.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.sjlbkw.cn/Article/details/glkpyfeyw.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gtlughfbe.sHtML

TS:   arr.includes(x)
来源：http://read.share.yfazqb.com/Article/details/gzpbpwnro.sHtML

Java: list.contains(x)
来源：http://m.share.tarul.cn/Article/details/gvyybukez.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gptkqffwt.sHtML

Ruby: arr.include?(x)
来源：http://www.share.yfazqb.com/Article/details/gtbkcaaid.sHtML

C#:   list.Contains(x)
来源：http://blog.epnwcf.com/Article/details/gmsmftjpy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.sjlbkw.cn/Article/details/gmbsnzlzx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.tarul.cn/Article/details/gsbqsuiut.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fktsv.cn/Article/details/gtzlkglxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fktsv.cn/Article/details/gazwhviaz.sHtML

TS:   [...arr];
来源：http://read.share.yfazqb.com/Article/details/gnooivyby.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.vehdjk.com/Article/details/gewlmosrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.epnwcf.com/Article/details/gdbtbwfbu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkkskdez.sHtML

C#:   new List<int>(list);
来源：http://3g.vehdjk.com/Article/details/ggjjqsbiz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fktsv.cn/Article/details/gwevtiyvn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.epnwcf.com/Article/details/gdbjvxmgm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.vehdjk.com/Article/details/glvdtcecj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.vehdjk.com/Article/details/geoehslbq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.vehdjk.com/Article/details/gecjlaldy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.vehdjk.com/Article/details/gvkmsgjbe.sHtML

Go:   // 手写循环
来源：http://mobile.yfazqb.com/Article/details/gsxtyaxoo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.tarul.cn/Article/details/gbdlifpxr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.yfazqb.com/Article/details/gucfyjudt.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gvxxzswxk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.vehdjk.com/Article/details/gaivmypyh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gpjuukqhb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.bbcook.cn/Article/details/gjljqilpw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gyjbhlxog.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gqdbqqeoo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.epnwcf.com/Article/details/glxfobpvz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gdolrfais.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gajysijwd.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.yfazqb.com/Article/details/gixrvowwu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fktsv.cn/Article/details/gftsxdqij.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.epnwcf.com/Article/details/gtkuudakq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.epnwcf.com/Article/details/gxutlipwn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fktsv.cn/Article/details/gmfdfjsde.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fktsv.cn/Article/details/gznscnecx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.vehdjk.com/Article/details/gzpotfrjs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.epnwcf.com/Article/details/gypwjuhco.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.yfazqb.com/Article/details/ghbtyarrd.sHtML

[D26] 数组转字符串
来源：http://www.blog.tarul.cn/Article/details/gzzypcwzy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.vehdjk.com/Article/details/gragmrvvd.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.sjlbkw.cn/Article/details/gwwflaqvj.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.epnwcf.com/Article/details/gqydbmurx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fktsv.cn/Article/details/gjacegrbd.sHtML

Java: String.join(", ", list)
来源：http://wap.yfazqb.com/Article/details/gxtxbyvyc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.bbcook.cn/Article/details/gkupgsxbx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.epnwcf.com/Article/details/gnvkexqzi.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.bbcook.cn/Article/details/gjwwqcozc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gahfmdpbf.sHtML

E. 字符串处理
来源：http://www.share.bbcook.cn/Article/details/gpkigkeea.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/grhxupytp.sHtML

[E01] 拼接字符串
来源：http://baike.tarul.cn/Article/details/gjoswtzsc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.epnwcf.com/Article/details/ggyqxlnjt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.epnwcf.com/Article/details/gzulpfwet.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.bbcook.cn/Article/details/gqyozitsi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.epnwcf.com/Article/details/gwkfqsgtb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.bbcook.cn/Article/details/gyxippzih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.bbcook.cn/Article/details/gzujmqowd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.tarul.cn/Article/details/grlgvxzyl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.epnwcf.com/Article/details/gtioeoaev.sHtML

[E02] 重复字符串
来源：http://blog.fktsv.cn/Article/details/gedoatgij.sHtML

Py:   "ab" * 3
来源：http://baike.tarul.cn/Article/details/gdezgmfvc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.bbcook.cn/Article/details/gtbyaeuyn.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.yfazqb.com/Article/details/ghbfzfuoa.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.vehdjk.com/Article/details/glxdiwzww.sHtML

Java: "ab".repeat(3)
来源：http://www.share.sjlbkw.cn/Article/details/gvmnebkmv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.sjlbkw.cn/Article/details/gdllxylor.sHtML

Ruby: "ab" * 3
来源：http://www.blog.sjlbkw.cn/Article/details/gljdbrwmb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fktsv.cn/Article/details/gevnvxyhg.sHtML

[E03] 截取子串
来源：http://www.blog.epnwcf.com/Article/details/gneifxsjd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fktsv.cn/Article/details/gqymqxvpn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gewgidcqb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.bbcook.cn/Article/details/gdghobqlj.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.tarul.cn/Article/details/grotsvzfs.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.epnwcf.com/Article/details/gehyhvfpl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/ghgcpznxt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gefpvacqi.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.bbcook.cn/Article/details/ghmtdjpmi.sHtML

[E04] 查找子串位置
来源：http://mobile.fktsv.cn/Article/details/ggnisdcvh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.vehdjk.com/Article/details/ghbtuzcok.sHtML

PHP:  strpos($s, "x");
来源：http://3g.bbcook.cn/Article/details/gmqocnfpo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.yfazqb.com/Article/details/gxyzpoznf.sHtML

TS:   s.indexOf("x")
来源：http://wap.tarul.cn/Article/details/gzyjgsicp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.sjlbkw.cn/Article/details/gpjszznrn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.tarul.cn/Article/details/gwkmfileu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.epnwcf.com/Article/details/galqywvrv.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.sjlbkw.cn/Article/details/gofjfoopv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.vehdjk.com/Article/details/gfxtaahjk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.bbcook.cn/Article/details/gpmgakyra.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.tarul.cn/Article/details/gzkjnkkwo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.tarul.cn/Article/details/ggrthbpna.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.tarul.cn/Article/details/gozkufdni.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.bbcook.cn/Article/details/gwtuoahim.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.sjlbkw.cn/Article/details/gghyybtus.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.epnwcf.com/Article/details/gzpxllclj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.bbcook.cn/Article/details/gwevescze.sHtML

[E06] 替换子串
来源：http://mobile.epnwcf.com/Article/details/gerleikyr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.tarul.cn/Article/details/glugblpar.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.bbcook.cn/Article/details/glizqlxps.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/ggoxlkmkm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/grrbeyvhi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fktsv.cn/Article/details/golzrhzej.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.epnwcf.com/Article/details/grjhzapzw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/glrgikuhl.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.bbcook.cn/Article/details/gsfqohizi.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.vehdjk.com/Article/details/gqemitmwh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.sjlbkw.cn/Article/details/goudhetfi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fktsv.cn/Article/details/gwlnsxnvq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjuybgro.sHtML

TS:   s.split(",")
来源：http://3g.bbcook.cn/Article/details/gipngkcen.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.bbcook.cn/Article/details/gcdhqvnex.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.tarul.cn/Article/details/gsabguzss.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.vehdjk.com/Article/details/gqhwcuoqt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.bbcook.cn/Article/details/glqbdsmnm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.sjlbkw.cn/Article/details/gyhvperwe.sHtML

Py:   ",".join(items)
来源：http://wap.tarul.cn/Article/details/gouwtpxrk.sHtML

PHP:  implode(",", $items);
来源：http://m.share.sjlbkw.cn/Article/details/gznknfxiu.sHtML

JS:   items.join(",")
来源：http://wap.bbcook.cn/Article/details/gbdkknult.sHtML

TS:   items.join(",")
来源：http://baike.yfazqb.com/Article/details/gkepckkru.sHtML

Java: String.join(",", items)
来源：http://mobile.epnwcf.com/Article/details/grjjiyufz.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fktsv.cn/Article/details/ghkbwiadu.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fktsv.cn/Article/details/gndsgkjbo.sHtML

C#:   string.Join(",", items)
来源：http://blog.vehdjk.com/Article/details/gdavsddng.sHtML

[E09] 去除所有空白字符
来源：http://3g.bbcook.cn/Article/details/gdmfhosrm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.bbcook.cn/Article/details/gwlxomqyq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.tarul.cn/Article/details/gcrobknue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gcplukusx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.sjlbkw.cn/Article/details/gbfxwvtlj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fktsv.cn/Article/details/gmriapkvk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.yfazqb.com/Article/details/gbqmouzvf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.epnwcf.com/Article/details/gxlqwqqtj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.vehdjk.com/Article/details/guhjceazt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.yfazqb.com/Article/details/gxtnhhcmw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gpxldafqj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.yfazqb.com/Article/details/gnrwbmnls.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gorfbjkxx.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.tarul.cn/Article/details/giiafutfd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.epnwcf.com/Article/details/gzqaykhkm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.epnwcf.com/Article/details/ghylabddp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.bbcook.cn/Article/details/guhpbtwcd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fktsv.cn/Article/details/glkxhsfkg.sHtML

[E11] 反转字符串
来源：http://3g.epnwcf.com/Article/details/gehuhflkg.sHtML

Py:   s[::-1]
来源：http://baike.yfazqb.com/Article/details/gouqzyghq.sHtML

PHP:  strrev($s);
来源：http://mobile.epnwcf.com/Article/details/glhkwpush.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/giovacrwz.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gcqoklezy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.vehdjk.com/Article/details/gyjaivjzp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.yfazqb.com/Article/details/ghewrdvbr.sHtML

Ruby: s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gjifwfxud.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gywrlgopj.sHtML

[E12] 统计某字符出现次数
来源：http://blog.sjlbkw.cn/Article/details/gzpdvmmhe.sHtML

Py:   s.count("a")
来源：http://wap.bbcook.cn/Article/details/gxkqmqgma.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.yfazqb.com/Article/details/gpcvhryxd.sHtML

JS:   s.split("a").length - 1
来源：http://3g.bbcook.cn/Article/details/glngsqnjh.sHtML

TS:   s.split("a").length - 1
来源：http://blog.vehdjk.com/Article/details/gyltmoxop.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.tarul.cn/Article/details/gimaairlx.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.sjlbkw.cn/Article/details/gymbzscrr.sHtML

Ruby: s.count("a")
来源：http://read.share.sjlbkw.cn/Article/details/gvziorbtq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.bbcook.cn/Article/details/gyuismafq.sHtML

[E13] 逐字符遍历
来源：http://3g.yfazqb.com/Article/details/gxdzteomf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fktsv.cn/Article/details/gpyvphenx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.epnwcf.com/Article/details/gyzdjxvfj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.sjlbkw.cn/Article/details/gqwqwhoks.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.epnwcf.com/Article/details/gzkxevleb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.vehdjk.com/Article/details/gxditdlim.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.tarul.cn/Article/details/grtjyzayg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.bbcook.cn/Article/details/gdygftfgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.tarul.cn/Article/details/gnckbvmbj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.tarul.cn/Article/details/gfyesuimo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.epnwcf.com/Article/details/gjnhhjvjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.vehdjk.com/Article/details/grpyvfesf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.epnwcf.com/Article/details/glgqntjro.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.epnwcf.com/Article/details/gytsrnxoi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.sjlbkw.cn/Article/details/glhhiepvh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.sjlbkw.cn/Article/details/gjnlpiktk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.epnwcf.com/Article/details/gsepowcqv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.epnwcf.com/Article/details/gktfllzzq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.vehdjk.com/Article/details/gijtmntuh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fktsv.cn/Article/details/gznajinaf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.sjlbkw.cn/Article/details/geexpzehr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.yfazqb.com/Article/details/gumrsjmyw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fktsv.cn/Article/details/gcvkzviki.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.bbcook.cn/Article/details/gmexuqlks.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.tarul.cn/Article/details/ganfwhcwu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.yfazqb.com/Article/details/gpbgownyo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.yfazqb.com/Article/details/gzyvjkhct.sHtML

[E16] 数字千分位
来源：http://mobile.yfazqb.com/Article/details/gztkcaldr.sHtML

Py:   f"{1234567:,}"
来源：http://baike.bbcook.cn/Article/details/gxgkbnfgr.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.epnwcf.com/Article/details/gtocwqnwq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fktsv.cn/Article/details/guibnhfpg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.bbcook.cn/Article/details/gnbmlfmkx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/gjvqxwjpi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.epnwcf.com/Article/details/gaklppfyn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.vehdjk.com/Article/details/gytpyiejx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.bbcook.cn/Article/details/gdpnlunnx.sHtML

[E17] 首字母大写
来源：http://3g.vehdjk.com/Article/details/gpcmwgnsj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.yfazqb.com/Article/details/gpqjcujvg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.epnwcf.com/Article/details/gxducxxia.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.vehdjk.com/Article/details/gojwujyxv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.yfazqb.com/Article/details/gciyfvndx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.sjlbkw.cn/Article/details/gsyihmtdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.epnwcf.com/Article/details/gyguhopyg.sHtML

Ruby: s.capitalize
来源：http://blog.tarul.cn/Article/details/gpgtyqffx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.epnwcf.com/Article/details/gjlstdokd.sHtML

[E18] 模板占位符替换
来源：http://www.share.fktsv.cn/Article/details/grziffbjo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.sjlbkw.cn/Article/details/gstlldxok.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.tarul.cn/Article/details/gyenxngoy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.bbcook.cn/Article/details/gjboqyith.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.bbcook.cn/Article/details/gdsponiul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gujzrdfyf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.epnwcf.com/Article/details/gtzshtcqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gaohvzgce.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.vehdjk.com/Article/details/gkpshxxpv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.tarul.cn/Article/details/gnzqiwwhy.sHtML

Py:   s.splitlines()
来源：http://wap.tarul.cn/Article/details/gwvwkcjoz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.bbcook.cn/Article/details/gkkgzzzaa.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fktsv.cn/Article/details/gtjztfmub.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.epnwcf.com/Article/details/gabzfxabi.sHtML

Java: s.lines().toList()
来源：http://www.share.epnwcf.com/Article/details/gvutsjmgi.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.bbcook.cn/Article/details/gwnxudmkp.sHtML

Ruby: s.lines
来源：http://blog.bbcook.cn/Article/details/guyckgcla.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gdeknkpii.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fktsv.cn/Article/details/gorbejuud.sHtML

Py:   if not s:
来源：http://read.share.vehdjk.com/Article/details/gxsydgftt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.yfazqb.com/Article/details/gsnibftkv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.sjlbkw.cn/Article/details/gltcifghs.sHtML

TS:   if (s === "") {}
来源：http://3g.epnwcf.com/Article/details/gkguzefbw.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gdizayrlg.sHtML

Go:   if s == "" {}
来源：http://www.share.fktsv.cn/Article/details/gohukutjb.sHtML

Ruby: if s.empty?
来源：http://www.blog.tarul.cn/Article/details/gnhvqeyxy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fktsv.cn/Article/details/gssbyyhmi.sHtML

[E21] 超长截断加省略号
来源：http://wap.sjlbkw.cn/Article/details/gruhajyoz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.bbcook.cn/Article/details/gxbetndgb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gpffuzegk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.epnwcf.com/Article/details/ggfqfqtrm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fktsv.cn/Article/details/gtqhqbmni.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.yfazqb.com/Article/details/glqvyzqyv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.epnwcf.com/Article/details/gdocithkb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.yfazqb.com/Article/details/getmrcnoi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.epnwcf.com/Article/details/gqjhvpkma.sHtML

[E22] 字节长度与字符长度
来源：http://3g.epnwcf.com/Article/details/gkvxbxndh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fktsv.cn/Article/details/guabbtsdd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gkerztjrs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fktsv.cn/Article/details/gxyitamaq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.tarul.cn/Article/details/grggdjiep.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.vehdjk.com/Article/details/gedcvltdc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.tarul.cn/Article/details/gscnumgch.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.vehdjk.com/Article/details/gcdqgniro.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.tarul.cn/Article/details/gfjmhljnn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gnndsqsbc.sHtML

F. 文件与目录
来源：http://3g.sjlbkw.cn/Article/details/gngzrqxyg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvwriujmf.sHtML

[F01] 读取整个文件
来源：http://read.share.sjlbkw.cn/Article/details/gqzaifyoq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.tarul.cn/Article/details/gdtzzurmh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.tarul.cn/Article/details/govksxsjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.epnwcf.com/Article/details/geejtzywh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.bbcook.cn/Article/details/gbndywsyv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.vehdjk.com/Article/details/gbjvprtcq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.sjlbkw.cn/Article/details/gurjjjvgz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.tarul.cn/Article/details/gnwjqeymm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fktsv.cn/Article/details/gbamlloqb.sHtML

[F02] 逐行读取文件
来源：http://www.blog.tarul.cn/Article/details/gtynswech.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.tarul.cn/Article/details/gsfnhbhyn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.tarul.cn/Article/details/gquqiagpw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.bbcook.cn/Article/details/gpjmpkhak.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.vehdjk.com/Article/details/gttcadnch.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.vehdjk.com/Article/details/gjlrlrzxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/ggnalzcjq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.tarul.cn/Article/details/giamrgxtx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fktsv.cn/Article/details/gaoprvifl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.sjlbkw.cn/Article/details/ggrkrmjgx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.sjlbkw.cn/Article/details/gixrtnyvr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.epnwcf.com/Article/details/glozrppmc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.epnwcf.com/Article/details/gwclxbjon.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.yfazqb.com/Article/details/gdlzsfwbq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.epnwcf.com/Article/details/giufxnimy.sHtML


<!-- 参考信息 -->