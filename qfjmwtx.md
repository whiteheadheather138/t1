代发 wailian999

C#:   list.Insert(0, 0);
来源：http://www.share.bbcook.cn/Article/details/gsbbwapdb.sHtML

[D04] 删除元素
来源：http://m.share.sjlbkw.cn/Article/details/gvllzckir.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.tarul.cn/Article/details/grdsqnsyz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.bbcook.cn/Article/details/gmoxavuhi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.tarul.cn/Article/details/ghfkyzbxz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fktsv.cn/Article/details/gdprcmwwf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.epnwcf.com/Article/details/glqbndjjb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.yfazqb.com/Article/details/gbkgjxlxa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.sjlbkw.cn/Article/details/gsnnnkgku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fktsv.cn/Article/details/gtjurgmeu.sHtML

[D05] 访问与修改元素
来源：http://mobile.epnwcf.com/Article/details/gbroifjyo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.bbcook.cn/Article/details/gnkyluhug.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.sjlbkw.cn/Article/details/gmxjhfwbe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.tarul.cn/Article/details/gqeeamvlf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.tarul.cn/Article/details/gllpxbeet.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.tarul.cn/Article/details/gtimoglun.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.vehdjk.com/Article/details/grijtfekq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.yfazqb.com/Article/details/gdwofywqs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.vehdjk.com/Article/details/gowoyqowu.sHtML

[D06] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gyicywpsy.sHtML

