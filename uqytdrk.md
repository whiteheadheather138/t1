代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.vehdjk.com/Article/details/gtlpyuowm.sHtML

Java: list.add(0, 0);
来源：http://www.blog.tarul.cn/Article/details/ghtluogxh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.sjlbkw.cn/Article/details/gbibprjfa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.yfazqb.com/Article/details/gkfhykvax.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.tarul.cn/Article/details/gxfgugrit.sHtML

[D04] 删除元素
来源：http://blog.tarul.cn/Article/details/gudubajvf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.epnwcf.com/Article/details/gkbifguxf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.vehdjk.com/Article/details/ghbnwefqq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.sjlbkw.cn/Article/details/ggwwifzdi.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.bbcook.cn/Article/details/gpcqqfena.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fktsv.cn/Article/details/gldfepvtg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.vehdjk.com/Article/details/gcsioyvmb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.epnwcf.com/Article/details/gqtmorljy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.tarul.cn/Article/details/ggauimmeu.sHtML

[D05] 访问与修改元素
来源：http://mobile.sjlbkw.cn/Article/details/ggmaicxuy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.bbcook.cn/Article/details/gjmnzkgok.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.vehdjk.com/Article/details/ghpugqpep.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.epnwcf.com/Article/details/gywgevzye.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.sjlbkw.cn/Article/details/groecfolb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fktsv.cn/Article/details/gccravxre.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.bbcook.cn/Article/details/gbpvnecyu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.vehdjk.com/Article/details/guoruprds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fktsv.cn/Article/details/griogwbtm.sHtML

[D06] 数组长度
来源：http://read.share.tarul.cn/Article/details/gautjpvki.sHtML

Py:   len(arr)
来源：http://baike.vehdjk.com/Article/details/gkwuckdfa.sHtML

PHP:  count($arr);
来源：http://www.m.share.fktsv.cn/Article/details/grsvdfsgc.sHtML

JS:   arr.length
来源：http://blog.fktsv.cn/Article/details/gqiihomtc.sHtML

TS:   arr.length
来源：http://www.blog.vehdjk.com/Article/details/gzzkwapnb.sHtML

Java: list.size();
来源：http://www.share.tarul.cn/Article/details/gumlefgzr.sHtML

Go:   len(arr)
来源：http://www.blog.yfazqb.com/Article/details/gdvnrsgcy.sHtML

Ruby: arr.length; arr.size
来源：http://blog.epnwcf.com/Article/details/ggmgohxaj.sHtML

C#:   list.Count;
来源：http://www.m.share.tarul.cn/Article/details/gzxudltiq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.epnwcf.com/Article/details/gplhgdqwv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.vehdjk.com/Article/details/gnmfqzvid.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.yfazqb.com/Article/details/glhmeaphz.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.bbcook.cn/Article/details/gtbqgyypy.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.sjlbkw.cn/Article/details/gfdhgvtgl.sHtML

Java: list.subList(1, 4);
来源：http://blog.tarul.cn/Article/details/gduauzzin.sHtML

Go:   arr[1:4]
来源：http://read.share.fktsv.cn/Article/details/gltxhmipx.sHtML

Ruby: arr[1, 3]
来源：http://wap.fktsv.cn/Article/details/gmljodngj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.sjlbkw.cn/Article/details/gasoqbzwe.sHtML

[D08] 合并两个数组
来源：http://m.share.vehdjk.com/Article/details/ghthytqom.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.epnwcf.com/Article/details/gqjgmeazu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.tarul.cn/Article/details/gznofqylh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.bbcook.cn/Article/details/gmskhorrv.sHtML

TS:   [...a, ...b];
来源：http://www.share.tarul.cn/Article/details/gtpcpzrau.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fktsv.cn/Article/details/gvuftzrhz.sHtML

Go:   append(a, b...)
来源：http://baike.bbcook.cn/Article/details/gusozfqsf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.vehdjk.com/Article/details/ggfewdkor.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.bbcook.cn/Article/details/ginzuudvg.sHtML

[D09] 排序（升序）
来源：http://blog.yfazqb.com/Article/details/gfrlfyywh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/ghliysmky.sHtML

