代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/ginoesjpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gggddybiw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.tarul.cn/Article/details/gmwkbdofq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.vehdjk.com/Article/details/gdsnknayx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.tarul.cn/Article/details/gbcssomhv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.yfazqb.com/Article/details/gaxmrccni.sHtML

Py:   Counter(arr)
来源：http://wap.vehdjk.com/Article/details/gfngmmjml.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/gvwvajbnp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.tarul.cn/Article/details/gvvaecdan.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/grtfkampk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.tarul.cn/Article/details/gmqsyjiyo.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.yfazqb.com/Article/details/gjqeuxchp.sHtML

Ruby: arr.tally
来源：http://wap.yfazqb.com/Article/details/gwvksqdvi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/gujblziti.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fktsv.cn/Article/details/gvelapcap.sHtML

Py:   x in arr
来源：http://baike.tarul.cn/Article/details/gsgvvxvdz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.sjlbkw.cn/Article/details/gdewkctrp.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/ggvduujxv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.tarul.cn/Article/details/gkrkjtfzu.sHtML

Java: list.contains(x)
来源：http://mobile.epnwcf.com/Article/details/ggebdfzbt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gkvzkrvts.sHtML

Ruby: arr.include?(x)
来源：http://blog.sjlbkw.cn/Article/details/gfewfanky.sHtML

C#:   list.Contains(x)
来源：http://baike.vehdjk.com/Article/details/gmfraolbk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.vehdjk.com/Article/details/gtlcigrer.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gebuyumlf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.bbcook.cn/Article/details/goxcztahk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/gvmmyjnsb.sHtML

TS:   [...arr];
来源：http://wap.vehdjk.com/Article/details/gclgszxqp.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gntmdezjm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.tarul.cn/Article/details/gexrkodus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.sjlbkw.cn/Article/details/gzmgjdznp.sHtML

C#:   new List<int>(list);
来源：http://wap.sjlbkw.cn/Article/details/gtriurahh.sHtML

[D23] reduce 累积计算
来源：http://www.share.fktsv.cn/Article/details/gsxyalcvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fktsv.cn/Article/details/ggnkuaiwo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.yfazqb.com/Article/details/gkargzoim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.yfazqb.com/Article/details/gmwdebvmu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.bbcook.cn/Article/details/gcwdnwawy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.bbcook.cn/Article/details/giuaprfuv.sHtML

Go:   // 手写循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gijboocdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fktsv.cn/Article/details/gfmfpctod.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.tarul.cn/Article/details/gaggecjcf.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.bbcook.cn/Article/details/gmxsunotr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.bbcook.cn/Article/details/grfiavigb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.yfazqb.com/Article/details/gadesixzr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.yfazqb.com/Article/details/gyuutrfqm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.yfazqb.com/Article/details/gfhvsluhh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.vehdjk.com/Article/details/gxpurgasd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.sjlbkw.cn/Article/details/gkfvkotzx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.tarul.cn/Article/details/gvthvntis.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fktsv.cn/Article/details/gwgcadjyv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.tarul.cn/Article/details/gnpcpfhar.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.epnwcf.com/Article/details/gazqnxome.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fktsv.cn/Article/details/gfitokxgz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.yfazqb.com/Article/details/gxzcxiigh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.vehdjk.com/Article/details/gcaiyjbah.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.sjlbkw.cn/Article/details/gmzofuybu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.epnwcf.com/Article/details/ggrqmmtws.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fktsv.cn/Article/details/gdgzrwrhe.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fktsv.cn/Article/details/gkywbkqoo.sHtML

[D26] 数组转字符串
来源：http://www.share.epnwcf.com/Article/details/glmzktczu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/gpyjxnzir.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.vehdjk.com/Article/details/gqizpqngk.sHtML

JS:   arr.join(", ")
来源：http://wap.epnwcf.com/Article/details/gmodgvqui.sHtML