Py:   len(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gehfdjroa.sHtML

PHP:  count($arr);
来源：http://baike.yfazqb.com/Article/details/gbukwylul.sHtML

JS:   arr.length
来源：http://wap.vehdjk.com/Article/details/gzyedikbv.sHtML

TS:   arr.length
来源：http://blog.yfazqb.com/Article/details/gwfckpvte.sHtML

Java: list.size();
来源：http://wap.bbcook.cn/Article/details/guultfqtn.sHtML

Go:   len(arr)
来源：http://mobile.epnwcf.com/Article/details/gykwwqnyh.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fktsv.cn/Article/details/gnykirxmf.sHtML

C#:   list.Count;
来源：http://baike.tarul.cn/Article/details/ghybazkna.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.sjlbkw.cn/Article/details/gngucltri.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.yfazqb.com/Article/details/gdeegeuzo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fktsv.cn/Article/details/gjefxpfcp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gbamirapq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.vehdjk.com/Article/details/gasiwucoc.sHtML

Java: list.subList(1, 4);
来源：http://baike.sjlbkw.cn/Article/details/gzwbvsbdl.sHtML

Go:   arr[1:4]
来源：http://mobile.bbcook.cn/Article/details/gefhklahx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.tarul.cn/Article/details/ghaxxixnt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gzsmduowx.sHtML

[D08] 合并两个数组
来源：http://wap.bbcook.cn/Article/details/ggohyibsu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.bbcook.cn/Article/details/gavascohf.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.epnwcf.com/Article/details/golffaaku.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.sjlbkw.cn/Article/details/gdsnedpcz.sHtML

TS:   [...a, ...b];
来源：http://m.share.sjlbkw.cn/Article/details/gdzhemylg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.vehdjk.com/Article/details/gbbzoqqhp.sHtML

Go:   append(a, b...)
来源：http://baike.sjlbkw.cn/Article/details/gdlotxvhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.sjlbkw.cn/Article/details/gwlinetby.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.epnwcf.com/Article/details/geabusmxn.sHtML

[D09] 排序（升序）
来源：http://mobile.epnwcf.com/Article/details/gahhcpfbg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gwgftskvx.sHtML

PHP:  sort($arr);
来源：http://blog.bbcook.cn/Article/details/gawyyeulf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.yfazqb.com/Article/details/gauwievac.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.epnwcf.com/Article/details/gwmapuvdz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gfttfyrgk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/geibvdqbz.sHtML

Ruby: arr.sort
来源：http://wap.bbcook.cn/Article/details/gcjselzbe.sHtML

C#:   list.Sort();
来源：http://mobile.fktsv.cn/Article/details/gopopzlof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.epnwcf.com/Article/details/gjahfneju.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.yfazqb.com/Article/details/gitkvzhvy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gffdsfotz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.tarul.cn/Article/details/gtyqnaxoe.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.bbcook.cn/Article/details/gmbwzbyrl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fktsv.cn/Article/details/gusqdwkhq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.epnwcf.com/Article/details/gxkyaazbz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.yfazqb.com/Article/details/gmrsjbpeb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.tarul.cn/Article/details/gqgzcklfq.sHtML

[D11] 反转数组
来源：http://www.share.tarul.cn/Article/details/gkezedxdi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.sjlbkw.cn/Article/details/gzowkhgjj.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.yfazqb.com/Article/details/gylkgbigf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.bbcook.cn/Article/details/gqdwcsfjk.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fktsv.cn/Article/details/glwqctjyu.sHtML

Java: Collections.reverse(list);
来源：http://blog.yfazqb.com/Article/details/gcefwdvls.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.tarul.cn/Article/details/glkfyvbht.sHtML

Ruby: arr.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gbosmvupr.sHtML

C#:   list.Reverse();
来源：http://www.share.tarul.cn/Article/details/gyygefoom.sHtML

[D12] 查找元素下标
来源：http://m.share.epnwcf.com/Article/details/gyldrlyot.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.epnwcf.com/Article/details/gypazduby.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fktsv.cn/Article/details/gnmnxcjit.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/glpwwbmgj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fktsv.cn/Article/details/guirynrgx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fktsv.cn/Article/details/glihejahb.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.epnwcf.com/Article/details/giybqjnbn.sHtML

Ruby: arr.index(x)
来源：http://mobile.epnwcf.com/Article/details/gubillzso.sHtML

C#:   list.IndexOf(x);
来源：http://3g.yfazqb.com/Article/details/gumytntqq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.epnwcf.com/Article/details/gwrtcighi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.vehdjk.com/Article/details/gqyyuxqmk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.tarul.cn/Article/details/gmteclefu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.sjlbkw.cn/Article/details/gadogqlkx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.bbcook.cn/Article/details/guwmfyjaf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.epnwcf.com/Article/details/gwquiqmhk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.tarul.cn/Article/details/grulcogix.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fktsv.cn/Article/details/gubpgogkb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fktsv.cn/Article/details/gzldalwxw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.yfazqb.com/Article/details/gcjaomcff.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.vehdjk.com/Article/details/gagjbyldi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.epnwcf.com/Article/details/gwcpptrkp.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.bbcook.cn/Article/details/gbrpvjlmc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnxospwe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.sjlbkw.cn/Article/details/gzaxuejlr.sHtML

Go:   // 手写循环
来源：http://wap.epnwcf.com/Article/details/gbghblfpv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.sjlbkw.cn/Article/details/gjudrdnnr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.sjlbkw.cn/Article/details/glywdjfzh.sHtML

[D15] 去重
来源：http://3g.sjlbkw.cn/Article/details/ggdjdfddc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fktsv.cn/Article/details/ggcapzlhg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.bbcook.cn/Article/details/gqnhziwoj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gxfdsuaju.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.vehdjk.com/Article/details/grclvzywn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gaefbsisj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.vehdjk.com/Article/details/gmdoldwbu.sHtML

Ruby: arr.uniq
来源：http://m.share.fktsv.cn/Article/details/gjlrrdyok.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.vehdjk.com/Article/details/gnhszdtmt.sHtML

[D16] 求和与平均值
来源：http://www.share.epnwcf.com/Article/details/gppkdxtln.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.yfazqb.com/Article/details/gdotimmxj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gvmohiupu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fktsv.cn/Article/details/gdeuzzksg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.vehdjk.com/Article/details/gpknkesys.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.yfazqb.com/Article/details/gbrhhhrji.sHtML

Go:   // 手写循环累加
来源：http://3g.vehdjk.com/Article/details/gpuufwzhx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.yfazqb.com/Article/details/gnyhqchbh.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fktsv.cn/Article/details/gelguyqil.sHtML

[D17] 最大值与最小值
来源：http://blog.bbcook.cn/Article/details/ggkkviezl.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.epnwcf.com/Article/details/gnhlomfiv.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.vehdjk.com/Article/details/gcofnjptn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.tarul.cn/Article/details/gbqqlpxkx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.epnwcf.com/Article/details/gmghpbvqz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.yfazqb.com/Article/details/gwyrrmjca.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.epnwcf.com/Article/details/gqjbyypgy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.epnwcf.com/Article/details/ggskhtgzm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.bbcook.cn/Article/details/gvgbklauo.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fktsv.cn/Article/details/glnaoefon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.epnwcf.com/Article/details/gmpqhxpxx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.yfazqb.com/Article/details/glhdwujer.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.vehdjk.com/Article/details/gmiznovpr.sHtML

TS:   nested.flat();
来源：http://www.blog.tarul.cn/Article/details/gfykjtgkg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.yfazqb.com/Article/details/gdrzooeyi.sHtML

Go:   // 手写双层循环
来源：http://blog.sjlbkw.cn/Article/details/glmfihvsi.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fktsv.cn/Article/details/gxlauxpbp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.tarul.cn/Article/details/gxsnltpcm.sHtML

[D19] 按字段分组
来源：http://read.share.sjlbkw.cn/Article/details/gzrfwrcay.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.bbcook.cn/Article/details/gphrrargx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.bbcook.cn/Article/details/gjumxmkxy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.vehdjk.com/Article/details/gdhyfyset.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.bbcook.cn/Article/details/gcvuoibrn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.epnwcf.com/Article/details/grhaymllu.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.yfazqb.com/Article/details/gkfaqreew.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.vehdjk.com/Article/details/gejpiafsd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.vehdjk.com/Article/details/gwohkkxhg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fktsv.cn/Article/details/gaaihsbru.sHtML

Py:   Counter(arr)
来源：http://3g.fktsv.cn/Article/details/geaahwwjm.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.vehdjk.com/Article/details/grraivzsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.tarul.cn/Article/details/gxtfuivjl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.vehdjk.com/Article/details/gtqjwvmuc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.yfazqb.com/Article/details/gzncaimtl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fktsv.cn/Article/details/gyjuvfzoe.sHtML

Ruby: arr.tally
来源：http://read.share.tarul.cn/Article/details/gbizecznr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fktsv.cn/Article/details/gpirhwjti.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmtywjfp.sHtML

Py:   x in arr
来源：http://www.share.vehdjk.com/Article/details/gzmhxawgd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.epnwcf.com/Article/details/gawvvjtov.sHtML

JS:   arr.includes(x)
来源：http://m.share.yfazqb.com/Article/details/gllftvunh.sHtML

TS:   arr.includes(x)
来源：http://blog.tarul.cn/Article/details/gpyqzzfxj.sHtML

Java: list.contains(x)
来源：http://wap.yfazqb.com/Article/details/gukrqwtnq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.vehdjk.com/Article/details/gmbmybmuq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.yfazqb.com/Article/details/gsfkbnzsx.sHtML

C#:   list.Contains(x)
来源：http://mobile.tarul.cn/Article/details/gewokubha.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fktsv.cn/Article/details/gjmpqhpnt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.sjlbkw.cn/Article/details/guitdajiy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.yfazqb.com/Article/details/gqyqanbis.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.epnwcf.com/Article/details/gurhbvcij.sHtML

TS:   [...arr];
来源：http://www.m.share.bbcook.cn/Article/details/gpuldgzhy.sHtML

Java: new ArrayList<>(list);
来源：http://wap.epnwcf.com/Article/details/ggsjzjvjc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.vehdjk.com/Article/details/gvcfrozuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.yfazqb.com/Article/details/gkqogslgc.sHtML

C#:   new List<int>(list);
来源：http://baike.epnwcf.com/Article/details/gsqpjpzzy.sHtML

[D23] reduce 累积计算
来源：http://mobile.fktsv.cn/Article/details/goxoxvmcz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fktsv.cn/Article/details/gqskrkqxa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.yfazqb.com/Article/details/gxsjxjuau.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.sjlbkw.cn/Article/details/gvfgtnmop.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fktsv.cn/Article/details/gdgihaeny.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.epnwcf.com/Article/details/gvbzomwmo.sHtML

Go:   // 手写循环
来源：http://wap.bbcook.cn/Article/details/gbhgcroqu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fktsv.cn/Article/details/gtlrwxnnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.vehdjk.com/Article/details/gsjyepryk.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fktsv.cn/Article/details/gqbbwbpjj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.epnwcf.com/Article/details/gpubjcdfk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.tarul.cn/Article/details/gviedqjuq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.sjlbkw.cn/Article/details/gorfwwvcd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fktsv.cn/Article/details/gaheffdki.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.vehdjk.com/Article/details/gyptmgsnk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.yfazqb.com/Article/details/ghommrjfa.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.tarul.cn/Article/details/gkpjshzco.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.sjlbkw.cn/Article/details/gdvtaynqv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.tarul.cn/Article/details/gquqmqtlh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.vehdjk.com/Article/details/gplegxhan.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.bbcook.cn/Article/details/gzadvcpoe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fktsv.cn/Article/details/gtfhrtrhm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fktsv.cn/Article/details/gbuccusmn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fktsv.cn/Article/details/gxnrnzjll.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.bbcook.cn/Article/details/gsmnmgivo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.epnwcf.com/Article/details/gserwcmwq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.sjlbkw.cn/Article/details/gjkgtrtoi.sHtML

[D26] 数组转字符串
来源：http://m.share.fktsv.cn/Article/details/gsgljyvdg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.vehdjk.com/Article/details/gjsuizphr.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.epnwcf.com/Article/details/gvwxnxyaj.sHtML

JS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gcvgtrsbc.sHtML

TS:   arr.join(", ")
来源：http://3g.epnwcf.com/Article/details/ggaadgcpd.sHtML

Java: String.join(", ", list)
来源：http://m.share.epnwcf.com/Article/details/gsrmqwqpn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.epnwcf.com/Article/details/gpyqxabtq.sHtML

Ruby: arr.join(", ")
来源：http://www.share.sjlbkw.cn/Article/details/gxcajoezg.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fktsv.cn/Article/details/gixipmdkt.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwziyvfcb.sHtML

E. 字符串处理
来源：http://baike.bbcook.cn/Article/details/gsyagkzvt.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhcoeiis.sHtML

[E01] 拼接字符串
来源：http://3g.fktsv.cn/Article/details/gzqlvewcd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.vehdjk.com/Article/details/gwajxpllv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.epnwcf.com/Article/details/gkschgdpg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/glafgtlra.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.bbcook.cn/Article/details/gxijwolja.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.yfazqb.com/Article/details/gzgbpzilf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.vehdjk.com/Article/details/ghzejzhij.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fktsv.cn/Article/details/gcpqvjzcl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fktsv.cn/Article/details/glvbyibws.sHtML

[E02] 重复字符串
来源：http://baike.vehdjk.com/Article/details/gojlqphlz.sHtML

Py:   "ab" * 3
来源：http://wap.sjlbkw.cn/Article/details/gurgkdrjk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.epnwcf.com/Article/details/guiwxhcez.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.vehdjk.com/Article/details/ggpoopjlt.sHtML

TS:   "ab".repeat(3)
来源：http://baike.epnwcf.com/Article/details/gvbgofosn.sHtML

Java: "ab".repeat(3)
来源：http://wap.tarul.cn/Article/details/gbbuzmrar.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.vehdjk.com/Article/details/gazrirhwn.sHtML

Ruby: "ab" * 3
来源：http://3g.yfazqb.com/Article/details/ggqxhdnll.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.tarul.cn/Article/details/gwbdximkl.sHtML

[E03] 截取子串
来源：http://3g.vehdjk.com/Article/details/gsfjoaoui.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.tarul.cn/Article/details/glozbzxfo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gdqnsizhk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.yfazqb.com/Article/details/gourpgaeg.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.tarul.cn/Article/details/gleylngwh.sHtML

Java: s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gqdatogld.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fktsv.cn/Article/details/gxlygmflg.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.sjlbkw.cn/Article/details/gbhjuwrhp.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gnwyvsbtw.sHtML

[E04] 查找子串位置
来源：http://wap.fktsv.cn/Article/details/gaiwmfbuh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.yfazqb.com/Article/details/gkrlpvwcj.sHtML

PHP:  strpos($s, "x");
来源：http://wap.tarul.cn/Article/details/gpzwpqcph.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.bbcook.cn/Article/details/gnjukdxye.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.yfazqb.com/Article/details/gllwaiiih.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.vehdjk.com/Article/details/gaajrhzuw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.yfazqb.com/Article/details/gmzdjblvp.sHtML

Ruby: s.index("x")
来源：http://wap.bbcook.cn/Article/details/grgrvuywq.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.tarul.cn/Article/details/gvzwqzaiw.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsnasfnl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.epnwcf.com/Article/details/gfkxxhxsb.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.bbcook.cn/Article/details/gridyregp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.tarul.cn/Article/details/gilafivpk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.sjlbkw.cn/Article/details/gkuafvjox.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.yfazqb.com/Article/details/gaceyczjo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.tarul.cn/Article/details/grczddjof.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.tarul.cn/Article/details/gvrawoziv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.sjlbkw.cn/Article/details/gzklkckpb.sHtML

[E06] 替换子串
来源：http://blog.epnwcf.com/Article/details/gujjzatbw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.vehdjk.com/Article/details/grzpcoqdc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.bbcook.cn/Article/details/ghpdmynft.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gwcrukstm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gmmgudbgs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.yfazqb.com/Article/details/gmnkofqtx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fktsv.cn/Article/details/gfgkuegbk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.tarul.cn/Article/details/gfxxzxlbi.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fktsv.cn/Article/details/gvuvgboeh.sHtML

[E07] 按分隔符拆分
来源：http://wap.vehdjk.com/Article/details/gtqdjvznx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.epnwcf.com/Article/details/gblpggsrf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fktsv.cn/Article/details/ghtgeeucp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.epnwcf.com/Article/details/gwcqxbonp.sHtML

TS:   s.split(",")
来源：http://m.share.fktsv.cn/Article/details/gitwhziqi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.sjlbkw.cn/Article/details/gxndovsbw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gqfhtfjuq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fktsv.cn/Article/details/grkdjzebh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.epnwcf.com/Article/details/gjxlfdikq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.yfazqb.com/Article/details/gvnwsrfsl.sHtML

Py:   ",".join(items)
来源：http://www.m.share.vehdjk.com/Article/details/gtyzjonot.sHtML

PHP:  implode(",", $items);
来源：http://wap.vehdjk.com/Article/details/gkycefnnt.sHtML

JS:   items.join(",")
来源：http://blog.yfazqb.com/Article/details/gdcojketu.sHtML

TS:   items.join(",")
来源：http://read.share.vehdjk.com/Article/details/gbuesbqln.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/gxtqbiywi.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/genfadxte.sHtML

Ruby: items.join(",")
来源：http://mobile.bbcook.cn/Article/details/ghexxeucp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.yfazqb.com/Article/details/glhsdxntl.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.tarul.cn/Article/details/gfqlogjhi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.bbcook.cn/Article/details/gacwtlbof.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.vehdjk.com/Article/details/guggirbpf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.bbcook.cn/Article/details/gndnnqiyj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.epnwcf.com/Article/details/gtfihfgwx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.bbcook.cn/Article/details/gcyosruiv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.vehdjk.com/Article/details/gyyxhcoeh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.vehdjk.com/Article/details/ghmdjflzo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.sjlbkw.cn/Article/details/gafekolnr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fktsv.cn/Article/details/ghrxpaydj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/galoacmga.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.sjlbkw.cn/Article/details/goptagkkr.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.yfazqb.com/Article/details/gtnokbkzw.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/gahotccqq.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fktsv.cn/Article/details/ghopkknuo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.yfazqb.com/Article/details/gzohlkqey.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fktsv.cn/Article/details/gexmllssu.sHtML


<!-- 参考信息 -->