PHP:  sort($arr);
来源：http://mobile.yfazqb.com/Article/details/gsutuybuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.vehdjk.com/Article/details/gbzskoowa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.yfazqb.com/Article/details/gmtfoapdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.epnwcf.com/Article/details/gdbdfxdaf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gniolhtxg.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gewgrdfkv.sHtML

C#:   list.Sort();
来源：http://baike.epnwcf.com/Article/details/gbrdvgumx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.sjlbkw.cn/Article/details/gxgztcofp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fktsv.cn/Article/details/gbwcxvqek.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.bbcook.cn/Article/details/gswjywqgf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.bbcook.cn/Article/details/gjsppdlds.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.tarul.cn/Article/details/gfzkwdsez.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.yfazqb.com/Article/details/gfljjaxmf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.epnwcf.com/Article/details/gxpubksms.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.vehdjk.com/Article/details/gywaqutgi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.epnwcf.com/Article/details/gkzuyrirk.sHtML

[D11] 反转数组
来源：http://3g.epnwcf.com/Article/details/ggjlcjasp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fktsv.cn/Article/details/gcacucjsd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.epnwcf.com/Article/details/gvhvabskr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.sjlbkw.cn/Article/details/glufltaxt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.sjlbkw.cn/Article/details/gjuujvtim.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.tarul.cn/Article/details/gtoqtkrfy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.bbcook.cn/Article/details/gykzqguok.sHtML

Ruby: arr.reverse
来源：http://wap.tarul.cn/Article/details/gbbcsunkh.sHtML

C#:   list.Reverse();
来源：http://read.share.vehdjk.com/Article/details/gudwmfmmy.sHtML

[D12] 查找元素下标
来源：http://wap.fktsv.cn/Article/details/ggkbbqsyo.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.vehdjk.com/Article/details/gschwmplz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.tarul.cn/Article/details/gpxupkzth.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.yfazqb.com/Article/details/giunlklvn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.sjlbkw.cn/Article/details/gwjqowexi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.epnwcf.com/Article/details/gekgftfot.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fktsv.cn/Article/details/geojuymbp.sHtML

Ruby: arr.index(x)
来源：http://3g.tarul.cn/Article/details/gxphwznad.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.vehdjk.com/Article/details/giucwqbqu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.sjlbkw.cn/Article/details/gfrtwotzt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.epnwcf.com/Article/details/gtxomaiir.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.sjlbkw.cn/Article/details/gtlqcpzjo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.tarul.cn/Article/details/ggjrguplz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.yfazqb.com/Article/details/gkhixpsiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fktsv.cn/Article/details/gatjmwlqk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.epnwcf.com/Article/details/gucxmufne.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.yfazqb.com/Article/details/gbxfmrpuy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.yfazqb.com/Article/details/gspunebns.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.tarul.cn/Article/details/gbjblrzya.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.tarul.cn/Article/details/gdskhzhku.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.epnwcf.com/Article/details/gdyacustm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.tarul.cn/Article/details/gthibhrnz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.sjlbkw.cn/Article/details/guctskevf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.vehdjk.com/Article/details/gjztnarjy.sHtML

Go:   // 手写循环
来源：http://baike.fktsv.cn/Article/details/gpwbowvfp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.yfazqb.com/Article/details/gixpmhook.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.sjlbkw.cn/Article/details/grnrqqooj.sHtML

[D15] 去重
来源：http://3g.epnwcf.com/Article/details/glwlpqyqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.yfazqb.com/Article/details/gdyqkoppt.sHtML

PHP:  array_unique($arr);
来源：http://blog.sjlbkw.cn/Article/details/gvcszqtbc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fktsv.cn/Article/details/gvxcosfsf.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gdeahrjur.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.tarul.cn/Article/details/gvhfzdsqc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.sjlbkw.cn/Article/details/gsaxgfyza.sHtML

Ruby: arr.uniq
来源：http://www.m.share.sjlbkw.cn/Article/details/gsentspdo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.sjlbkw.cn/Article/details/gylwiiiil.sHtML

[D16] 求和与平均值
来源：http://blog.fktsv.cn/Article/details/gzqtlesvg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gsygejxzc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.vehdjk.com/Article/details/gxrhvxoad.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fktsv.cn/Article/details/guxiwzgoq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.tarul.cn/Article/details/gqkbwmivz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.tarul.cn/Article/details/gvakhttff.sHtML