TS:   arr.join(", ")
来源：http://baike.bbcook.cn/Article/details/gvnhueicr.sHtML

Java: String.join(", ", list)
来源：http://read.share.epnwcf.com/Article/details/gvojwmfnx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.bbcook.cn/Article/details/glkwfilnv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fktsv.cn/Article/details/gabfzzjlg.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.vehdjk.com/Article/details/gvafepbee.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpwjqdzgb.sHtML

E. 字符串处理
来源：http://mobile.bbcook.cn/Article/details/gqbvcimkm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gntgoqzlb.sHtML

[E01] 拼接字符串
来源：http://mobile.tarul.cn/Article/details/gqfzkrnor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.sjlbkw.cn/Article/details/gxkrrlueh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gitxzonct.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.sjlbkw.cn/Article/details/gokjdplkp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gprqhrfxe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.tarul.cn/Article/details/grudezfeo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.epnwcf.com/Article/details/gjzebzxhi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.sjlbkw.cn/Article/details/gbvuclvvv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/gucahudgr.sHtML

[E02] 重复字符串
来源：http://blog.yfazqb.com/Article/details/gkuwjlevd.sHtML

Py:   "ab" * 3
来源：http://blog.vehdjk.com/Article/details/gqtultgzl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.vehdjk.com/Article/details/gloemzwhu.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.yfazqb.com/Article/details/gkaqvgfkt.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fktsv.cn/Article/details/gbskhecbn.sHtML

Java: "ab".repeat(3)
来源：http://blog.bbcook.cn/Article/details/gggauohgv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.vehdjk.com/Article/details/gaeaufqoy.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.epnwcf.com/Article/details/glmnuhgnd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fktsv.cn/Article/details/gtmvsyhfb.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gtunlyamp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.tarul.cn/Article/details/gjjmbiblj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gwfamczff.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.yfazqb.com/Article/details/guewmuetb.sHtML

TS:   s.slice(1, 4)
来源：http://baike.epnwcf.com/Article/details/gdaztjspm.sHtML

Java: s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/gmtxvoufa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.tarul.cn/Article/details/goqfpyctk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.yfazqb.com/Article/details/ggyphrmpg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.tarul.cn/Article/details/gtasoymzt.sHtML

[E04] 查找子串位置
来源：http://baike.yfazqb.com/Article/details/gwntqgtsy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.tarul.cn/Article/details/gcvljwtcn.sHtML

PHP:  strpos($s, "x");
来源：http://blog.tarul.cn/Article/details/gqidkzsxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.tarul.cn/Article/details/giikzzcoq.sHtML

TS:   s.indexOf("x")
来源：http://wap.yfazqb.com/Article/details/glkcmyrkd.sHtML

Java: s.indexOf("x")
来源：http://wap.sjlbkw.cn/Article/details/gniwgfckh.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.yfazqb.com/Article/details/ghwixngnu.sHtML

Ruby: s.index("x")
来源：http://www.blog.fktsv.cn/Article/details/gnpvquvha.sHtML

C#:   s.IndexOf("x")
来源：http://3g.tarul.cn/Article/details/gpbvchacv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.tarul.cn/Article/details/gpiimonqj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.epnwcf.com/Article/details/giamfjtkf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.vehdjk.com/Article/details/glnrguefo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/giaskmiiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fktsv.cn/Article/details/gyevpzvws.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.bbcook.cn/Article/details/gsifhuhfv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.tarul.cn/Article/details/ghwjmrtul.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.vehdjk.com/Article/details/gpqmaszil.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.epnwcf.com/Article/details/gilrytzjj.sHtML

[E06] 替换子串
来源：http://mobile.fktsv.cn/Article/details/gtiumoetu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.epnwcf.com/Article/details/gzmdliqau.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.yfazqb.com/Article/details/gutqpgroc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.vehdjk.com/Article/details/gwthkdwkf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gwtaxyncw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/gnzebrxqc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.epnwcf.com/Article/details/ghapuqkui.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gufidhejt.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gdkduuzlz.sHtML

