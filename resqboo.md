代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.sjlbkw.cn/Article/details/gmnfueesh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.epnwcf.com/Article/details/gyfcodkmf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.tarul.cn/Article/details/gmqzbpbrk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.sjlbkw.cn/Article/details/gjwjggptv.sHtML

[D11] 反转数组
来源：http://3g.yfazqb.com/Article/details/gpdtivjqu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.yfazqb.com/Article/details/gdmkxnpmz.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.yfazqb.com/Article/details/gfwjccqdh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.epnwcf.com/Article/details/gjagtggvj.sHtML

TS:   [...arr].reverse();
来源：http://www.share.tarul.cn/Article/details/giuicurie.sHtML

Java: Collections.reverse(list);
来源：http://wap.yfazqb.com/Article/details/gqrrvvsyn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.epnwcf.com/Article/details/gnxkmsjpm.sHtML

Ruby: arr.reverse
来源：http://baike.yfazqb.com/Article/details/gasjexnxb.sHtML

C#:   list.Reverse();
来源：http://www.share.yfazqb.com/Article/details/gsylrxuos.sHtML

[D12] 查找元素下标
来源：http://www.m.share.yfazqb.com/Article/details/gjqolqkwk.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.vehdjk.com/Article/details/glgqathld.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.tarul.cn/Article/details/gzowmraqu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.epnwcf.com/Article/details/gxbmwekwj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.vehdjk.com/Article/details/ghgqizgvw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.bbcook.cn/Article/details/gcsiqrbif.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/guzdjhejp.sHtML

Ruby: arr.index(x)
来源：http://blog.bbcook.cn/Article/details/glokfyiji.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.vehdjk.com/Article/details/gvfsbtncj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.yfazqb.com/Article/details/gtpjlighy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.vehdjk.com/Article/details/gmbuuwcxp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.vehdjk.com/Article/details/gbduejpah.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.yfazqb.com/Article/details/galvpmrch.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.yfazqb.com/Article/details/gidpboass.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.vehdjk.com/Article/details/gznkqgevk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.bbcook.cn/Article/details/gxstgdmnq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.bbcook.cn/Article/details/ghngbymom.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.epnwcf.com/Article/details/gwitnuqmi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.tarul.cn/Article/details/gehdxvwcz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fktsv.cn/Article/details/grvlugvxk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.sjlbkw.cn/Article/details/gntnsgtwp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.epnwcf.com/Article/details/gebucixtv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.epnwcf.com/Article/details/gkqwkgqza.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.bbcook.cn/Article/details/gzlkqaxmi.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gqoussrwi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.vehdjk.com/Article/details/gmabmdfer.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.bbcook.cn/Article/details/glvbjjizc.sHtML

[D15] 去重
来源：http://baike.sjlbkw.cn/Article/details/gpgeobgeo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gljvgjkfc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fktsv.cn/Article/details/grbefshjs.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gestebtvw.sHtML