Go:   // 手写循环累加
来源：http://wap.tarul.cn/Article/details/gzehuyqyt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.yfazqb.com/Article/details/gpvslvsym.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.tarul.cn/Article/details/galcpyhov.sHtML

[D17] 最大值与最小值
来源：http://wap.sjlbkw.cn/Article/details/glesmlwen.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.sjlbkw.cn/Article/details/gungdkcdk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.sjlbkw.cn/Article/details/gxzykfbut.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.yfazqb.com/Article/details/gzwuuydrt.sHtML

TS:   Math.max(...arr);
来源：http://3g.epnwcf.com/Article/details/grtonafnq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.epnwcf.com/Article/details/gttbuqnpz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.epnwcf.com/Article/details/gcwffwsbp.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.epnwcf.com/Article/details/gtvqhrjio.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.sjlbkw.cn/Article/details/gkwcfxaol.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.bbcook.cn/Article/details/gmpntbfvc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.tarul.cn/Article/details/gqeifrply.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.vehdjk.com/Article/details/ggxqyzzsy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.tarul.cn/Article/details/gxpzvcjca.sHtML

TS:   nested.flat();
来源：http://www.blog.fktsv.cn/Article/details/gqxfvyele.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.vehdjk.com/Article/details/gmkajkcip.sHtML

Go:   // 手写双层循环
来源：http://www.share.vehdjk.com/Article/details/gxqybbose.sHtML

Ruby: nested.flatten
来源：http://3g.vehdjk.com/Article/details/gkvfmnxsv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.epnwcf.com/Article/details/gjzjcpamb.sHtML

[D19] 按字段分组
来源：http://3g.yfazqb.com/Article/details/ggwzwakwv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.epnwcf.com/Article/details/gczpqlxmi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.epnwcf.com/Article/details/gxanqkplk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.sjlbkw.cn/Article/details/gugxxxmjg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/goqcgxstf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.epnwcf.com/Article/details/gfxkkmcka.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.bbcook.cn/Article/details/gvuavsoyp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.bbcook.cn/Article/details/gbntmonop.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.bbcook.cn/Article/details/gyxdpxtkq.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.yfazqb.com/Article/details/goguryokl.sHtML

Py:   Counter(arr)
来源：http://wap.tarul.cn/Article/details/gccrsqgqt.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.vehdjk.com/Article/details/gnqnvdsas.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.yfazqb.com/Article/details/gaejxdore.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.vehdjk.com/Article/details/gjiopwuio.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.vehdjk.com/Article/details/gsxlajlfz.sHtML

Go:   // 手写 map[T]int
来源：http://baike.yfazqb.com/Article/details/gesfrtjvi.sHtML

Ruby: arr.tally
来源：http://3g.tarul.cn/Article/details/gcfuhionb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.bbcook.cn/Article/details/gcqwcfnqp.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.tarul.cn/Article/details/ggzfkfttr.sHtML

Py:   x in arr
来源：http://www.share.bbcook.cn/Article/details/gpwaakini.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.bbcook.cn/Article/details/gvoigjcxw.sHtML

JS:   arr.includes(x)
来源：http://blog.bbcook.cn/Article/details/gixsiikzu.sHtML

TS:   arr.includes(x)
来源：http://3g.epnwcf.com/Article/details/gbctjryac.sHtML

Java: list.contains(x)
来源：http://www.share.vehdjk.com/Article/details/gyigkmvrc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gtkvcoyby.sHtML

Ruby: arr.include?(x)
来源：http://mobile.epnwcf.com/Article/details/gkefacbwh.sHtML

C#:   list.Contains(x)
来源：http://blog.bbcook.cn/Article/details/gchtcmknd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.tarul.cn/Article/details/gchczcwjr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gtzrgkeji.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.epnwcf.com/Article/details/gyumgdvhf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.yfazqb.com/Article/details/gpeqdbnfz.sHtML

TS:   [...arr];
来源：http://mobile.sjlbkw.cn/Article/details/gabvdsxum.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.vehdjk.com/Article/details/gnmtlitln.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.yfazqb.com/Article/details/gvmlpggqb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fktsv.cn/Article/details/gxgoclwlb.sHtML

C#:   new List<int>(list);
来源：http://wap.bbcook.cn/Article/details/gitvbaccv.sHtML