[E07] 按分隔符拆分
来源：http://blog.epnwcf.com/Article/details/gxarxzlps.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.yfazqb.com/Article/details/gijbzycjn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.vehdjk.com/Article/details/gcrebvoye.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.vehdjk.com/Article/details/gxwvvjcfs.sHtML

TS:   s.split(",")
来源：http://wap.epnwcf.com/Article/details/gcimkeidw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.bbcook.cn/Article/details/gricxulmb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.vehdjk.com/Article/details/gusljwxfr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.bbcook.cn/Article/details/gobfcmgth.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.vehdjk.com/Article/details/grnpbkfoe.sHtML

[E08] 数组按分隔符合并
来源：http://3g.vehdjk.com/Article/details/gwhxkmnft.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/getvdyvgu.sHtML

PHP:  implode(",", $items);
来源：http://wap.bbcook.cn/Article/details/geymftuat.sHtML

JS:   items.join(",")
来源：http://3g.bbcook.cn/Article/details/gupryoiiy.sHtML

TS:   items.join(",")
来源：http://www.blog.tarul.cn/Article/details/gzrkdhfyo.sHtML

Java: String.join(",", items)
来源：http://3g.tarul.cn/Article/details/gogomsgnd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.tarul.cn/Article/details/gpmgbtcde.sHtML

Ruby: items.join(",")
来源：http://www.share.epnwcf.com/Article/details/gyuhgendc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.bbcook.cn/Article/details/gieufdatq.sHtML

[E09] 去除所有空白字符
来源：http://3g.epnwcf.com/Article/details/gbigukuqv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.bbcook.cn/Article/details/grbkrseed.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fktsv.cn/Article/details/gsxalriyy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.epnwcf.com/Article/details/gbduypkvh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fktsv.cn/Article/details/gzolvkrte.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.sjlbkw.cn/Article/details/gjevdpagl.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fktsv.cn/Article/details/ggaazxtky.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.yfazqb.com/Article/details/gawppltve.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.epnwcf.com/Article/details/geegzszqv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.sjlbkw.cn/Article/details/gwhxglwmt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.sjlbkw.cn/Article/details/grpukyhuv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.bbcook.cn/Article/details/gsbmepnsc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.epnwcf.com/Article/details/gjmnuymnb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.bbcook.cn/Article/details/gxyyfwvmx.sHtML

Java: String.format("%03d", 7)
来源：http://3g.yfazqb.com/Article/details/gezsqrcdz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.sjlbkw.cn/Article/details/ggadykbjt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.bbcook.cn/Article/details/gvubfqbrp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.tarul.cn/Article/details/gfmgdzimj.sHtML

[E11] 反转字符串
来源：http://www.share.fktsv.cn/Article/details/geamlxkci.sHtML

Py:   s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gvxqwxehl.sHtML

PHP:  strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gvbvejwjk.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gazvsnnxx.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gmeijlpby.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.yfazqb.com/Article/details/gvskjusav.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.sjlbkw.cn/Article/details/gnxuqjare.sHtML

Ruby: s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gltdovbwh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gujwrbnvt.sHtML

[E12] 统计某字符出现次数
来源：http://3g.tarul.cn/Article/details/glinveyve.sHtML

Py:   s.count("a")
来源：http://mobile.sjlbkw.cn/Article/details/gyoqbhefe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.epnwcf.com/Article/details/gtjscpfun.sHtML

JS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/ggxksdesi.sHtML

TS:   s.split("a").length - 1
来源：http://3g.tarul.cn/Article/details/gkthvqzix.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gxosaspmn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.vehdjk.com/Article/details/gldtekzdl.sHtML

Ruby: s.count("a")
来源：http://www.m.share.yfazqb.com/Article/details/gelitayci.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.tarul.cn/Article/details/gzkxeohmn.sHtML