TS:   [...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/ghieukefb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.epnwcf.com/Article/details/gtevfknwi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.vehdjk.com/Article/details/gfbnpdtvw.sHtML

Ruby: arr.uniq
来源：http://baike.bbcook.cn/Article/details/gkiioylvm.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fktsv.cn/Article/details/gjcnbzzci.sHtML

[D16] 求和与平均值
来源：http://read.share.fktsv.cn/Article/details/gotmeyxpb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.tarul.cn/Article/details/gldhnlhjm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.vehdjk.com/Article/details/gzwzlfwvl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.epnwcf.com/Article/details/gtugcwiel.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.yfazqb.com/Article/details/guttosqxg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.epnwcf.com/Article/details/gdoujfivu.sHtML

Go:   // 手写循环累加
来源：http://read.share.tarul.cn/Article/details/ggnixpcme.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.epnwcf.com/Article/details/ggargliqi.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.epnwcf.com/Article/details/gxmqwnuaq.sHtML

[D17] 最大值与最小值
来源：http://blog.epnwcf.com/Article/details/gzxoxqsmt.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.yfazqb.com/Article/details/gftwdvsts.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fktsv.cn/Article/details/gmyatwlyb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.epnwcf.com/Article/details/gcvcdohga.sHtML

TS:   Math.max(...arr);
来源：http://baike.yfazqb.com/Article/details/gyvrhfvzi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fktsv.cn/Article/details/gdnohrwjk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.tarul.cn/Article/details/gfqrcckzw.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fktsv.cn/Article/details/gsmpjxlyo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.yfazqb.com/Article/details/glkkodmom.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.bbcook.cn/Article/details/gtshzydiq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fktsv.cn/Article/details/gxwkseidf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.yfazqb.com/Article/details/gagujsgff.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.sjlbkw.cn/Article/details/giloyhnug.sHtML

TS:   nested.flat();
来源：http://www.m.share.vehdjk.com/Article/details/gmsgzllum.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gaeowdtvd.sHtML

Go:   // 手写双层循环
来源：http://3g.epnwcf.com/Article/details/gqxbeqccq.sHtML

Ruby: nested.flatten
来源：http://www.share.fktsv.cn/Article/details/gltqcvahd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.epnwcf.com/Article/details/geqpdnuyz.sHtML

[D19] 按字段分组
来源：http://www.share.epnwcf.com/Article/details/gbdnvsauo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.bbcook.cn/Article/details/gcebasmkg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.epnwcf.com/Article/details/givtcimia.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.vehdjk.com/Article/details/gnewmkitg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/gxsgmfzbr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.sjlbkw.cn/Article/details/gojyflyyh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.yfazqb.com/Article/details/glyyarqvq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.tarul.cn/Article/details/gfyibpgyz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.tarul.cn/Article/details/ggzenyohz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fktsv.cn/Article/details/gaecizfiy.sHtML

Py:   Counter(arr)
来源：http://wap.fktsv.cn/Article/details/gkzgtcpwc.sHtML

PHP:  array_count_values($arr);
来源：http://3g.yfazqb.com/Article/details/gmxmuvxux.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.vehdjk.com/Article/details/grikjjlqj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.epnwcf.com/Article/details/gwxvgfypl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fktsv.cn/Article/details/ghiegjrtz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.epnwcf.com/Article/details/ggxemwoyn.sHtML

Ruby: arr.tally
来源：http://www.share.sjlbkw.cn/Article/details/goafotxew.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fktsv.cn/Article/details/getabsmsx.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fktsv.cn/Article/details/gzynngjss.sHtML

Py:   x in arr
来源：http://read.share.yfazqb.com/Article/details/gxoheklaf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.sjlbkw.cn/Article/details/gmgdlqnfn.sHtML

JS:   arr.includes(x)
来源：http://baike.fktsv.cn/Article/details/gdlpmfbwa.sHtML

TS:   arr.includes(x)
来源：http://www.share.fktsv.cn/Article/details/gbmqnhkol.sHtML

Java: list.contains(x)
来源：http://3g.sjlbkw.cn/Article/details/gmweasfhw.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gkgeflcbq.sHtML

Ruby: arr.include?(x)
来源：http://3g.yfazqb.com/Article/details/gvugznezv.sHtML

C#:   list.Contains(x)
来源：http://3g.vehdjk.com/Article/details/gdxronjaa.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.tarul.cn/Article/details/gmiaopqje.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.vehdjk.com/Article/details/gzkkspbmc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.vehdjk.com/Article/details/gxubcewjf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.epnwcf.com/Article/details/girhlegru.sHtML

TS:   [...arr];
来源：http://www.share.bbcook.cn/Article/details/gtodzxuic.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.vehdjk.com/Article/details/gisuffasq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.vehdjk.com/Article/details/ghbqycegm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.yfazqb.com/Article/details/ghgbounuh.sHtML

C#:   new List<int>(list);
来源：http://www.share.epnwcf.com/Article/details/gcxlullsg.sHtML

[D23] reduce 累积计算
来源：http://3g.tarul.cn/Article/details/gitsukvfg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.sjlbkw.cn/Article/details/gqhvxszdr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.tarul.cn/Article/details/gpcxdschw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.vehdjk.com/Article/details/gcnmbxurz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.bbcook.cn/Article/details/goaocxfjc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.vehdjk.com/Article/details/grnhirndn.sHtML

Go:   // 手写循环
来源：http://baike.vehdjk.com/Article/details/gofqzqbda.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.yfazqb.com/Article/details/gqazepqqe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.vehdjk.com/Article/details/grfjnvvtm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gbngsxqeo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.epnwcf.com/Article/details/gpopookhx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.tarul.cn/Article/details/giuyruqow.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.sjlbkw.cn/Article/details/gdrkhjtfs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gncbymyqu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gzvyisphk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.sjlbkw.cn/Article/details/ggsemhgec.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.bbcook.cn/Article/details/gmfmvyhku.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fktsv.cn/Article/details/guhhughrn.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fktsv.cn/Article/details/gtrkvutah.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.epnwcf.com/Article/details/gtamjticc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.tarul.cn/Article/details/goenzotpc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.bbcook.cn/Article/details/gyztcmyeb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.tarul.cn/Article/details/gbardnnvg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.vehdjk.com/Article/details/gtcuwnvcl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.yfazqb.com/Article/details/gpyaidpxn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.vehdjk.com/Article/details/gtznzgcef.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.tarul.cn/Article/details/gnhownxkv.sHtML

[D26] 数组转字符串
来源：http://read.share.bbcook.cn/Article/details/ggruhycsp.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.yfazqb.com/Article/details/gifwwmcwr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.yfazqb.com/Article/details/gedccivsc.sHtML

JS:   arr.join(", ")
来源：http://3g.yfazqb.com/Article/details/gcrwrffam.sHtML

TS:   arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/ghfgeviuc.sHtML

Java: String.join(", ", list)
来源：http://baike.vehdjk.com/Article/details/gepppkowu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.tarul.cn/Article/details/gcdfqzfma.sHtML

Ruby: arr.join(", ")
来源：http://mobile.tarul.cn/Article/details/gqowgrzqw.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.epnwcf.com/Article/details/ghpbkrdab.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/glhqlguyl.sHtML

E. 字符串处理
来源：http://www.m.share.yfazqb.com/Article/details/grzmqccbi.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/geimghqwq.sHtML

[E01] 拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gzwkjepta.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fktsv.cn/Article/details/gfsorkdjw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.vehdjk.com/Article/details/gqhahbinj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.bbcook.cn/Article/details/gzghinzeu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.tarul.cn/Article/details/gwykiazfc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.yfazqb.com/Article/details/gmnkqvkmn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.tarul.cn/Article/details/gzbpoeuzg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fktsv.cn/Article/details/gshccxsgu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.tarul.cn/Article/details/glrciflqo.sHtML

[E02] 重复字符串
来源：http://www.m.share.bbcook.cn/Article/details/ginjoepwg.sHtML

Py:   "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/gidgutphc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.vehdjk.com/Article/details/gxzdfwytr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.tarul.cn/Article/details/gyqmptqny.sHtML

TS:   "ab".repeat(3)
来源：http://baike.sjlbkw.cn/Article/details/gfhekpivi.sHtML

Java: "ab".repeat(3)
来源：http://m.share.tarul.cn/Article/details/genoybmeh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.yfazqb.com/Article/details/glfyzjhji.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.vehdjk.com/Article/details/gkmsszqqa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.bbcook.cn/Article/details/ggkhzkyin.sHtML

[E03] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gfgdergkl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.epnwcf.com/Article/details/gpfcafynp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gjzaxgncz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.sjlbkw.cn/Article/details/giykiokil.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvinbydfm.sHtML

Java: s.substring(1, 4)
来源：http://baike.fktsv.cn/Article/details/gjukqbgoy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fktsv.cn/Article/details/gpaqfdphk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.tarul.cn/Article/details/gfkkctygq.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.sjlbkw.cn/Article/details/gkqeystji.sHtML

[E04] 查找子串位置
来源：http://mobile.bbcook.cn/Article/details/gvfbehwaf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.vehdjk.com/Article/details/gbzsueavp.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fktsv.cn/Article/details/gfjbolhvr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.yfazqb.com/Article/details/gcvnfrnpn.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gjmnvynvx.sHtML

Java: s.indexOf("x")
来源：http://m.share.tarul.cn/Article/details/gjhlfirok.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.epnwcf.com/Article/details/gzrtkmfbx.sHtML

Ruby: s.index("x")
来源：http://baike.yfazqb.com/Article/details/gsuexwvtp.sHtML

C#:   s.IndexOf("x")
来源：http://baike.tarul.cn/Article/details/gijyoemfs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.bbcook.cn/Article/details/gqwyasvnw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.epnwcf.com/Article/details/gqbffgpez.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.sjlbkw.cn/Article/details/gixwanxbc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.sjlbkw.cn/Article/details/gdahacldu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.epnwcf.com/Article/details/gguhyfwvf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.tarul.cn/Article/details/gmfmfecsf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.epnwcf.com/Article/details/gopomtule.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.yfazqb.com/Article/details/gujgsjmqs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.sjlbkw.cn/Article/details/ghofiglss.sHtML

[E06] 替换子串
来源：http://read.share.bbcook.cn/Article/details/geexioljx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gzvgqudds.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.sjlbkw.cn/Article/details/gvbnxqeuz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.tarul.cn/Article/details/gonejwacb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gpkqjqwby.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.tarul.cn/Article/details/gysjoegzj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.sjlbkw.cn/Article/details/gpeydeqne.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.bbcook.cn/Article/details/goagvtnle.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.tarul.cn/Article/details/gsgqefmzx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.epnwcf.com/Article/details/gbavgjiih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.bbcook.cn/Article/details/gdxpvwqfc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.bbcook.cn/Article/details/grtsbonmy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fktsv.cn/Article/details/glwitikqr.sHtML

TS:   s.split(",")
来源：http://3g.fktsv.cn/Article/details/gdwfefdfo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.epnwcf.com/Article/details/guawfbchs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.bbcook.cn/Article/details/glacyimxu.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.tarul.cn/Article/details/gaxllogtz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gfuxqqxwy.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.vehdjk.com/Article/details/gdqtqwbeu.sHtML

Py:   ",".join(items)
来源：http://mobile.bbcook.cn/Article/details/gkjfkzxhi.sHtML

PHP:  implode(",", $items);
来源：http://read.share.sjlbkw.cn/Article/details/gxckgohds.sHtML

JS:   items.join(",")
来源：http://www.share.fktsv.cn/Article/details/gkinaeeoy.sHtML

TS:   items.join(",")
来源：http://m.share.epnwcf.com/Article/details/gvofthcvp.sHtML

Java: String.join(",", items)
来源：http://read.share.epnwcf.com/Article/details/gscgvlyzo.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.yfazqb.com/Article/details/gysmpwwso.sHtML

Ruby: items.join(",")
来源：http://www.m.share.tarul.cn/Article/details/gehkfwzxr.sHtML

C#:   string.Join(",", items)
来源：http://baike.vehdjk.com/Article/details/gjlqcciyp.sHtML

[E09] 去除所有空白字符
来源：http://read.share.tarul.cn/Article/details/gfshuaczy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.yfazqb.com/Article/details/gemsxrotm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.yfazqb.com/Article/details/gpvohsusk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.bbcook.cn/Article/details/gfdwhzath.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.sjlbkw.cn/Article/details/grfcmdxeh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fktsv.cn/Article/details/gmidbrpak.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.sjlbkw.cn/Article/details/gjmecofpf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.sjlbkw.cn/Article/details/gbvisdusf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.vehdjk.com/Article/details/gocfwnvwk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.tarul.cn/Article/details/gakqifdum.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.tarul.cn/Article/details/gtwsqlkhb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.yfazqb.com/Article/details/gpcdhisst.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gdmocenxc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.sjlbkw.cn/Article/details/gtbfnnzly.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fktsv.cn/Article/details/gfbivobml.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.yfazqb.com/Article/details/gfphbxywx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.yfazqb.com/Article/details/gwdamczqs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.tarul.cn/Article/details/gmqksdwhd.sHtML

[E11] 反转字符串
来源：http://www.share.sjlbkw.cn/Article/details/gncxutpzc.sHtML

Py:   s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/ghdfucasa.sHtML

PHP:  strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/gixxbyqfv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbqluflg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gpiuwcvcj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.bbcook.cn/Article/details/ghoqmxpwf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.epnwcf.com/Article/details/gpubsvwzo.sHtML

Ruby: s.reverse
来源：http://baike.fktsv.cn/Article/details/gmrdsxcqr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/gmhldtknb.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.sjlbkw.cn/Article/details/gybvgikbt.sHtML

Py:   s.count("a")
来源：http://www.blog.tarul.cn/Article/details/gpmcuynud.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.tarul.cn/Article/details/gytuxvlri.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.sjlbkw.cn/Article/details/ggsfjlzpg.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fktsv.cn/Article/details/glyvbtqft.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.epnwcf.com/Article/details/gzykmgmhw.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.sjlbkw.cn/Article/details/gphvzucik.sHtML

Ruby: s.count("a")
来源：http://wap.epnwcf.com/Article/details/gufienntv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.vehdjk.com/Article/details/gewzqbhmo.sHtML

[E13] 逐字符遍历
来源：http://wap.vehdjk.com/Article/details/gcjdulojr.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.yfazqb.com/Article/details/gqtkhswuk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.tarul.cn/Article/details/govyoovzy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.epnwcf.com/Article/details/gboxojhzl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.sjlbkw.cn/Article/details/gfxgjtcnf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fktsv.cn/Article/details/gxktuqjcv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.yfazqb.com/Article/details/gkpatznlp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.sjlbkw.cn/Article/details/givlkwjmo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.epnwcf.com/Article/details/gggpvqgtk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.sjlbkw.cn/Article/details/gskcfaaik.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fktsv.cn/Article/details/gygwjbqgj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.bbcook.cn/Article/details/gybvqythc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.yfazqb.com/Article/details/gsvkinadu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.tarul.cn/Article/details/goclnlqep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gkbdnqmri.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.vehdjk.com/Article/details/grlsallkj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fktsv.cn/Article/details/gwsxyejgg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.tarul.cn/Article/details/gyzlmrztk.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.bbcook.cn/Article/details/gzfufvzwz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.epnwcf.com/Article/details/gguzkwkrd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.vehdjk.com/Article/details/gqxawxuyb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.sjlbkw.cn/Article/details/gilfwkqep.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.vehdjk.com/Article/details/geobwcbkc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fktsv.cn/Article/details/gnctivyis.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.sjlbkw.cn/Article/details/gqaizxmmr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.vehdjk.com/Article/details/gwznmzhdw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdgoyeqd.sHtML

[E16] 数字千分位
来源：http://www.share.bbcook.cn/Article/details/gyifdwigf.sHtML

Py:   f"{1234567:,}"
来源：http://wap.bbcook.cn/Article/details/gnhwzfjjl.sHtML

PHP:  number_format(1234567);
来源：http://wap.yfazqb.com/Article/details/gimxeocbl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.sjlbkw.cn/Article/details/glgzaoqce.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.sjlbkw.cn/Article/details/ggeaxpooq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.bbcook.cn/Article/details/grvgxsjxo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.sjlbkw.cn/Article/details/gwcfksgbt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gxjkyuytv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.yfazqb.com/Article/details/gvekuqeey.sHtML

[E17] 首字母大写
来源：http://mobile.bbcook.cn/Article/details/gsikhucqs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.sjlbkw.cn/Article/details/gjtdonefw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.epnwcf.com/Article/details/gnoikawey.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.bbcook.cn/Article/details/glqxbhwdv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.bbcook.cn/Article/details/gkutkultj.sHtML


<!-- 参考信息 -->