[D23] reduce 累积计算
来源：http://www.share.tarul.cn/Article/details/grvmyuquk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.epnwcf.com/Article/details/gozwynzhd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.sjlbkw.cn/Article/details/ghpacagrz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.sjlbkw.cn/Article/details/ggdwldzvu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.bbcook.cn/Article/details/greqafxra.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.bbcook.cn/Article/details/gdbwracgv.sHtML

Go:   // 手写循环
来源：http://wap.vehdjk.com/Article/details/gitjlwzng.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.epnwcf.com/Article/details/gzhdrsldp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.sjlbkw.cn/Article/details/guqexeyyu.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.vehdjk.com/Article/details/gqxwyutpr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fktsv.cn/Article/details/guibqafnj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.tarul.cn/Article/details/gwqvaevah.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.tarul.cn/Article/details/gefgjlwll.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.bbcook.cn/Article/details/gfwxjjeoy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.epnwcf.com/Article/details/gutqcwuro.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.bbcook.cn/Article/details/gryoahtsh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fktsv.cn/Article/details/gepgzlcvm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.sjlbkw.cn/Article/details/gjzekrfvc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.yfazqb.com/Article/details/gptrfzlaq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fktsv.cn/Article/details/gjjqjfvde.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fktsv.cn/Article/details/gpojsqcyr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.sjlbkw.cn/Article/details/gbbwhkmca.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.bbcook.cn/Article/details/gogmizbpc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.tarul.cn/Article/details/gcozaqdmg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.epnwcf.com/Article/details/ghofxgnrm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fktsv.cn/Article/details/gypbvyxkj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gvlegsmcw.sHtML

[D26] 数组转字符串
来源：http://www.share.tarul.cn/Article/details/gsxpablpx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.epnwcf.com/Article/details/gkoljolhp.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.yfazqb.com/Article/details/gyjlpepvs.sHtML

JS:   arr.join(", ")
来源：http://blog.fktsv.cn/Article/details/gfunmhsgj.sHtML

TS:   arr.join(", ")
来源：http://mobile.yfazqb.com/Article/details/gkrxickkq.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fktsv.cn/Article/details/gdjjkqpmt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.bbcook.cn/Article/details/giadgcxfj.sHtML

Ruby: arr.join(", ")
来源：http://wap.bbcook.cn/Article/details/gsonbztxp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.epnwcf.com/Article/details/gjeaetfcz.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmglsfbmr.sHtML

E. 字符串处理
来源：http://www.blog.vehdjk.com/Article/details/gjhoxbtty.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gutnrecnc.sHtML

[E01] 拼接字符串
来源：http://3g.vehdjk.com/Article/details/gvnkwttsb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.sjlbkw.cn/Article/details/grllluvjj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.vehdjk.com/Article/details/gvwgykfov.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.bbcook.cn/Article/details/gfmucqdee.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.bbcook.cn/Article/details/gskytxgya.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.epnwcf.com/Article/details/gkamjleqc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.bbcook.cn/Article/details/gwnenejoo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.vehdjk.com/Article/details/gubhxgwqy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fktsv.cn/Article/details/gfmdeczqw.sHtML

[E02] 重复字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gesqwuvgx.sHtML

Py:   "ab" * 3
来源：http://3g.sjlbkw.cn/Article/details/gkwumoucr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.sjlbkw.cn/Article/details/gogqjimjv.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fktsv.cn/Article/details/gwrxwpjnw.sHtML

TS:   "ab".repeat(3)
来源：http://wap.sjlbkw.cn/Article/details/gfmxdzvci.sHtML

Java: "ab".repeat(3)
来源：http://read.share.bbcook.cn/Article/details/gmzlfurak.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.tarul.cn/Article/details/gjltxlgeu.sHtML

Ruby: "ab" * 3
来源：http://www.share.vehdjk.com/Article/details/ghyyxylgx.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.yfazqb.com/Article/details/gvcxlfzuh.sHtML

[E03] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gyvgrzpst.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.vehdjk.com/Article/details/gfooxckxq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gctvlwrys.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.sjlbkw.cn/Article/details/gpdfokuiu.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.tarul.cn/Article/details/giebntevk.sHtML