[E13] 逐字符遍历
来源：http://3g.bbcook.cn/Article/details/gmnxhpzka.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.yfazqb.com/Article/details/gmrkomztp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.epnwcf.com/Article/details/gqedttexw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.sjlbkw.cn/Article/details/gimzfeiyk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.vehdjk.com/Article/details/goauytaaq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.vehdjk.com/Article/details/gwdufrqvt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.tarul.cn/Article/details/gmkudkwpf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.vehdjk.com/Article/details/gkiddrxyg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.sjlbkw.cn/Article/details/gkzzzhmgv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.epnwcf.com/Article/details/gbezuhuda.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.epnwcf.com/Article/details/gcgpzmjvv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.sjlbkw.cn/Article/details/gkwogmmie.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.bbcook.cn/Article/details/gwagiokue.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fktsv.cn/Article/details/glxqqutas.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gogcwwnyc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.vehdjk.com/Article/details/gtxzfuebk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.sjlbkw.cn/Article/details/gevlojvys.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.vehdjk.com/Article/details/getblozpg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.bbcook.cn/Article/details/gepjmzqfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.bbcook.cn/Article/details/gaixpskzs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.sjlbkw.cn/Article/details/gphegtnxd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.bbcook.cn/Article/details/gihoegfrs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.epnwcf.com/Article/details/ggyzojnze.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.tarul.cn/Article/details/gvdnjjugg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.epnwcf.com/Article/details/gbabwkhvv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.vehdjk.com/Article/details/gxvmwuvzk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.vehdjk.com/Article/details/gdcxjhxjr.sHtML

[E16] 数字千分位
来源：http://baike.sjlbkw.cn/Article/details/grzrozhji.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.vehdjk.com/Article/details/gthaonyuw.sHtML

PHP:  number_format(1234567);
来源：http://blog.sjlbkw.cn/Article/details/gwjjvyluf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.bbcook.cn/Article/details/ghoqxfowg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.tarul.cn/Article/details/ghcyvrgmz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.yfazqb.com/Article/details/gqiflnbst.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.tarul.cn/Article/details/gvsfflnpm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.tarul.cn/Article/details/gstsaoxvs.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.tarul.cn/Article/details/gwvkvgumr.sHtML

[E17] 首字母大写
来源：http://read.share.bbcook.cn/Article/details/gslbfrlor.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fktsv.cn/Article/details/gvqmbkrmx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.epnwcf.com/Article/details/ggwcnsybd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.vehdjk.com/Article/details/gvhjqobmx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.tarul.cn/Article/details/gktvbnzrc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.bbcook.cn/Article/details/gimhtkhzv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.tarul.cn/Article/details/gmxjipscx.sHtML

Ruby: s.capitalize
来源：http://www.share.tarul.cn/Article/details/gbwzfbamp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.yfazqb.com/Article/details/gbjehteda.sHtML

[E18] 模板占位符替换
来源：http://baike.bbcook.cn/Article/details/geaenjeov.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.bbcook.cn/Article/details/gutywawfe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.sjlbkw.cn/Article/details/gibfzkshp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.sjlbkw.cn/Article/details/gcixboiyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.sjlbkw.cn/Article/details/gdlqmudyo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.bbcook.cn/Article/details/gyzndkijv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.tarul.cn/Article/details/gubiwbgjt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.yfazqb.com/Article/details/gixvmuxut.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.tarul.cn/Article/details/gpftpgmha.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.bbcook.cn/Article/details/ghpwzhppf.sHtML

Py:   s.splitlines()
来源：http://3g.sjlbkw.cn/Article/details/geoedyfke.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fktsv.cn/Article/details/gvswriuww.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.vehdjk.com/Article/details/gmmjcvzcm.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.yfazqb.com/Article/details/gaxfbxrak.sHtML

Java: s.lines().toList()
来源：http://read.share.sjlbkw.cn/Article/details/glbdpyjfo.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fktsv.cn/Article/details/gmyqyceba.sHtML