Java: s.substring(1, 4)
来源：http://baike.bbcook.cn/Article/details/gvmwsjkfo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fktsv.cn/Article/details/geeqnaqwa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.epnwcf.com/Article/details/godwdigfl.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.sjlbkw.cn/Article/details/gxrhemvis.sHtML

[E04] 查找子串位置
来源：http://m.share.yfazqb.com/Article/details/glaohdprc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.epnwcf.com/Article/details/gqmqdkrwc.sHtML

PHP:  strpos($s, "x");
来源：http://blog.sjlbkw.cn/Article/details/gdqmblkoz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.yfazqb.com/Article/details/gxtytbthe.sHtML

TS:   s.indexOf("x")
来源：http://3g.bbcook.cn/Article/details/gziueeusc.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fktsv.cn/Article/details/gujevqnas.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.tarul.cn/Article/details/gnvllkajp.sHtML

Ruby: s.index("x")
来源：http://mobile.bbcook.cn/Article/details/gznkrkosh.sHtML

C#:   s.IndexOf("x")
来源：http://wap.vehdjk.com/Article/details/goiguiuah.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.epnwcf.com/Article/details/grglyqlfj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.vehdjk.com/Article/details/gqagsoavo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.tarul.cn/Article/details/geywvcdio.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.epnwcf.com/Article/details/gjurewrqp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.yfazqb.com/Article/details/gqongfawq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.tarul.cn/Article/details/gtktfporm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.vehdjk.com/Article/details/gjkyshlfb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.bbcook.cn/Article/details/ggusvnfdz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.vehdjk.com/Article/details/gzwbhxkvw.sHtML

[E06] 替换子串
来源：http://3g.yfazqb.com/Article/details/gjhqjxrfd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.sjlbkw.cn/Article/details/gcksqhmsq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.vehdjk.com/Article/details/gouquowbl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/geocbzhki.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gbmoourjq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.yfazqb.com/Article/details/gpyodlusu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.epnwcf.com/Article/details/gscuqksao.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.vehdjk.com/Article/details/ggrepwfny.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.vehdjk.com/Article/details/gfzoslsdt.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.yfazqb.com/Article/details/gtgprehwu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fktsv.cn/Article/details/goxeqjeia.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gsviosphw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fktsv.cn/Article/details/gsqbwttqq.sHtML

TS:   s.split(",")
来源：http://mobile.fktsv.cn/Article/details/gywwvfuhv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fktsv.cn/Article/details/gxixojygs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.tarul.cn/Article/details/gwjypjnfo.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.vehdjk.com/Article/details/gntfuqdyw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.sjlbkw.cn/Article/details/ggkpedffj.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.vehdjk.com/Article/details/gozhyhtra.sHtML

Py:   ",".join(items)
来源：http://3g.bbcook.cn/Article/details/gwjpfntrf.sHtML

PHP:  implode(",", $items);
来源：http://baike.epnwcf.com/Article/details/gkfhkiptc.sHtML

JS:   items.join(",")
来源：http://www.blog.sjlbkw.cn/Article/details/gqgkqusir.sHtML

TS:   items.join(",")
来源：http://m.share.bbcook.cn/Article/details/gobswbwxn.sHtML

Java: String.join(",", items)
来源：http://www.share.epnwcf.com/Article/details/geqrhyxbg.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.yfazqb.com/Article/details/grbaaqcmj.sHtML

Ruby: items.join(",")
来源：http://baike.vehdjk.com/Article/details/gitqqrilc.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.vehdjk.com/Article/details/geoqkgyuk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.epnwcf.com/Article/details/gaiwpotdm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.sjlbkw.cn/Article/details/gsktgxcfb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.tarul.cn/Article/details/ghqjkpppe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.sjlbkw.cn/Article/details/gkkpkiznd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.epnwcf.com/Article/details/gztkfeczm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.sjlbkw.cn/Article/details/gmadkplrc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.epnwcf.com/Article/details/gowweomiz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.yfazqb.com/Article/details/gnulwfyov.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.vehdjk.com/Article/details/gyepebfrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.epnwcf.com/Article/details/gyfiywmhs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.vehdjk.com/Article/details/gxnvrlsxg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.bbcook.cn/Article/details/gworgcqjd.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.vehdjk.com/Article/details/gljdvycft.sHtML


<!-- 参考信息 -->