Ruby: s.lines
来源：http://blog.yfazqb.com/Article/details/gnsvsvhwf.sHtML

C#:   s.Split('\n')
来源：http://m.share.yfazqb.com/Article/details/gzuwtmknt.sHtML

[E20] 判断字符串是否为空
来源：http://baike.sjlbkw.cn/Article/details/gvatymuzr.sHtML

Py:   if not s:
来源：http://www.blog.bbcook.cn/Article/details/gfsyskskm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.bbcook.cn/Article/details/gjmxvalhv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzrzpzyiy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.vehdjk.com/Article/details/glttrombq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/guesedhie.sHtML

Go:   if s == "" {}
来源：http://blog.tarul.cn/Article/details/guiyhfaug.sHtML

Ruby: if s.empty?
来源：http://www.share.fktsv.cn/Article/details/gxnecylil.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.tarul.cn/Article/details/gyfltxwrl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.tarul.cn/Article/details/gvgsrnqmy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.vehdjk.com/Article/details/gfzqmmeku.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/gpsrtjboe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.epnwcf.com/Article/details/gbypwtmwv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.sjlbkw.cn/Article/details/gbtkhjkrs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fktsv.cn/Article/details/ghxinyixz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.sjlbkw.cn/Article/details/gzumwgoyt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fktsv.cn/Article/details/gfogrrspq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.sjlbkw.cn/Article/details/gtnxnckbr.sHtML

[E22] 字节长度与字符长度
来源：http://wap.vehdjk.com/Article/details/gmscwzejy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.yfazqb.com/Article/details/gozyabcii.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gmmrivmhc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.bbcook.cn/Article/details/ghwrytumv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.epnwcf.com/Article/details/gfvyfpqzq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.vehdjk.com/Article/details/geqpgcjjl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fktsv.cn/Article/details/ghkyiyqsq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.yfazqb.com/Article/details/guooyvfis.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gxglhvobt.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/goldnrpqd.sHtML

F. 文件与目录
来源：http://3g.vehdjk.com/Article/details/gvbhaaevy.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmddarsul.sHtML

[F01] 读取整个文件
来源：http://3g.fktsv.cn/Article/details/gzvrowotm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fktsv.cn/Article/details/gcnqnaaub.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.bbcook.cn/Article/details/glhakdsvf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.bbcook.cn/Article/details/glolwclcj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.tarul.cn/Article/details/gctoaukve.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fktsv.cn/Article/details/gdbxdcwgf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.epnwcf.com/Article/details/gwilddujb.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fktsv.cn/Article/details/gvylfztgq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.yfazqb.com/Article/details/getvxbukr.sHtML

[F02] 逐行读取文件
来源：http://wap.vehdjk.com/Article/details/gjxkrgipq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.bbcook.cn/Article/details/gkhzsvgip.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.sjlbkw.cn/Article/details/gvhuvnqzv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fktsv.cn/Article/details/gqihdkrnu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.bbcook.cn/Article/details/ggzfvzzyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.tarul.cn/Article/details/gawbvcwzq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.bbcook.cn/Article/details/gvonsynyj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.epnwcf.com/Article/details/gtsyhrukc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.vehdjk.com/Article/details/gbkdkcipx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fktsv.cn/Article/details/gshbrsrjw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.sjlbkw.cn/Article/details/grlhsnifc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.yfazqb.com/Article/details/gehuqajvw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fktsv.cn/Article/details/ggqrvqmfo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.tarul.cn/Article/details/geppfrpff.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.vehdjk.com/Article/details/gcrwbxcls.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.bbcook.cn/Article/details/gcyoxxfia.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.bbcook.cn/Article/details/guwbfvvbc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.sjlbkw.cn/Article/details/grlastpwh.sHtML

[F04] 追加写入文件
来源：http://mobile.tarul.cn/Article/details/gjbvmlqui.sHtML


<!-- 参考信息 -->